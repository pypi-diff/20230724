# Comparing `tmp/oceanum-0.7.9.tar.gz` & `tmp/oceanum-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oceanum-0.7.9.tar", last modified: Tue Jul 11 07:09:15 2023, max compression
+gzip compressed data, was "oceanum-0.8.0.tar", last modified: Mon Jul 24 03:58:58 2023, max compression
```

## Comparing `oceanum-0.7.9.tar` & `oceanum-0.8.0.tar`

### file list

```diff
@@ -1,187 +1,70 @@
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.991456 oceanum-0.7.9/
--rw-rw-r--   0 dave      (1000) dave      (1000)     1834 2023-05-14 22:31:40.000000 oceanum-0.7.9/.gitignore
--rw-rw-r--   0 dave      (1000) dave      (1000)      167 2023-05-14 22:31:40.000000 oceanum-0.7.9/.gitlab-ci.yml
--rw-rw-r--   0 dave      (1000) dave      (1000)      151 2023-05-14 22:31:40.000000 oceanum-0.7.9/AUTHORS.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)     3501 2023-05-14 22:31:40.000000 oceanum-0.7.9/CONTRIBUTING.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)       89 2023-05-14 22:31:40.000000 oceanum-0.7.9/HISTORY.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)     1077 2023-05-14 22:31:40.000000 oceanum-0.7.9/LICENSE
--rw-rw-r--   0 dave      (1000) dave      (1000)      262 2023-05-14 22:31:40.000000 oceanum-0.7.9/MANIFEST.in
--rw-rw-r--   0 dave      (1000) dave      (1000)     2245 2023-05-14 22:31:40.000000 oceanum-0.7.9/Makefile
--rw-rw-r--   0 dave      (1000) dave      (1000)     1200 2023-07-11 07:09:15.991456 oceanum-0.7.9/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)      364 2023-05-14 22:31:40.000000 oceanum-0.7.9/README.md
--rw-rw-r--   0 dave      (1000) dave      (1000)      788 2023-05-14 22:31:40.000000 oceanum-0.7.9/README.rst
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.839452 oceanum-0.7.9/docs/
--rw-rw-r--   0 dave      (1000) dave      (1000)      639 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/Makefile
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.827452 oceanum-0.7.9/docs/_build/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.851452 oceanum-0.7.9/docs/_build/doctrees/
--rw-rw-r--   0 dave      (1000) dave      (1000)     7953 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/doctrees/about.doctree
--rw-rw-r--   0 dave      (1000) dave      (1000)     9406 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/doctrees/api.doctree
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.827452 oceanum-0.7.9/docs/_build/doctrees/classes/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.871453 oceanum-0.7.9/docs/_build/doctrees/classes/datamesh/
--rw-rw-r--   0 dave      (1000) dave      (1000)    29966 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/doctrees/classes/datamesh/oceanum.datamesh.Catalog.doctree
--rw-rw-r--   0 dave      (1000) dave      (1000)   110431 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/doctrees/classes/datamesh/oceanum.datamesh.Connector.doctree
--rw-rw-r--   0 dave      (1000) dave      (1000)    69623 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/doctrees/classes/datamesh/oceanum.datamesh.Datasource.doctree
--rw-rw-r--   0 dave      (1000) dave      (1000)    33031 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/doctrees/classes/datamesh/oceanum.datamesh.Query.doctree
--rw-rw-r--   0 dave      (1000) dave      (1000)   188704 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/doctrees/environment.pickle
--rw-rw-r--   0 dave      (1000) dave      (1000)     2827 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/doctrees/index.doctree
--rw-rw-r--   0 dave      (1000) dave      (1000)     7395 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/doctrees/installation.doctree
--rw-rw-r--   0 dave      (1000) dave      (1000)     2701 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/doctrees/modules.doctree
--rw-rw-r--   0 dave      (1000) dave      (1000)   366728 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/doctrees/oceanum.datamesh.doctree
--rw-rw-r--   0 dave      (1000) dave      (1000)     4792 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/doctrees/oceanum.doctree
--rw-rw-r--   0 dave      (1000) dave      (1000)     7535 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/doctrees/usage.doctree
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.891453 oceanum-0.7.9/docs/_build/html/
--rw-rw-r--   0 dave      (1000) dave      (1000)      230 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/.buildinfo
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.891453 oceanum-0.7.9/docs/_build/html/_modules/
--rw-rw-r--   0 dave      (1000) dave      (1000)     6581 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_modules/index.html
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.827452 oceanum-0.7.9/docs/_build/html/_modules/oceanum/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.895454 oceanum-0.7.9/docs/_build/html/_modules/oceanum/datamesh/
--rw-rw-r--   0 dave      (1000) dave      (1000)    20408 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_modules/oceanum/datamesh/catalog.html
--rw-rw-r--   0 dave      (1000) dave      (1000)    85038 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_modules/oceanum/datamesh/connection.html
--rw-rw-r--   0 dave      (1000) dave      (1000)    52867 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_modules/oceanum/datamesh/datasource.html
--rw-rw-r--   0 dave      (1000) dave      (1000)    35899 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_modules/oceanum/datamesh/query.html
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.907454 oceanum-0.7.9/docs/_build/html/_sources/
--rw-rw-r--   0 dave      (1000) dave      (1000)       73 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_sources/about.rst.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)      593 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_sources/api.rst.txt
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.827452 oceanum-0.7.9/docs/_build/html/_sources/classes/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.911454 oceanum-0.7.9/docs/_build/html/_sources/classes/datamesh/
--rw-rw-r--   0 dave      (1000) dave      (1000)      406 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_sources/classes/datamesh/oceanum.datamesh.Catalog.rst.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)      713 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_sources/classes/datamesh/oceanum.datamesh.Connector.rst.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)      131 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_sources/classes/datamesh/oceanum.datamesh.Datasource.rst.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)      116 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_sources/classes/datamesh/oceanum.datamesh.Query.rst.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)      160 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_sources/index.rst.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)     1133 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_sources/installation.rst.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       58 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_sources/modules.rst.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)      967 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_sources/oceanum.datamesh.rst.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)      365 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_sources/oceanum.rst.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)     1437 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_sources/usage.rst.txt
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.939455 oceanum-0.7.9/docs/_build/html/_static/
--rw-rw-r--   0 dave      (1000) dave      (1000)     4418 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-rw-r--   0 dave      (1000) dave      (1000)      121 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/autodoc_pydantic.css
--rw-rw-r--   0 dave      (1000) dave      (1000)    11521 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/banner_dark.svg
--rw-rw-r--   0 dave      (1000) dave      (1000)    14621 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/basic.css
--rw-rw-r--   0 dave      (1000) dave      (1000)     4472 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/doctools.js
--rw-rw-r--   0 dave      (1000) dave      (1000)      419 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/documentation_options.js
--rw-rw-r--   0 dave      (1000) dave      (1000)      286 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/file.png
--rw-rw-r--   0 dave      (1000) dave      (1000)   288580 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/jquery-3.6.0.js
--rw-rw-r--   0 dave      (1000) dave      (1000)    89501 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/jquery.js
--rw-rw-r--   0 dave      (1000) dave      (1000)     4758 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/language_data.js
--rw-rw-r--   0 dave      (1000) dave      (1000)       90 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/minus.png
--rw-rw-r--   0 dave      (1000) dave      (1000)       90 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/plus.png
--rw-rw-r--   0 dave      (1000) dave      (1000)    15069 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/pygments.css
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.943455 oceanum-0.7.9/docs/_build/html/_static/scripts/
--rw-rw-r--   0 dave      (1000) dave      (1000)    88212 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/scripts/pydata-sphinx-theme.js
--rw-rw-r--   0 dave      (1000) dave      (1000)    18215 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/searchtools.js
--rw-rw-r--   0 dave      (1000) dave      (1000)     4712 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/sphinx_highlight.js
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.943455 oceanum-0.7.9/docs/_build/html/_static/styles/
--rw-rw-r--   0 dave      (1000) dave      (1000)   171194 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/styles/pydata-sphinx-theme.css
--rw-rw-r--   0 dave      (1000) dave      (1000)      106 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/styles/theme.css
--rw-rw-r--   0 dave      (1000) dave      (1000)    68420 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/underscore-1.13.1.js
--rw-rw-r--   0 dave      (1000) dave      (1000)    19530 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/underscore.js
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.827452 oceanum-0.7.9/docs/_build/html/_static/vendor/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.827452 oceanum-0.7.9/docs/_build/html/_static/vendor/fontawesome/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.943455 oceanum-0.7.9/docs/_build/html/_static/vendor/fontawesome/5.13.0/
--rw-rw-r--   0 dave      (1000) dave      (1000)     1548 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/vendor/fontawesome/5.13.0/LICENSE.txt
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.943455 oceanum-0.7.9/docs/_build/html/_static/vendor/fontawesome/5.13.0/css/
--rw-rw-r--   0 dave      (1000) dave      (1000)    58578 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/vendor/fontawesome/5.13.0/css/all.min.css
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.967455 oceanum-0.7.9/docs/_build/html/_static/vendor/fontawesome/5.13.0/webfonts/
--rw-rw-r--   0 dave      (1000) dave      (1000)   133034 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.eot
--rw-rw-r--   0 dave      (1000) dave      (1000)   715890 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.svg
--rw-rw-r--   0 dave      (1000) dave      (1000)   132728 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.ttf
--rw-rw-r--   0 dave      (1000) dave      (1000)    89824 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.woff
--rw-rw-r--   0 dave      (1000) dave      (1000)    76612 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.woff2
--rw-rw-r--   0 dave      (1000) dave      (1000)    34390 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.eot
--rw-rw-r--   0 dave      (1000) dave      (1000)   144322 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.svg
--rw-rw-r--   0 dave      (1000) dave      (1000)    34092 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.ttf
--rw-rw-r--   0 dave      (1000) dave      (1000)    16800 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.woff
--rw-rw-r--   0 dave      (1000) dave      (1000)    13584 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.woff2
--rw-rw-r--   0 dave      (1000) dave      (1000)   202902 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.eot
--rw-rw-r--   0 dave      (1000) dave      (1000)   897426 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.svg
--rw-rw-r--   0 dave      (1000) dave      (1000)   202616 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.ttf
--rw-rw-r--   0 dave      (1000) dave      (1000)   103300 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.woff
--rw-rw-r--   0 dave      (1000) dave      (1000)    79444 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.woff2
--rw-rw-r--   0 dave      (1000) dave      (1000)     1361 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/webpack-macros.html
--rw-rw-r--   0 dave      (1000) dave      (1000)    10044 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/about.html
--rw-rw-r--   0 dave      (1000) dave      (1000)     9934 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/api.html
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.827452 oceanum-0.7.9/docs/_build/html/classes/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.971455 oceanum-0.7.9/docs/_build/html/classes/datamesh/
--rw-rw-r--   0 dave      (1000) dave      (1000)    18843 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/classes/datamesh/oceanum.datamesh.Catalog.html
--rw-rw-r--   0 dave      (1000) dave      (1000)    44376 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/classes/datamesh/oceanum.datamesh.Connector.html
--rw-rw-r--   0 dave      (1000) dave      (1000)    37152 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/classes/datamesh/oceanum.datamesh.Datasource.html
--rw-rw-r--   0 dave      (1000) dave      (1000)    21536 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/classes/datamesh/oceanum.datamesh.Query.html
--rw-rw-r--   0 dave      (1000) dave      (1000)    35493 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/genindex.html
--rw-rw-r--   0 dave      (1000) dave      (1000)     8374 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/index.html
--rw-rw-r--   0 dave      (1000) dave      (1000)     9389 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/installation.html
--rw-rw-r--   0 dave      (1000) dave      (1000)     8086 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/modules.html
--rw-rw-r--   0 dave      (1000) dave      (1000)     1427 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/objects.inv
--rw-rw-r--   0 dave      (1000) dave      (1000)   182788 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/oceanum.datamesh.html
--rw-rw-r--   0 dave      (1000) dave      (1000)    32052 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/oceanum.html
--rw-rw-r--   0 dave      (1000) dave      (1000)     7827 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/py-modindex.html
--rw-rw-r--   0 dave      (1000) dave      (1000)     6915 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/search.html
--rw-rw-r--   0 dave      (1000) dave      (1000)    33738 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/searchindex.js
--rw-rw-r--   0 dave      (1000) dave      (1000)    13261 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/usage.html
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.831452 oceanum-0.7.9/docs/_templates/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.971455 oceanum-0.7.9/docs/_templates/autosummary/
--rw-rw-r--   0 dave      (1000) dave      (1000)      481 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_templates/autosummary/class.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)       73 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/about.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      593 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/api.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)    11521 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/banner_dark.svg
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.831452 oceanum-0.7.9/docs/classes/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.975456 oceanum-0.7.9/docs/classes/datamesh/
--rw-rw-r--   0 dave      (1000) dave      (1000)      406 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/classes/datamesh/oceanum.datamesh.Catalog.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      713 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/classes/datamesh/oceanum.datamesh.Connector.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      131 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/classes/datamesh/oceanum.datamesh.Datasource.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      116 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/classes/datamesh/oceanum.datamesh.Query.rst
--rwxrwxr-x   0 dave      (1000) dave      (1000)     5654 2023-07-11 03:17:01.000000 oceanum-0.7.9/docs/conf.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      522 2023-07-11 03:17:01.000000 oceanum-0.7.9/docs/index.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)     1133 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/installation.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      801 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/make.bat
--rw-rw-r--   0 dave      (1000) dave      (1000)       58 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/modules.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)    15086 2023-07-11 03:17:01.000000 oceanum-0.7.9/docs/oceanum-favicon.ico
--rw-rw-r--   0 dave      (1000) dave      (1000)      967 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/oceanum.datamesh.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      365 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/oceanum.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)       45 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/requirements.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)     1437 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/usage.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-07-11 03:28:18.000000 oceanum-0.7.9/log.txt
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.979456 oceanum-0.7.9/oceanum/
--rw-rw-r--   0 dave      (1000) dave      (1000)      292 2023-05-14 22:31:40.000000 oceanum-0.7.9/oceanum/.editorconfig
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.983456 oceanum-0.7.9/oceanum/.github/
--rw-rw-r--   0 dave      (1000) dave      (1000)      318 2023-05-14 22:31:40.000000 oceanum-0.7.9/oceanum/.github/ISSUE_TEMPLATE.md
--rw-rw-r--   0 dave      (1000) dave      (1000)     1172 2023-05-14 22:31:40.000000 oceanum-0.7.9/oceanum/.gitignore
--rw-rw-r--   0 dave      (1000) dave      (1000)      290 2023-05-14 22:31:40.000000 oceanum-0.7.9/oceanum/.travis.yml
--rw-rw-r--   0 dave      (1000) dave      (1000)      474 2023-07-11 03:18:32.000000 oceanum-0.7.9/oceanum/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      313 2023-05-14 22:31:40.000000 oceanum-0.7.9/oceanum/cli.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.983456 oceanum-0.7.9/oceanum/datamesh/
--rw-rw-r--   0 dave      (1000) dave      (1000)      122 2023-05-14 22:31:40.000000 oceanum-0.7.9/oceanum/datamesh/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     3425 2023-05-14 22:31:40.000000 oceanum-0.7.9/oceanum/datamesh/catalog.py
--rw-rw-r--   0 dave      (1000) dave      (1000)    20940 2023-07-11 03:58:41.000000 oceanum-0.7.9/oceanum/datamesh/connection.py
--rw-rw-r--   0 dave      (1000) dave      (1000)    10443 2023-07-11 03:34:29.000000 oceanum-0.7.9/oceanum/datamesh/datasource.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      144 2023-05-14 22:31:40.000000 oceanum-0.7.9/oceanum/datamesh/exceptions.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     7537 2023-07-11 03:34:33.000000 oceanum-0.7.9/oceanum/datamesh/query.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     5037 2023-06-14 04:46:09.000000 oceanum-0.7.9/oceanum/datamesh/zarr.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.983456 oceanum-0.7.9/oceanum.egg-info/
--rw-rw-r--   0 dave      (1000) dave      (1000)     1200 2023-07-11 07:09:14.000000 oceanum-0.7.9/oceanum.egg-info/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)     5979 2023-07-11 07:09:15.000000 oceanum-0.7.9/oceanum.egg-info/SOURCES.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-07-11 07:09:14.000000 oceanum-0.7.9/oceanum.egg-info/dependency_links.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       45 2023-07-11 07:09:15.000000 oceanum-0.7.9/oceanum.egg-info/entry_points.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-07-11 07:09:14.000000 oceanum-0.7.9/oceanum.egg-info/not-zip-safe
--rw-rw-r--   0 dave      (1000) dave      (1000)      128 2023-07-11 07:09:15.000000 oceanum-0.7.9/oceanum.egg-info/requires.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        8 2023-07-11 07:09:15.000000 oceanum-0.7.9/oceanum.egg-info/top_level.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)      126 2023-07-11 07:03:39.000000 oceanum-0.7.9/requirements.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)      124 2023-05-14 22:31:40.000000 oceanum-0.7.9/requirements_dev.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)      419 2023-07-11 07:09:15.991456 oceanum-0.7.9/setup.cfg
--rw-rw-r--   0 dave      (1000) dave      (1000)     1373 2023-05-14 22:31:40.000000 oceanum-0.7.9/setup.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.987456 oceanum-0.7.9/tests/
--rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-05-14 22:31:40.000000 oceanum-0.7.9/tests/__init__.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.991456 oceanum-0.7.9/tests/data/
--rw-rw-r--   0 dave      (1000) dave      (1000)    21010 2023-05-14 22:31:40.000000 oceanum-0.7.9/tests/data/grid_data_1.nc
--rw-rw-r--   0 dave      (1000) dave      (1000)  2029589 2023-05-14 22:31:40.000000 oceanum-0.7.9/tests/data/ocean_test_1.mp4
--rw-rw-r--   0 dave      (1000) dave      (1000)     1727 2023-05-14 22:31:40.000000 oceanum-0.7.9/tests/data/point_data_1.csv
--rw-rw-r--   0 dave      (1000) dave      (1000)     1222 2023-05-14 22:31:40.000000 oceanum-0.7.9/tests/test_catalog.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1072 2023-05-14 22:31:40.000000 oceanum-0.7.9/tests/test_datamesh_connect.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1643 2023-05-14 22:31:40.000000 oceanum-0.7.9/tests/test_datamesh_load.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2578 2023-05-14 22:31:40.000000 oceanum-0.7.9/tests/test_datamesh_query.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     3255 2023-05-14 22:31:40.000000 oceanum-0.7.9/tests/test_datamesh_write.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2936 2023-05-14 22:31:40.000000 oceanum-0.7.9/tests/test_datasource.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1482 2023-05-14 22:31:40.000000 oceanum-0.7.9/tests/test_query.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      805 2023-05-14 22:31:40.000000 oceanum-0.7.9/tests/test_video_compat.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      618 2023-05-14 22:31:40.000000 oceanum-0.7.9/tox.ini
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-24 03:58:58.823247 oceanum-0.8.0/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      151 2023-05-14 22:31:40.000000 oceanum-0.8.0/AUTHORS.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3501 2023-05-14 22:31:40.000000 oceanum-0.8.0/CONTRIBUTING.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)       89 2023-05-14 22:31:40.000000 oceanum-0.8.0/HISTORY.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1077 2023-05-14 22:31:40.000000 oceanum-0.8.0/LICENSE
+-rw-rw-r--   0 dave      (1000) dave      (1000)      262 2023-05-14 22:31:40.000000 oceanum-0.8.0/MANIFEST.in
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1180 2023-07-24 03:58:58.823247 oceanum-0.8.0/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)      788 2023-05-14 22:31:40.000000 oceanum-0.8.0/README.rst
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-24 03:58:58.811247 oceanum-0.8.0/docs/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      639 2023-05-14 22:31:40.000000 oceanum-0.8.0/docs/Makefile
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-24 03:58:58.807247 oceanum-0.8.0/docs/_build/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-24 03:58:58.807247 oceanum-0.8.0/docs/_build/html/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-24 03:58:58.811247 oceanum-0.8.0/docs/_build/html/_static/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      286 2023-05-14 22:31:40.000000 oceanum-0.8.0/docs/_build/html/_static/file.png
+-rw-rw-r--   0 dave      (1000) dave      (1000)       90 2023-05-14 22:31:40.000000 oceanum-0.8.0/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 dave      (1000) dave      (1000)       90 2023-05-14 22:31:40.000000 oceanum-0.8.0/docs/_build/html/_static/plus.png
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-24 03:58:58.807247 oceanum-0.8.0/docs/_templates/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-24 03:58:58.811247 oceanum-0.8.0/docs/_templates/autosummary/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      481 2023-05-14 22:31:40.000000 oceanum-0.8.0/docs/_templates/autosummary/class.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)       73 2023-05-14 22:31:40.000000 oceanum-0.8.0/docs/about.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      593 2023-05-14 22:31:40.000000 oceanum-0.8.0/docs/api.rst
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-24 03:58:58.807247 oceanum-0.8.0/docs/classes/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-24 03:58:58.815247 oceanum-0.8.0/docs/classes/datamesh/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      406 2023-05-14 22:31:40.000000 oceanum-0.8.0/docs/classes/datamesh/oceanum.datamesh.Catalog.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      713 2023-05-14 22:31:40.000000 oceanum-0.8.0/docs/classes/datamesh/oceanum.datamesh.Connector.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      131 2023-05-14 22:31:40.000000 oceanum-0.8.0/docs/classes/datamesh/oceanum.datamesh.Datasource.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      116 2023-05-14 22:31:40.000000 oceanum-0.8.0/docs/classes/datamesh/oceanum.datamesh.Query.rst
+-rwxrwxr-x   0 dave      (1000) dave      (1000)     5654 2023-07-11 03:17:01.000000 oceanum-0.8.0/docs/conf.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      522 2023-07-11 03:17:01.000000 oceanum-0.8.0/docs/index.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1133 2023-05-14 22:31:40.000000 oceanum-0.8.0/docs/installation.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      801 2023-05-14 22:31:40.000000 oceanum-0.8.0/docs/make.bat
+-rw-rw-r--   0 dave      (1000) dave      (1000)       58 2023-05-14 22:31:40.000000 oceanum-0.8.0/docs/modules.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      967 2023-05-14 22:31:40.000000 oceanum-0.8.0/docs/oceanum.datamesh.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      365 2023-05-14 22:31:40.000000 oceanum-0.8.0/docs/oceanum.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1437 2023-05-14 22:31:40.000000 oceanum-0.8.0/docs/usage.rst
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-24 03:58:58.815247 oceanum-0.8.0/oceanum/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      474 2023-07-24 02:08:43.000000 oceanum-0.8.0/oceanum/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      313 2023-05-14 22:31:40.000000 oceanum-0.8.0/oceanum/cli.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-24 03:58:58.819247 oceanum-0.8.0/oceanum/datamesh/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      122 2023-05-14 22:31:40.000000 oceanum-0.8.0/oceanum/datamesh/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3425 2023-05-14 22:31:40.000000 oceanum-0.8.0/oceanum/datamesh/catalog.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    21008 2023-07-24 03:18:35.000000 oceanum-0.8.0/oceanum/datamesh/connection.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    11333 2023-07-24 03:03:59.000000 oceanum-0.8.0/oceanum/datamesh/datasource.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      144 2023-05-14 22:31:40.000000 oceanum-0.8.0/oceanum/datamesh/exceptions.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     7849 2023-07-24 03:17:32.000000 oceanum-0.8.0/oceanum/datamesh/query.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     5037 2023-06-14 04:46:09.000000 oceanum-0.8.0/oceanum/datamesh/zarr.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-24 03:58:58.815247 oceanum-0.8.0/oceanum.egg-info/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1180 2023-07-24 03:58:58.000000 oceanum-0.8.0/oceanum.egg-info/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1384 2023-07-24 03:58:58.000000 oceanum-0.8.0/oceanum.egg-info/SOURCES.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-07-24 03:58:58.000000 oceanum-0.8.0/oceanum.egg-info/dependency_links.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       45 2023-07-24 03:58:58.000000 oceanum-0.8.0/oceanum.egg-info/entry_points.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-07-24 03:58:58.000000 oceanum-0.8.0/oceanum.egg-info/not-zip-safe
+-rw-rw-r--   0 dave      (1000) dave      (1000)      128 2023-07-24 03:58:58.000000 oceanum-0.8.0/oceanum.egg-info/requires.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        8 2023-07-24 03:58:58.000000 oceanum-0.8.0/oceanum.egg-info/top_level.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)      419 2023-07-24 03:58:58.823247 oceanum-0.8.0/setup.cfg
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1373 2023-05-14 22:31:40.000000 oceanum-0.8.0/setup.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-24 03:58:58.819247 oceanum-0.8.0/tests/
+-rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-05-14 22:31:40.000000 oceanum-0.8.0/tests/__init__.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-24 03:58:58.823247 oceanum-0.8.0/tests/data/
+-rw-rw-r--   0 dave      (1000) dave      (1000)    21010 2023-05-14 22:31:40.000000 oceanum-0.8.0/tests/data/grid_data_1.nc
+-rw-rw-r--   0 dave      (1000) dave      (1000)  2029589 2023-05-14 22:31:40.000000 oceanum-0.8.0/tests/data/ocean_test_1.mp4
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1727 2023-05-14 22:31:40.000000 oceanum-0.8.0/tests/data/point_data_1.csv
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1222 2023-05-14 22:31:40.000000 oceanum-0.8.0/tests/test_catalog.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1072 2023-05-14 22:31:40.000000 oceanum-0.8.0/tests/test_datamesh_connect.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1643 2023-05-14 22:31:40.000000 oceanum-0.8.0/tests/test_datamesh_load.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2578 2023-05-14 22:31:40.000000 oceanum-0.8.0/tests/test_datamesh_query.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3255 2023-05-14 22:31:40.000000 oceanum-0.8.0/tests/test_datamesh_write.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2958 2023-07-11 22:58:57.000000 oceanum-0.8.0/tests/test_datasource.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1482 2023-07-11 23:07:04.000000 oceanum-0.8.0/tests/test_query.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      805 2023-05-14 22:31:40.000000 oceanum-0.8.0/tests/test_video_compat.py
```

### Comparing `oceanum-0.7.9/CONTRIBUTING.rst` & `oceanum-0.8.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.9/LICENSE` & `oceanum-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.9/PKG-INFO` & `oceanum-0.8.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: oceanum
-Version: 0.7.9
+Version: 0.8.0
 Summary: Library for oceanum.io services
 Home-page: https://github.com/oceanum/oceanum-python
 Author: Oceanum Developers
 Author-email: developers@oceanum.science
 License: MIT license
 Keywords: oceanum
