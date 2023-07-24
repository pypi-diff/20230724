# Comparing `tmp/serialtools-0.5.0.tar.gz` & `tmp/serialtools-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serialtools-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "serialtools-0.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `serialtools-0.5.0.tar` & `serialtools-0.6.0.tar`

### file list

```diff
@@ -1,104 +1,104 @@
--rw-r--r--   0        0        0      330 2023-06-02 06:55:40.811546 serialtools-0.5.0/.gitignore
--rw-r--r--   0        0        0      119 2023-06-21 10:33:17.761717 serialtools-0.5.0/.gitlab-ci.yml
--rw-r--r--   0        0        0      657 2023-06-21 08:53:39.687960 serialtools-0.5.0/LICENSE
--rw-r--r--   0        0        0      444 2023-06-21 10:33:17.761717 serialtools-0.5.0/README.md
--rw-r--r--   0        0        0      638 2023-06-21 10:33:17.761717 serialtools-0.5.0/docs/Makefile
--rw-r--r--   0        0        0     1014 2023-06-26 12:52:04.102651 serialtools-0.5.0/docs/build/html/_sources/index.rst.txt
--rw-r--r--   0        0        0       70 2023-06-21 10:33:17.761717 serialtools-0.5.0/docs/build/html/_sources/modules.rst.txt
--rw-r--r--   0        0        0      157 2023-06-21 10:33:17.761717 serialtools-0.5.0/docs/build/html/_sources/serialtools.apps.decode.rst.txt
--rw-r--r--   0        0        0      151 2023-06-21 10:33:17.761717 serialtools-0.5.0/docs/build/html/_sources/serialtools.apps.dump.rst.txt
--rw-r--r--   0        0        0      163 2023-06-26 12:52:04.102651 serialtools-0.5.0/docs/build/html/_sources/serialtools.apps.rawsplit.rst.txt
--rw-r--r--   0        0        0      302 2023-06-21 10:33:17.761717 serialtools-0.5.0/docs/build/html/_sources/serialtools.apps.rst.txt
--rw-r--r--   0        0        0      151 2023-06-21 10:33:17.761717 serialtools-0.5.0/docs/build/html/_sources/serialtools.apps.send.rst.txt
--rw-r--r--   0        0        0      133 2023-06-21 10:33:17.761717 serialtools-0.5.0/docs/build/html/_sources/serialtools.bus.rst.txt
--rw-r--r--   0        0        0      148 2023-06-21 10:33:17.761717 serialtools-0.5.0/docs/build/html/_sources/serialtools.database.rst.txt
--rw-r--r--   0        0        0      171 2023-06-21 10:33:17.761717 serialtools-0.5.0/docs/build/html/_sources/serialtools.database_config.rst.txt
--rw-r--r--   0        0        0      360 2023-06-21 10:33:17.765050 serialtools-0.5.0/docs/build/html/_sources/serialtools.rst.txt
--rw-r--r--   0        0        0     4289 2023-07-24 09:29:30.775804 serialtools-0.5.0/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0        0        0    14813 2023-07-24 09:29:32.512455 serialtools-0.5.0/docs/build/html/_static/basic.css
--rw-r--r--   0        0        0     3229 2023-06-21 10:33:17.765050 serialtools-0.5.0/docs/build/html/_static/css/badge_only.css
--rw-r--r--   0        0        0    87624 2023-06-21 10:33:17.765050 serialtools-0.5.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0        0        0    67312 2023-06-21 10:33:17.765050 serialtools-0.5.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0        0        0    86288 2023-06-21 10:33:17.765050 serialtools-0.5.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0        0        0    66444 2023-06-21 10:33:17.765050 serialtools-0.5.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0        0        0   165742 2023-06-21 10:33:17.765050 serialtools-0.5.0/docs/build/html/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0        0        0   444379 2023-06-21 10:33:17.768383 serialtools-0.5.0/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0        0        0   165548 2023-06-21 10:33:17.771717 serialtools-0.5.0/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0        0        0    98024 2023-06-21 10:33:17.771717 serialtools-0.5.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0        0        0    77160 2023-06-21 10:33:17.771717 serialtools-0.5.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0        0        0   323344 2023-06-21 10:33:17.771717 serialtools-0.5.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0        0        0   193308 2023-06-21 10:33:17.775050 serialtools-0.5.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0        0        0   309728 2023-06-21 10:33:17.775050 serialtools-0.5.0/docs/build/html/_static/css/fonts/lato-bold.woff
--rw-r--r--   0        0        0   184912 2023-06-21 10:33:17.775050 serialtools-0.5.0/docs/build/html/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0        0        0   328412 2023-06-21 10:33:17.778383 serialtools-0.5.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0        0        0   195704 2023-06-21 10:33:17.778383 serialtools-0.5.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0        0        0   309192 2023-06-21 10:33:17.778383 serialtools-0.5.0/docs/build/html/_static/css/fonts/lato-normal.woff
--rw-r--r--   0        0        0   182708 2023-06-21 10:33:17.778383 serialtools-0.5.0/docs/build/html/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0        0        0   135314 2023-06-21 10:33:17.781717 serialtools-0.5.0/docs/build/html/_static/css/theme.css
--rw-r--r--   0        0        0     4472 2023-06-21 10:33:17.781717 serialtools-0.5.0/docs/build/html/_static/doctools.js
--rw-r--r--   0        0        0      421 2023-07-24 09:30:04.135508 serialtools-0.5.0/docs/build/html/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2023-06-21 10:33:17.781717 serialtools-0.5.0/docs/build/html/_static/file.png
--rw-r--r--   0        0        0    89501 2023-07-24 09:29:30.775804 serialtools-0.5.0/docs/build/html/_static/jquery.js
--rw-r--r--   0        0        0      934 2023-06-21 10:33:17.781717 serialtools-0.5.0/docs/build/html/_static/js/badge_only.js
--rw-r--r--   0        0        0     4370 2023-06-21 10:33:17.781717 serialtools-0.5.0/docs/build/html/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0        0        0     2734 2023-06-21 10:33:17.781717 serialtools-0.5.0/docs/build/html/_static/js/html5shiv.min.js
--rw-r--r--   0        0        0     5023 2023-06-21 10:33:17.781717 serialtools-0.5.0/docs/build/html/_static/js/theme.js
--rw-r--r--   0        0        0     4758 2023-07-24 09:29:32.512455 serialtools-0.5.0/docs/build/html/_static/language_data.js
--rw-r--r--   0        0        0       90 2023-06-21 10:33:17.781717 serialtools-0.5.0/docs/build/html/_static/minus.png
--rw-r--r--   0        0        0       46 2023-06-21 10:33:17.781717 serialtools-0.5.0/docs/build/html/_static/no-ligatures-in-code.css
--rw-r--r--   0        0        0       90 2023-06-21 10:33:17.781717 serialtools-0.5.0/docs/build/html/_static/plus.png
--rw-r--r--   0        0        0     4819 2023-07-24 09:29:32.505788 serialtools-0.5.0/docs/build/html/_static/pygments.css
--rw-r--r--   0        0        0    18215 2023-06-21 10:33:17.781717 serialtools-0.5.0/docs/build/html/_static/searchtools.js
--rw-r--r--   0        0        0     4712 2023-06-21 10:33:17.781717 serialtools-0.5.0/docs/build/html/_static/sphinx_highlight.js
--rw-r--r--   0        0        0      204 2023-06-21 10:33:17.781717 serialtools-0.5.0/docs/build/html/_static/sphinx_paramlinks.css
--rw-r--r--   0        0        0      117 2023-06-21 10:33:17.781717 serialtools-0.5.0/docs/build/html/_static/tab-size.css
--rw-r--r--   0        0        0    29298 2023-07-24 09:30:04.135508 serialtools-0.5.0/docs/build/html/genindex.html
--rw-r--r--   0        0        0    16388 2023-07-24 09:30:04.135508 serialtools-0.5.0/docs/build/html/index.html
--rw-r--r--   0        0        0    11076 2023-07-24 09:30:04.135508 serialtools-0.5.0/docs/build/html/modules.html
--rw-r--r--   0        0        0     1381 2023-07-24 09:30:04.135508 serialtools-0.5.0/docs/build/html/objects.inv
--rw-r--r--   0        0        0     6959 2023-07-24 09:30:04.135508 serialtools-0.5.0/docs/build/html/py-modindex.html
--rw-r--r--   0        0        0     4930 2023-07-24 09:30:04.135508 serialtools-0.5.0/docs/build/html/search.html
--rw-r--r--   0        0        0    25673 2023-07-24 09:30:04.135508 serialtools-0.5.0/docs/build/html/searchindex.js
--rw-r--r--   0        0        0    14727 2023-07-24 09:30:04.135508 serialtools-0.5.0/docs/build/html/serialtools.apps.decode.html
--rw-r--r--   0        0        0    12315 2023-07-24 09:30:04.135508 serialtools-0.5.0/docs/build/html/serialtools.apps.dump.html
--rw-r--r--   0        0        0    10619 2023-07-24 09:30:04.135508 serialtools-0.5.0/docs/build/html/serialtools.apps.html
--rw-r--r--   0        0        0    13490 2023-07-24 09:30:04.135508 serialtools-0.5.0/docs/build/html/serialtools.apps.rawsplit.html
--rw-r--r--   0        0        0    10817 2023-07-24 09:30:04.138841 serialtools-0.5.0/docs/build/html/serialtools.apps.send.html
--rw-r--r--   0        0        0    48784 2023-07-24 09:30:04.138841 serialtools-0.5.0/docs/build/html/serialtools.bus.html
--rw-r--r--   0        0        0    76321 2023-07-24 09:30:04.138841 serialtools-0.5.0/docs/build/html/serialtools.database.html
--rw-r--r--   0        0        0    39042 2023-07-24 09:30:04.138841 serialtools-0.5.0/docs/build/html/serialtools.database_config.html
--rw-r--r--   0        0        0    33294 2023-07-24 09:30:04.138841 serialtools-0.5.0/docs/build/html/serialtools.html
--rw-r--r--   0        0        0      804 2023-06-21 10:33:17.785050 serialtools-0.5.0/docs/make.bat
--rw-r--r--   0        0        0       46 2023-06-21 10:33:17.785050 serialtools-0.5.0/docs/source/_static/no-ligatures-in-code.css
--rw-r--r--   0        0        0      117 2023-06-21 10:33:17.785050 serialtools-0.5.0/docs/source/_static/tab-size.css
--rw-r--r--   0        0        0     3095 2023-07-24 09:30:04.138841 serialtools-0.5.0/docs/source/conf.py
--rw-r--r--   0        0        0     1014 2023-07-24 09:29:29.629147 serialtools-0.5.0/docs/source/index.rst
--rw-r--r--   0        0        0       70 2023-07-24 09:29:29.555815 serialtools-0.5.0/docs/source/modules.rst
--rw-r--r--   0        0        0      157 2023-07-24 09:29:29.555815 serialtools-0.5.0/docs/source/serialtools.apps.decode.rst
--rw-r--r--   0        0        0      151 2023-07-24 09:29:29.559148 serialtools-0.5.0/docs/source/serialtools.apps.dump.rst
--rw-r--r--   0        0        0      163 2023-07-24 09:29:29.555815 serialtools-0.5.0/docs/source/serialtools.apps.rawsplit.rst
--rw-r--r--   0        0        0      302 2023-07-24 09:29:29.555815 serialtools-0.5.0/docs/source/serialtools.apps.rst
--rw-r--r--   0        0        0      151 2023-07-24 09:29:29.555815 serialtools-0.5.0/docs/source/serialtools.apps.send.rst
--rw-r--r--   0        0        0      133 2023-07-24 09:29:29.559148 serialtools-0.5.0/docs/source/serialtools.bus.rst
--rw-r--r--   0        0        0      148 2023-07-24 09:29:29.559148 serialtools-0.5.0/docs/source/serialtools.database.rst
--rw-r--r--   0        0        0      171 2023-07-24 09:29:29.555815 serialtools-0.5.0/docs/source/serialtools.database_config.rst
--rw-r--r--   0        0        0      360 2023-07-24 09:29:29.555815 serialtools-0.5.0/docs/source/serialtools.rst
--rw-r--r--   0        0        0      170 2023-06-23 15:21:45.869968 serialtools-0.5.0/mypy.ini
--rw-r--r--   0        0        0     4135 2023-06-21 10:33:17.785050 serialtools-0.5.0/prepare_for_gitlab_pages.py
--rw-r--r--   0        0        0      786 2023-06-23 15:21:45.869968 serialtools-0.5.0/pyproject.toml
--rwxr-xr-x   0        0        0    12230 2023-06-21 10:33:17.785050 serialtools-0.5.0/release.sh
--rw-r--r--   0        0        0       83 2023-06-21 10:33:17.785050 serialtools-0.5.0/requirements-release.txt
--rw-r--r--   0        0        0       22 2023-06-21 10:33:17.785050 serialtools-0.5.0/requirements-test.txt
--rw-r--r--   0        0        0       87 2023-07-24 09:30:04.138841 serialtools-0.5.0/src/serialtools/__init__.py
--rw-r--r--   0        0        0     1448 2023-07-24 09:29:29.549148 serialtools-0.5.0/src/serialtools/__main__.py
--rw-r--r--   0        0        0      345 2023-07-24 09:29:29.552481 serialtools-0.5.0/src/serialtools/apps/__init__.py
--rw-r--r--   0        0        0     1143 2023-07-24 09:29:29.555815 serialtools-0.5.0/src/serialtools/apps/decode.py
--rw-r--r--   0        0        0     1386 2023-07-24 09:29:29.552481 serialtools-0.5.0/src/serialtools/apps/dump.py
--rw-r--r--   0        0        0     1369 2023-07-24 09:29:29.552481 serialtools-0.5.0/src/serialtools/apps/rawsplit.py
--rw-r--r--   0        0        0      880 2023-07-24 09:29:29.552481 serialtools-0.5.0/src/serialtools/apps/send.py
--rw-r--r--   0        0        0     7396 2023-07-24 09:30:04.138841 serialtools-0.5.0/src/serialtools/bus.py
--rw-r--r--   0        0        0    15088 2023-07-24 09:30:04.138841 serialtools-0.5.0/src/serialtools/database.py
--rw-r--r--   0        0        0     6228 2023-07-24 09:30:04.138841 serialtools-0.5.0/src/serialtools/database_config.py
--rw-r--r--   0        0        0        0 2022-11-03 16:33:53.710006 serialtools-0.5.0/src/serialtools/py.typed
--rw-r--r--   0        0        0      336 2023-06-23 15:21:45.869968 serialtools-0.5.0/tox.ini
--rw-r--r--   0        0        0     1156 1970-01-01 00:00:00.000000 serialtools-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      330 2023-06-02 06:55:40.811546 serialtools-0.6.0/.gitignore
+-rw-r--r--   0        0        0      119 2023-06-21 10:33:17.761717 serialtools-0.6.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0      657 2023-06-21 08:53:39.687960 serialtools-0.6.0/LICENSE
+-rw-r--r--   0        0        0      444 2023-06-21 10:33:17.761717 serialtools-0.6.0/README.md
+-rw-r--r--   0        0        0      638 2023-06-21 10:33:17.761717 serialtools-0.6.0/docs/Makefile
+-rw-r--r--   0        0        0     1014 2023-07-24 09:32:02.524482 serialtools-0.6.0/docs/build/html/_sources/index.rst.txt
+-rw-r--r--   0        0        0       70 2023-06-21 10:33:17.761717 serialtools-0.6.0/docs/build/html/_sources/modules.rst.txt
+-rw-r--r--   0        0        0      157 2023-06-21 10:33:17.761717 serialtools-0.6.0/docs/build/html/_sources/serialtools.apps.decode.rst.txt
+-rw-r--r--   0        0        0      151 2023-06-21 10:33:17.761717 serialtools-0.6.0/docs/build/html/_sources/serialtools.apps.dump.rst.txt
+-rw-r--r--   0        0        0      163 2023-07-24 09:32:02.524482 serialtools-0.6.0/docs/build/html/_sources/serialtools.apps.rawsplit.rst.txt
+-rw-r--r--   0        0        0      302 2023-06-21 10:33:17.761717 serialtools-0.6.0/docs/build/html/_sources/serialtools.apps.rst.txt
+-rw-r--r--   0        0        0      151 2023-06-21 10:33:17.761717 serialtools-0.6.0/docs/build/html/_sources/serialtools.apps.send.rst.txt
+-rw-r--r--   0        0        0      133 2023-06-21 10:33:17.761717 serialtools-0.6.0/docs/build/html/_sources/serialtools.bus.rst.txt
+-rw-r--r--   0        0        0      148 2023-06-21 10:33:17.761717 serialtools-0.6.0/docs/build/html/_sources/serialtools.database.rst.txt
+-rw-r--r--   0        0        0      171 2023-06-21 10:33:17.761717 serialtools-0.6.0/docs/build/html/_sources/serialtools.database_config.rst.txt
+-rw-r--r--   0        0        0      360 2023-06-21 10:33:17.765050 serialtools-0.6.0/docs/build/html/_sources/serialtools.rst.txt
+-rw-r--r--   0        0        0     4289 2023-07-24 12:22:47.729156 serialtools-0.6.0/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0        0        0    14813 2023-07-24 12:22:49.169146 serialtools-0.6.0/docs/build/html/_static/basic.css
+-rw-r--r--   0        0        0     3229 2023-06-21 10:33:17.765050 serialtools-0.6.0/docs/build/html/_static/css/badge_only.css
+-rw-r--r--   0        0        0    87624 2023-06-21 10:33:17.765050 serialtools-0.6.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0        0        0    67312 2023-06-21 10:33:17.765050 serialtools-0.6.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0        0        0    86288 2023-06-21 10:33:17.765050 serialtools-0.6.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0        0        0    66444 2023-06-21 10:33:17.765050 serialtools-0.6.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0        0        0   165742 2023-06-21 10:33:17.765050 serialtools-0.6.0/docs/build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0        0        0   444379 2023-06-21 10:33:17.768383 serialtools-0.6.0/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0        0        0   165548 2023-06-21 10:33:17.771717 serialtools-0.6.0/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0        0        0    98024 2023-06-21 10:33:17.771717 serialtools-0.6.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0        0        0    77160 2023-06-21 10:33:17.771717 serialtools-0.6.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0        0        0   323344 2023-06-21 10:33:17.771717 serialtools-0.6.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0        0        0   193308 2023-06-21 10:33:17.775050 serialtools-0.6.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0        0        0   309728 2023-06-21 10:33:17.775050 serialtools-0.6.0/docs/build/html/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0        0        0   184912 2023-06-21 10:33:17.775050 serialtools-0.6.0/docs/build/html/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0        0        0   328412 2023-06-21 10:33:17.778383 serialtools-0.6.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0        0        0   195704 2023-06-21 10:33:17.778383 serialtools-0.6.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0        0        0   309192 2023-06-21 10:33:17.778383 serialtools-0.6.0/docs/build/html/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0        0        0   182708 2023-06-21 10:33:17.778383 serialtools-0.6.0/docs/build/html/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0        0        0   135314 2023-06-21 10:33:17.781717 serialtools-0.6.0/docs/build/html/_static/css/theme.css
+-rw-r--r--   0        0        0     4472 2023-06-21 10:33:17.781717 serialtools-0.6.0/docs/build/html/_static/doctools.js
+-rw-r--r--   0        0        0      421 2023-07-24 12:23:43.145457 serialtools-0.6.0/docs/build/html/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2023-06-21 10:33:17.781717 serialtools-0.6.0/docs/build/html/_static/file.png
+-rw-r--r--   0        0        0    89501 2023-07-24 12:22:47.729156 serialtools-0.6.0/docs/build/html/_static/jquery.js
+-rw-r--r--   0        0        0      934 2023-06-21 10:33:17.781717 serialtools-0.6.0/docs/build/html/_static/js/badge_only.js
+-rw-r--r--   0        0        0     4370 2023-06-21 10:33:17.781717 serialtools-0.6.0/docs/build/html/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0        0        0     2734 2023-06-21 10:33:17.781717 serialtools-0.6.0/docs/build/html/_static/js/html5shiv.min.js
+-rw-r--r--   0        0        0     5023 2023-06-21 10:33:17.781717 serialtools-0.6.0/docs/build/html/_static/js/theme.js
+-rw-r--r--   0        0        0     4758 2023-07-24 12:22:49.172479 serialtools-0.6.0/docs/build/html/_static/language_data.js
+-rw-r--r--   0        0        0       90 2023-06-21 10:33:17.781717 serialtools-0.6.0/docs/build/html/_static/minus.png
+-rw-r--r--   0        0        0       46 2023-06-21 10:33:17.781717 serialtools-0.6.0/docs/build/html/_static/no-ligatures-in-code.css
+-rw-r--r--   0        0        0       90 2023-06-21 10:33:17.781717 serialtools-0.6.0/docs/build/html/_static/plus.png
+-rw-r--r--   0        0        0     4819 2023-07-24 12:22:49.165813 serialtools-0.6.0/docs/build/html/_static/pygments.css
+-rw-r--r--   0        0        0    18215 2023-06-21 10:33:17.781717 serialtools-0.6.0/docs/build/html/_static/searchtools.js
+-rw-r--r--   0        0        0     4712 2023-06-21 10:33:17.781717 serialtools-0.6.0/docs/build/html/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0      204 2023-06-21 10:33:17.781717 serialtools-0.6.0/docs/build/html/_static/sphinx_paramlinks.css
+-rw-r--r--   0        0        0      117 2023-06-21 10:33:17.781717 serialtools-0.6.0/docs/build/html/_static/tab-size.css
+-rw-r--r--   0        0        0    29740 2023-07-24 12:23:43.145457 serialtools-0.6.0/docs/build/html/genindex.html
+-rw-r--r--   0        0        0    16388 2023-07-24 12:23:43.145457 serialtools-0.6.0/docs/build/html/index.html
+-rw-r--r--   0        0        0    11076 2023-07-24 12:23:43.145457 serialtools-0.6.0/docs/build/html/modules.html
+-rw-r--r--   0        0        0     1397 2023-07-24 12:23:43.145457 serialtools-0.6.0/docs/build/html/objects.inv
+-rw-r--r--   0        0        0     6959 2023-07-24 12:23:43.145457 serialtools-0.6.0/docs/build/html/py-modindex.html
+-rw-r--r--   0        0        0     4930 2023-07-24 12:23:43.145457 serialtools-0.6.0/docs/build/html/search.html
+-rw-r--r--   0        0        0    26142 2023-07-24 12:23:43.145457 serialtools-0.6.0/docs/build/html/searchindex.js
+-rw-r--r--   0        0        0    14727 2023-07-24 12:23:43.145457 serialtools-0.6.0/docs/build/html/serialtools.apps.decode.html
+-rw-r--r--   0        0        0    12315 2023-07-24 12:23:43.145457 serialtools-0.6.0/docs/build/html/serialtools.apps.dump.html
+-rw-r--r--   0        0        0    10619 2023-07-24 12:23:43.145457 serialtools-0.6.0/docs/build/html/serialtools.apps.html
+-rw-r--r--   0        0        0    13490 2023-07-24 12:23:43.145457 serialtools-0.6.0/docs/build/html/serialtools.apps.rawsplit.html
+-rw-r--r--   0        0        0    10817 2023-07-24 12:23:43.145457 serialtools-0.6.0/docs/build/html/serialtools.apps.send.html
+-rw-r--r--   0        0        0    48784 2023-07-24 12:23:43.145457 serialtools-0.6.0/docs/build/html/serialtools.bus.html
+-rw-r--r--   0        0        0    79368 2023-07-24 12:23:43.145457 serialtools-0.6.0/docs/build/html/serialtools.database.html
+-rw-r--r--   0        0        0    39042 2023-07-24 12:23:43.145457 serialtools-0.6.0/docs/build/html/serialtools.database_config.html
+-rw-r--r--   0        0        0    33985 2023-07-24 12:23:43.145457 serialtools-0.6.0/docs/build/html/serialtools.html
+-rw-r--r--   0        0        0      804 2023-06-21 10:33:17.785050 serialtools-0.6.0/docs/make.bat
+-rw-r--r--   0        0        0       46 2023-06-21 10:33:17.785050 serialtools-0.6.0/docs/source/_static/no-ligatures-in-code.css
+-rw-r--r--   0        0        0      117 2023-06-21 10:33:17.785050 serialtools-0.6.0/docs/source/_static/tab-size.css
+-rw-r--r--   0        0        0     3095 2023-07-24 12:23:43.145457 serialtools-0.6.0/docs/source/conf.py
+-rw-r--r--   0        0        0     1014 2023-07-24 12:22:46.822495 serialtools-0.6.0/docs/source/index.rst
+-rw-r--r--   0        0        0       70 2023-07-24 12:22:46.755829 serialtools-0.6.0/docs/source/modules.rst
+-rw-r--r--   0        0        0      157 2023-07-24 12:22:46.755829 serialtools-0.6.0/docs/source/serialtools.apps.decode.rst
+-rw-r--r--   0        0        0      151 2023-07-24 12:22:46.755829 serialtools-0.6.0/docs/source/serialtools.apps.dump.rst
+-rw-r--r--   0        0        0      163 2023-07-24 12:22:46.755829 serialtools-0.6.0/docs/source/serialtools.apps.rawsplit.rst
+-rw-r--r--   0        0        0      302 2023-07-24 12:22:46.755829 serialtools-0.6.0/docs/source/serialtools.apps.rst
+-rw-r--r--   0        0        0      151 2023-07-24 12:22:46.755829 serialtools-0.6.0/docs/source/serialtools.apps.send.rst
+-rw-r--r--   0        0        0      133 2023-07-24 12:22:46.755829 serialtools-0.6.0/docs/source/serialtools.bus.rst
+-rw-r--r--   0        0        0      148 2023-07-24 12:22:46.755829 serialtools-0.6.0/docs/source/serialtools.database.rst
+-rw-r--r--   0        0        0      171 2023-07-24 12:22:46.755829 serialtools-0.6.0/docs/source/serialtools.database_config.rst
+-rw-r--r--   0        0        0      360 2023-07-24 12:22:46.755829 serialtools-0.6.0/docs/source/serialtools.rst
+-rw-r--r--   0        0        0      170 2023-07-24 09:57:32.776198 serialtools-0.6.0/mypy.ini
+-rw-r--r--   0        0        0     4135 2023-06-21 10:33:17.785050 serialtools-0.6.0/prepare_for_gitlab_pages.py
+-rw-r--r--   0        0        0      786 2023-07-24 09:57:32.776198 serialtools-0.6.0/pyproject.toml
+-rwxr-xr-x   0        0        0    12230 2023-06-21 10:33:17.785050 serialtools-0.6.0/release.sh
+-rw-r--r--   0        0        0       83 2023-06-21 10:33:17.785050 serialtools-0.6.0/requirements-release.txt
+-rw-r--r--   0        0        0       22 2023-06-21 10:33:17.785050 serialtools-0.6.0/requirements-test.txt
+-rw-r--r--   0        0        0       87 2023-07-24 12:23:43.148790 serialtools-0.6.0/src/serialtools/__init__.py
+-rw-r--r--   0        0        0     1448 2023-07-24 12:22:46.752495 serialtools-0.6.0/src/serialtools/__main__.py
+-rw-r--r--   0        0        0      345 2023-07-24 12:22:46.752495 serialtools-0.6.0/src/serialtools/apps/__init__.py
+-rw-r--r--   0        0        0     1143 2023-07-24 12:22:46.755829 serialtools-0.6.0/src/serialtools/apps/decode.py
+-rw-r--r--   0        0        0     1386 2023-07-24 12:22:46.752495 serialtools-0.6.0/src/serialtools/apps/dump.py
+-rw-r--r--   0        0        0     1369 2023-07-24 12:22:46.752495 serialtools-0.6.0/src/serialtools/apps/rawsplit.py
+-rw-r--r--   0        0        0      880 2023-07-24 12:22:46.752495 serialtools-0.6.0/src/serialtools/apps/send.py
+-rw-r--r--   0        0        0     7396 2023-07-24 12:22:46.749162 serialtools-0.6.0/src/serialtools/bus.py
+-rw-r--r--   0        0        0    16017 2023-07-24 12:23:43.148790 serialtools-0.6.0/src/serialtools/database.py
+-rw-r--r--   0        0        0     6228 2023-07-24 12:22:46.749162 serialtools-0.6.0/src/serialtools/database_config.py
+-rw-r--r--   0        0        0        0 2022-11-03 16:33:53.710006 serialtools-0.6.0/src/serialtools/py.typed
+-rw-r--r--   0        0        0      336 2023-07-24 09:57:32.776198 serialtools-0.6.0/tox.ini
+-rw-r--r--   0        0        0     1156 1970-01-01 00:00:00.000000 serialtools-0.6.0/PKG-INFO
```

