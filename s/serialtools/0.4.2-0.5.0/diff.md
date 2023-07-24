# Comparing `tmp/serialtools-0.4.2.tar.gz` & `tmp/serialtools-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serialtools-0.4.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "serialtools-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `serialtools-0.4.2.tar` & `serialtools-0.5.0.tar`

### file list

```diff
@@ -1,104 +1,104 @@
--rw-r--r--   0        0        0      330 2023-06-02 06:55:40.811546 serialtools-0.4.2/.gitignore
--rw-r--r--   0        0        0      119 2023-06-21 10:33:17.761717 serialtools-0.4.2/.gitlab-ci.yml
--rw-r--r--   0        0        0      657 2023-06-21 08:53:39.687960 serialtools-0.4.2/LICENSE
--rw-r--r--   0        0        0      444 2023-06-21 10:33:17.761717 serialtools-0.4.2/README.md
--rw-r--r--   0        0        0      638 2023-06-21 10:33:17.761717 serialtools-0.4.2/docs/Makefile
--rw-r--r--   0        0        0     1014 2023-06-26 12:52:04.102651 serialtools-0.4.2/docs/build/html/_sources/index.rst.txt
--rw-r--r--   0        0        0       70 2023-06-21 10:33:17.761717 serialtools-0.4.2/docs/build/html/_sources/modules.rst.txt
--rw-r--r--   0        0        0      157 2023-06-21 10:33:17.761717 serialtools-0.4.2/docs/build/html/_sources/serialtools.apps.decode.rst.txt
--rw-r--r--   0        0        0      151 2023-06-21 10:33:17.761717 serialtools-0.4.2/docs/build/html/_sources/serialtools.apps.dump.rst.txt
--rw-r--r--   0        0        0      163 2023-06-26 12:52:04.102651 serialtools-0.4.2/docs/build/html/_sources/serialtools.apps.rawsplit.rst.txt
--rw-r--r--   0        0        0      302 2023-06-21 10:33:17.761717 serialtools-0.4.2/docs/build/html/_sources/serialtools.apps.rst.txt
--rw-r--r--   0        0        0      151 2023-06-21 10:33:17.761717 serialtools-0.4.2/docs/build/html/_sources/serialtools.apps.send.rst.txt
--rw-r--r--   0        0        0      133 2023-06-21 10:33:17.761717 serialtools-0.4.2/docs/build/html/_sources/serialtools.bus.rst.txt
--rw-r--r--   0        0        0      148 2023-06-21 10:33:17.761717 serialtools-0.4.2/docs/build/html/_sources/serialtools.database.rst.txt
--rw-r--r--   0        0        0      171 2023-06-21 10:33:17.761717 serialtools-0.4.2/docs/build/html/_sources/serialtools.database_config.rst.txt
--rw-r--r--   0        0        0      360 2023-06-21 10:33:17.765050 serialtools-0.4.2/docs/build/html/_sources/serialtools.rst.txt
--rw-r--r--   0        0        0     4289 2023-07-18 10:22:40.597240 serialtools-0.4.2/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0        0        0    14813 2023-07-18 10:22:42.037230 serialtools-0.4.2/docs/build/html/_static/basic.css
--rw-r--r--   0        0        0     3229 2023-06-21 10:33:17.765050 serialtools-0.4.2/docs/build/html/_static/css/badge_only.css
--rw-r--r--   0        0        0    87624 2023-06-21 10:33:17.765050 serialtools-0.4.2/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0        0        0    67312 2023-06-21 10:33:17.765050 serialtools-0.4.2/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0        0        0    86288 2023-06-21 10:33:17.765050 serialtools-0.4.2/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0        0        0    66444 2023-06-21 10:33:17.765050 serialtools-0.4.2/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0        0        0   165742 2023-06-21 10:33:17.765050 serialtools-0.4.2/docs/build/html/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0        0        0   444379 2023-06-21 10:33:17.768383 serialtools-0.4.2/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0        0        0   165548 2023-06-21 10:33:17.771717 serialtools-0.4.2/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0        0        0    98024 2023-06-21 10:33:17.771717 serialtools-0.4.2/docs/build/html/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0        0        0    77160 2023-06-21 10:33:17.771717 serialtools-0.4.2/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0        0        0   323344 2023-06-21 10:33:17.771717 serialtools-0.4.2/docs/build/html/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0        0        0   193308 2023-06-21 10:33:17.775050 serialtools-0.4.2/docs/build/html/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0        0        0   309728 2023-06-21 10:33:17.775050 serialtools-0.4.2/docs/build/html/_static/css/fonts/lato-bold.woff
--rw-r--r--   0        0        0   184912 2023-06-21 10:33:17.775050 serialtools-0.4.2/docs/build/html/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0        0        0   328412 2023-06-21 10:33:17.778383 serialtools-0.4.2/docs/build/html/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0        0        0   195704 2023-06-21 10:33:17.778383 serialtools-0.4.2/docs/build/html/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0        0        0   309192 2023-06-21 10:33:17.778383 serialtools-0.4.2/docs/build/html/_static/css/fonts/lato-normal.woff
--rw-r--r--   0        0        0   182708 2023-06-21 10:33:17.778383 serialtools-0.4.2/docs/build/html/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0        0        0   135314 2023-06-21 10:33:17.781717 serialtools-0.4.2/docs/build/html/_static/css/theme.css
--rw-r--r--   0        0        0     4472 2023-06-21 10:33:17.781717 serialtools-0.4.2/docs/build/html/_static/doctools.js
--rw-r--r--   0        0        0      421 2023-07-18 10:23:12.383677 serialtools-0.4.2/docs/build/html/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2023-06-21 10:33:17.781717 serialtools-0.4.2/docs/build/html/_static/file.png
--rw-r--r--   0        0        0    89501 2023-07-18 10:22:40.597240 serialtools-0.4.2/docs/build/html/_static/jquery.js
--rw-r--r--   0        0        0      934 2023-06-21 10:33:17.781717 serialtools-0.4.2/docs/build/html/_static/js/badge_only.js
--rw-r--r--   0        0        0     4370 2023-06-21 10:33:17.781717 serialtools-0.4.2/docs/build/html/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0        0        0     2734 2023-06-21 10:33:17.781717 serialtools-0.4.2/docs/build/html/_static/js/html5shiv.min.js
--rw-r--r--   0        0        0     5023 2023-06-21 10:33:17.781717 serialtools-0.4.2/docs/build/html/_static/js/theme.js
--rw-r--r--   0        0        0     4758 2023-07-18 10:22:42.040563 serialtools-0.4.2/docs/build/html/_static/language_data.js
--rw-r--r--   0        0        0       90 2023-06-21 10:33:17.781717 serialtools-0.4.2/docs/build/html/_static/minus.png
--rw-r--r--   0        0        0       46 2023-06-21 10:33:17.781717 serialtools-0.4.2/docs/build/html/_static/no-ligatures-in-code.css
--rw-r--r--   0        0        0       90 2023-06-21 10:33:17.781717 serialtools-0.4.2/docs/build/html/_static/plus.png
--rw-r--r--   0        0        0     4819 2023-07-18 10:22:42.033896 serialtools-0.4.2/docs/build/html/_static/pygments.css
--rw-r--r--   0        0        0    18215 2023-06-21 10:33:17.781717 serialtools-0.4.2/docs/build/html/_static/searchtools.js
--rw-r--r--   0        0        0     4712 2023-06-21 10:33:17.781717 serialtools-0.4.2/docs/build/html/_static/sphinx_highlight.js
--rw-r--r--   0        0        0      204 2023-06-21 10:33:17.781717 serialtools-0.4.2/docs/build/html/_static/sphinx_paramlinks.css
--rw-r--r--   0        0        0      117 2023-06-21 10:33:17.781717 serialtools-0.4.2/docs/build/html/_static/tab-size.css
--rw-r--r--   0        0        0    28591 2023-07-18 10:23:12.383677 serialtools-0.4.2/docs/build/html/genindex.html
--rw-r--r--   0        0        0    15924 2023-07-18 10:23:12.383677 serialtools-0.4.2/docs/build/html/index.html
--rw-r--r--   0        0        0    10612 2023-07-18 10:23:12.383677 serialtools-0.4.2/docs/build/html/modules.html
--rw-r--r--   0        0        0     1348 2023-07-18 10:22:42.050563 serialtools-0.4.2/docs/build/html/objects.inv
--rw-r--r--   0        0        0     6959 2023-07-18 10:23:12.383677 serialtools-0.4.2/docs/build/html/py-modindex.html
--rw-r--r--   0        0        0     4930 2023-07-18 10:23:12.383677 serialtools-0.4.2/docs/build/html/search.html
--rw-r--r--   0        0        0    24908 2023-07-18 10:22:42.050563 serialtools-0.4.2/docs/build/html/searchindex.js
--rw-r--r--   0        0        0    14727 2023-07-18 10:23:12.383677 serialtools-0.4.2/docs/build/html/serialtools.apps.decode.html
--rw-r--r--   0        0        0    12315 2023-07-18 10:23:12.383677 serialtools-0.4.2/docs/build/html/serialtools.apps.dump.html
--rw-r--r--   0        0        0    10619 2023-07-18 10:23:12.383677 serialtools-0.4.2/docs/build/html/serialtools.apps.html
--rw-r--r--   0        0        0    13490 2023-07-18 10:23:12.387011 serialtools-0.4.2/docs/build/html/serialtools.apps.rawsplit.html
--rw-r--r--   0        0        0    10817 2023-07-18 10:23:12.387011 serialtools-0.4.2/docs/build/html/serialtools.apps.send.html
--rw-r--r--   0        0        0    48292 2023-07-18 10:23:12.387011 serialtools-0.4.2/docs/build/html/serialtools.bus.html
--rw-r--r--   0        0        0    74268 2023-07-18 10:23:12.387011 serialtools-0.4.2/docs/build/html/serialtools.database.html
--rw-r--r--   0        0        0    34482 2023-07-18 10:23:12.387011 serialtools-0.4.2/docs/build/html/serialtools.database_config.html
--rw-r--r--   0        0        0    32348 2023-07-18 10:23:12.387011 serialtools-0.4.2/docs/build/html/serialtools.html
--rw-r--r--   0        0        0      804 2023-06-21 10:33:17.785050 serialtools-0.4.2/docs/make.bat
--rw-r--r--   0        0        0       46 2023-06-21 10:33:17.785050 serialtools-0.4.2/docs/source/_static/no-ligatures-in-code.css
--rw-r--r--   0        0        0      117 2023-06-21 10:33:17.785050 serialtools-0.4.2/docs/source/_static/tab-size.css
--rw-r--r--   0        0        0     3095 2023-07-18 10:23:12.387011 serialtools-0.4.2/docs/source/conf.py
--rw-r--r--   0        0        0     1014 2023-07-18 10:22:39.730580 serialtools-0.4.2/docs/source/index.rst
--rw-r--r--   0        0        0       70 2023-07-18 10:22:39.670580 serialtools-0.4.2/docs/source/modules.rst
--rw-r--r--   0        0        0      157 2023-07-18 10:22:39.670580 serialtools-0.4.2/docs/source/serialtools.apps.decode.rst
--rw-r--r--   0        0        0      151 2023-07-18 10:22:39.670580 serialtools-0.4.2/docs/source/serialtools.apps.dump.rst
--rw-r--r--   0        0        0      163 2023-07-18 10:22:39.670580 serialtools-0.4.2/docs/source/serialtools.apps.rawsplit.rst
--rw-r--r--   0        0        0      302 2023-07-18 10:22:39.670580 serialtools-0.4.2/docs/source/serialtools.apps.rst
--rw-r--r--   0        0        0      151 2023-07-18 10:22:39.670580 serialtools-0.4.2/docs/source/serialtools.apps.send.rst
--rw-r--r--   0        0        0      133 2023-07-18 10:22:39.670580 serialtools-0.4.2/docs/source/serialtools.bus.rst
--rw-r--r--   0        0        0      148 2023-07-18 10:22:39.670580 serialtools-0.4.2/docs/source/serialtools.database.rst
--rw-r--r--   0        0        0      171 2023-07-18 10:22:39.670580 serialtools-0.4.2/docs/source/serialtools.database_config.rst
--rw-r--r--   0        0        0      360 2023-07-18 10:22:39.670580 serialtools-0.4.2/docs/source/serialtools.rst
--rw-r--r--   0        0        0      170 2023-06-23 15:21:45.869968 serialtools-0.4.2/mypy.ini
--rw-r--r--   0        0        0     4135 2023-06-21 10:33:17.785050 serialtools-0.4.2/prepare_for_gitlab_pages.py
--rw-r--r--   0        0        0      786 2023-06-23 15:21:45.869968 serialtools-0.4.2/pyproject.toml
--rwxr-xr-x   0        0        0    12230 2023-06-21 10:33:17.785050 serialtools-0.4.2/release.sh
--rw-r--r--   0        0        0       83 2023-06-21 10:33:17.785050 serialtools-0.4.2/requirements-release.txt
--rw-r--r--   0        0        0       22 2023-06-21 10:33:17.785050 serialtools-0.4.2/requirements-test.txt
--rw-r--r--   0        0        0       87 2023-07-18 10:23:12.387011 serialtools-0.4.2/src/serialtools/__init__.py
--rw-r--r--   0        0        0     1448 2023-07-18 10:22:39.667247 serialtools-0.4.2/src/serialtools/__main__.py
--rw-r--r--   0        0        0      345 2023-07-18 10:22:39.667247 serialtools-0.4.2/src/serialtools/apps/__init__.py
--rw-r--r--   0        0        0     1143 2023-07-18 10:22:39.670580 serialtools-0.4.2/src/serialtools/apps/decode.py
--rw-r--r--   0        0        0     1386 2023-07-18 10:23:12.387011 serialtools-0.4.2/src/serialtools/apps/dump.py
--rw-r--r--   0        0        0     1369 2023-07-18 10:22:39.667247 serialtools-0.4.2/src/serialtools/apps/rawsplit.py
--rw-r--r--   0        0        0      880 2023-07-18 10:22:39.667247 serialtools-0.4.2/src/serialtools/apps/send.py
--rw-r--r--   0        0        0     7356 2023-07-18 10:22:39.663913 serialtools-0.4.2/src/serialtools/bus.py
--rw-r--r--   0        0        0    15004 2023-07-18 10:22:39.663913 serialtools-0.4.2/src/serialtools/database.py
--rw-r--r--   0        0        0     5481 2023-07-18 10:22:39.663913 serialtools-0.4.2/src/serialtools/database_config.py
--rw-r--r--   0        0        0        0 2022-11-03 16:33:53.710006 serialtools-0.4.2/src/serialtools/py.typed
--rw-r--r--   0        0        0      336 2023-06-23 15:21:45.869968 serialtools-0.4.2/tox.ini
--rw-r--r--   0        0        0     1156 1970-01-01 00:00:00.000000 serialtools-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      330 2023-06-02 06:55:40.811546 serialtools-0.5.0/.gitignore
+-rw-r--r--   0        0        0      119 2023-06-21 10:33:17.761717 serialtools-0.5.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0      657 2023-06-21 08:53:39.687960 serialtools-0.5.0/LICENSE
+-rw-r--r--   0        0        0      444 2023-06-21 10:33:17.761717 serialtools-0.5.0/README.md
+-rw-r--r--   0        0        0      638 2023-06-21 10:33:17.761717 serialtools-0.5.0/docs/Makefile
+-rw-r--r--   0        0        0     1014 2023-06-26 12:52:04.102651 serialtools-0.5.0/docs/build/html/_sources/index.rst.txt
+-rw-r--r--   0        0        0       70 2023-06-21 10:33:17.761717 serialtools-0.5.0/docs/build/html/_sources/modules.rst.txt
+-rw-r--r--   0        0        0      157 2023-06-21 10:33:17.761717 serialtools-0.5.0/docs/build/html/_sources/serialtools.apps.decode.rst.txt
+-rw-r--r--   0        0        0      151 2023-06-21 10:33:17.761717 serialtools-0.5.0/docs/build/html/_sources/serialtools.apps.dump.rst.txt
+-rw-r--r--   0        0        0      163 2023-06-26 12:52:04.102651 serialtools-0.5.0/docs/build/html/_sources/serialtools.apps.rawsplit.rst.txt
+-rw-r--r--   0        0        0      302 2023-06-21 10:33:17.761717 serialtools-0.5.0/docs/build/html/_sources/serialtools.apps.rst.txt
+-rw-r--r--   0        0        0      151 2023-06-21 10:33:17.761717 serialtools-0.5.0/docs/build/html/_sources/serialtools.apps.send.rst.txt
+-rw-r--r--   0        0        0      133 2023-06-21 10:33:17.761717 serialtools-0.5.0/docs/build/html/_sources/serialtools.bus.rst.txt
+-rw-r--r--   0        0        0      148 2023-06-21 10:33:17.761717 serialtools-0.5.0/docs/build/html/_sources/serialtools.database.rst.txt
+-rw-r--r--   0        0        0      171 2023-06-21 10:33:17.761717 serialtools-0.5.0/docs/build/html/_sources/serialtools.database_config.rst.txt
+-rw-r--r--   0        0        0      360 2023-06-21 10:33:17.765050 serialtools-0.5.0/docs/build/html/_sources/serialtools.rst.txt
+-rw-r--r--   0        0        0     4289 2023-07-24 09:29:30.775804 serialtools-0.5.0/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0        0        0    14813 2023-07-24 09:29:32.512455 serialtools-0.5.0/docs/build/html/_static/basic.css
+-rw-r--r--   0        0        0     3229 2023-06-21 10:33:17.765050 serialtools-0.5.0/docs/build/html/_static/css/badge_only.css
+-rw-r--r--   0        0        0    87624 2023-06-21 10:33:17.765050 serialtools-0.5.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0        0        0    67312 2023-06-21 10:33:17.765050 serialtools-0.5.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0        0        0    86288 2023-06-21 10:33:17.765050 serialtools-0.5.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0        0        0    66444 2023-06-21 10:33:17.765050 serialtools-0.5.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0        0        0   165742 2023-06-21 10:33:17.765050 serialtools-0.5.0/docs/build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0        0        0   444379 2023-06-21 10:33:17.768383 serialtools-0.5.0/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0        0        0   165548 2023-06-21 10:33:17.771717 serialtools-0.5.0/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0        0        0    98024 2023-06-21 10:33:17.771717 serialtools-0.5.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0        0        0    77160 2023-06-21 10:33:17.771717 serialtools-0.5.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0        0        0   323344 2023-06-21 10:33:17.771717 serialtools-0.5.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0        0        0   193308 2023-06-21 10:33:17.775050 serialtools-0.5.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0        0        0   309728 2023-06-21 10:33:17.775050 serialtools-0.5.0/docs/build/html/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0        0        0   184912 2023-06-21 10:33:17.775050 serialtools-0.5.0/docs/build/html/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0        0        0   328412 2023-06-21 10:33:17.778383 serialtools-0.5.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0        0        0   195704 2023-06-21 10:33:17.778383 serialtools-0.5.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0        0        0   309192 2023-06-21 10:33:17.778383 serialtools-0.5.0/docs/build/html/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0        0        0   182708 2023-06-21 10:33:17.778383 serialtools-0.5.0/docs/build/html/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0        0        0   135314 2023-06-21 10:33:17.781717 serialtools-0.5.0/docs/build/html/_static/css/theme.css
+-rw-r--r--   0        0        0     4472 2023-06-21 10:33:17.781717 serialtools-0.5.0/docs/build/html/_static/doctools.js
+-rw-r--r--   0        0        0      421 2023-07-24 09:30:04.135508 serialtools-0.5.0/docs/build/html/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2023-06-21 10:33:17.781717 serialtools-0.5.0/docs/build/html/_static/file.png
+-rw-r--r--   0        0        0    89501 2023-07-24 09:29:30.775804 serialtools-0.5.0/docs/build/html/_static/jquery.js
+-rw-r--r--   0        0        0      934 2023-06-21 10:33:17.781717 serialtools-0.5.0/docs/build/html/_static/js/badge_only.js
+-rw-r--r--   0        0        0     4370 2023-06-21 10:33:17.781717 serialtools-0.5.0/docs/build/html/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0        0        0     2734 2023-06-21 10:33:17.781717 serialtools-0.5.0/docs/build/html/_static/js/html5shiv.min.js
+-rw-r--r--   0        0        0     5023 2023-06-21 10:33:17.781717 serialtools-0.5.0/docs/build/html/_static/js/theme.js
+-rw-r--r--   0        0        0     4758 2023-07-24 09:29:32.512455 serialtools-0.5.0/docs/build/html/_static/language_data.js
+-rw-r--r--   0        0        0       90 2023-06-21 10:33:17.781717 serialtools-0.5.0/docs/build/html/_static/minus.png
+-rw-r--r--   0        0        0       46 2023-06-21 10:33:17.781717 serialtools-0.5.0/docs/build/html/_static/no-ligatures-in-code.css
+-rw-r--r--   0        0        0       90 2023-06-21 10:33:17.781717 serialtools-0.5.0/docs/build/html/_static/plus.png
+-rw-r--r--   0        0        0     4819 2023-07-24 09:29:32.505788 serialtools-0.5.0/docs/build/html/_static/pygments.css
+-rw-r--r--   0        0        0    18215 2023-06-21 10:33:17.781717 serialtools-0.5.0/docs/build/html/_static/searchtools.js
+-rw-r--r--   0        0        0     4712 2023-06-21 10:33:17.781717 serialtools-0.5.0/docs/build/html/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0      204 2023-06-21 10:33:17.781717 serialtools-0.5.0/docs/build/html/_static/sphinx_paramlinks.css
+-rw-r--r--   0        0        0      117 2023-06-21 10:33:17.781717 serialtools-0.5.0/docs/build/html/_static/tab-size.css
+-rw-r--r--   0        0        0    29298 2023-07-24 09:30:04.135508 serialtools-0.5.0/docs/build/html/genindex.html
+-rw-r--r--   0        0        0    16388 2023-07-24 09:30:04.135508 serialtools-0.5.0/docs/build/html/index.html
+-rw-r--r--   0        0        0    11076 2023-07-24 09:30:04.135508 serialtools-0.5.0/docs/build/html/modules.html
+-rw-r--r--   0        0        0     1381 2023-07-24 09:30:04.135508 serialtools-0.5.0/docs/build/html/objects.inv
+-rw-r--r--   0        0        0     6959 2023-07-24 09:30:04.135508 serialtools-0.5.0/docs/build/html/py-modindex.html
+-rw-r--r--   0        0        0     4930 2023-07-24 09:30:04.135508 serialtools-0.5.0/docs/build/html/search.html
+-rw-r--r--   0        0        0    25673 2023-07-24 09:30:04.135508 serialtools-0.5.0/docs/build/html/searchindex.js
+-rw-r--r--   0        0        0    14727 2023-07-24 09:30:04.135508 serialtools-0.5.0/docs/build/html/serialtools.apps.decode.html
+-rw-r--r--   0        0        0    12315 2023-07-24 09:30:04.135508 serialtools-0.5.0/docs/build/html/serialtools.apps.dump.html
+-rw-r--r--   0        0        0    10619 2023-07-24 09:30:04.135508 serialtools-0.5.0/docs/build/html/serialtools.apps.html
+-rw-r--r--   0        0        0    13490 2023-07-24 09:30:04.135508 serialtools-0.5.0/docs/build/html/serialtools.apps.rawsplit.html
+-rw-r--r--   0        0        0    10817 2023-07-24 09:30:04.138841 serialtools-0.5.0/docs/build/html/serialtools.apps.send.html
+-rw-r--r--   0        0        0    48784 2023-07-24 09:30:04.138841 serialtools-0.5.0/docs/build/html/serialtools.bus.html
+-rw-r--r--   0        0        0    76321 2023-07-24 09:30:04.138841 serialtools-0.5.0/docs/build/html/serialtools.database.html
+-rw-r--r--   0        0        0    39042 2023-07-24 09:30:04.138841 serialtools-0.5.0/docs/build/html/serialtools.database_config.html
+-rw-r--r--   0        0        0    33294 2023-07-24 09:30:04.138841 serialtools-0.5.0/docs/build/html/serialtools.html
+-rw-r--r--   0        0        0      804 2023-06-21 10:33:17.785050 serialtools-0.5.0/docs/make.bat
+-rw-r--r--   0        0        0       46 2023-06-21 10:33:17.785050 serialtools-0.5.0/docs/source/_static/no-ligatures-in-code.css
+-rw-r--r--   0        0        0      117 2023-06-21 10:33:17.785050 serialtools-0.5.0/docs/source/_static/tab-size.css
+-rw-r--r--   0        0        0     3095 2023-07-24 09:30:04.138841 serialtools-0.5.0/docs/source/conf.py
+-rw-r--r--   0        0        0     1014 2023-07-24 09:29:29.629147 serialtools-0.5.0/docs/source/index.rst
+-rw-r--r--   0        0        0       70 2023-07-24 09:29:29.555815 serialtools-0.5.0/docs/source/modules.rst
+-rw-r--r--   0        0        0      157 2023-07-24 09:29:29.555815 serialtools-0.5.0/docs/source/serialtools.apps.decode.rst
+-rw-r--r--   0        0        0      151 2023-07-24 09:29:29.559148 serialtools-0.5.0/docs/source/serialtools.apps.dump.rst
+-rw-r--r--   0        0        0      163 2023-07-24 09:29:29.555815 serialtools-0.5.0/docs/source/serialtools.apps.rawsplit.rst
+-rw-r--r--   0        0        0      302 2023-07-24 09:29:29.555815 serialtools-0.5.0/docs/source/serialtools.apps.rst
+-rw-r--r--   0        0        0      151 2023-07-24 09:29:29.555815 serialtools-0.5.0/docs/source/serialtools.apps.send.rst
+-rw-r--r--   0        0        0      133 2023-07-24 09:29:29.559148 serialtools-0.5.0/docs/source/serialtools.bus.rst
+-rw-r--r--   0        0        0      148 2023-07-24 09:29:29.559148 serialtools-0.5.0/docs/source/serialtools.database.rst
+-rw-r--r--   0        0        0      171 2023-07-24 09:29:29.555815 serialtools-0.5.0/docs/source/serialtools.database_config.rst
+-rw-r--r--   0        0        0      360 2023-07-24 09:29:29.555815 serialtools-0.5.0/docs/source/serialtools.rst
+-rw-r--r--   0        0        0      170 2023-06-23 15:21:45.869968 serialtools-0.5.0/mypy.ini
+-rw-r--r--   0        0        0     4135 2023-06-21 10:33:17.785050 serialtools-0.5.0/prepare_for_gitlab_pages.py
+-rw-r--r--   0        0        0      786 2023-06-23 15:21:45.869968 serialtools-0.5.0/pyproject.toml
+-rwxr-xr-x   0        0        0    12230 2023-06-21 10:33:17.785050 serialtools-0.5.0/release.sh
+-rw-r--r--   0        0        0       83 2023-06-21 10:33:17.785050 serialtools-0.5.0/requirements-release.txt
+-rw-r--r--   0        0        0       22 2023-06-21 10:33:17.785050 serialtools-0.5.0/requirements-test.txt
+-rw-r--r--   0        0        0       87 2023-07-24 09:30:04.138841 serialtools-0.5.0/src/serialtools/__init__.py
+-rw-r--r--   0        0        0     1448 2023-07-24 09:29:29.549148 serialtools-0.5.0/src/serialtools/__main__.py
+-rw-r--r--   0        0        0      345 2023-07-24 09:29:29.552481 serialtools-0.5.0/src/serialtools/apps/__init__.py
+-rw-r--r--   0        0        0     1143 2023-07-24 09:29:29.555815 serialtools-0.5.0/src/serialtools/apps/decode.py
+-rw-r--r--   0        0        0     1386 2023-07-24 09:29:29.552481 serialtools-0.5.0/src/serialtools/apps/dump.py
+-rw-r--r--   0        0        0     1369 2023-07-24 09:29:29.552481 serialtools-0.5.0/src/serialtools/apps/rawsplit.py
+-rw-r--r--   0        0        0      880 2023-07-24 09:29:29.552481 serialtools-0.5.0/src/serialtools/apps/send.py
+-rw-r--r--   0        0        0     7396 2023-07-24 09:30:04.138841 serialtools-0.5.0/src/serialtools/bus.py
+-rw-r--r--   0        0        0    15088 2023-07-24 09:30:04.138841 serialtools-0.5.0/src/serialtools/database.py
+-rw-r--r--   0        0        0     6228 2023-07-24 09:30:04.138841 serialtools-0.5.0/src/serialtools/database_config.py
+-rw-r--r--   0        0        0        0 2022-11-03 16:33:53.710006 serialtools-0.5.0/src/serialtools/py.typed
+-rw-r--r--   0        0        0      336 2023-06-23 15:21:45.869968 serialtools-0.5.0/tox.ini
+-rw-r--r--   0        0        0     1156 1970-01-01 00:00:00.000000 serialtools-0.5.0/PKG-INFO
```