-Platform: UNKNOWN
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ==============
 oceanum-python
 ==============
 
@@ -49,9 +48,7 @@
 History
 =======
 
 0.4.2 (2022-05-20)
 ------------------
 
 * First release on PyPI.
-
-
```

### Comparing `oceanum-0.7.9/README.rst` & `oceanum-0.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.9/docs/Makefile` & `oceanum-0.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.9/docs/_build/html/_sources/api.rst.txt` & `oceanum-0.8.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.9/docs/_build/html/_sources/classes/datamesh/oceanum.datamesh.Connector.rst.txt` & `oceanum-0.8.0/docs/classes/datamesh/oceanum.datamesh.Connector.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.9/docs/_build/html/_sources/installation.rst.txt` & `oceanum-0.8.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.9/docs/_build/html/_sources/oceanum.datamesh.rst.txt` & `oceanum-0.8.0/docs/oceanum.datamesh.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.9/docs/_build/html/_sources/usage.rst.txt` & `oceanum-0.8.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.9/docs/conf.py` & `oceanum-0.8.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.9/docs/index.rst` & `oceanum-0.8.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.9/docs/make.bat` & `oceanum-0.8.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.9/oceanum/datamesh/catalog.py` & `oceanum-0.8.0/oceanum/datamesh/catalog.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.9/oceanum/datamesh/connection.py` & `oceanum-0.8.0/oceanum/datamesh/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import pandas
 import shapely
 import warnings
 import tempfile
 from urllib.parse import urlparse
 import asyncio
 from functools import wraps, partial