### Comparing `serialtools-0.5.0/LICENSE` & `serialtools-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `serialtools-0.5.0/docs/Makefile` & `serialtools-0.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `serialtools-0.5.0/docs/build/html/_sources/index.rst.txt` & `serialtools-0.6.0/docs/build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `serialtools-0.5.0/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js` & `serialtools-0.6.0/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.5.0/docs/build/html/_static/basic.css` & `serialtools-0.6.0/docs/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `serialtools-0.5.0/docs/build/html/_static/css/badge_only.css` & `serialtools-0.6.0/docs/build/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `serialtools-0.5.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff` & `serialtools-0.6.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `serialtools-0.5.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2` & `serialtools-0.6.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `serialtools-0.5.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff` & `serialtools-0.6.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `serialtools-0.5.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2` & `serialtools-0.6.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `serialtools-0.5.0/docs/build/html/_static/css/fonts/fontawesome-webfont.eot` & `serialtools-0.6.0/docs/build/html/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `serialtools-0.5.0/docs/build/html/_static/css/fonts/fontawesome-webfont.svg` & `serialtools-0.6.0/docs/build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `serialtools-0.5.0/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf` & `serialtools-0.6.0/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `serialtools-0.5.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff` & `serialtools-0.6.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `serialtools-0.5.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2` & `serialtools-0.6.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `serialtools-0.5.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff` & `serialtools-0.6.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `serialtools-0.5.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff2` & `serialtools-0.6.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `serialtools-0.5.0/docs/build/html/_static/css/fonts/lato-bold.woff` & `serialtools-0.6.0/docs/build/html/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `serialtools-0.5.0/docs/build/html/_static/css/fonts/lato-bold.woff2` & `serialtools-0.6.0/docs/build/html/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `serialtools-0.5.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff` & `serialtools-0.6.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `serialtools-0.5.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff2` & `serialtools-0.6.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `serialtools-0.5.0/docs/build/html/_static/css/fonts/lato-normal.woff` & `serialtools-0.6.0/docs/build/html/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `serialtools-0.5.0/docs/build/html/_static/css/fonts/lato-normal.woff2` & `serialtools-0.6.0/docs/build/html/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `serialtools-0.5.0/docs/build/html/_static/css/theme.css` & `serialtools-0.6.0/docs/build/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `serialtools-0.5.0/docs/build/html/_static/doctools.js` & `serialtools-0.6.0/docs/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.5.0/docs/build/html/_static/jquery.js` & `serialtools-0.6.0/docs/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.5.0/docs/build/html/_static/js/badge_only.js` & `serialtools-0.6.0/docs/build/html/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.5.0/docs/build/html/_static/js/html5shiv-printshiv.min.js` & `serialtools-0.6.0/docs/build/html/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.5.0/docs/build/html/_static/js/html5shiv.min.js` & `serialtools-0.6.0/docs/build/html/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.5.0/docs/build/html/_static/js/theme.js` & `serialtools-0.6.0/docs/build/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.5.0/docs/build/html/_static/language_data.js` & `serialtools-0.6.0/docs/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.5.0/docs/build/html/_static/pygments.css` & `serialtools-0.6.0/docs/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `serialtools-0.5.0/docs/build/html/_static/searchtools.js` & `serialtools-0.6.0/docs/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.5.0/docs/build/html/_static/sphinx_highlight.js` & `serialtools-0.6.0/docs/build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.5.0/docs/build/html/genindex.html` & `serialtools-0.6.0/docs/build/html/genindex.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Index &mdash; serialtools v0.5.0 documentation</title>
+  <title>Index &mdash; serialtools v0.6.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -31,15 +31,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.5.0
+                v0.6.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -258,14 +258,16 @@
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="serialtools.database.html#serialtools.database.ByteSpec.format_allowed_values">format_allowed_values() (serialtools.database.ByteSpec method)</a>
 </li>
       <li><a href="serialtools.database.html#serialtools.database.format_bytes">format_bytes() (in module serialtools.database)</a>
 </li>
       <li><a href="serialtools.database.html#serialtools.database.Message.format_raw">format_raw() (serialtools.database.Message method)</a>
 </li>