### Comparing `serialtools-0.4.2/LICENSE` & `serialtools-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.2/docs/Makefile` & `serialtools-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.2/docs/build/html/_sources/index.rst.txt` & `serialtools-0.5.0/docs/build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.2/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js` & `serialtools-0.5.0/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.2/docs/build/html/_static/basic.css` & `serialtools-0.5.0/docs/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.2/docs/build/html/_static/css/badge_only.css` & `serialtools-0.5.0/docs/build/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.2/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff` & `serialtools-0.5.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.2/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2` & `serialtools-0.5.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.2/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff` & `serialtools-0.5.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.2/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2` & `serialtools-0.5.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.2/docs/build/html/_static/css/fonts/fontawesome-webfont.eot` & `serialtools-0.5.0/docs/build/html/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.2/docs/build/html/_static/css/fonts/fontawesome-webfont.svg` & `serialtools-0.5.0/docs/build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.2/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf` & `serialtools-0.5.0/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.2/docs/build/html/_static/css/fonts/fontawesome-webfont.woff` & `serialtools-0.5.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.2/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2` & `serialtools-0.5.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.2/docs/build/html/_static/css/fonts/lato-bold-italic.woff` & `serialtools-0.5.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.2/docs/build/html/_static/css/fonts/lato-bold-italic.woff2` & `serialtools-0.5.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.2/docs/build/html/_static/css/fonts/lato-bold.woff` & `serialtools-0.5.0/docs/build/html/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.2/docs/build/html/_static/css/fonts/lato-bold.woff2` & `serialtools-0.5.0/docs/build/html/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.2/docs/build/html/_static/css/fonts/lato-normal-italic.woff` & `serialtools-0.5.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.2/docs/build/html/_static/css/fonts/lato-normal-italic.woff2` & `serialtools-0.5.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.2/docs/build/html/_static/css/fonts/lato-normal.woff` & `serialtools-0.5.0/docs/build/html/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.2/docs/build/html/_static/css/fonts/lato-normal.woff2` & `serialtools-0.5.0/docs/build/html/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.2/docs/build/html/_static/css/theme.css` & `serialtools-0.5.0/docs/build/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.2/docs/build/html/_static/doctools.js` & `serialtools-0.5.0/docs/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.2/docs/build/html/_static/jquery.js` & `serialtools-0.5.0/docs/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.2/docs/build/html/_static/js/badge_only.js` & `serialtools-0.5.0/docs/build/html/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.2/docs/build/html/_static/js/html5shiv-printshiv.min.js` & `serialtools-0.5.0/docs/build/html/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.2/docs/build/html/_static/js/html5shiv.min.js` & `serialtools-0.5.0/docs/build/html/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.2/docs/build/html/_static/js/theme.js` & `serialtools-0.5.0/docs/build/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.2/docs/build/html/_static/language_data.js` & `serialtools-0.5.0/docs/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.2/docs/build/html/_static/pygments.css` & `serialtools-0.5.0/docs/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.2/docs/build/html/_static/searchtools.js` & `serialtools-0.5.0/docs/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.2/docs/build/html/_static/sphinx_highlight.js` & `serialtools-0.5.0/docs/build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.2/docs/build/html/genindex.html` & `serialtools-0.5.0/docs/build/html/genindex.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Index &mdash; serialtools v0.4.2 documentation</title>
+  <title>Index &mdash; serialtools v0.5.0 documentation</title>
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
-                v0.4.2
+                v0.5.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -197,14 +197,16 @@
       <li><a href="serialtools.apps.decode.html#serialtools.apps.decode.decode">decode() (in module serialtools.apps.decode)</a>
 
       <ul>
         <li><a href="serialtools.apps.rawsplit.html#serialtools.apps.rawsplit.decode">(in module serialtools.apps.rawsplit)</a>
 </li>
         <li><a href="serialtools.database.html#serialtools.database.Database.decode">(serialtools.database.Database method)</a>
 </li>