+from contextlib import contextmanager
 
 from .datasource import Datasource, _datasource_props, _datasource_driver
 from .catalog import Catalog
 from .query import Query, Stage, Container, TimeFilter, GeoFilter
 from .zarr import zarr_write
 from .exceptions import DatameshConnectError, DatameshQueryError, DatameshWriteError
 
@@ -41,14 +42,25 @@
             loop = asyncio.get_event_loop()
         pfunc = partial(func, *args, **kwargs)
         return await loop.run_in_executor(executor, pfunc)
 
     return run
 
 
+# Windows compatibility tempfile
+@contextmanager
+def tempFile(mode="wb"):
+    file = tempfile.NamedTemporaryFile(mode, delete=False)
+    try:
+        yield file
+    finally:
+        file.close()
+        os.unlink(file.name)
+
+
 class Connector(object):
     """Datamesh connector class.
 
     All datamesh operations are methods of this class
     """
 
     def __init__(
@@ -194,15 +206,15 @@
             )
         if not resp.status_code == 200:
             msg = resp.json()["detail"]
             raise DatameshConnectError(msg)
         return Datasource(**resp.json())
 
     def _stage_request(self, query, cache=False):
-        qhash = hashlib.sha224(query.json().encode()).hexdigest()
+        qhash = hashlib.sha224(query.model_dump_json().encode()).hexdigest()
 
         resp = requests.post(
             f"{self._gateway}/oceanql/stage/",
             headers=self._auth_headers,
             data=query.json(),
         )
         if resp.status_code >= 400:
@@ -235,24 +247,23 @@
             resp = requests.post(
                 f"{self._gateway}/oceanql/", headers=headers, data=query.json()
             )
             if resp.status_code >= 400:
                 msg = resp.json()["detail"]
                 raise DatameshQueryError(msg)
             else:
-                with tempfile.NamedTemporaryFile("wb", delete=False) as f:
+                with tempFile("wb") as f:
                     f.write(resp.content)
                     f.seek(0)
                     if stage.container == Container.Dataset:
                         ds = xarray.load_dataset(f.name)
                     elif stage.container == Container.GeoDataFrame:
                         ds = geopandas.read_parquet(f.name)
                     else:
                         ds = pandas.read_parquet(f.name)
-                os.unlink(f.name)
                 return ds
 
     def get_catalog(self, search=None, timefilter=None, geofilter=None):
         """Get datamesh catalog
 
         Args:
             search (string, optional): Search string for filtering datasources
@@ -446,39 +457,37 @@
                 "Datasource ID must only contain lowercase letters, numbers, dashes and underscores"
             )
         try:
             ds = self.get_datasource(datasource_id)
         except DatameshConnectError as e:
             overwrite = True
         if data is not None:
-            with tempfile.NamedTemporaryFile("w+b", delete=False) as f:
-                try:
-                    if isinstance(data, xarray.Dataset):
-                        ds = zarr_write(
-                            self,
-                            datasource_id,
-                            data,
-                            append,
-                            overwrite,
-                        )
-                    else:
+            try:
+                if isinstance(data, xarray.Dataset):
+                    ds = zarr_write(
+                        self,
+                        datasource_id,
+                        data,
+                        append,
+                        overwrite,
+                    )
+                else:
+                    with tempFile("w+b") as f:
                         data.to_parquet(f, index=True)
                         f.seek(0)
                         ds = self._data_write(
                             datasource_id,
                             f.read(),
                             "application/parquet",
                             append,
                             overwrite,
                         )
-                    ds._exists = True
-                except Exception as e:
-                    raise DatameshWriteError(e)
-                finally:
-                    os.remove(f.name)
+                ds._exists = True
+            except Exception as e:
+                raise DatameshWriteError(e)
         elif overwrite:
             ds = Datasource(id=datasource_id, geom=geometry, **properties)
         for key in properties:
             if key not in ["driver", "schema"]:
                 setattr(ds, key, properties[key])
         if geometry:
             ds.geom = geometry
```

### Comparing `oceanum-0.7.9/oceanum/datamesh/datasource.py` & `oceanum-0.8.0/oceanum/datamesh/datasource.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,56 +2,58 @@
 import datetime
 import re
 import pandas
 import geopandas
 import xarray
 import asyncio
 import shapely
-from pydantic import BaseModel, Field, AnyHttpUrl, PrivateAttr, constr
+from pydantic import (
+    ConfigDict,
+    BaseModel,
+    Field,
+    AnyHttpUrl,
+    PrivateAttr,
+    constr,
+    BeforeValidator,
+)
+from pydantic_core import core_schema
 from pydantic.json import timedelta_isoformat
 from typing_extensions import Annotated
 from typing import Optional, Dict, Union, List, NamedTuple
 from enum import Enum
 from .query import Query, Timestamp
 
 
-def geojson(shape):
-    return shape.__geo_interface__
-
-
 class DatasourceException(Exception):
     pass
 
 
-class Timeperiod(datetime.timedelta):
-    @classmethod
-    def __get_validators__(cls):
-        yield cls.validate
+def parse_period(period):
+    try:
+        m = re.match(
+            r"^P(?:(\d+)Y)?(?:(\d+)M)?(?:(\d+)D)?T?(?:(\d+)H)?(?:(\d+)M)?(?:(\d+(?:.\d+)?)S)?$",
+            period,
+        )
+        if m is None:
+            raise serializers.ValidationError("invalid ISO 8601 duration string")
+        days = 0
+        hours = 0
+        minutes = 0
+        if m[3]:
+            days = int(m[3])
+        if m[4]:
+            hours = int(m[4])
+        if m[5]:
+            minutes = int(m[5])
+        return datetime.timedelta(days=days, hours=hours, minutes=minutes)
+    except:
+        raise "Period string not valid"
 
-    @classmethod
-    def validate(cls, period):
-        try:
-            m = re.match(
-                r"^P(?:(\d+)Y)?(?:(\d+)M)?(?:(\d+)D)?T?(?:(\d+)H)?(?:(\d+)M)?(?:(\d+(?:.\d+)?)S)?$",
-                period,
-            )
-            if m is None:
-                raise serializers.ValidationError("invalid ISO 8601 duration string")
-            days = 0
-            hours = 0
-            minutes = 0
-            if m[3]:
-                days = int(m[3])
-            if m[4]:
-                hours = int(m[4])
-            if m[5]:
-                minutes = int(m[5])
-            return datetime.timedelta(days=days, hours=hours, minutes=minutes)
-        except:
-            raise "Period string not valid"
+
+Timeperiod = Annotated[datetime.timedelta, BeforeValidator(parse_period)]
 
 
 LonField = Annotated[
     Union[float, int],
     Field(
         title="Coordinate longitude",
         ge=-180,
@@ -65,41 +67,67 @@
         title="Coordinate latitude",
         ge=-90,
         le=90,
     ),
 ]
 
 
-class Geometry:
+class _GeometryAnnotation:
     @classmethod
-    def __get_validators__(cls):
-        yield cls.validate
+    def __get_pydantic_core_schema__(cls, source, handler):
+        def validate(geometry):
+            if isinstance(geometry, dict):
+                try:
+                    geometry = shapely.geometry.shape(geometry)
+                except:
+                    "Not a valid GeoJSON dictionary"
+            if (
+                isinstance(geometry, shapely.geometry.Point)
+                or isinstance(geometry, shapely.geometry.MultiPoint)
+                or isinstance(geometry, shapely.geometry.Polygon)
+            ):
+                return geometry
+            else:
+                raise BaseException("Geometry must be Point, MultiPoint or Polygon")
+
+        from_geometry_schema = core_schema.no_info_plain_validator_function(validate)
+
+        return core_schema.json_or_python_schema(
+            json_schema=from_geometry_schema,
+            python_schema=core_schema.union_schema(
+                [
+                    core_schema.is_instance_schema(shapely.geometry.Point),
+                    core_schema.is_instance_schema(shapely.geometry.MultiPoint),
+                    core_schema.is_instance_schema(shapely.geometry.Polygon),
+                    from_geometry_schema,
+                ]
+            ),
+            serialization=core_schema.plain_serializer_function_ser_schema(
+                lambda x: shapely.to_geojson(x)
+            ),
+        )
 
     @classmethod
-    def validate(cls, geometry):
-        if isinstance(geometry, dict):
-            try:
-                geometry = shapely.geometry.shape(geometry)
-            except:
-                "Not a valid GeoJSON dictionary"
-        if (
-            isinstance(geometry, shapely.geometry.Point)
-            or isinstance(geometry, shapely.geometry.MultiPoint)
-            or isinstance(geometry, shapely.geometry.Polygon)
-        ):
-            return geometry
-        else:
-            raise BaseException("Geometry must be Point, MultiPoint or Polygon")
+    def __get_pydantic_json_schema__(cls, schema, handler):
+        return {"type": "object"}
+
+
+Geometry = Annotated[
+    Union[
+        shapely.geometry.Point, shapely.geometry.MultiPoint, shapely.geometry.Polygon
+    ],
+    _GeometryAnnotation,
+]
 
 
 class Schema(BaseModel):
-    attrs: Optional[dict] = Field(title="Global attributes")
-    dims: Optional[dict] = Field(title="Dimensions")
-    coords: Optional[dict] = Field(title="Coordinates")
-    data_vars: Optional[dict] = Field(title="Data variables")
+    attrs: Optional[dict] = Field(title="Global attributes", default={})
+    dims: Optional[dict] = Field(title="Dimensions", default={})
+    coords: Optional[dict] = Field(title="Coordinates", default={})
+    data_vars: Optional[dict] = Field(title="Data variables", default={})
 
 
 class Coordinates(Enum):
     """Coordinate keys"""
 
     Ensemble = "e"
     Rasterband = "b"
@@ -148,15 +176,15 @@
     id: str = Field(
         title="Datasource ID",
         description="Unique ID for the datasource",
         min_length=3,
         max_length=80,
         strip_whitespace=True,
         to_lower=True,
-        regex=r"^[a-z0-9-_]+$",
+        pattern=r"^[a-z0-9-_]+$",
     )
     name: str = Field(
         title="Datasource name",
         description="Human readable name for the datasource",
         max_length=64,
     )
     description: Optional[str] = Field(
@@ -199,15 +227,15 @@
         description="Additional datasource descriptive metadata",
         default="",
     )
     dataschema: Optional[Schema] = Field(
         alias="schema",
         title="Schema",
         description="Datasource schema",
-        default=Schema(attrs={}, dims=[], coords={}, data_vars={}),
+        default=Schema(attrs={}, dims={}, coords={}, data_vars={}),
     )
     coordinates: Dict[Coordinates, str] = Field(
         title="Coordinate keys",
         description="""
         Coordinates in datasource, referenced by standard coordinate keys. The dictionary keys map to coordinates variables in the datasource.
             Ensemble: "e"
             Rasterband: "b"