+      <li><a href="serialtools.database.html#serialtools.database.Message.format_raw_data">format_raw_data() (serialtools.database.Message method)</a>
+</li>
       <li><a href="serialtools.database.html#serialtools.database.Message.format_timestamp">format_timestamp() (serialtools.database.Message method)</a>
 </li>
   </ul></td>
 </tr></table>
 
 <h2 id="G">G</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
@@ -433,14 +435,16 @@
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="serialtools.database.html#serialtools.database.Reader">Reader (class in serialtools.database)</a>
 </li>
       <li><a href="serialtools.bus.html#serialtools.bus.ReadFromFileBus">ReadFromFileBus (class in serialtools.bus)</a>
 </li>
       <li><a href="serialtools.bus.html#serialtools.bus.ReadFromParameterBus">ReadFromParameterBus (class in serialtools.bus)</a>
 </li>
+      <li><a href="serialtools.database.html#serialtools.database.Reader.retry_byte">retry_byte() (serialtools.database.Reader method)</a>
+</li>
       <li><a href="serialtools.bus.html#serialtools.bus.BusCreator.rtscts">rtscts (serialtools.bus.BusCreator attribute)</a>
 </li>
       <li><a href="serialtools.database_config.html#serialtools.database_config.Message.run_parsed">run_parsed() (serialtools.database_config.Message method)</a>
 
       <ul>
         <li><a href="serialtools.database_config.html#serialtools.database_config.Param.run_parsed">(serialtools.database_config.Param method)</a>
 </li>