+        <li><a href="serialtools.database.html#serialtools.database.Message.decode">(serialtools.database.Message method)</a>
+</li>
       </ul></li>
   </ul></td>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="serialtools.database_config.html#serialtools.database_config.Param.defined_parameters">defined_parameters (serialtools.database_config.Param attribute)</a>
 </li>
       <li><a href="serialtools.bus.html#serialtools.bus.BusCreator.dsrdtr">dsrdtr (serialtools.bus.BusCreator attribute)</a>
 </li>
@@ -314,14 +316,24 @@
 </tr></table>
 
 <h2 id="L">L</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="serialtools.database.html#serialtools.database.Endianness.LITTLE">LITTLE (serialtools.database.Endianness attribute)</a>
 </li>
+      <li><a href="serialtools.database_config.html#serialtools.database_config.load_file">load_file() (in module serialtools.database_config)</a>
+
+      <ul>
+        <li><a href="serialtools.database_config.html#serialtools.database_config.DatabaseCreator.load_file">(serialtools.database_config.DatabaseCreator method)</a>
+</li>
+      </ul></li>
+  </ul></td>
+  <td style="width: 33%; vertical-align: top;"><ul>
+      <li><a href="serialtools.database_config.html#serialtools.database_config.LoggingCallback">LoggingCallback (class in serialtools.database_config)</a>
+</li>
   </ul></td>
 </tr></table>
 
 <h2 id="M">M</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="serialtools.apps.decode.html#serialtools.apps.decode.main">main() (in module serialtools.apps.decode)</a>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 
 
 serialtools