@@ -232,36 +260,29 @@
         description="URL to further details about the datasource",
         default=None,
     )
     last_modified: Optional[datetime.datetime] = Field(
         title="Last modified time",
         description="Last time datasource was modified",
         default=datetime.datetime.utcnow(),
-        allow_mutation=False,
+        frozen=True,
     )
     driver_args: Optional[dict] = Field(
         alias="args",
         title="Driver arguments",
         description="Driver arguments for datasource. These are driver dependent.",
-        allow_mutation=False,
+        frozen=True,
         default={},
     )
-    driver: str = Field(allow_mutation=False)
+    driver: str = Field(frozen=True)
     _exists: bool = PrivateAttr(default=False)
     _detail: bool = PrivateAttr(default=False)
-
-    class Config:
-        use_enum_values = True
-        validate_assignment = True
-        json_encoders = {
-            Timeperiod: timedelta_isoformat,
-            shapely.geometry.Point: geojson,
-            shapely.geometry.MultiPoint: geojson,
-            shapely.geometry.Polygon: geojson,
-        }
+    # TODO[pydantic]: The following keys were removed: `json_encoders`.
+    # Check https://docs.pydantic.dev/dev-v2/migration/#changes-to-config for more information.
+    model_config = ConfigDict(use_enum_values=True, validate_assignment=True)
 
     def __str__(self):
         if self._detail:
             return f"""
         {self.name} [{self.id}]
             Extent: {self.bounds}
             Timerange: {self.tstart} to {self.tend}
```

### Comparing `oceanum-0.7.9/oceanum/datamesh/query.py` & `oceanum-0.8.0/oceanum/datamesh/query.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,55 @@
 import datetime
-import orjson
 import pandas as pd
 import numpy as np
-from pydantic import BaseModel, Field, validator
+from pydantic import (
+    field_validator,
+    ConfigDict,
+    BaseModel,
+    Field,
+    BeforeValidator,
+    WithJsonSchema,
+)
 from typing import Optional, Dict, Union, List
+from typing_extensions import Annotated
 from enum import Enum
 from geojson_pydantic import Feature, FeatureCollection
 
 
-def _orjson_dumps(val, *, default):
-    return orjson.dumps(val, default=default).decode()
-
-
 class QueryError(Exception):
     pass
 
 
-class Timestamp(pd.Timestamp):
-    @classmethod
-    def __get_validators__(cls):
-        yield cls.validate
-
-    @classmethod
-    def validate(cls, v):
-        if not (
-            isinstance(v, str)
-            or isinstance(v, datetime.datetime)
-            or isinstance(v, datetime.date)
-            or isinstance(v, pd.Timestamp)
-        ):
-            raise TypeError("datetime or time string required")
-        try:
-            time = cls(v)
-            if not time.tz:
-                time = time.tz_localize("UTC")
-            return time.tz_convert(None).to_datetime64()
-        except Exception as e:
-            raise TypeError(f"Timestamp format not valid: {e}")
+def parse_time(v):
+    if not (
+        isinstance(v, str)
+        or isinstance(v, datetime.datetime)
+        or isinstance(v, datetime.date)
+        or isinstance(v, pd.Timestamp)
+    ):
+        raise TypeError("datetime or time string required")
+    try:
+        time = pd.Timestamp(v)
+        if not time.tz:
+            time = time.tz_localize("UTC")
+        return pd.to_datetime(time.tz_convert(None))
+    except Exception as e:
+        raise TypeError(f"Timestamp format not valid: {e}")
+
+
+Timestamp = Annotated[
+    datetime.datetime,
+    Field(
+        default=None,
+        title="Timestamp",
+        description="Timestamp as python datetime, numpy datetime64 or pandas Timestamp",
+    ),
+    BeforeValidator(parse_time),
+    WithJsonSchema({"type": "string", "format": "date-time"}),
+]
 
 
 class GeoFilterType(Enum):
     feature = "feature"
     # radius = "radius"
     bbox = "bbox"
 
@@ -85,15 +94,16 @@
     )
     resolution: Optional[float] = Field(
         title="Maximum spatial resolution of data",
         default=0.0,
         description="Maximum resolution of the data for downsampling in CRS units. Only works for feature datasources.",
     )
 
-    @validator("geom", pre=True)
+    @field_validator("geom", mode="before")
+    @classmethod
     def validate_geom(cls, v):
         if isinstance(v, list):
             if len(v) != 4:
                 raise ValueError(
                     "bbox must be a list of length 4: [x_min,y_min,x_max,y_max]"
                 )
         elif isinstance(v, dict):
@@ -170,14 +180,19 @@
 # geodf   ∩  bbox -> clipped geodf (optional resolution)
 # geodf   ∩  feature -> intersecting features from geodf (optional resolution)
 # Dataframe with x and y coordinates will be supported (not implemented yet)
 # df      ∩  bbox -> subset df within bbox
 # df      ∩  features -> subset of df within (resolution) of features
 
 
+class CoordSelector(BaseModel):
+    coord: str = Field(title="Coordinate name")
+    value: List[str | int | float] = Field(title="Coordinate value")
+
+
 class Query(BaseModel):
     """
     Datamesh query
     """
 
     datasource: str = Field(
         title="The id of the datasource",
@@ -204,30 +219,28 @@
         title="Time filter",
         default=None,
         description="Temporal filter or interplator",
     )
     geofilter: Optional[GeoFilter] = Field(
         title="Spatial filter or interpolator", default=None
     )
+    coordfilter: Optional[List[CoordSelector]] = Field(
+        title="List of additional coordinate filters", default=None
+    )
     crs: Optional[Union[str, int]] = Field(
         title="Spatial reference for filter and output",
         default=None,
         description="Valid CRS string for returned data",
     )
     aggregate: Optional[Aggregate] = Field(
         title="Aggregation operators to apply",
         default=None,
         description="Optional aggregation operators to apply to query after filtering",
     )
 
-    class Config:
-        json_loads = orjson.loads
-        json_dumps = _orjson_dumps
-        json_encoders = {np.datetime64: str}
-
 
 class Container(str, Enum):
     GeoDataFrame = "geodataframe"
     DataFrame = "dataframe"
     Dataset = "dataset"
```

### Comparing `oceanum-0.7.9/oceanum/datamesh/zarr.py` & `oceanum-0.8.0/oceanum/datamesh/zarr.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.9/oceanum.egg-info/PKG-INFO` & `oceanum-0.8.0/oceanum.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: oceanum
-Version: 0.7.9
+Version: 0.8.0
 Summary: Library for oceanum.io services
 Home-page: https://github.com/oceanum/oceanum-python
 Author: Oceanum Developers
 Author-email: developers@oceanum.science
 License: MIT license
 Keywords: oceanum
-Platform: UNKNOWN
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ==============
 oceanum-python
 ==============
 
@@ -49,9 +48,7 @@
 History
 =======
 
 0.4.2 (2022-05-20)
 ------------------
 
 * First release on PyPI.
-
-
```

### Comparing `oceanum-0.7.9/setup.py` & `oceanum-0.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.9/tests/data/grid_data_1.nc` & `oceanum-0.8.0/tests/data/grid_data_1.nc`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.9/tests/data/ocean_test_1.mp4` & `oceanum-0.8.0/tests/data/ocean_test_1.mp4`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.9/tests/data/point_data_1.csv` & `oceanum-0.8.0/tests/data/point_data_1.csv`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.9/tests/test_catalog.py` & `oceanum-0.8.0/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.9/tests/test_datamesh_connect.py` & `oceanum-0.8.0/tests/test_datamesh_connect.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.9/tests/test_datamesh_load.py` & `oceanum-0.8.0/tests/test_datamesh_load.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.9/tests/test_datamesh_query.py` & `oceanum-0.8.0/tests/test_datamesh_query.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.9/tests/test_datamesh_write.py` & `oceanum-0.8.0/tests/test_datamesh_write.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.9/tests/test_datasource.py` & `oceanum-0.8.0/tests/test_datasource.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
         name="Test datasource",
         tstart="2000-01-01T00:00:00Z",
         geom={"type": "MultiPoint", "coordinates": [[173, -39], [174, -40]]},
         schema=schema,
         coordinates={"t": "time"},
         driver="dum",
     )
+    ds._detail = True
     assert ds.bounds == (
         173.0,
         -40,
         174,
         -39,
     )
     assert ds.attributes["name"] == "test"
```

### Comparing `oceanum-0.7.9/tests/test_query.py` & `oceanum-0.8.0/tests/test_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
                     "type": "Polygon",
                     "coordinates": [
                         [
                             [114.59562876453432, -28.77320223799819],
                             [114.59885236328529, -28.77290277153547],
                             [114.59911343041955, -28.77161672273214],
                             [114.59586208356448, -28.771921278480875],
-                            [114.59562876453431, -28.77320223799819],
+                            [114.59562876453432, -28.77320223799819],
                         ]
                     ],
                 },
                 "properties": {},
             },
         },
     )
```

### Comparing `oceanum-0.7.9/tests/test_video_compat.py` & `oceanum-0.8.0/tests/test_video_compat.py`

 * *Files identical despite different names*