@@ -542,22 +546,24 @@
 </tr></table>
 
 <h2 id="T">T</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="serialtools.database.html#serialtools.database.Type.TEXT">TEXT (serialtools.database.Type attribute)</a>
 </li>
+      <li><a href="serialtools.database.html#serialtools.database.Reader.timeout">timeout (serialtools.database.Reader attribute)</a>
+</li>
+  </ul></td>
+  <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="serialtools.bus.html#serialtools.bus.ReadFromFileBus.timestamp">timestamp (serialtools.bus.ReadFromFileBus attribute)</a>
 
       <ul>
         <li><a href="serialtools.bus.html#serialtools.bus.WriteToFileBus.timestamp">(serialtools.bus.WriteToFileBus attribute)</a>
 </li>
       </ul></li>
-  </ul></td>
-  <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="serialtools.database.html#serialtools.database.Type">Type (class in serialtools.database)</a>
 </li>
   </ul></td>
 </tr></table>
 
 <h2 id="U">U</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 
 
 serialtools
-v0.5.0
+v0.6.0
 [q                   ]
     * serialtools_package
     * serialtools.apps.decode_module
     * serialtools.apps.dump_module
     * serialtools.apps.rawsplit_module
     * serialtools.apps.send_module
     * serialtools.bus_module