-v0.4.2
+v0.5.0
 [q                   ]
     * serialtools_package
     * serialtools.apps.decode_module
     * serialtools.apps.dump_module
     * serialtools.apps.rawsplit_module
     * serialtools.apps.send_module
     * serialtools.bus_module
@@ -58,22 +58,24 @@
     * cancel_write()_                           * create_args()_
       (serialtools.bus.ReadFromFileBus            (serialtools.bus.BusCreator_method)
       method)                                   * create_bus()_
           o (serialtools.bus.WriteToFileBus       (serialtools.bus.BusCreator_method)
             method)
 ***** D *****
     * Database_(class_in
-      serialtools.database)                    * defined_parameters_
-    * DatabaseCreator_(class_in                  (serialtools.database_config.Param
-      serialtools.database_config)               attribute)
-    * decode()_(in_module                      * dsrdtr_(serialtools.bus.BusCreator
-      serialtools.apps.decode)                   attribute)
-          o (in_module                         * dump()_(in_module
-            serialtools.apps.rawsplit)           serialtools.apps.dump)
-          o (serialtools.database.Database
+      serialtools.database)
+    * DatabaseCreator_(class_in                * defined_parameters_
+      serialtools.database_config)               (serialtools.database_config.Param
+    * decode()_(in_module                        attribute)
+      serialtools.apps.decode)                 * dsrdtr_(serialtools.bus.BusCreator
+          o (in_module                           attribute)
+            serialtools.apps.rawsplit)         * dump()_(in_module
+          o (serialtools.database.Database       serialtools.apps.dump)
+            method)
+          o (serialtools.database.Message
             method)
 ***** E *****
     * encode()_
       (serialtools.database.Database     * endianness_(serialtools.database.Database
       method)                              attribute)
     * encode_range()_                          o (serialtools.database_config.DatabaseCreator
       (serialtools.database.Database             attribute)
@@ -114,14 +116,18 @@
       method)                                       * integer()_(in_module
           o (serialtools.database_config.Param        serialtools.database_config)
             method)
           o (serialtools.database_config.Signal
             method)
 ***** L *****
     * LITTLE_(serialtools.database.Endianness_attribute)
+    * load_file()_(in_module                                 * LoggingCallback_(class_in
+      serialtools.database_config)                             serialtools.database_config)
+          o (serialtools.database_config.DatabaseCreator
+            method)
 ***** M *****
     * main()_(in_module
       serialtools.apps.decode)
           o (in_module
             serialtools.apps.dump)
           o (in_module
             serialtools.apps.rawsplit)         * module
```

### Comparing `serialtools-0.4.2/docs/build/html/index.html` & `serialtools-0.5.0/docs/build/html/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Welcome to serialtools’ documentation! &mdash; serialtools v0.4.2 documentation</title>
+  <title>Welcome to serialtools’ documentation! &mdash; serialtools v0.5.0 documentation</title>
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
-                v0.4.2
+                v0.5.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -141,19 +141,21 @@
 <li class="toctree-l2"><a class="reference internal" href="serialtools.database.html#serialtools.database.Signal"><code class="docutils literal notranslate"><span class="pre">Signal</span></code></a></li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.database.html#serialtools.database.Type"><code class="docutils literal notranslate"><span class="pre">Type</span></code></a></li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.database.html#serialtools.database.format_bytes"><code class="docutils literal notranslate"><span class="pre">format_bytes()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.database_config.html">serialtools.database_config module</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.database_config.html#serialtools.database_config.DatabaseCreator"><code class="docutils literal notranslate"><span class="pre">DatabaseCreator</span></code></a></li>
+<li class="toctree-l2"><a class="reference internal" href="serialtools.database_config.html#serialtools.database_config.LoggingCallback"><code class="docutils literal notranslate"><span class="pre">LoggingCallback</span></code></a></li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.database_config.html#serialtools.database_config.Message"><code class="docutils literal notranslate"><span class="pre">Message</span></code></a></li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.database_config.html#serialtools.database_config.Param"><code class="docutils literal notranslate"><span class="pre">Param</span></code></a></li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.database_config.html#serialtools.database_config.Signal"><code class="docutils literal notranslate"><span class="pre">Signal</span></code></a></li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.database_config.html#serialtools.database_config.get_database"><code class="docutils literal notranslate"><span class="pre">get_database()</span></code></a></li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.database_config.html#serialtools.database_config.integer"><code class="docutils literal notranslate"><span class="pre">integer()</span></code></a></li>
+<li class="toctree-l2"><a class="reference internal" href="serialtools.database_config.html#serialtools.database_config.load_file"><code class="docutils literal notranslate"><span class="pre">load_file()</span></code></a></li>
 </ul>
 </li>
 </ul>
 </div>
 </section>
 <section id="indices-and-tables">
 <h2>Indices and tables<a class="headerlink" href="#indices-and-tables" title="Permalink to this heading"></a></h2>
```

#### html2text {}

```diff
@@ -4,15 +4,15 @@
 
 
 
 
 
 
 serialtools
-v0.4.2
+v0.5.0
 [q                   ]
     * serialtools_package
     * serialtools.apps.decode_module
     * serialtools.apps.dump_module
     * serialtools.apps.rawsplit_module
     * serialtools.apps.send_module
     * serialtools.bus_module
@@ -63,19 +63,21 @@
           o MessageSpec
           o Reader
           o Signal
           o Type
           o format_bytes()
     * serialtools.database_config_module
           o DatabaseCreator
+          o LoggingCallback
           o Message
           o Param
           o Signal
           o get_database()
           o integer()
+          o load_file()
 
 ***** Indices and tablesï *****
     * Index
     * Module_Index
     * Search_Page
 
 ***** Linksï *****
```

### Comparing `serialtools-0.4.2/docs/build/html/modules.html` & `serialtools-0.5.0/docs/build/html/modules.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools &mdash; serialtools v0.4.2 documentation</title>
+  <title>serialtools &mdash; serialtools v0.5.0 documentation</title>
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
-                v0.4.2
+                v0.5.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -114,19 +114,21 @@
 <li class="toctree-l4"><a class="reference internal" href="serialtools.database.html#serialtools.database.Signal"><code class="docutils literal notranslate"><span class="pre">Signal</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="serialtools.database.html#serialtools.database.Type"><code class="docutils literal notranslate"><span class="pre">Type</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="serialtools.database.html#serialtools.database.format_bytes"><code class="docutils literal notranslate"><span class="pre">format_bytes()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database_config.html">serialtools.database_config module</a><ul>
 <li class="toctree-l4"><a class="reference internal" href="serialtools.database_config.html#serialtools.database_config.DatabaseCreator"><code class="docutils literal notranslate"><span class="pre">DatabaseCreator</span></code></a></li>
+<li class="toctree-l4"><a class="reference internal" href="serialtools.database_config.html#serialtools.database_config.LoggingCallback"><code class="docutils literal notranslate"><span class="pre">LoggingCallback</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="serialtools.database_config.html#serialtools.database_config.Message"><code class="docutils literal notranslate"><span class="pre">Message</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="serialtools.database_config.html#serialtools.database_config.Param"><code class="docutils literal notranslate"><span class="pre">Param</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="serialtools.database_config.html#serialtools.database_config.Signal"><code class="docutils literal notranslate"><span class="pre">Signal</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="serialtools.database_config.html#serialtools.database_config.get_database"><code class="docutils literal notranslate"><span class="pre">get_database()</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="serialtools.database_config.html#serialtools.database_config.integer"><code class="docutils literal notranslate"><span class="pre">integer()</span></code></a></li>
+<li class="toctree-l4"><a class="reference internal" href="serialtools.database_config.html#serialtools.database_config.load_file"><code class="docutils literal notranslate"><span class="pre">load_file()</span></code></a></li>
 </ul>
 </li>
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.html#module-serialtools">Module contents</a></li>
 </ul>
 </li>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 
 
 serialtools
-v0.4.2
+v0.5.0
 [q                   ]
     * serialtools_package
     * serialtools.apps.decode_module
     * serialtools.apps.dump_module
     * serialtools.apps.rawsplit_module
     * serialtools.apps.send_module
     * serialtools.bus_module
@@ -43,17 +43,19 @@
                       # MessageSpec
                       # Reader
                       # Signal
                       # Type
                       # format_bytes()
                 # serialtools.database_config_module
                       # DatabaseCreator
+                      # LoggingCallback
                       # Message
                       # Param
                       # Signal
                       # get_database()
                       # integer()
+                      # load_file()
           o Module_contents
 
 ===============================================================================
 © Copyright 2023, erzo.
 Built with Sphinx using a theme provided by Read_the_Docs.
```

### Comparing `serialtools-0.4.2/docs/build/html/py-modindex.html` & `serialtools-0.5.0/docs/build/html/py-modindex.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Python Module Index &mdash; serialtools v0.4.2 documentation</title>
+  <title>Python Module Index &mdash; serialtools v0.5.0 documentation</title>
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
-                v0.4.2
+                v0.5.0
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
-v0.4.2
+v0.5.0
 [q                   ]
     * serialtools_package
     * serialtools.apps.decode_module
     * serialtools.apps.dump_module
     * serialtools.apps.rawsplit_module
     * serialtools.apps.send_module
     * serialtools.bus_module
```

### Comparing `serialtools-0.4.2/docs/build/html/search.html` & `serialtools-0.5.0/docs/build/html/search.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Search &mdash; serialtools v0.4.2 documentation</title>
+  <title>Search &mdash; serialtools v0.5.0 documentation</title>
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
-                v0.4.2
+                v0.5.0
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
-v0.4.2
+v0.5.0
 [q                   ]
     * serialtools_package
     * serialtools.apps.decode_module
     * serialtools.apps.dump_module
     * serialtools.apps.rawsplit_module
     * serialtools.apps.send_module
     * serialtools.bus_module
```

### Comparing `serialtools-0.4.2/docs/build/html/searchindex.js` & `serialtools-0.5.0/docs/build/html/searchindex.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -132,15 +132,15 @@
         "i": [8, 9, 10],
         "access": [8, 9, 10],
         "attribut": [8, 9, 10],
         "If": [8, 9, 10],
         "you": [8, 9, 10],
         "want": [8, 9, 10],
         "need": [8, 9, 10],
-        "fn": 8,
+        "fn": [8, 10],
         "paramet": [8, 10],
         "name": [8, 9],
         "contain": [8, 9],
         "data": [8, 9],
         "separ": 8,
         "space": 8,
         "option": 8,
@@ -158,15 +158,15 @@
         "sequenc": [9, 10],
         "paramref": 9,
         "either": 9,
         "number": 9,
         "previou": 9,
         "spec": 9,
         "specifi": 9,
-        "map": 9,
+        "map": [9, 10],
         "message_spec": [2, 9],
         "8": 9,
         "address": [2, 9],
         "dict": [9, 10],
         "length_in_byt": 9,
         "callabl": 9,
         "all": 9,
@@ -238,15 +238,15 @@
         "defin": 10,
         "command": 10,
         "val": 10,
         "sourc": 0,
         "code": 0,
         "bug": 0,
         "tracker": 0,
-        "log": 0,
+        "log": [0, 10],
         "pypi": 0,
         "part": [6, 9],
         "consist": [6, 9],
         "itself": 9,
         "possibl": 9,
         "create_arg": [2, 8],
         "send_msg": [2, 9],
@@ -269,15 +269,25 @@
         "signific": 9,
         "mutual": 9,
         "exclus": 9,
         "onli": 9,
         "one": 9,
         "them": 9,
         "mai": 9,
-        "pass": 9
+        "pass": 9,
+        "loggingcallback": [0, 1, 2, 10],
+        "load_fil": [0, 1, 2, 10],
+        "logger": 10,
+        "rootlogg": 10,
+        "root": 10,
+        "level": 10,
+        "collect": 10,
+        "abc": 10,
+        "confattr": 10,
+        "notificationlevel": 10
     },
     "objects": {
         "": [
             [2, 0, 0, "-", "serialtools"]
         ],
         "serialtools": [
             [3, 0, 0, "-", "apps"],
@@ -391,14 +401,15 @@
             [9, 4, 1, "", "word_length_in_bits"]
         ],
         "serialtools.database.Endianness": [
             [9, 4, 1, "", "BIG"],
             [9, 4, 1, "", "LITTLE"]
         ],
         "serialtools.database.Message": [
+            [9, 3, 1, "", "decode"],
             [9, 3, 1, "", "format"],
             [9, 3, 1, "", "format_raw"],
             [9, 3, 1, "", "format_timestamp"]
         ],
         "serialtools.database.MessageSpec": [
             [9, 4, 1, "", "ADDRESS"]
         ],
@@ -421,23 +432,26 @@
             [9, 4, 1, "", "FLOAT"],
             [9, 4, 1, "", "INT"],
             [9, 4, 1, "", "TEXT"],
             [9, 4, 1, "", "UINT"]
         ],
         "serialtools.database_config": [
             [10, 2, 1, "", "DatabaseCreator"],
+            [10, 2, 1, "", "LoggingCallback"],
             [10, 2, 1, "", "Message"],
             [10, 2, 1, "", "Param"],
             [10, 2, 1, "", "Signal"],
             [10, 1, 1, "", "get_database"],
-            [10, 1, 1, "", "integer"]
+            [10, 1, 1, "", "integer"],
+            [10, 1, 1, "", "load_file"]
         ],
         "serialtools.database_config.DatabaseCreator": [
             [10, 4, 1, "", "endianness"],
             [10, 3, 1, "", "get"],
+            [10, 3, 1, "", "load_file"],
             [10, 4, 1, "", "word_length_in_bits"]
         ],
         "serialtools.database_config.Message": [
             [10, 3, 1, "", "init_parser"],
             [10, 4, 1, "", "message"],
             [10, 3, 1, "", "run_parsed"]
         ],
@@ -802,14 +816,17 @@
         ],
         "uint (serialtools.database.type attribute)": [
             [9, "serialtools.database.Type.UINT"]
         ],
         "decode() (serialtools.database.database method)": [
             [9, "serialtools.database.Database.decode"]
         ],
+        "decode() (serialtools.database.message method)": [
+            [9, "serialtools.database.Message.decode"]
+        ],
         "encode() (serialtools.database.database method)": [
             [9, "serialtools.database.Database.encode"]
         ],
         "encode_range() (serialtools.database.database method)": [
             [9, "serialtools.database.Database.encode_range"]
         ],
         "endianness (serialtools.database.database attribute)": [
@@ -883,14 +900,17 @@
         ],
         "word_length_in_bits (serialtools.database.database attribute)": [
             [9, "serialtools.database.Database.word_length_in_bits"]
         ],
         "databasecreator (class in serialtools.database_config)": [
             [10, "serialtools.database_config.DatabaseCreator"]
         ],
+        "loggingcallback (class in serialtools.database_config)": [
+            [10, "serialtools.database_config.LoggingCallback"]
+        ],
         "message (class in serialtools.database_config)": [
             [10, "serialtools.database_config.Message"]
         ],
         "param (class in serialtools.database_config)": [
             [10, "serialtools.database_config.Param"]
         ],
         "signal (class in serialtools.database_config)": [
@@ -916,14 +936,20 @@
         ],
         "init_parser() (serialtools.database_config.signal method)": [
             [10, "serialtools.database_config.Signal.init_parser"]
         ],
         "integer() (in module serialtools.database_config)": [
             [10, "serialtools.database_config.integer"]
         ],
+        "load_file() (in module serialtools.database_config)": [
+            [10, "serialtools.database_config.load_file"]
+        ],
+        "load_file() (serialtools.database_config.databasecreator method)": [
+            [10, "serialtools.database_config.DatabaseCreator.load_file"]
+        ],
         "message (serialtools.database_config.message attribute)": [
             [10, "serialtools.database_config.Message.message"]
         ],
         "parse_allowed_values() (serialtools.database_config.param method)": [
             [10, "serialtools.database_config.Param.parse_allowed_values"]
         ],
         "run_parsed() (serialtools.database_config.message method)": [
```

### Comparing `serialtools-0.4.2/docs/build/html/serialtools.apps.decode.html` & `serialtools-0.5.0/docs/build/html/serialtools.apps.decode.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools.apps.decode module &mdash; serialtools v0.4.2 documentation</title>
+  <title>serialtools.apps.decode module &mdash; serialtools v0.5.0 documentation</title>
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
-                v0.4.2
+                v0.5.0
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
-v0.4.2
+v0.5.0
 [q                   ]
     * serialtools_package
           o Subpackages
                 # serialtools.apps_package
                       # Submodules
                       # Module_contents
           o Submodules
```

### Comparing `serialtools-0.4.2/docs/build/html/serialtools.apps.dump.html` & `serialtools-0.5.0/docs/build/html/serialtools.apps.dump.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools.apps.dump module &mdash; serialtools v0.4.2 documentation</title>
+  <title>serialtools.apps.dump module &mdash; serialtools v0.5.0 documentation</title>
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
-                v0.4.2
+                v0.5.0
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
-v0.4.2
+v0.5.0
 [q                   ]
     * serialtools_package
           o Subpackages
                 # serialtools.apps_package
                       # Submodules
                       # Module_contents
           o Submodules
```

### Comparing `serialtools-0.4.2/docs/build/html/serialtools.apps.html` & `serialtools-0.5.0/docs/build/html/serialtools.apps.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools.apps package &mdash; serialtools v0.4.2 documentation</title>
+  <title>serialtools.apps package &mdash; serialtools v0.5.0 documentation</title>
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
-                v0.4.2
+                v0.5.0
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
-v0.4.2
+v0.5.0
 [q                   ]
     * serialtools_package
           o Subpackages
                 # serialtools.apps_package
                       # Submodules
                       # Module_contents
           o Submodules
```

### Comparing `serialtools-0.4.2/docs/build/html/serialtools.apps.rawsplit.html` & `serialtools-0.5.0/docs/build/html/serialtools.apps.rawsplit.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools.apps.rawsplit module &mdash; serialtools v0.4.2 documentation</title>
+  <title>serialtools.apps.rawsplit module &mdash; serialtools v0.5.0 documentation</title>
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
-                v0.4.2
+                v0.5.0
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
-v0.4.2
+v0.5.0
 [q                   ]
     * serialtools_package
     * serialtools.apps.decode_module
     * serialtools.apps.dump_module
     * serialtools.apps.rawsplit_module
           o add_arguments()
           o add_parser()
```

### Comparing `serialtools-0.4.2/docs/build/html/serialtools.apps.send.html` & `serialtools-0.5.0/docs/build/html/serialtools.apps.send.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools.apps.send module &mdash; serialtools v0.4.2 documentation</title>
+  <title>serialtools.apps.send module &mdash; serialtools v0.5.0 documentation</title>
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
-                v0.4.2
+                v0.5.0
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
-v0.4.2
+v0.5.0
 [q                   ]
     * serialtools_package
           o Subpackages
                 # serialtools.apps_package
                       # Submodules
                       # Module_contents
           o Submodules
```

### Comparing `serialtools-0.4.2/docs/build/html/serialtools.bus.html` & `serialtools-0.5.0/docs/build/html/serialtools.bus.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools.bus module &mdash; serialtools v0.4.2 documentation</title>
+  <title>serialtools.bus module &mdash; serialtools v0.5.0 documentation</title>
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
-                v0.4.2
+                v0.5.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -176,15 +176,15 @@
 <dd><p>Each instance of this class represents a setting which can be changed in a config file.</p>
 <p>This class implements the <a class="reference external" href="https://docs.python.org/3/reference/datamodel.html#implementing-descriptors">descriptor protocol</a> to return <code class="xref py py-attr docutils literal notranslate"><span class="pre">value</span></code> if an instance of this class is accessed as an instance attribute.
 If you want to get this object you need to access it as a class attribute.</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="serialtools.bus.BusCreator.create_args">
-<span class="sig-name descname"><span class="pre">create_args</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="o"><span class="pre">*</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">port</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">baudrate</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">virtual</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)"><span class="pre">bool</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/argparse.html#argparse.Namespace" title="(in Python v3.11)"><span class="pre">Namespace</span></a></span></span><a class="headerlink" href="#serialtools.bus.BusCreator.create_args" title="Permalink to this definition"></a></dt>
+<span class="sig-name descname"><span class="pre">create_args</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="o"><span class="pre">*</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">port</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">baudrate</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">virtual</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)"><span class="pre">bool</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">rx_only</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)"><span class="pre">bool</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/argparse.html#argparse.Namespace" title="(in Python v3.11)"><span class="pre">Namespace</span></a></span></span><a class="headerlink" href="#serialtools.bus.BusCreator.create_args" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="serialtools.bus.BusCreator.create_bus">
 <span class="sig-name descname"><span class="pre">create_bus</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">args</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/argparse.html#argparse.Namespace" title="(in Python v3.11)"><span class="pre">Namespace</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Serial</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference internal" href="#serialtools.bus.ReadFromFileBus" title="serialtools.bus.ReadFromFileBus"><span class="pre">ReadFromFileBus</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference internal" href="#serialtools.bus.WriteToFileBus" title="serialtools.bus.WriteToFileBus"><span class="pre">WriteToFileBus</span></a></span></span><a class="headerlink" href="#serialtools.bus.BusCreator.create_bus" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 
 
 
 
 
 
 serialtools
-v0.4.2
+v0.5.0
 [q                   ]
     * serialtools_package
           o Subpackages
           o Submodules
                 # serialtools.bus_module
                       # BusCreator
                       # ReadFromFileBus
@@ -89,15 +89,16 @@
         bytesizeï
             Each instance of this class represents a setting which can be
             changed in a config file.
             This class implements the descriptor_protocol to return value if an
             instance of this class is accessed as an instance attribute. If you
             want to get this object you need to access it as a class attribute.
         create_args(*, port: str | None = None, baudrate: int | None = None,
-        virtual: bool | None = None) &#x2192; Namespaceï
+        virtual: bool | None = None, rx_only: bool = False) &#x2192;
+        Namespaceï
         create_bus(args: Namespace) &#x2192; Serial | ReadFromFileBus |
         WriteToFileBusï
         dsrdtrï
             Each instance of this class represents a setting which can be
             changed in a config file.
             This class implements the descriptor_protocol to return value if an
             instance of this class is accessed as an instance attribute. If you