@@ -81,21 +81,24 @@
       (serialtools.database.Database             attribute)
       method)                            * error()_(in_module_serialtools.apps.decode)
     * Endianness_(class_in                     o (in_module_serialtools.apps.rawsplit)
       serialtools.database)
 ***** F *****
                                                       * format_allowed_values()_
                                                         (serialtools.database.ByteSpec
-    * FLOAT_(serialtools.database.Type_attribute)       method)
-    * fn_(serialtools.bus.ReadFromFileBus             * format_bytes()_(in_module
-      parameter)                                        serialtools.database)
-          o (serialtools.bus.ReadFromParameterBus     * format_raw()_
-            parameter)                                  (serialtools.database.Message
-    * format()_(serialtools.database.Message            method)
-      method)                                         * format_timestamp()_
+                                                        method)
+    * FLOAT_(serialtools.database.Type_attribute)     * format_bytes()_(in_module
+    * fn_(serialtools.bus.ReadFromFileBus               serialtools.database)
+      parameter)                                      * format_raw()_
+          o (serialtools.bus.ReadFromParameterBus       (serialtools.database.Message
+            parameter)                                  method)
+    * format()_(serialtools.database.Message          * format_raw_data()_
+      method)                                           (serialtools.database.Message
+                                                        method)
+                                                      * format_timestamp()_
                                                         (serialtools.database.Message
                                                         method)
 ***** G *****
                                                        * get_length()_
     * get()_                                             (serialtools.database.ByteSpec
       (serialtools.database_config.DatabaseCreator       method)
       method)                                          * get_signal()_
@@ -156,24 +159,25 @@
                                              * port_(serialtools.bus.BusCreator_attribute)
 ***** R *****
     * read()_                                   * Reader_(class_in_serialtools.database)
       (serialtools.bus.ReadFromFileBus          * ReadFromFileBus_(class_in
       method)                                     serialtools.bus)
           o (serialtools.bus.WriteToFileBus     * ReadFromParameterBus_(class_in
             method)                               serialtools.bus)
-          o (serialtools.database.Reader        * rtscts_(serialtools.bus.BusCreator
-            method)                               attribute)
-    * read_byte()_                              * run_parsed()_
+          o (serialtools.database.Reader        * retry_byte()_(serialtools.database.Reader
+            method)                               method)
+    * read_byte()_                              * rtscts_(serialtools.bus.BusCreator
+      (serialtools.database.Reader_method)        attribute)
+    * read_in_other_thread()_                   * run_parsed()_
       (serialtools.database.Reader_method)        (serialtools.database_config.Message
-    * read_in_other_thread()_                     method)
+    * read_msg()_                                 method)
       (serialtools.database.Reader_method)            o (serialtools.database_config.Param
-    * read_msg()_                                       method)
-      (serialtools.database.Reader_method)            o (serialtools.database_config.Signal
     * read_n_bytes()_                                   method)
-      (serialtools.database.Reader_method)
+      (serialtools.database.Reader_method)            o (serialtools.database_config.Signal
+                                                        method)
 ***** S *****
     * send()_(in_module                * serialtools.bus
       serialtools.apps.send)                 o module
     * send_msg()_                      * serialtools.database
       (serialtools.database.Reader           o module
       method)                          * serialtools.database_config
     * serialtools                            o module
@@ -185,21 +189,20 @@
     * serialtools.apps.dump                  o (serialtools.database_config.Signal
           o module                             attribute)
     * serialtools.apps.rawsplit        * stop()_(serialtools.database.Reader
           o module                       method)
     * serialtools.apps.send            * stopbits_(serialtools.bus.BusCreator
           o module                       attribute)
 ***** T *****