```

### Comparing `serialtools-0.4.2/docs/build/html/serialtools.database.html` & `serialtools-0.5.0/docs/build/html/serialtools.database.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools.database module &mdash; serialtools v0.4.2 documentation</title>
+  <title>serialtools.database module &mdash; serialtools v0.5.0 documentation</title>
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
-                v0.4.2
+                v0.5.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -97,14 +97,15 @@
 </li>
 <li class="toctree-l2"><a class="reference internal" href="#serialtools.database.Endianness"><code class="docutils literal notranslate"><span class="pre">Endianness</span></code></a><ul>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Endianness.BIG"><code class="docutils literal notranslate"><span class="pre">Endianness.BIG</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Endianness.LITTLE"><code class="docutils literal notranslate"><span class="pre">Endianness.LITTLE</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="#serialtools.database.Message"><code class="docutils literal notranslate"><span class="pre">Message</span></code></a><ul>
+<li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Message.decode"><code class="docutils literal notranslate"><span class="pre">Message.decode()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Message.format"><code class="docutils literal notranslate"><span class="pre">Message.format()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Message.format_raw"><code class="docutils literal notranslate"><span class="pre">Message.format_raw()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Message.format_timestamp"><code class="docutils literal notranslate"><span class="pre">Message.format_timestamp()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="#serialtools.database.MessageSpec"><code class="docutils literal notranslate"><span class="pre">MessageSpec</span></code></a><ul>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.MessageSpec.ADDRESS"><code class="docutils literal notranslate"><span class="pre">MessageSpec.ADDRESS</span></code></a></li>
@@ -266,14 +267,19 @@
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="serialtools.database.Message">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">serialtools.database.</span></span><span class="sig-name descname"><span class="pre">Message</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">db</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="#serialtools.database.Database" title="serialtools.database.Database"><span class="pre">Database</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">timestamp</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/datetime.html#datetime.datetime" title="(in Python v3.11)"><span class="pre">datetime</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">values</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/collections.abc.html#collections.abc.Mapping" title="(in Python v3.11)"><span class="pre">Mapping</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytes" title="(in Python v3.11)"><span class="pre">bytes</span></a><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#serialtools.database.Message" title="Permalink to this definition"></a></dt>
 <dd><p>Bases: <a class="reference external" href="https://docs.python.org/3/library/functions.html#object" title="(in Python v3.11)"><code class="xref py py-class docutils literal notranslate"><span class="pre">object</span></code></a></p>
 <dl class="py method">
+<dt class="sig sig-object py" id="serialtools.database.Message.decode">
+<span class="sig-name descname"><span class="pre">decode</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/collections.abc.html#collections.abc.Mapping" title="(in Python v3.11)"><span class="pre">Mapping</span></a><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#serialtools.database.Signal" title="serialtools.database.Signal"><span class="pre">Signal</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#float" title="(in Python v3.11)"><span class="pre">float</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)"><span class="pre">bool</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#serialtools.database.Message.decode" title="Permalink to this definition"></a></dt>
+<dd></dd></dl>
+
+<dl class="py method">
 <dt class="sig sig-object py" id="serialtools.database.Message.format">
 <span class="sig-name descname"><span class="pre">format</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a></span></span><a class="headerlink" href="#serialtools.database.Message.format" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="serialtools.database.Message.format_raw">
 <span class="sig-name descname"><span class="pre">format_raw</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a></span></span><a class="headerlink" href="#serialtools.database.Message.format_raw" title="Permalink to this definition"></a></dt>
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 
 
 
 
 
 
 serialtools
-v0.4.2
+v0.5.0
 [q                   ]
     * serialtools_package
           o Subpackages
           o Submodules
                 # serialtools.bus_module
                 # serialtools.database_module
                       # ByteSpec
@@ -47,14 +47,15 @@
                 # Database.message_spec
                 # Database.signals
                 # Database.word_length_in_bits
           o Endianness
                 # Endianness.BIG
                 # Endianness.LITTLE
           o Message
+                # Message.decode()
                 # Message.format()
                 # Message.format_raw()
                 # Message.format_timestamp()
           o MessageSpec
                 # MessageSpec.ADDRESS
           o Reader
                 # Reader.ignore_bytes_between_messages
@@ -116,14 +117,15 @@
   qualname=None, type=None, start=1, boundary=None)ï
       Bases: Enum
         BIG= 1ï
         LITTLE= 2ï
   classserialtools.database.Message(db: Database, timestamp: datetime | None,
   values: Mapping[str, bytes])ï
       Bases: object
+        decode() &#x2192; Mapping[Signal, int | float | bool | str]ï
         format() &#x2192; strï
         format_raw() &#x2192; strï
         format_timestamp() &#x2192; strï
   classserialtools.database.MessageSpec(params: Sequence[ByteSpec], *,
   implicit_address: int | None = None)ï
       Bases: object
         ADDRESS= 'address'ï
```

### Comparing `serialtools-0.4.2/docs/build/html/serialtools.database_config.html` & `serialtools-0.5.0/docs/build/html/serialtools.database_config.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools.database_config module &mdash; serialtools v0.4.2 documentation</title>
+  <title>serialtools.database_config module &mdash; serialtools v0.5.0 documentation</title>
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
-                v0.4.2
+                v0.5.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -52,19 +52,21 @@
 <li class="toctree-l1 current"><a class="reference internal" href="serialtools.html">serialtools package</a><ul class="current">
 <li class="toctree-l2"><a class="reference internal" href="serialtools.html#subpackages">Subpackages</a></li>
 <li class="toctree-l2 current"><a class="reference internal" href="serialtools.html#submodules">Submodules</a><ul class="current">
 <li class="toctree-l3"><a class="reference internal" href="serialtools.bus.html">serialtools.bus module</a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html">serialtools.database module</a></li>
 <li class="toctree-l3 current"><a class="current reference internal" href="#">serialtools.database_config module</a><ul>
 <li class="toctree-l4"><a class="reference internal" href="#serialtools.database_config.DatabaseCreator"><code class="docutils literal notranslate"><span class="pre">DatabaseCreator</span></code></a></li>
+<li class="toctree-l4"><a class="reference internal" href="#serialtools.database_config.LoggingCallback"><code class="docutils literal notranslate"><span class="pre">LoggingCallback</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="#serialtools.database_config.Message"><code class="docutils literal notranslate"><span class="pre">Message</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="#serialtools.database_config.Param"><code class="docutils literal notranslate"><span class="pre">Param</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="#serialtools.database_config.Signal"><code class="docutils literal notranslate"><span class="pre">Signal</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="#serialtools.database_config.get_database"><code class="docutils literal notranslate"><span class="pre">get_database()</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="#serialtools.database_config.integer"><code class="docutils literal notranslate"><span class="pre">integer()</span></code></a></li>
+<li class="toctree-l4"><a class="reference internal" href="#serialtools.database_config.load_file"><code class="docutils literal notranslate"><span class="pre">load_file()</span></code></a></li>
 </ul>
 </li>
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.html#module-serialtools">Module contents</a></li>
 </ul>
 </li>
@@ -74,17 +76,19 @@
 <li class="toctree-l1"><a class="reference internal" href="serialtools.apps.send.html">serialtools.apps.send module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.bus.html">serialtools.bus module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.database.html">serialtools.database module</a></li>
 <li class="toctree-l1 current"><a class="current reference internal" href="#">serialtools.database_config module</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="#serialtools.database_config.DatabaseCreator"><code class="docutils literal notranslate"><span class="pre">DatabaseCreator</span></code></a><ul>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database_config.DatabaseCreator.endianness"><code class="docutils literal notranslate"><span class="pre">DatabaseCreator.endianness</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database_config.DatabaseCreator.get"><code class="docutils literal notranslate"><span class="pre">DatabaseCreator.get()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#serialtools.database_config.DatabaseCreator.load_file"><code class="docutils literal notranslate"><span class="pre">DatabaseCreator.load_file()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database_config.DatabaseCreator.word_length_in_bits"><code class="docutils literal notranslate"><span class="pre">DatabaseCreator.word_length_in_bits</span></code></a></li>
 </ul>
 </li>
+<li class="toctree-l2"><a class="reference internal" href="#serialtools.database_config.LoggingCallback"><code class="docutils literal notranslate"><span class="pre">LoggingCallback</span></code></a></li>
 <li class="toctree-l2"><a class="reference internal" href="#serialtools.database_config.Message"><code class="docutils literal notranslate"><span class="pre">Message</span></code></a><ul>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database_config.Message.init_parser"><code class="docutils literal notranslate"><span class="pre">Message.init_parser()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database_config.Message.message"><code class="docutils literal notranslate"><span class="pre">Message.message</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database_config.Message.run_parsed"><code class="docutils literal notranslate"><span class="pre">Message.run_parsed()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="#serialtools.database_config.Param"><code class="docutils literal notranslate"><span class="pre">Param</span></code></a><ul>
@@ -98,14 +102,15 @@
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database_config.Signal.init_parser"><code class="docutils literal notranslate"><span class="pre">Signal.init_parser()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database_config.Signal.run_parsed"><code class="docutils literal notranslate"><span class="pre">Signal.run_parsed()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database_config.Signal.signals"><code class="docutils literal notranslate"><span class="pre">Signal.signals</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="#serialtools.database_config.get_database"><code class="docutils literal notranslate"><span class="pre">get_database()</span></code></a></li>
 <li class="toctree-l2"><a class="reference internal" href="#serialtools.database_config.integer"><code class="docutils literal notranslate"><span class="pre">integer()</span></code></a></li>
+<li class="toctree-l2"><a class="reference internal" href="#serialtools.database_config.load_file"><code class="docutils literal notranslate"><span class="pre">load_file()</span></code></a></li>
 </ul>
 </li>
 </ul>
 
         </div>
       </div>
     </nav>
@@ -144,25 +149,36 @@
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="serialtools.database_config.DatabaseCreator.get">
 <span class="sig-name descname"><span class="pre">get</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="o"><span class="pre">*</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">require_signals</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)"><span class="pre">bool</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">True</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="serialtools.database.html#serialtools.database.Database" title="serialtools.database.Database"><span class="pre">Database</span></a></span></span><a class="headerlink" href="#serialtools.database_config.DatabaseCreator.get" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
 
+<dl class="py method">
+<dt class="sig sig-object py" id="serialtools.database_config.DatabaseCreator.load_file">
+<span class="sig-name descname"><span class="pre">load_file</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">fn</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="serialtools.database.html#serialtools.database.Database" title="serialtools.database.Database"><span class="pre">Database</span></a></span></span><a class="headerlink" href="#serialtools.database_config.DatabaseCreator.load_file" title="Permalink to this definition"></a></dt>
+<dd></dd></dl>
+
 <dl class="py attribute">
 <dt class="sig sig-object py" id="serialtools.database_config.DatabaseCreator.word_length_in_bits">
 <span class="sig-name descname"><span class="pre">word_length_in_bits</span></span><a class="headerlink" href="#serialtools.database_config.DatabaseCreator.word_length_in_bits" title="Permalink to this definition"></a></dt>
 <dd><p>Each instance of this class represents a setting which can be changed in a config file.</p>
 <p>This class implements the <a class="reference external" href="https://docs.python.org/3/reference/datamodel.html#implementing-descriptors">descriptor protocol</a> to return <code class="xref py py-attr docutils literal notranslate"><span class="pre">value</span></code> if an instance of this class is accessed as an instance attribute.
 If you want to get this object you need to access it as a class attribute.</p>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