-    * TEXT_(serialtools.database.Type
-      attribute)
-    * timestamp_                                * Type_(class_in
-      (serialtools.bus.ReadFromFileBus            serialtools.database)
-      attribute)
-          o (serialtools.bus.WriteToFileBus
-            attribute)
+    * TEXT_                            * timestamp_
+      (serialtools.database.Type         (serialtools.bus.ReadFromFileBus
+      attribute)                         attribute)
+    * timeout_                               o (serialtools.bus.WriteToFileBus
+      (serialtools.database.Reader             attribute)
+      attribute)                       * Type_(class_in_serialtools.database)
 ***** U *****
     * UINT_(serialtools.database.Type_attribute)
 ***** V *****
                                       * vport_(serialtools.bus.BusCreator
     * virtual_                          attribute)
       (serialtools.bus.BusCreator     * vport_other_
       attribute)                        (serialtools.bus.BusCreator
```

### Comparing `serialtools-0.5.0/docs/build/html/index.html` & `serialtools-0.6.0/docs/build/html/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Welcome to serialtools’ documentation! &mdash; serialtools v0.5.0 documentation</title>
+  <title>Welcome to serialtools’ documentation! &mdash; serialtools v0.6.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -33,15 +33,15 @@
 
           
           
           <a href="#" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.5.0
+                v0.6.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -4,15 +4,15 @@
 
 
 
 
 
 
 serialtools
-v0.5.0
+v0.6.0
 [q                   ]
     * serialtools_package
     * serialtools.apps.decode_module
     * serialtools.apps.dump_module
     * serialtools.apps.rawsplit_module
     * serialtools.apps.send_module
     * serialtools.bus_module
```

### Comparing `serialtools-0.5.0/docs/build/html/modules.html` & `serialtools-0.6.0/docs/build/html/modules.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools &mdash; serialtools v0.5.0 documentation</title>
+  <title>serialtools &mdash; serialtools v0.6.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -32,15 +32,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.5.0
+                v0.6.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 
 
 serialtools
-v0.5.0
+v0.6.0
 [q                   ]
     * serialtools_package
     * serialtools.apps.decode_module
     * serialtools.apps.dump_module
     * serialtools.apps.rawsplit_module
     * serialtools.apps.send_module
     * serialtools.bus_module
```

### Comparing `serialtools-0.5.0/docs/build/html/py-modindex.html` & `serialtools-0.6.0/docs/build/html/py-modindex.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Python Module Index &mdash; serialtools v0.5.0 documentation</title>
+  <title>Python Module Index &mdash; serialtools v0.6.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -34,15 +34,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.5.0
+                v0.6.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 
 
 serialtools
-v0.5.0
+v0.6.0
 [q                   ]
     * serialtools_package
     * serialtools.apps.decode_module
     * serialtools.apps.dump_module
     * serialtools.apps.rawsplit_module
     * serialtools.apps.send_module
     * serialtools.bus_module
```

### Comparing `serialtools-0.5.0/docs/build/html/search.html` & `serialtools-0.6.0/docs/build/html/search.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Search &mdash; serialtools v0.5.0 documentation</title>
+  <title>Search &mdash; serialtools v0.6.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
     
   <!--[if lt IE 9]>
@@ -34,15 +34,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.5.0
+                v0.6.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="#" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 
 
 serialtools
-v0.5.0
+v0.6.0
 [q                   ]
     * serialtools_package
     * serialtools.apps.decode_module
     * serialtools.apps.dump_module
     * serialtools.apps.rawsplit_module
     * serialtools.apps.send_module
     * serialtools.bus_module
```

### Comparing `serialtools-0.5.0/docs/build/html/searchindex.js` & `serialtools-0.6.0/docs/build/html/searchindex.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -279,15 +279,18 @@
         "logger": 10,
         "rootlogg": 10,
         "root": 10,
         "level": 10,
         "collect": 10,
         "abc": 10,
         "confattr": 10,
-        "notificationlevel": 10
+        "notificationlevel": 10,
+        "format_raw_data": [2, 9],
+        "retry_byt": [2, 9],
+        "timeout": [2, 9]
     },
     "objects": {
         "": [
             [2, 0, 0, "-", "serialtools"]
         ],
         "serialtools": [
             [3, 0, 0, "-", "apps"],
@@ -404,28 +407,31 @@
             [9, 4, 1, "", "BIG"],
             [9, 4, 1, "", "LITTLE"]
         ],
         "serialtools.database.Message": [
             [9, 3, 1, "", "decode"],
             [9, 3, 1, "", "format"],
             [9, 3, 1, "", "format_raw"],
+            [9, 3, 1, "", "format_raw_data"],
             [9, 3, 1, "", "format_timestamp"]
         ],
         "serialtools.database.MessageSpec": [
             [9, 4, 1, "", "ADDRESS"]
         ],
         "serialtools.database.Reader": [
             [9, 4, 1, "", "ignore_bytes_between_messages"],
             [9, 3, 1, "", "read"],
             [9, 3, 1, "", "read_byte"],
             [9, 3, 1, "", "read_in_other_thread"],
             [9, 3, 1, "", "read_msg"],
             [9, 3, 1, "", "read_n_bytes"],
+            [9, 3, 1, "", "retry_byte"],
             [9, 3, 1, "", "send_msg"],
-            [9, 3, 1, "", "stop"]
+            [9, 3, 1, "", "stop"],
+            [9, 4, 1, "", "timeout"]
         ],
         "serialtools.database.Signal": [
             [9, 3, 1, "", "get_bitstruct_fmt"],
             [9, 3, 1, "", "init"]
         ],
         "serialtools.database.Type": [
             [9, 4, 1, "", "BOOL"],
@@ -840,14 +846,17 @@
         ],
         "format_bytes() (in module serialtools.database)": [
             [9, "serialtools.database.format_bytes"]
         ],
         "format_raw() (serialtools.database.message method)": [
             [9, "serialtools.database.Message.format_raw"]
         ],
+        "format_raw_data() (serialtools.database.message method)": [
+            [9, "serialtools.database.Message.format_raw_data"]
+        ],
         "format_timestamp() (serialtools.database.message method)": [
             [9, "serialtools.database.Message.format_timestamp"]
         ],
         "get_bitstruct_fmt() (serialtools.database.signal method)": [
             [9, "serialtools.database.Signal.get_bitstruct_fmt"]
         ],
         "get_endianness_fmt() (serialtools.database.database method)": [
@@ -882,26 +891,32 @@
         ],
         "read_msg() (serialtools.database.reader method)": [
             [9, "serialtools.database.Reader.read_msg"]
         ],
         "read_n_bytes() (serialtools.database.reader method)": [
             [9, "serialtools.database.Reader.read_n_bytes"]
         ],
+        "retry_byte() (serialtools.database.reader method)": [
+            [9, "serialtools.database.Reader.retry_byte"]
+        ],
         "send_msg() (serialtools.database.reader method)": [
             [9, "serialtools.database.Reader.send_msg"]
         ],
         "serialtools.database": [
             [9, "module-serialtools.database"]
         ],
         "signals (serialtools.database.database attribute)": [
             [9, "serialtools.database.Database.signals"]
         ],
         "stop() (serialtools.database.reader method)": [
             [9, "serialtools.database.Reader.stop"]
         ],
+        "timeout (serialtools.database.reader attribute)": [
+            [9, "serialtools.database.Reader.timeout"]
+        ],
         "word_length_in_bits (serialtools.database.database attribute)": [
             [9, "serialtools.database.Database.word_length_in_bits"]
         ],
         "databasecreator (class in serialtools.database_config)": [
             [10, "serialtools.database_config.DatabaseCreator"]
         ],
         "loggingcallback (class in serialtools.database_config)": [
```

### Comparing `serialtools-0.5.0/docs/build/html/serialtools.apps.decode.html` & `serialtools-0.6.0/docs/build/html/serialtools.apps.decode.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools.apps.decode module &mdash; serialtools v0.5.0 documentation</title>
+  <title>serialtools.apps.decode module &mdash; serialtools v0.6.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -34,15 +34,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.5.0
+                v0.6.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 
 
 
 
 
 
 serialtools
-v0.5.0
+v0.6.0
 [q                   ]
     * serialtools_package
           o Subpackages
                 # serialtools.apps_package
                       # Submodules
                       # Module_contents
           o Submodules
```

### Comparing `serialtools-0.5.0/docs/build/html/serialtools.apps.dump.html` & `serialtools-0.6.0/docs/build/html/serialtools.apps.dump.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools.apps.dump module &mdash; serialtools v0.5.0 documentation</title>
+  <title>serialtools.apps.dump module &mdash; serialtools v0.6.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -34,15 +34,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.5.0
+                v0.6.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 
 
 
 
 
 
 serialtools
-v0.5.0
+v0.6.0
 [q                   ]
     * serialtools_package
           o Subpackages
                 # serialtools.apps_package
                       # Submodules
                       # Module_contents
           o Submodules
```

### Comparing `serialtools-0.5.0/docs/build/html/serialtools.apps.html` & `serialtools-0.6.0/docs/build/html/serialtools.apps.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools.apps package &mdash; serialtools v0.5.0 documentation</title>
+  <title>serialtools.apps package &mdash; serialtools v0.6.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -34,15 +34,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.5.0
+                v0.6.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 
 
 
 
 
 
 serialtools
-v0.5.0
+v0.6.0
 [q                   ]
     * serialtools_package
           o Subpackages
                 # serialtools.apps_package
                       # Submodules
                       # Module_contents
           o Submodules
```

### Comparing `serialtools-0.5.0/docs/build/html/serialtools.apps.rawsplit.html` & `serialtools-0.6.0/docs/build/html/serialtools.apps.rawsplit.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools.apps.rawsplit module &mdash; serialtools v0.5.0 documentation</title>
+  <title>serialtools.apps.rawsplit module &mdash; serialtools v0.6.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -33,15 +33,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.5.0
+                v0.6.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -4,15 +4,15 @@
 
 
 
 
 
 
 serialtools
-v0.5.0
+v0.6.0
 [q                   ]
     * serialtools_package
     * serialtools.apps.decode_module
     * serialtools.apps.dump_module
     * serialtools.apps.rawsplit_module
           o add_arguments()
           o add_parser()
```

### Comparing `serialtools-0.5.0/docs/build/html/serialtools.apps.send.html` & `serialtools-0.6.0/docs/build/html/serialtools.apps.send.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools.apps.send module &mdash; serialtools v0.5.0 documentation</title>
+  <title>serialtools.apps.send module &mdash; serialtools v0.6.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -34,15 +34,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.5.0
+                v0.6.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 
 
 
 
 
 
 serialtools
-v0.5.0
+v0.6.0
 [q                   ]
     * serialtools_package
           o Subpackages
                 # serialtools.apps_package
                       # Submodules
                       # Module_contents
           o Submodules
```

### Comparing `serialtools-0.5.0/docs/build/html/serialtools.bus.html` & `serialtools-0.6.0/docs/build/html/serialtools.bus.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools.bus module &mdash; serialtools v0.5.0 documentation</title>
+  <title>serialtools.bus module &mdash; serialtools v0.6.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -34,15 +34,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.5.0
+                v0.6.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 
 
 
 
 
 
 serialtools
-v0.5.0
+v0.6.0
 [q                   ]
     * serialtools_package
           o Subpackages
           o Submodules
                 # serialtools.bus_module
                       # BusCreator
                       # ReadFromFileBus
```

### Comparing `serialtools-0.5.0/docs/build/html/serialtools.database.html` & `serialtools-0.6.0/docs/build/html/serialtools.database.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools.database module &mdash; serialtools v0.5.0 documentation</title>
+  <title>serialtools.database module &mdash; serialtools v0.6.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -34,15 +34,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.5.0
+                v0.6.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -100,30 +100,33 @@
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Endianness.LITTLE"><code class="docutils literal notranslate"><span class="pre">Endianness.LITTLE</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="#serialtools.database.Message"><code class="docutils literal notranslate"><span class="pre">Message</span></code></a><ul>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Message.decode"><code class="docutils literal notranslate"><span class="pre">Message.decode()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Message.format"><code class="docutils literal notranslate"><span class="pre">Message.format()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Message.format_raw"><code class="docutils literal notranslate"><span class="pre">Message.format_raw()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Message.format_raw_data"><code class="docutils literal notranslate"><span class="pre">Message.format_raw_data()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Message.format_timestamp"><code class="docutils literal notranslate"><span class="pre">Message.format_timestamp()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="#serialtools.database.MessageSpec"><code class="docutils literal notranslate"><span class="pre">MessageSpec</span></code></a><ul>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.MessageSpec.ADDRESS"><code class="docutils literal notranslate"><span class="pre">MessageSpec.ADDRESS</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="#serialtools.database.Reader"><code class="docutils literal notranslate"><span class="pre">Reader</span></code></a><ul>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Reader.ignore_bytes_between_messages"><code class="docutils literal notranslate"><span class="pre">Reader.ignore_bytes_between_messages</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Reader.read"><code class="docutils literal notranslate"><span class="pre">Reader.read()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Reader.read_byte"><code class="docutils literal notranslate"><span class="pre">Reader.read_byte()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Reader.read_in_other_thread"><code class="docutils literal notranslate"><span class="pre">Reader.read_in_other_thread()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Reader.read_msg"><code class="docutils literal notranslate"><span class="pre">Reader.read_msg()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Reader.read_n_bytes"><code class="docutils literal notranslate"><span class="pre">Reader.read_n_bytes()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Reader.retry_byte"><code class="docutils literal notranslate"><span class="pre">Reader.retry_byte()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Reader.send_msg"><code class="docutils literal notranslate"><span class="pre">Reader.send_msg()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Reader.stop"><code class="docutils literal notranslate"><span class="pre">Reader.stop()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Reader.timeout"><code class="docutils literal notranslate"><span class="pre">Reader.timeout</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="#serialtools.database.Signal"><code class="docutils literal notranslate"><span class="pre">Signal</span></code></a><ul>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Signal.get_bitstruct_fmt"><code class="docutils literal notranslate"><span class="pre">Signal.get_bitstruct_fmt()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Signal.init"><code class="docutils literal notranslate"><span class="pre">Signal.init()</span></code></a></li>
 </ul>
 </li>
@@ -282,14 +285,19 @@
 
 <dl class="py method">
 <dt class="sig sig-object py" id="serialtools.database.Message.format_raw">
 <span class="sig-name descname"><span class="pre">format_raw</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a></span></span><a class="headerlink" href="#serialtools.database.Message.format_raw" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
 
 <dl class="py method">
+<dt class="sig sig-object py" id="serialtools.database.Message.format_raw_data">
+<span class="sig-name descname"><span class="pre">format_raw_data</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a></span></span><a class="headerlink" href="#serialtools.database.Message.format_raw_data" title="Permalink to this definition"></a></dt>
+<dd></dd></dl>
+
+<dl class="py method">
 <dt class="sig sig-object py" id="serialtools.database.Message.format_timestamp">
 <span class="sig-name descname"><span class="pre">format_timestamp</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a></span></span><a class="headerlink" href="#serialtools.database.Message.format_timestamp" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
@@ -337,23 +345,36 @@
 
 <dl class="py method">
 <dt class="sig sig-object py" id="serialtools.database.Reader.read_n_bytes">
 <span class="sig-name descname"><span class="pre">read_n_bytes</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">n</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytes" title="(in Python v3.11)"><span class="pre">bytes</span></a></span></span><a class="headerlink" href="#serialtools.database.Reader.read_n_bytes" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
 
 <dl class="py method">
+<dt class="sig sig-object py" id="serialtools.database.Reader.retry_byte">
+<span class="sig-name descname"><span class="pre">retry_byte</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">b</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span></span><a class="headerlink" href="#serialtools.database.Reader.retry_byte" title="Permalink to this definition"></a></dt>
+<dd></dd></dl>
+
+<dl class="py method">
 <dt class="sig sig-object py" id="serialtools.database.Reader.send_msg">
 <span class="sig-name descname"><span class="pre">send_msg</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">msg</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="#serialtools.database.Message" title="serialtools.database.Message"><span class="pre">Message</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span></span><a class="headerlink" href="#serialtools.database.Reader.send_msg" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="serialtools.database.Reader.stop">
 <span class="sig-name descname"><span class="pre">stop</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span></span><a class="headerlink" href="#serialtools.database.Reader.stop" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
 
+<dl class="py attribute">
+<dt class="sig sig-object py" id="serialtools.database.Reader.timeout">
+<span class="sig-name descname"><span class="pre">timeout</span></span><a class="headerlink" href="#serialtools.database.Reader.timeout" title="Permalink to this definition"></a></dt>
+<dd><p>Each instance of this class represents a setting which can be changed in a config file.</p>
+<p>This class implements the <a class="reference external" href="https://docs.python.org/3/reference/datamodel.html#implementing-descriptors">descriptor protocol</a> to return <code class="xref py py-attr docutils literal notranslate"><span class="pre">value</span></code> if an instance of this class is accessed as an instance attribute.
+If you want to get this object you need to access it as a class attribute.</p>
+</dd></dl>
+
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="serialtools.database.Signal">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">serialtools.database.</span></span><span class="sig-name descname"><span class="pre">Signal</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">name</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">type</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="#serialtools.database.Type" title="serialtools.database.Type"><span class="pre">Type</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">address</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">bits</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">startbit</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">lsb</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">scale</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#float" title="(in Python v3.11)"><span class="pre">float</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">offset</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#float" title="(in Python v3.11)"><span class="pre">float</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">unit</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">''</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#serialtools.database.Signal" title="Permalink to this definition"></a></dt>
 <dd><p>Bases: <a class="reference external" href="https://docs.python.org/3/library/functions.html#object" title="(in Python v3.11)"><code class="xref py py-class docutils literal notranslate"><span class="pre">object</span></code></a></p>
 <dl class="field-list simple">
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 
 
 
 
 
 
 serialtools
-v0.5.0
+v0.6.0
 [q                   ]
     * serialtools_package
           o Subpackages
           o Submodules
                 # serialtools.bus_module
                 # serialtools.database_module
                       # ByteSpec
@@ -50,26 +50,29 @@
           o Endianness
                 # Endianness.BIG
                 # Endianness.LITTLE
           o Message
                 # Message.decode()
                 # Message.format()
                 # Message.format_raw()
+                # Message.format_raw_data()
                 # Message.format_timestamp()
           o MessageSpec
                 # MessageSpec.ADDRESS
           o Reader
                 # Reader.ignore_bytes_between_messages
                 # Reader.read()
                 # Reader.read_byte()
                 # Reader.read_in_other_thread()
                 # Reader.read_msg()
                 # Reader.read_n_bytes()
+                # Reader.retry_byte()
                 # Reader.send_msg()
                 # Reader.stop()
+                # Reader.timeout
           o Signal
                 # Signal.get_bitstruct_fmt()
                 # Signal.init()
           o Type
                 # Type.BOOL
                 # Type.FLOAT
                 # Type.INT
@@ -120,14 +123,15 @@
         LITTLE= 2ï
   classserialtools.database.Message(db: Database, timestamp: datetime | None,
   values: Mapping[str, bytes])ï
       Bases: object
         decode() &#x2192; Mapping[Signal, int | float | bool | str]ï
         format() &#x2192; strï
         format_raw() &#x2192; strï
+        format_raw_data() &#x2192; strï
         format_timestamp() &#x2192; strï
   classserialtools.database.MessageSpec(params: Sequence[ByteSpec], *,
   implicit_address: int | None = None)ï
       Bases: object
         ADDRESS= 'address'ï
   classserialtools.database.Reader(bus: serial.Serial | ReadFromFileBus |
   WriteToFileBus, db: Database)ï
@@ -140,16 +144,23 @@
             want to get this object you need to access it as a class attribute.
         read() &#x2192; Iterator[Message]ï
         read_byte() &#x2192; intï
         read_in_other_thread(callback: Callable[[Message], None]) &#x2192;
         Noneï
         read_msg() &#x2192; Message | Noneï
         read_n_bytes(n: int) &#x2192; bytesï
+        retry_byte(b: int) &#x2192; Noneï
         send_msg(msg: Message) &#x2192; Noneï
         stop() &#x2192; Noneï
+        timeoutï
+            Each instance of this class represents a setting which can be
+            changed in a config file.
+            This class implements the descriptor_protocol to return value if an
+            instance of this class is accessed as an instance attribute. If you
+            want to get this object you need to access it as a class attribute.
   classserialtools.database.Signal(name: str, type: Type, address: int, *,
   bits: int | None = None, startbit: int | None = None, lsb: int | None = None,
   scale: float = 1, offset: float = 0, unit: str = '')ï
       Bases: object
         Paramref name:
             The name of the signal
         Paramref type:
```

### Comparing `serialtools-0.5.0/docs/build/html/serialtools.database_config.html` & `serialtools-0.6.0/docs/build/html/serialtools.database_config.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools.database_config module &mdash; serialtools v0.5.0 documentation</title>
+  <title>serialtools.database_config module &mdash; serialtools v0.6.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -34,15 +34,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.5.0
+                v0.6.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 
 
 
 
 
 
 serialtools
-v0.5.0
+v0.6.0
 [q                   ]
     * serialtools_package
           o Subpackages
           o Submodules
                 # serialtools.bus_module
                 # serialtools.database_module
                 # serialtools.database_config_module
```

### Comparing `serialtools-0.5.0/docs/build/html/serialtools.html` & `serialtools-0.6.0/docs/build/html/serialtools.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools package &mdash; serialtools v0.5.0 documentation</title>
+  <title>serialtools package &mdash; serialtools v0.6.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -34,15 +34,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.5.0
+                v0.6.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -205,30 +205,33 @@
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Endianness.LITTLE"><code class="docutils literal notranslate"><span class="pre">Endianness.LITTLE</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.database.html#serialtools.database.Message"><code class="docutils literal notranslate"><span class="pre">Message</span></code></a><ul>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Message.decode"><code class="docutils literal notranslate"><span class="pre">Message.decode()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Message.format"><code class="docutils literal notranslate"><span class="pre">Message.format()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Message.format_raw"><code class="docutils literal notranslate"><span class="pre">Message.format_raw()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Message.format_raw_data"><code class="docutils literal notranslate"><span class="pre">Message.format_raw_data()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Message.format_timestamp"><code class="docutils literal notranslate"><span class="pre">Message.format_timestamp()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.database.html#serialtools.database.MessageSpec"><code class="docutils literal notranslate"><span class="pre">MessageSpec</span></code></a><ul>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.MessageSpec.ADDRESS"><code class="docutils literal notranslate"><span class="pre">MessageSpec.ADDRESS</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.database.html#serialtools.database.Reader"><code class="docutils literal notranslate"><span class="pre">Reader</span></code></a><ul>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Reader.ignore_bytes_between_messages"><code class="docutils literal notranslate"><span class="pre">Reader.ignore_bytes_between_messages</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Reader.read"><code class="docutils literal notranslate"><span class="pre">Reader.read()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Reader.read_byte"><code class="docutils literal notranslate"><span class="pre">Reader.read_byte()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Reader.read_in_other_thread"><code class="docutils literal notranslate"><span class="pre">Reader.read_in_other_thread()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Reader.read_msg"><code class="docutils literal notranslate"><span class="pre">Reader.read_msg()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Reader.read_n_bytes"><code class="docutils literal notranslate"><span class="pre">Reader.read_n_bytes()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Reader.retry_byte"><code class="docutils literal notranslate"><span class="pre">Reader.retry_byte()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Reader.send_msg"><code class="docutils literal notranslate"><span class="pre">Reader.send_msg()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Reader.stop"><code class="docutils literal notranslate"><span class="pre">Reader.stop()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Reader.timeout"><code class="docutils literal notranslate"><span class="pre">Reader.timeout</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.database.html#serialtools.database.Signal"><code class="docutils literal notranslate"><span class="pre">Signal</span></code></a><ul>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Signal.get_bitstruct_fmt"><code class="docutils literal notranslate"><span class="pre">Signal.get_bitstruct_fmt()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Signal.init"><code class="docutils literal notranslate"><span class="pre">Signal.init()</span></code></a></li>
 </ul>
 </li>
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 
 
 
 
 
 
 serialtools
-v0.5.0
+v0.6.0
 [q                   ]
     * serialtools_package
           o Subpackages
                 # serialtools.apps_package
           o Submodules
                 # serialtools.bus_module
                 # serialtools.database_module
@@ -104,26 +104,29 @@
           o Endianness
                 # Endianness.BIG
                 # Endianness.LITTLE
           o Message
                 # Message.decode()
                 # Message.format()
                 # Message.format_raw()
+                # Message.format_raw_data()
                 # Message.format_timestamp()
           o MessageSpec
                 # MessageSpec.ADDRESS
           o Reader
                 # Reader.ignore_bytes_between_messages
                 # Reader.read()
                 # Reader.read_byte()
                 # Reader.read_in_other_thread()
                 # Reader.read_msg()
                 # Reader.read_n_bytes()
+                # Reader.retry_byte()
                 # Reader.send_msg()
                 # Reader.stop()
+                # Reader.timeout
           o Signal
                 # Signal.get_bitstruct_fmt()
                 # Signal.init()
           o Type
                 # Type.BOOL
                 # Type.FLOAT
                 # Type.INT
```

### Comparing `serialtools-0.5.0/docs/make.bat` & `serialtools-0.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `serialtools-0.5.0/docs/source/conf.py` & `serialtools-0.6.0/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'serialtools'
 copyright = '2023, erzo'
 author = 'erzo'
-release = 'v0.5.0'
+release = 'v0.6.0'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ['sphinx.ext.autodoc', 'sphinx.ext.intersphinx', 'sphinx_paramlinks']
 
 templates_path = ['_templates']
```

### Comparing `serialtools-0.5.0/docs/source/index.rst` & `serialtools-0.6.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `serialtools-0.5.0/prepare_for_gitlab_pages.py` & `serialtools-0.6.0/prepare_for_gitlab_pages.py`

 * *Files identical despite different names*

### Comparing `serialtools-0.5.0/pyproject.toml` & `serialtools-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `serialtools-0.5.0/release.sh` & `serialtools-0.6.0/release.sh`

 * *Files identical despite different names*

### Comparing `serialtools-0.5.0/src/serialtools/__main__.py` & `serialtools-0.6.0/src/serialtools/__main__.py`

 * *Files identical despite different names*

### Comparing `serialtools-0.5.0/src/serialtools/apps/decode.py` & `serialtools-0.6.0/src/serialtools/apps/decode.py`

 * *Files identical despite different names*

### Comparing `serialtools-0.5.0/src/serialtools/apps/dump.py` & `serialtools-0.6.0/src/serialtools/apps/dump.py`

 * *Files identical despite different names*

### Comparing `serialtools-0.5.0/src/serialtools/apps/rawsplit.py` & `serialtools-0.6.0/src/serialtools/apps/rawsplit.py`

 * *Files identical despite different names*

### Comparing `serialtools-0.5.0/src/serialtools/apps/send.py` & `serialtools-0.6.0/src/serialtools/apps/send.py`

 * *Files identical despite different names*

### Comparing `serialtools-0.5.0/src/serialtools/bus.py` & `serialtools-0.6.0/src/serialtools/bus.py`

 * *Files identical despite different names*

### Comparing `serialtools-0.5.0/src/serialtools/database.py` & `serialtools-0.6.0/src/serialtools/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,20 +102,23 @@
 		self.values = values
 
 	def format_timestamp(self) -> str:
 		if self.timestamp is None:
 			return ''
 		return self.timestamp.strftime('%H:%M:%S.%f')
 
+	def format_raw_data(self) -> str:
+		return ' '.join(format_bytes(b) for b in self.values.values())
+
 	def format_raw(self) -> str:
 		timestamp = self.format_timestamp()
 		if timestamp:
 			timestamp += ' '
 
-		values = ' '.join(format_bytes(b) for b in self.values.values())
+		values = self.format_raw_data()
 		return timestamp + values
 
 	def decode(self) -> 'Mapping[Signal, int|float|bool|str]':
 		if 'address' in self.values:
 			address, = self.values['address']
 		else:
 			implicit_address = self.db.message_spec.implicit_address
@@ -128,23 +131,31 @@
 
 	def format(self) -> str:
 		out = self.format_raw()
 		for sig, val in self.decode().items():
 			out += f"\n\t{sig.name}: {val}{sig.unit}"
 		return out
 
+	def __str__(self) -> str:
+		return self.format_raw()
+
 
 class Reader:
 
 	ignore_bytes_between_messages = Config('reader.ignore-bytes-between-messages', [0xFF], unit='', help="If these bytes are encountered between two messages they are ignored instead of printing an error.")
+	timeout = Config('reader.timeout', 100, unit='ms', help="If nothing is received for this time span the message is considered to be incomplete")
 
 	def __init__(self, bus: Bus, db: 'Database') -> None:
 		self._stopped = False
 		self.bus = bus
 		self.db = db
+		self._retry_byte: 'int|None' = None
+
+	def retry_byte(self, b: int) -> None:
+		self._retry_byte = b
 
 	def read_in_other_thread(self, callback: 'Callable[[Message], None]') -> None:
 		threading.Thread(target=self._read_in_other_thread, args=(callback,)).start()
 
 	def _read_in_other_thread(self, callback: 'Callable[[Message], None]') -> None:
 		for msg in self.read():
 			callback(msg)
@@ -161,32 +172,40 @@
 					logger.error(str(e))
 		except EOFError:
 			pass
 
 	def read_msg(self) -> 'Message|None':
 		values: 'dict[str, bytes]' = {}
 		first_byte = True
+		timeout = self.timeout / 1000
 		for spec in self.db.message_spec:
 			val = []
 			for i in range(spec.get_length(values)):
 				allowed_values = spec.allowed_values
 				while True:
+					t0 = get_timestamp(self.bus)
 					read_byte = self.read_n_bytes(1)
 					if not read_byte:
 						if first_byte:
 							return None
 						raise ValueError(f"Bus closed before message was complete")
 					b, = read_byte
+					t1 = get_timestamp(self.bus)
+					if not first_byte and t0 is not None and t1 is not None:
+						dt = (t1 - t0).total_seconds()
+						if timeout >= 0 and dt > timeout:
+							self.retry_byte(b)
+							raise ValueError(f"[{t0}] Timeout, {dt*1000:1.0f}ms have passed since receiving the last byte so I don't think this one belongs to the same message.")
 
 					if allowed_values is not None:
 						allowed_values = [val for val in allowed_values if val[i]==b]
 						if not allowed_values:
 							if first_byte and b in self.ignore_bytes_between_messages:
 								continue
-							raise ValueError(f"Received unexpected value for byte {i} of {spec.name}: {b:02x}, should be {spec.format_allowed_values()}")
+							raise ValueError(f"[{t0}] Received unexpected value for byte {i} of {spec.name}: {b:02x}, should be {spec.format_allowed_values()}")
 					break
 				val.append(b)
 				first_byte = False
 			values[spec.name] = bytes(val)
 
 		return Message(self.db, values=values, timestamp=get_timestamp(self.bus))
 
@@ -210,15 +229,22 @@
 		assert len(out) == 1
 		b = out[0]
 		return b
 
 	def read_n_bytes(self, n: int) -> bytes:
 		if self._stopped:
 			raise EOFError
-		out = typing.cast(bytes, self.bus.read(n))
+		if self._retry_byte:
+			out = bytes([self._retry_byte])
+			self._retry_byte = None
+			if n == 1:
+				return out
+			out += self.bus.read(n)
+		else:
+			out = self.bus.read(n)
 		if self._stopped:
 			raise EOFError
 		return out
 
 	def stop(self) -> None:
 		self._stopped = True
 		self.bus.cancel_read()
```

### Comparing `serialtools-0.5.0/src/serialtools/database_config.py` & `serialtools-0.6.0/src/serialtools/database_config.py`

 * *Files identical despite different names*

### Comparing `serialtools-0.5.0/PKG-INFO` & `serialtools-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serialtools
-Version: 0.5.0
+Version: 0.6.0
 Summary: Tools to work with a serial bus
 Author-email: erzo <erzo@posteo.de>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
```