+<dt class="sig sig-object py" id="serialtools.database_config.LoggingCallback">
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">serialtools.database_config.</span></span><span class="sig-name descname"><span class="pre">LoggingCallback</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">*</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">logger:</span> <span class="pre">~logging.Logger</span> <span class="pre">=</span> <span class="pre">&lt;RootLogger</span> <span class="pre">root</span> <span class="pre">(WARNING)&gt;</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">levels:</span> <span class="pre">~collections.abc.Mapping[~confattr.configfile.NotificationLevel</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">int]</span> <span class="pre">=</span> <span class="pre">{}</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#serialtools.database_config.LoggingCallback" title="Permalink to this definition"></a></dt>
+<dd><p>Bases: <a class="reference external" href="https://docs.python.org/3/library/functions.html#object" title="(in Python v3.11)"><code class="xref py py-class docutils literal notranslate"><span class="pre">object</span></code></a></p>
+</dd></dl>
+
+<dl class="py class">
 <dt class="sig sig-object py" id="serialtools.database_config.Message">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">serialtools.database_config.</span></span><span class="sig-name descname"><span class="pre">Message</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">config_file</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">ConfigFile</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#serialtools.database_config.Message" title="Permalink to this definition"></a></dt>
 <dd><p>Bases: <code class="xref py py-class docutils literal notranslate"><span class="pre">ConfigFileArgparseCommand</span></code></p>
 <dl class="py method">
 <dt class="sig sig-object py" id="serialtools.database_config.Message.init_parser">
 <span class="sig-name descname"><span class="pre">init_parser</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">parser</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/argparse.html#argparse.ArgumentParser" title="(in Python v3.11)"><span class="pre">ArgumentParser</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span></span><a class="headerlink" href="#serialtools.database_config.Message.init_parser" title="Permalink to this definition"></a></dt>
 <dd><dl class="field-list simple">
@@ -257,14 +273,19 @@
 <dd></dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="serialtools.database_config.integer">
 <span class="sig-prename descclassname"><span class="pre">serialtools.database_config.</span></span><span class="sig-name descname"><span class="pre">integer</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">val</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a></span></span><a class="headerlink" href="#serialtools.database_config.integer" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
 
+<dl class="py function">
+<dt class="sig sig-object py" id="serialtools.database_config.load_file">
+<span class="sig-prename descclassname"><span class="pre">serialtools.database_config.</span></span><span class="sig-name descname"><span class="pre">load_file</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">fn</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="serialtools.database.html#serialtools.database.Database" title="serialtools.database.Database"><span class="pre">Database</span></a></span></span><a class="headerlink" href="#serialtools.database_config.load_file" title="Permalink to this definition"></a></dt>
+<dd></dd></dl>
+
 </section>
 
 
            </div>
           </div>
           <footer><div class="rst-footer-buttons" role="navigation" aria-label="Footer">
         <a href="serialtools.database.html" class="btn btn-neutral float-left" title="serialtools.database module" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
```

#### html2text {}

```diff
@@ -5,40 +5,44 @@
 
 
 
 
 
 
 serialtools
-v0.4.2
+v0.5.0
 [q                   ]
     * serialtools_package
           o Subpackages
           o Submodules
                 # serialtools.bus_module
                 # serialtools.database_module
                 # serialtools.database_config_module
                       # DatabaseCreator
+                      # LoggingCallback
                       # Message
                       # Param
                       # Signal
                       # get_database()
                       # integer()
+                      # load_file()
           o Module_contents
     * serialtools.apps.decode_module
     * serialtools.apps.dump_module
     * serialtools.apps.rawsplit_module
     * serialtools.apps.send_module
     * serialtools.bus_module
     * serialtools.database_module
     * serialtools.database_config_module
           o DatabaseCreator
                 # DatabaseCreator.endianness
                 # DatabaseCreator.get()
+                # DatabaseCreator.load_file()
                 # DatabaseCreator.word_length_in_bits
+          o LoggingCallback
           o Message
                 # Message.init_parser()
                 # Message.message
                 # Message.run_parsed()
           o Param
                 # Param.defined_parameters
                 # Param.init_parser()
@@ -46,32 +50,38 @@
                 # Param.run_parsed()
           o Signal
                 # Signal.init_parser()
                 # Signal.run_parsed()
                 # Signal.signals
           o get_database()
           o integer()
+          o load_file()
    serialtools
     * serialtools_package
     * serialtools.database_config module
     * View_page_source
 ===============================================================================
 ****** serialtools.database_config moduleï ******
   classserialtools.database_config.DatabaseCreatorï
       Bases: object
         endiannessï
             A setting without a default value which requires the user to
             explicitly set a value in the config file.
         get(*, require_signals: bool = True) &#x2192; Databaseï
+        load_file(fn: str) &#x2192; Databaseï
         word_length_in_bitsï
             Each instance of this class represents a setting which can be
             changed in a config file.
             This class implements the descriptor_protocol to return value if an
             instance of this class is accessed as an instance attribute. If you
             want to get this object you need to access it as a class attribute.
+  classserialtools.database_config.LoggingCallback(*, logger: ~logging.Logger =
+  <RootLogger root (WARNING)>, levels: ~collections.abc.Mapping
+  [~confattr.configfile.NotificationLevel, int] = {})ï
+      Bases: object
   classserialtools.database_config.Message(config_file: ConfigFile)ï
       Bases: ConfigFileArgparseCommand
         init_parser(parser: ArgumentParser) &#x2192; Noneï
               Parameters:
                   parserÂ¶ â The parser to add arguments to. This is the same
                   object like parser.
             This is an abstract method which must be implemented by subclasses.
@@ -103,11 +113,12 @@
             Use ArgumentParser.add_argument() to add arguments to parser.
         run_parsed(args: Namespace) &#x2192; Noneï
             This is an abstract method which must be implemented by subclasses.
         signals: list[db.Signal]= []ï
   serialtools.database_config.get_database(*, require_signals: bool = True)
   &#x2192; Databaseï
   serialtools.database_config.integer(val: str) &#x2192; intï
+  serialtools.database_config.load_file(fn: str) &#x2192; Databaseï
 Previous Next
 ===============================================================================
 © Copyright 2023, erzo.
 Built with Sphinx using a theme provided by Read_the_Docs.
```

### Comparing `serialtools-0.4.2/docs/build/html/serialtools.html` & `serialtools-0.5.0/docs/build/html/serialtools.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools package &mdash; serialtools v0.4.2 documentation</title>
+  <title>serialtools package &mdash; serialtools v0.5.0 documentation</title>
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
-                v0.4.2
+                v0.5.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -202,14 +202,15 @@
 </li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.database.html#serialtools.database.Endianness"><code class="docutils literal notranslate"><span class="pre">Endianness</span></code></a><ul>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Endianness.BIG"><code class="docutils literal notranslate"><span class="pre">Endianness.BIG</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Endianness.LITTLE"><code class="docutils literal notranslate"><span class="pre">Endianness.LITTLE</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.database.html#serialtools.database.Message"><code class="docutils literal notranslate"><span class="pre">Message</span></code></a><ul>
+<li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Message.decode"><code class="docutils literal notranslate"><span class="pre">Message.decode()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Message.format"><code class="docutils literal notranslate"><span class="pre">Message.format()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Message.format_raw"><code class="docutils literal notranslate"><span class="pre">Message.format_raw()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Message.format_timestamp"><code class="docutils literal notranslate"><span class="pre">Message.format_timestamp()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.database.html#serialtools.database.MessageSpec"><code class="docutils literal notranslate"><span class="pre">MessageSpec</span></code></a><ul>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.MessageSpec.ADDRESS"><code class="docutils literal notranslate"><span class="pre">MessageSpec.ADDRESS</span></code></a></li>
@@ -242,17 +243,19 @@
 <li class="toctree-l2"><a class="reference internal" href="serialtools.database.html#serialtools.database.format_bytes"><code class="docutils literal notranslate"><span class="pre">format_bytes()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.database_config.html">serialtools.database_config module</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.database_config.html#serialtools.database_config.DatabaseCreator"><code class="docutils literal notranslate"><span class="pre">DatabaseCreator</span></code></a><ul>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database_config.html#serialtools.database_config.DatabaseCreator.endianness"><code class="docutils literal notranslate"><span class="pre">DatabaseCreator.endianness</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database_config.html#serialtools.database_config.DatabaseCreator.get"><code class="docutils literal notranslate"><span class="pre">DatabaseCreator.get()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="serialtools.database_config.html#serialtools.database_config.DatabaseCreator.load_file"><code class="docutils literal notranslate"><span class="pre">DatabaseCreator.load_file()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database_config.html#serialtools.database_config.DatabaseCreator.word_length_in_bits"><code class="docutils literal notranslate"><span class="pre">DatabaseCreator.word_length_in_bits</span></code></a></li>
 </ul>
 </li>
+<li class="toctree-l2"><a class="reference internal" href="serialtools.database_config.html#serialtools.database_config.LoggingCallback"><code class="docutils literal notranslate"><span class="pre">LoggingCallback</span></code></a></li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.database_config.html#serialtools.database_config.Message"><code class="docutils literal notranslate"><span class="pre">Message</span></code></a><ul>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database_config.html#serialtools.database_config.Message.init_parser"><code class="docutils literal notranslate"><span class="pre">Message.init_parser()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database_config.html#serialtools.database_config.Message.message"><code class="docutils literal notranslate"><span class="pre">Message.message</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database_config.html#serialtools.database_config.Message.run_parsed"><code class="docutils literal notranslate"><span class="pre">Message.run_parsed()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.database_config.html#serialtools.database_config.Param"><code class="docutils literal notranslate"><span class="pre">Param</span></code></a><ul>
@@ -266,14 +269,15 @@
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database_config.html#serialtools.database_config.Signal.init_parser"><code class="docutils literal notranslate"><span class="pre">Signal.init_parser()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database_config.html#serialtools.database_config.Signal.run_parsed"><code class="docutils literal notranslate"><span class="pre">Signal.run_parsed()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database_config.html#serialtools.database_config.Signal.signals"><code class="docutils literal notranslate"><span class="pre">Signal.signals</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.database_config.html#serialtools.database_config.get_database"><code class="docutils literal notranslate"><span class="pre">get_database()</span></code></a></li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.database_config.html#serialtools.database_config.integer"><code class="docutils literal notranslate"><span class="pre">integer()</span></code></a></li>
+<li class="toctree-l2"><a class="reference internal" href="serialtools.database_config.html#serialtools.database_config.load_file"><code class="docutils literal notranslate"><span class="pre">load_file()</span></code></a></li>
 </ul>
 </li>
 </ul>
 </div>
 </section>
 <section id="module-serialtools">
 <span id="module-contents"></span><h2>Module contents<a class="headerlink" href="#module-serialtools" title="Permalink to this heading"></a></h2>
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 
 
 
 
 
 
 serialtools
-v0.4.2
+v0.5.0
 [q                   ]
     * serialtools_package
           o Subpackages
                 # serialtools.apps_package
           o Submodules
                 # serialtools.bus_module
                 # serialtools.database_module
@@ -101,14 +101,15 @@
                 # Database.message_spec
                 # Database.signals
                 # Database.word_length_in_bits
           o Endianness
                 # Endianness.BIG
                 # Endianness.LITTLE
           o Message
+                # Message.decode()
                 # Message.format()
                 # Message.format_raw()
                 # Message.format_timestamp()
           o MessageSpec
                 # MessageSpec.ADDRESS
           o Reader
                 # Reader.ignore_bytes_between_messages
@@ -129,15 +130,17 @@
                 # Type.TEXT
                 # Type.UINT
           o format_bytes()
     * serialtools.database_config_module
           o DatabaseCreator
                 # DatabaseCreator.endianness
                 # DatabaseCreator.get()
+                # DatabaseCreator.load_file()
                 # DatabaseCreator.word_length_in_bits
+          o LoggingCallback
           o Message
                 # Message.init_parser()
                 # Message.message
                 # Message.run_parsed()
           o Param
                 # Param.defined_parameters
                 # Param.init_parser()
@@ -145,14 +148,15 @@
                 # Param.run_parsed()
           o Signal
                 # Signal.init_parser()
                 # Signal.run_parsed()
                 # Signal.signals
           o get_database()
           o integer()
+          o load_file()
 
 ***** Module contentsï *****
 Tools to work with a serial bus
 
 Previous Next
 ===============================================================================
 © Copyright 2023, erzo.
```

### Comparing `serialtools-0.4.2/docs/make.bat` & `serialtools-0.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.2/docs/source/conf.py` & `serialtools-0.5.0/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'serialtools'
 copyright = '2023, erzo'
 author = 'erzo'
-release = 'v0.4.2'
+release = 'v0.5.0'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ['sphinx.ext.autodoc', 'sphinx.ext.intersphinx', 'sphinx_paramlinks']
 
 templates_path = ['_templates']
```

### Comparing `serialtools-0.4.2/docs/source/index.rst` & `serialtools-0.5.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.2/prepare_for_gitlab_pages.py` & `serialtools-0.5.0/prepare_for_gitlab_pages.py`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.2/pyproject.toml` & `serialtools-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.2/release.sh` & `serialtools-0.5.0/release.sh`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.2/src/serialtools/__main__.py` & `serialtools-0.5.0/src/serialtools/__main__.py`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.2/src/serialtools/apps/decode.py` & `serialtools-0.5.0/src/serialtools/apps/decode.py`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.2/src/serialtools/apps/dump.py` & `serialtools-0.5.0/src/serialtools/apps/dump.py`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.2/src/serialtools/apps/rawsplit.py` & `serialtools-0.5.0/src/serialtools/apps/rawsplit.py`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.2/src/serialtools/apps/send.py` & `serialtools-0.5.0/src/serialtools/apps/send.py`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.2/src/serialtools/bus.py` & `serialtools-0.5.0/src/serialtools/bus.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,17 +192,17 @@
 			help_port += ", a log file or '-' to read from stdin"
 		g.add_argument('-p', '-c', '--port', '--channel', help=help_port)
 		if rx_only:
 			g.add_argument('-m', '--message')
 		parser.add_argument('-b', '--baudrate', type=int)
 		parser.set_defaults(rx_only=rx_only)
 
-	def create_args(self, *, port: 'str|None' = None, baudrate: 'int|None' = None, virtual: 'bool|None' = None) -> argparse.Namespace:
+	def create_args(self, *, port: 'str|None' = None, baudrate: 'int|None' = None, virtual: 'bool|None' = None, rx_only: bool = False) -> argparse.Namespace:
 		parser = argparse.ArgumentParser()
-		self.add_arguments(parser)
+		self.add_arguments(parser, rx_only=rx_only)
 		args: 'list[str]' = []
 		if port:
 			args.append('--port')
 			args.append(port)
 		if baudrate:
 			args.append('--baudrate')
 			args.append(str(baudrate))
```

### Comparing `serialtools-0.4.2/src/serialtools/database.py` & `serialtools-0.5.0/src/serialtools/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,26 +110,29 @@
 		timestamp = self.format_timestamp()
 		if timestamp:
 			timestamp += ' '
 
 		values = ' '.join(format_bytes(b) for b in self.values.values())
 		return timestamp + values
 
-	def format(self) -> str:
-		out = self.format_raw()
+	def decode(self) -> 'Mapping[Signal, int|float|bool|str]':
 		if 'address' in self.values:
 			address, = self.values['address']
 		else:
 			implicit_address = self.db.message_spec.implicit_address
 			if implicit_address is None:
 				raise ValueError(f"Message has neither explicit nor implicit address")
 			address = implicit_address
 
 		data = self.values['data']
-		for sig, val in self.db.decode(address, data).items():
+		return self.db.decode(address, data)
+
+	def format(self) -> str:
+		out = self.format_raw()
+		for sig, val in self.decode().items():
 			out += f"\n\t{sig.name}: {val}{sig.unit}"
 		return out
 
 
 class Reader:
 
 	ignore_bytes_between_messages = Config('reader.ignore-bytes-between-messages', [0xFF], unit='', help="If these bytes are encountered between two messages they are ignored instead of printing an error.")
```

### Comparing `serialtools-0.4.2/src/serialtools/database_config.py` & `serialtools-0.5.0/src/serialtools/database_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 
 import argparse
 import math
-from collections.abc import Sequence
+import logging
+from collections.abc import Sequence, Mapping
 
-from confattr import ConfigFileArgparseCommand, ParseException, Config, ExplicitConfig
+from confattr import ConfigFileArgparseCommand, ParseException, Config, ConfigFile, ExplicitConfig, Message as ConfigMessage, NotificationLevel
 
 from . import database as db
 
 
 def integer(val: str) -> int:
 	if '*' in val:
 		vals = [int(v, base=0) for v in val.split('*')]
@@ -108,21 +109,44 @@
 		parser.add_argument('--scale', type=float, default=1, help="A factor which is multiplied to the raw value received on the bus in order to get a value in the specified unit")
 		parser.add_argument('--offset', type=float, default=0, help="A summand which is added to the raw value received on the bus in order to get a value in the specified unit")
 		parser.add_argument('--unit', default='', help="The unit of the value")
 
 	def run_parsed(self, args: argparse.Namespace) -> None:
 		self.signals.append(db.Signal(args.name, args.type, args.address, bits=args.bits, startbit=args.startbit, lsb=args.lsb, scale=args.scale, offset=args.offset, unit=args.unit))
 
+
+#TODO: move this to confattr
+class LoggingCallback:
+
+	def __init__(self, *, logger: logging.Logger = logging.root, levels: 'Mapping[NotificationLevel, int]' = {}) -> None:
+		self.logger = logger
+		self.levels = levels
+
+	def __call__(self, msg: ConfigMessage) -> None:
+		if msg.notification_level in self.levels:
+			lvl = self.levels[msg.notification_level]
+		else:
+			lvl = getattr(logging, msg.notification_level.value.upper())
+		self.logger.log(lvl, str(msg))
+
+
 class DatabaseCreator:
 
 	word_length_in_bits = Config('db.word-size', 8, unit='bits')
 	endianness = ExplicitConfig('db.endianness', db.Endianness)
 
 	def get(self, *, require_signals: bool = True) -> db.Database:
 		if not Message.message:
 			raise ValueError(f"message structure not defined")
 		if require_signals and not Signal.signals:
 			raise ValueError("no signals defined")
 		return db.Database(Message.message, Signal.signals, endianness=self.endianness, word_length_in_bits=self.word_length_in_bits)
 
+	def load_file(self, fn: str) -> db.Database:
+		cf = ConfigFile(appname='serialtools')
+		cf.set_ui_callback(LoggingCallback())
+		cf.load_file(fn)
+		return self.get()
+
 _db_creator = DatabaseCreator()
 get_database = _db_creator.get
+load_file = _db_creator.load_file
```

### Comparing `serialtools-0.4.2/PKG-INFO` & `serialtools-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serialtools
-Version: 0.4.2
+Version: 0.5.0
 Summary: Tools to work with a serial bus
 Author-email: erzo <erzo@posteo.de>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
```

