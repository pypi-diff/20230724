# Comparing `tmp/spyder-notebook-0.5.0.tar.gz` & `tmp/spyder-notebook-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spyder-notebook-0.5.0.tar", last modified: Sun Jul 23 12:20:15 2023, max compression
+gzip compressed data, was "spyder-notebook-0.5.1.tar", last modified: Mon Jul 24 11:02:46 2023, max compression
```

## Comparing `spyder-notebook-0.5.0.tar` & `spyder-notebook-0.5.1.tar`

### file list

```diff
@@ -1,384 +1,384 @@
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-23 12:20:15.553721 spyder-notebook-0.5.0/
--rw-r--r--   0 jitse     (1000) jitse     (1000)    34212 2023-07-23 00:09:44.000000 spyder-notebook-0.5.0/CHANGELOG.md
--rw-r--r--   0 jitse     (1000) jitse     (1000)     1286 2023-06-29 13:39:07.000000 spyder-notebook-0.5.0/LICENSE
--rw-r--r--   0 jitse     (1000) jitse     (1000)      403 2023-07-23 12:02:03.000000 spyder-notebook-0.5.0/MANIFEST.in
--rw-r--r--   0 jitse     (1000) jitse     (1000)     4705 2023-07-23 12:20:15.553721 spyder-notebook-0.5.0/PKG-INFO
--rw-r--r--   0 jitse     (1000) jitse     (1000)     4108 2023-06-29 13:39:07.000000 spyder-notebook-0.5.0/README.md
--rw-r--r--   0 jitse     (1000) jitse     (1000)      755 2023-02-05 14:13:01.000000 spyder-notebook-0.5.0/runtests.py
--rw-r--r--   0 jitse     (1000) jitse     (1000)       38 2023-07-23 12:20:15.553721 spyder-notebook-0.5.0/setup.cfg
--rw-r--r--   0 jitse     (1000) jitse     (1000)     3223 2023-07-22 23:28:28.000000 spyder-notebook-0.5.0/setup.py
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-23 12:20:15.521721 spyder-notebook-0.5.0/spyder_notebook/
--rw-r--r--   0 jitse     (1000) jitse     (1000)      857 2023-06-29 13:39:07.000000 spyder-notebook-0.5.0/spyder_notebook/__init__.py
--rw-r--r--   0 jitse     (1000) jitse     (1000)       92 2023-07-23 11:42:47.000000 spyder-notebook-0.5.0/spyder_notebook/_version.py
--rw-r--r--   0 jitse     (1000) jitse     (1000)      971 2023-02-05 14:13:44.000000 spyder-notebook-0.5.0/spyder_notebook/config.py
--rw-r--r--   0 jitse     (1000) jitse     (1000)     1260 2023-02-05 14:13:44.000000 spyder-notebook-0.5.0/spyder_notebook/confpage.py
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-23 12:20:15.521721 spyder-notebook-0.5.0/spyder_notebook/locale/
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-23 12:20:15.521721 spyder-notebook-0.5.0/spyder_notebook/locale/de/
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-23 12:20:15.525721 spyder-notebook-0.5.0/spyder_notebook/locale/de/LC_MESSAGES/
--rw-r--r--   0 jitse     (1000) jitse     (1000)     3658 2023-07-22 23:29:27.000000 spyder-notebook-0.5.0/spyder_notebook/locale/de/LC_MESSAGES/spyder_notebook.mo
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-23 12:20:15.521721 spyder-notebook-0.5.0/spyder_notebook/locale/es/
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-23 12:20:15.525721 spyder-notebook-0.5.0/spyder_notebook/locale/es/LC_MESSAGES/
--rw-r--r--   0 jitse     (1000) jitse     (1000)     2796 2023-07-22 23:29:27.000000 spyder-notebook-0.5.0/spyder_notebook/locale/es/LC_MESSAGES/spyder_notebook.mo
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-23 12:20:15.521721 spyder-notebook-0.5.0/spyder_notebook/locale/fr/
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-23 12:20:15.525721 spyder-notebook-0.5.0/spyder_notebook/locale/fr/LC_MESSAGES/
--rw-r--r--   0 jitse     (1000) jitse     (1000)      553 2023-07-22 23:29:27.000000 spyder-notebook-0.5.0/spyder_notebook/locale/fr/LC_MESSAGES/spyder_notebook.mo
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-23 12:20:15.521721 spyder-notebook-0.5.0/spyder_notebook/locale/hr/
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-23 12:20:15.525721 spyder-notebook-0.5.0/spyder_notebook/locale/hr/LC_MESSAGES/
--rw-r--r--   0 jitse     (1000) jitse     (1000)      630 2023-07-22 23:29:27.000000 spyder-notebook-0.5.0/spyder_notebook/locale/hr/LC_MESSAGES/spyder_notebook.mo
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-23 12:20:15.521721 spyder-notebook-0.5.0/spyder_notebook/locale/hu/
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-23 12:20:15.525721 spyder-notebook-0.5.0/spyder_notebook/locale/hu/LC_MESSAGES/
--rw-r--r--   0 jitse     (1000) jitse     (1000)      557 2023-07-22 23:29:27.000000 spyder-notebook-0.5.0/spyder_notebook/locale/hu/LC_MESSAGES/spyder_notebook.mo
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-23 12:20:15.521721 spyder-notebook-0.5.0/spyder_notebook/locale/ja/
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-23 12:20:15.525721 spyder-notebook-0.5.0/spyder_notebook/locale/ja/LC_MESSAGES/
--rw-r--r--   0 jitse     (1000) jitse     (1000)      549 2023-07-22 23:29:27.000000 spyder-notebook-0.5.0/spyder_notebook/locale/ja/LC_MESSAGES/spyder_notebook.mo
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-23 12:20:15.521721 spyder-notebook-0.5.0/spyder_notebook/locale/pl/
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-23 12:20:15.525721 spyder-notebook-0.5.0/spyder_notebook/locale/pl/LC_MESSAGES/
--rw-r--r--   0 jitse     (1000) jitse     (1000)      700 2023-07-22 23:29:27.000000 spyder-notebook-0.5.0/spyder_notebook/locale/pl/LC_MESSAGES/spyder_notebook.mo
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-23 12:20:15.521721 spyder-notebook-0.5.0/spyder_notebook/locale/pt_BR/
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-23 12:20:15.525721 spyder-notebook-0.5.0/spyder_notebook/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 jitse     (1000) jitse     (1000)     3493 2023-07-22 23:29:27.000000 spyder-notebook-0.5.0/spyder_notebook/locale/pt_BR/LC_MESSAGES/spyder_notebook.mo
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-23 12:20:15.521721 spyder-notebook-0.5.0/spyder_notebook/locale/ru/
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-23 12:20:15.525721 spyder-notebook-0.5.0/spyder_notebook/locale/ru/LC_MESSAGES/
--rw-r--r--   0 jitse     (1000) jitse     (1000)      720 2023-07-22 23:29:27.000000 spyder-notebook-0.5.0/spyder_notebook/locale/ru/LC_MESSAGES/spyder_notebook.mo
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-23 12:20:15.521721 spyder-notebook-0.5.0/spyder_notebook/locale/zh_CN/
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-23 12:20:15.525721 spyder-notebook-0.5.0/spyder_notebook/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 jitse     (1000) jitse     (1000)      562 2023-07-22 23:29:27.000000 spyder-notebook-0.5.0/spyder_notebook/locale/zh_CN/LC_MESSAGES/spyder_notebook.mo
--rw-r--r--   0 jitse     (1000) jitse     (1000)     3212 2023-07-22 23:30:14.000000 spyder-notebook-0.5.0/spyder_notebook/notebookplugin.py
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-23 12:20:15.525721 spyder-notebook-0.5.0/spyder_notebook/server/
--rw-r--r--   0 jitse     (1000) jitse     (1000)      211 2023-02-15 11:49:49.000000 spyder-notebook-0.5.0/spyder_notebook/server/__init__.py
--rw-r--r--   0 jitse     (1000) jitse     (1000)      257 2023-06-29 13:39:07.000000 spyder-notebook-0.5.0/spyder_notebook/server/__main__.py
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-23 12:20:15.521721 spyder-notebook-0.5.0/spyder_notebook/server/app/
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-23 12:20:15.521721 spyder-notebook-0.5.0/spyder_notebook/server/app/build/
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-23 12:20:15.521721 spyder-notebook-0.5.0/spyder_notebook/server/app/build/themes/
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-23 12:20:15.521721 spyder-notebook-0.5.0/spyder_notebook/server/app/build/themes/@jupyterlab/
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-23 12:20:15.525721 spyder-notebook-0.5.0/spyder_notebook/server/app/build/themes/@jupyterlab/theme-dark-extension/
--rw-r--r--   0 jitse     (1000) jitse     (1000)    17760 2023-07-23 12:20:10.000000 spyder-notebook-0.5.0/spyder_notebook/server/app/build/themes/@jupyterlab/theme-dark-extension/index.css
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-23 12:20:15.525721 spyder-notebook-0.5.0/spyder_notebook/server/app/build/themes/@jupyterlab/theme-light-extension/
--rw-r--r--   0 jitse     (1000) jitse     (1000)    16493 2023-07-23 12:20:10.000000 spyder-notebook-0.5.0/spyder_notebook/server/app/build/themes/@jupyterlab/theme-light-extension/index.css
--rw-r--r--   0 jitse     (1000) jitse     (1000)     3194 2023-06-29 13:39:07.000000 spyder-notebook-0.5.0/spyder_notebook/server/main.py
--rw-r--r--   0 jitse     (1000) jitse     (1000)     1503 2023-06-29 13:39:07.000000 spyder-notebook-0.5.0/spyder_notebook/server/notebook-template.html
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-23 12:20:15.549721 spyder-notebook-0.5.0/spyder_notebook/server/static/
--rw-r--r--   0 jitse     (1000) jitse     (1000)    34160 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/1cb1c39ea642f26a4dfe.woff
--rw-r--r--   0 jitse     (1000) jitse     (1000)     9600 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/26683bf201fb258a2237.woff
--rw-r--r--   0 jitse     (1000) jitse     (1000)     5464 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/30e889b58cbc51adfbb0.woff
--rw-r--r--   0 jitse     (1000) jitse     (1000)    15944 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/32792104b5ef69eded90.woff
--rw-r--r--   0 jitse     (1000) jitse     (1000)    20832 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/355254db9ca10a09a3b5.woff
--rw-r--r--   0 jitse     (1000) jitse     (1000)     1116 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/36e0d72d8a7afc696a3e.woff
--rw-r--r--   0 jitse     (1000) jitse     (1000)   203030 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/373c04fd2418f5c77eea.eot
--rw-r--r--   0 jitse     (1000) jitse     (1000)     5148 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/3bc6ecaae7ecf6f8d7f8.woff
--rw-r--r--   0 jitse     (1000) jitse     (1000)    40808 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/3de784d07b9fa8f104c1.woff
--rw-r--r--   0 jitse     (1000) jitse     (1000)   101648 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/3f6d3488cf65374f6f67.woff
--rw-r--r--   0 jitse     (1000) jitse     (1000)     1368 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/481e39042508ae313a60.woff
--rw-r--r--   0 jitse     (1000) jitse     (1000)     3244 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/5cda41563a095bd70c78.woff
--rw-r--r--   0 jitse     (1000) jitse     (1000)    22340 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/721921bab0d001ebff02.woff
--rw-r--r--   0 jitse     (1000) jitse     (1000)     1136 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/72bc573386dd1d48c5bb.woff
--rw-r--r--   0 jitse     (1000) jitse     (1000)    34034 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/79d088064beb3826054f.eot
--rw-r--r--   0 jitse     (1000) jitse     (1000)    21480 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/870673df72e70f87c91a.woff
--rw-r--r--   0 jitse     (1000) jitse     (1000)    34464 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/88b98cad3688915e50da.woff
--rw-r--r--   0 jitse     (1000) jitse     (1000)    76736 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/8ea8791754915a898a31.woff2
--rw-r--r--   0 jitse     (1000) jitse     (1000)    19776 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/8ea8dbb1b02e6f730f55.woff
--rw-r--r--   0 jitse     (1000) jitse     (1000)   918991 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/9674eb1bd55047179038.svg
--rw-r--r--   0 jitse     (1000) jitse     (1000)    78268 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/9834b82ad26e2a37583d.woff2
--rw-r--r--   0 jitse     (1000) jitse     (1000)     1885 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/_8883-_5fa1-_1b46-_2abd-_0836.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    19360 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/a009bea404f7a500ded4.woff
--rw-r--r--   0 jitse     (1000) jitse     (1000)   747927 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/a3b9817780214caf01e8.svg
--rw-r--r--   0 jitse     (1000) jitse     (1000)     9908 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/af04542b29eaac04550a.woff
--rw-r--r--   0 jitse     (1000) jitse     (1000)   202744 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/af6397503fcefbd61397.ttf
--rw-r--r--   0 jitse     (1000) jitse     (1000)    11852 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/af96f67d7accf5fd2a4a.woff
--rw-r--r--   0 jitse     (1000) jitse     (1000)    12660 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/b418136e3b384baaadec.woff
--rw-r--r--   0 jitse     (1000) jitse     (1000)   144714 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/be0a084962d8066884f7.svg
--rw-r--r--   0 jitse     (1000) jitse     (1000)    37590 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/build_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)   257114 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     5792 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/c49810b53ecc0d87d802.woff
--rw-r--r--   0 jitse     (1000) jitse     (1000)    17604 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/c56da8d69f1a0208b8e0.woff
--rw-r--r--   0 jitse     (1000) jitse     (1000)    16276 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/cb9e9e693192413cde2b.woff
--rw-r--r--   0 jitse     (1000) jitse     (1000)   133988 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/cda59d6efffa685830fd.ttf
--rw-r--r--   0 jitse     (1000) jitse     (1000)   134294 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/e4299464e7b012968eed.eot
--rw-r--r--   0 jitse     (1000) jitse     (1000)    13224 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/e42a88444448ac3d6054.woff2
--rw-r--r--   0 jitse     (1000) jitse     (1000)    33736 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/e8711bbb871afd8e9dea.ttf
--rw-r--r--   0 jitse     (1000) jitse     (1000)    89988 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/f9217f66874b0c01cd8c.woff
--rw-r--r--   0 jitse     (1000) jitse     (1000)    14628 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/fc6ddf5df402b263cfb1.woff
--rw-r--r--   0 jitse     (1000) jitse     (1000)     7541 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_lang-json_dist_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     6178 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_lang-wast_dist_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     5401 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_apl_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     3067 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_asciiarmor_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     9152 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_asn1_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     8537 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_asterisk_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     2931 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_brainfuck_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     3488 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_cmake_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    11185 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_cobol_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    10534 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_coffeescript_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     5598 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_commonlisp_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     7566 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_cypher_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     8408 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_d_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     2006 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_diff_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    11047 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_dockerfile_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     5555 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_dtd_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    11141 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_dylan_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     5741 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_ebnf_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     9545 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_ecl_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     4626 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_eiffel_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     5988 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_elm_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     9648 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_factor_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     5429 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_fcl_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     5803 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_forth_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     9807 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_fortran_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    11252 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_gas_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     6899 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_go_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     9313 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_groovy_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     9251 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_haskell_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     3297 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_http_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     6710 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_jinja2_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     8261 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_livescript_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     6867 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_lua_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     6428 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_mathematica_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     4668 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_mbox_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    10919 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_mirc_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    10124 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_mllike_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     6700 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_modelica_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     7813 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_mscgen_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     6318 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_mumps_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    11072 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_nginx_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     6397 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_ntriples_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     5448 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_octave_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     7644 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_oz_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     5217 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_pascal_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     6206 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_pig_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     3048 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_properties_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     3127 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_protobuf_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     8393 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_puppet_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     7826 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_q_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     7635 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_r_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     4570 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_rpm_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    11816 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_ruby_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     6350 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_shell_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     5151 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_sieve_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     5484 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_smalltalk_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     3339 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_solr_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     7872 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_sparql_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     3913 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_spreadsheet_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     8753 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_stex_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     8577 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_swift_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     5821 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_tcl_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     8824 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_tiddlywiki_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     9437 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_tiki_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     3801 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_toml_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     3179 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_troff_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     9703 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_ttcn-cfg_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    10517 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_ttcn_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     5659 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_turtle_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     9660 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_vb_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     7015 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_velocity_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     7568 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_vhdl_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     7032 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_webidl_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     6161 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_yacas_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     4569 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_yaml_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     4617 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_z80_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     6451 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyter-notebook_docmanager-extension_lib_index_js-_e4b40.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     6451 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyter-notebook_docmanager-extension_lib_index_js-_e4b41.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     4192 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyter-notebook_documentsearch-extension_lib_index_js-_32b90.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     4192 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyter-notebook_documentsearch-extension_lib_index_js-_32b91.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     8237 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyter-notebook_help-extension_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    14218 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyter-notebook_ui-components_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     4611 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_cell-toolbar-extension_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    12684 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_celltags-extension_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    10889 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_completer-extension_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    10106 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_htmlviewer-extension_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    16232 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_htmlviewer_lib_index_js-_f0bb0.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    16232 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_htmlviewer_lib_index_js-_f0bb1.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     9308 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_hub-extension_lib_index_js-_9dda0.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     9308 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_hub-extension_lib_index_js-_9dda1.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    11638 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_imageviewer-extension_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    13198 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_imageviewer_lib_index_js-_afb90.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    13198 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_imageviewer_lib_index_js-_afb91.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     4650 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_javascript-extension_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     7707 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_json-extension_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     5553 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_markedparser-extension_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    10722 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_mathjax-extension_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     5515 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_nbformat_lib_index_js-_a6f70.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     5515 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_nbformat_lib_index_js-_a6f71.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     9285 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_pdf-extension_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    13364 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_property-inspector_lib_index_js-_90690.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    13364 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_property-inspector_lib_index_js-_90691.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     6978 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_rendermime-extension_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     1683 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_rendermime-interfaces_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     3347 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_theme-dark-extension_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     3360 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_theme-light-extension_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    11921 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_tooltip_lib_index_js-_d1c70.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    11921 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_tooltip_lib_index_js-_d1c71.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    11080 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_translation-extension_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     3267 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_ui-components-extension_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     9222 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_vega5-extension_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     7269 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_lumino_disposable_dist_index_es6_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     8242 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_lumino_keyboard_dist_index_es6_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     7598 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_lumino_properties_dist_index_es6_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     9215 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_mathjax-full_js_mathjax_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    10388 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_mathjax-full_js_util_Options_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     6629 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_process_browser_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     6660 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/packages_application-extension_lib_index_js-_90450.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)     6660 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/packages_application-extension_lib_index_js-_90451.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)   170833 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_autocomplete_dist_index_js-node_modules_lezer_lr_dist_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    88348 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_commands_dist_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)   111075 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_lang-cpp_dist_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    35592 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_lang-css_dist_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    56584 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_lang-html_dist_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    46770 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_lang-java_dist_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)   102602 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_lang-javascript_dist_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)   108950 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_lang-markdown_dist_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)   107893 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_lang-php_dist_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    71985 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_lang-python_dist_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    77183 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_lang-rust_dist_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    45059 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_lang-sql_dist_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    25029 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_lang-xml_dist_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)   108331 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_language_dist_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    42827 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_clike_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    19460 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_clojure_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    13265 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_crystal_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    44777 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_css_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    19531 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_erlang_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    13733 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_gherkin_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    18343 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_haxe_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    15522 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_idl_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    41098 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_javascript_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    12430 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_julia_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    14518 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_nsis_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    31649 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_perl_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    13593 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_powershell_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    16191 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_python_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    15221 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_sas_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    13562 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_scheme_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    49821 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_sql_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    44130 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_stylus_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    14413 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_textile_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    14803 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_vbscript_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    24045 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_verilog_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    17016 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_xquery_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    57618 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_search_dist_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)   585046 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_view_dist_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    66298 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_fast-deep-equal_index_js-node_modules_json-schema-traverse_index_js-node-057f3c.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    46184 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyter-notebook_application-extension_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)  1039276 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyter-notebook_application-extension_style_index_js-node_modules_jupyt-7c11f7.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    42632 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyter-notebook_application_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    24589 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyter-notebook_notebook-extension_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    87145 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyter_ydoc_lib_index_js-node_modules_process_browser_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    65325 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_application-extension_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)   117692 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_application_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    35930 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_application_lib_mimerenderers_js-node_modules_jupyterlab_appl-fdcfe8.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)   146227 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_apputils-extension_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)   684647 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_apputils_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    21206 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_cell-toolbar_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)   155086 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_cells_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    44736 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_codeeditor_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    20938 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_codemirror-extension_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)   404138 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_codemirror_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)   106502 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_completer_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    62765 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_console_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    95087 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_coreutils_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    47796 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_debugger-extension_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)   255058 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_debugger_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)   419423 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_debugger_lib_panels_variables_gridpanel_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    52170 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_docmanager-extension_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    80126 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_docmanager_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)   106978 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_docregistry_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    15457 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_documentsearch-extension_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    69870 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_documentsearch_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    58595 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_filebrowser-extension_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)   189164 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_filebrowser_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    88266 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_fileeditor-extension_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    59831 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_fileeditor_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)   284183 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_json-extension_lib_component_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    18242 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_launcher_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    34884 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_logconsole_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    33781 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_lsp-extension_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)   360406 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_lsp_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    35395 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_mainmenu-extension_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    38403 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_mainmenu_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    15817 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_metadataform-extension_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    29514 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_metadataform_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)   161641 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_notebook-extension_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)   408495 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_notebook_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    47339 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_observables_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    59675 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_outputarea_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)   111820 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_rendermime_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    17290 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_running_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)   312806 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_services_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)   400161 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_settingregistry_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    82326 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_shortcuts-extension_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    27185 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_statedb_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    28515 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_statusbar_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    15306 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_toc-extension_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    54057 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_toc_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    16126 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_tooltip-extension_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    36200 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_translation_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)   705900 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_ui-components_lib_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    79999 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_lezer_common_dist_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    30691 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_lezer_highlight_dist_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)   114787 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_lib0_buffer_js-node_modules_lib0_encoding_js-node_modules_lib0_observabl-50dfe2.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)   198998 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_lodash-es__baseClone_js-node_modules_lodash-es_get_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    49615 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_lodash-es_has_js-node_modules_lodash-es_hasIn_js-node_modules_lodash-es_-930c1c.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    83073 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_lumino_algorithm_dist_index_es6_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    80996 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_lumino_application_dist_index_es6_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    40333 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_lumino_commands_dist_index_es6_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    19970 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_lumino_coreutils_dist_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    17562 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_lumino_domutils_dist_index_es6_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    37389 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_lumino_dragdrop_dist_index_es6_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    32321 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_lumino_messaging_dist_index_es6_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    20949 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_lumino_polling_dist_index_es6_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    21540 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_lumino_signaling_dist_index_es6_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    27016 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_lumino_virtualdom_dist_index_es6_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)   551610 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_lumino_widgets_dist_index_es6_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    84092 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_marked_lib_marked_esm_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    27354 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_a11y_assistive-mml_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    17105 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_adaptors_browserAdaptor_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)   118351 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_core_MathItem_js-node_modules_mathjax-full_js_core_MmlTr-144bb4.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    32398 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_core_MmlTree_MmlFactory_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)   129649 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_core_MmlTree_MmlNodes_mo_js-node_modules_mathjax-full_js-e92534.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    89680 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_handlers_html_HTMLHandler_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)   450064 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_input_tex_AllPackages_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)   126224 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_input_tex_Configuration_js-node_modules_mathjax-full_js_-8c4c26.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)   154837 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_input_tex_ParseOptions_js-node_modules_mathjax-full_js_i-0c5d92.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    37081 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_input_tex_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    33875 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_input_tex_require_RequireConfiguration_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)   234379 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_output_chtml_fonts_tex_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)   465381 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_output_chtml_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    33543 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_ui_safe_SafeHandler_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)  1078623 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_react-dom_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    21903 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_react-toastify_dist_react-toastify_esm_mjs.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)    92046 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_react_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)   327447 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_regexp-match-indices_index_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)   575730 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_rjsf_utils_dist_utils_esm_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)   320313 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_rjsf_validator-ajv8_dist_validator-ajv8_esm_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)  3384152 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_vega-embed_build_vega-embed_module_js.bundle.js
--rw-r--r--   0 jitse     (1000) jitse     (1000)   366817 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_yjs_dist_yjs_mjs.bundle.js
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-23 12:20:15.549721 spyder-notebook-0.5.0/spyder_notebook/tests/
--rw-r--r--   0 jitse     (1000) jitse     (1000)      817 2023-04-29 21:10:29.000000 spyder-notebook-0.5.0/spyder_notebook/tests/test_config.py
--rw-r--r--   0 jitse     (1000) jitse     (1000)     8125 2023-07-22 23:30:14.000000 spyder-notebook-0.5.0/spyder_notebook/tests/test_plugin.py
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-23 12:20:15.549721 spyder-notebook-0.5.0/spyder_notebook/utils/
--rw-r--r--   0 jitse     (1000) jitse     (1000)      350 2023-02-05 14:13:01.000000 spyder-notebook-0.5.0/spyder_notebook/utils/__init__.py
--rw-r--r--   0 jitse     (1000) jitse     (1000)      241 2023-02-05 14:13:44.000000 spyder-notebook-0.5.0/spyder_notebook/utils/localization.py
--rw-r--r--   0 jitse     (1000) jitse     (1000)    14226 2023-06-29 13:39:07.000000 spyder-notebook-0.5.0/spyder_notebook/utils/servermanager.py
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-23 12:20:15.549721 spyder-notebook-0.5.0/spyder_notebook/utils/templates/
--rwxr-xr-x   0 jitse     (1000) jitse     (1000)    16050 2023-06-29 13:39:07.000000 spyder-notebook-0.5.0/spyder_notebook/utils/templates/welcome-dark.html
--rw-r--r--   0 jitse     (1000) jitse     (1000)    15935 2023-06-29 13:39:07.000000 spyder-notebook-0.5.0/spyder_notebook/utils/templates/welcome.html
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-23 12:20:15.549721 spyder-notebook-0.5.0/spyder_notebook/utils/tests/
--rwxr-xr-x   0 jitse     (1000) jitse     (1000)     9910 2023-06-29 13:39:07.000000 spyder-notebook-0.5.0/spyder_notebook/utils/tests/test_servermanager.py
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-23 12:20:15.553721 spyder-notebook-0.5.0/spyder_notebook/widgets/
--rw-r--r--   0 jitse     (1000) jitse     (1000)      348 2023-02-05 14:13:01.000000 spyder-notebook-0.5.0/spyder_notebook/widgets/__init__.py
--rw-r--r--   0 jitse     (1000) jitse     (1000)    16346 2023-06-29 13:39:07.000000 spyder-notebook-0.5.0/spyder_notebook/widgets/client.py
--rw-r--r--   0 jitse     (1000) jitse     (1000)     2049 2023-02-11 22:17:54.000000 spyder-notebook-0.5.0/spyder_notebook/widgets/dom.py
--rwxr-xr-x   0 jitse     (1000) jitse     (1000)     3942 2023-02-05 14:13:44.000000 spyder-notebook-0.5.0/spyder_notebook/widgets/example_app.py
--rw-r--r--   0 jitse     (1000) jitse     (1000)    13830 2023-07-22 23:30:14.000000 spyder-notebook-0.5.0/spyder_notebook/widgets/main_widget.py
--rwxr-xr-x   0 jitse     (1000) jitse     (1000)    17725 2023-07-22 23:29:27.000000 spyder-notebook-0.5.0/spyder_notebook/widgets/notebooktabwidget.py
--rwxr-xr-x   0 jitse     (1000) jitse     (1000)     4344 2023-02-05 14:13:44.000000 spyder-notebook-0.5.0/spyder_notebook/widgets/serverinfo.py
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-23 12:20:15.553721 spyder-notebook-0.5.0/spyder_notebook/widgets/tests/
--rw-r--r--   0 jitse     (1000) jitse     (1000)     4079 2023-06-29 13:39:07.000000 spyder-notebook-0.5.0/spyder_notebook/widgets/tests/test_client.py
--rw-r--r--   0 jitse     (1000) jitse     (1000)     9534 2023-06-29 13:39:11.000000 spyder-notebook-0.5.0/spyder_notebook/widgets/tests/test_main_widget.py
--rwxr-xr-x   0 jitse     (1000) jitse     (1000)     7927 2023-07-22 23:29:27.000000 spyder-notebook-0.5.0/spyder_notebook/widgets/tests/test_notebooktabwidget.py
--rwxr-xr-x   0 jitse     (1000) jitse     (1000)     2511 2023-06-29 13:39:07.000000 spyder-notebook-0.5.0/spyder_notebook/widgets/tests/test_serverinfo.py
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-23 12:20:15.525721 spyder-notebook-0.5.0/spyder_notebook.egg-info/
--rw-r--r--   0 jitse     (1000) jitse     (1000)     4705 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook.egg-info/PKG-INFO
--rw-r--r--   0 jitse     (1000) jitse     (1000)    28935 2023-07-23 12:20:15.000000 spyder-notebook-0.5.0/spyder_notebook.egg-info/SOURCES.txt
--rw-r--r--   0 jitse     (1000) jitse     (1000)        1 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook.egg-info/dependency_links.txt
--rw-r--r--   0 jitse     (1000) jitse     (1000)       74 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook.egg-info/entry_points.txt
--rw-r--r--   0 jitse     (1000) jitse     (1000)       84 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook.egg-info/requires.txt
--rw-r--r--   0 jitse     (1000) jitse     (1000)       33 2023-07-23 12:20:14.000000 spyder-notebook-0.5.0/spyder_notebook.egg-info/top_level.txt
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-24 11:02:46.260125 spyder-notebook-0.5.1/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    34253 2023-07-24 11:00:57.000000 spyder-notebook-0.5.1/CHANGELOG.md
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     1286 2023-06-29 13:39:07.000000 spyder-notebook-0.5.1/LICENSE
+-rw-r--r--   0 jitse     (1000) jitse     (1000)      403 2023-07-23 19:37:34.000000 spyder-notebook-0.5.1/MANIFEST.in
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     4705 2023-07-24 11:02:46.260125 spyder-notebook-0.5.1/PKG-INFO
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     4108 2023-06-29 13:39:07.000000 spyder-notebook-0.5.1/README.md
+-rw-r--r--   0 jitse     (1000) jitse     (1000)      755 2023-02-05 14:13:01.000000 spyder-notebook-0.5.1/runtests.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)       38 2023-07-24 11:02:46.260125 spyder-notebook-0.5.1/setup.cfg
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     3224 2023-07-24 10:56:46.000000 spyder-notebook-0.5.1/setup.py
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-24 11:02:46.232125 spyder-notebook-0.5.1/spyder_notebook/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)      857 2023-06-29 13:39:07.000000 spyder-notebook-0.5.1/spyder_notebook/__init__.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)       92 2023-07-24 11:01:33.000000 spyder-notebook-0.5.1/spyder_notebook/_version.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)      971 2023-02-05 14:13:44.000000 spyder-notebook-0.5.1/spyder_notebook/config.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     1260 2023-02-05 14:13:44.000000 spyder-notebook-0.5.1/spyder_notebook/confpage.py
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-24 11:02:46.232125 spyder-notebook-0.5.1/spyder_notebook/locale/
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-24 11:02:46.232125 spyder-notebook-0.5.1/spyder_notebook/locale/de/
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-24 11:02:46.232125 spyder-notebook-0.5.1/spyder_notebook/locale/de/LC_MESSAGES/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     3658 2023-07-22 23:29:27.000000 spyder-notebook-0.5.1/spyder_notebook/locale/de/LC_MESSAGES/spyder_notebook.mo
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-24 11:02:46.232125 spyder-notebook-0.5.1/spyder_notebook/locale/es/
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-24 11:02:46.232125 spyder-notebook-0.5.1/spyder_notebook/locale/es/LC_MESSAGES/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     2796 2023-07-22 23:29:27.000000 spyder-notebook-0.5.1/spyder_notebook/locale/es/LC_MESSAGES/spyder_notebook.mo
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-24 11:02:46.232125 spyder-notebook-0.5.1/spyder_notebook/locale/fr/
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-24 11:02:46.232125 spyder-notebook-0.5.1/spyder_notebook/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)      553 2023-07-22 23:29:27.000000 spyder-notebook-0.5.1/spyder_notebook/locale/fr/LC_MESSAGES/spyder_notebook.mo
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-24 11:02:46.232125 spyder-notebook-0.5.1/spyder_notebook/locale/hr/
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-24 11:02:46.236125 spyder-notebook-0.5.1/spyder_notebook/locale/hr/LC_MESSAGES/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)      630 2023-07-22 23:29:27.000000 spyder-notebook-0.5.1/spyder_notebook/locale/hr/LC_MESSAGES/spyder_notebook.mo
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-24 11:02:46.232125 spyder-notebook-0.5.1/spyder_notebook/locale/hu/
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-24 11:02:46.236125 spyder-notebook-0.5.1/spyder_notebook/locale/hu/LC_MESSAGES/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)      557 2023-07-22 23:29:27.000000 spyder-notebook-0.5.1/spyder_notebook/locale/hu/LC_MESSAGES/spyder_notebook.mo
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-24 11:02:46.232125 spyder-notebook-0.5.1/spyder_notebook/locale/ja/
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-24 11:02:46.236125 spyder-notebook-0.5.1/spyder_notebook/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)      549 2023-07-22 23:29:27.000000 spyder-notebook-0.5.1/spyder_notebook/locale/ja/LC_MESSAGES/spyder_notebook.mo
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-24 11:02:46.232125 spyder-notebook-0.5.1/spyder_notebook/locale/pl/
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-24 11:02:46.236125 spyder-notebook-0.5.1/spyder_notebook/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)      700 2023-07-22 23:29:27.000000 spyder-notebook-0.5.1/spyder_notebook/locale/pl/LC_MESSAGES/spyder_notebook.mo
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-24 11:02:46.232125 spyder-notebook-0.5.1/spyder_notebook/locale/pt_BR/
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-24 11:02:46.236125 spyder-notebook-0.5.1/spyder_notebook/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     3493 2023-07-22 23:29:27.000000 spyder-notebook-0.5.1/spyder_notebook/locale/pt_BR/LC_MESSAGES/spyder_notebook.mo
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-24 11:02:46.232125 spyder-notebook-0.5.1/spyder_notebook/locale/ru/
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-24 11:02:46.236125 spyder-notebook-0.5.1/spyder_notebook/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)      720 2023-07-22 23:29:27.000000 spyder-notebook-0.5.1/spyder_notebook/locale/ru/LC_MESSAGES/spyder_notebook.mo
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-24 11:02:46.232125 spyder-notebook-0.5.1/spyder_notebook/locale/zh_CN/
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-24 11:02:46.236125 spyder-notebook-0.5.1/spyder_notebook/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)      562 2023-07-22 23:29:27.000000 spyder-notebook-0.5.1/spyder_notebook/locale/zh_CN/LC_MESSAGES/spyder_notebook.mo
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     3212 2023-07-23 21:35:45.000000 spyder-notebook-0.5.1/spyder_notebook/notebookplugin.py
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-24 11:02:46.236125 spyder-notebook-0.5.1/spyder_notebook/server/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)      211 2023-02-15 11:49:49.000000 spyder-notebook-0.5.1/spyder_notebook/server/__init__.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)      257 2023-06-29 13:39:07.000000 spyder-notebook-0.5.1/spyder_notebook/server/__main__.py
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-24 11:02:46.232125 spyder-notebook-0.5.1/spyder_notebook/server/app/
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-24 11:02:46.232125 spyder-notebook-0.5.1/spyder_notebook/server/app/build/
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-24 11:02:46.232125 spyder-notebook-0.5.1/spyder_notebook/server/app/build/themes/
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-24 11:02:46.232125 spyder-notebook-0.5.1/spyder_notebook/server/app/build/themes/@jupyterlab/
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-24 11:02:46.236125 spyder-notebook-0.5.1/spyder_notebook/server/app/build/themes/@jupyterlab/theme-dark-extension/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    17760 2023-07-24 11:02:40.000000 spyder-notebook-0.5.1/spyder_notebook/server/app/build/themes/@jupyterlab/theme-dark-extension/index.css
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-24 11:02:46.236125 spyder-notebook-0.5.1/spyder_notebook/server/app/build/themes/@jupyterlab/theme-light-extension/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    16493 2023-07-24 11:02:40.000000 spyder-notebook-0.5.1/spyder_notebook/server/app/build/themes/@jupyterlab/theme-light-extension/index.css
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     3194 2023-06-29 13:39:07.000000 spyder-notebook-0.5.1/spyder_notebook/server/main.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     1503 2023-06-29 13:39:07.000000 spyder-notebook-0.5.1/spyder_notebook/server/notebook-template.html
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-24 11:02:46.260125 spyder-notebook-0.5.1/spyder_notebook/server/static/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    34160 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/1cb1c39ea642f26a4dfe.woff
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     9600 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/26683bf201fb258a2237.woff
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     5464 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/30e889b58cbc51adfbb0.woff
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    15944 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/32792104b5ef69eded90.woff
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    20832 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/355254db9ca10a09a3b5.woff
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     1116 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/36e0d72d8a7afc696a3e.woff
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   203030 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/373c04fd2418f5c77eea.eot
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     5148 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/3bc6ecaae7ecf6f8d7f8.woff
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    40808 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/3de784d07b9fa8f104c1.woff
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   101648 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/3f6d3488cf65374f6f67.woff
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     1368 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/481e39042508ae313a60.woff
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     3244 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/5cda41563a095bd70c78.woff
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    22340 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/721921bab0d001ebff02.woff
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     1136 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/72bc573386dd1d48c5bb.woff
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    34034 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/79d088064beb3826054f.eot
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    21480 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/870673df72e70f87c91a.woff
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    34464 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/88b98cad3688915e50da.woff
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    76736 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/8ea8791754915a898a31.woff2
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    19776 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/8ea8dbb1b02e6f730f55.woff
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   918991 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/9674eb1bd55047179038.svg
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    78268 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/9834b82ad26e2a37583d.woff2
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     1885 2023-07-24 11:02:44.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/_8883-_5fa1-_1b46-_2abd-_0836.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    19360 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/a009bea404f7a500ded4.woff
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   747927 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/a3b9817780214caf01e8.svg
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     9908 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/af04542b29eaac04550a.woff
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   202744 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/af6397503fcefbd61397.ttf
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    11852 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/af96f67d7accf5fd2a4a.woff
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    12660 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/b418136e3b384baaadec.woff
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   144714 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/be0a084962d8066884f7.svg
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    37590 2023-07-24 11:02:44.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/build_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   257114 2023-07-24 11:02:44.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     5792 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/c49810b53ecc0d87d802.woff
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    17604 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/c56da8d69f1a0208b8e0.woff
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    16276 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/cb9e9e693192413cde2b.woff
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   133988 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/cda59d6efffa685830fd.ttf
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   134294 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/e4299464e7b012968eed.eot
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    13224 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/e42a88444448ac3d6054.woff2
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    33736 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/e8711bbb871afd8e9dea.ttf
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    89988 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/f9217f66874b0c01cd8c.woff
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    14628 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/fc6ddf5df402b263cfb1.woff
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     7541 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_lang-json_dist_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     6178 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_lang-wast_dist_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     5401 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_apl_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     3067 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_asciiarmor_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     9152 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_asn1_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     8537 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_asterisk_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     2931 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_brainfuck_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     3488 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_cmake_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    11185 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_cobol_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    10534 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_coffeescript_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     5598 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_commonlisp_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     7566 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_cypher_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     8408 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_d_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     2006 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_diff_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    11047 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_dockerfile_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     5555 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_dtd_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    11141 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_dylan_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     5741 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_ebnf_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     9545 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_ecl_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     4626 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_eiffel_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     5988 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_elm_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     9648 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_factor_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     5429 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_fcl_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     5803 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_forth_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     9807 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_fortran_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    11252 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_gas_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     6899 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_go_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     9313 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_groovy_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     9251 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_haskell_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     3297 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_http_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     6710 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_jinja2_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     8261 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_livescript_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     6867 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_lua_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     6428 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_mathematica_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     4668 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_mbox_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    10919 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_mirc_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    10124 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_mllike_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     6700 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_modelica_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     7813 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_mscgen_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     6318 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_mumps_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    11072 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_nginx_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     6397 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_ntriples_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     5448 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_octave_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     7644 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_oz_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     5217 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_pascal_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     6206 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_pig_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     3048 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_properties_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     3127 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_protobuf_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     8393 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_puppet_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     7826 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_q_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     7635 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_r_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     4570 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_rpm_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    11816 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_ruby_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     6350 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_shell_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     5151 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_sieve_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     5484 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_smalltalk_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     3339 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_solr_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     7872 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_sparql_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     3913 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_spreadsheet_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     8753 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_stex_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     8577 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_swift_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     5821 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_tcl_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     8824 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_tiddlywiki_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     9437 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_tiki_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     3801 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_toml_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     3179 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_troff_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     9703 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_ttcn-cfg_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    10517 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_ttcn_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     5659 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_turtle_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     9660 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_vb_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     7015 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_velocity_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     7568 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_vhdl_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     7032 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_webidl_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     6161 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_yacas_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     4569 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_yaml_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     4617 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_z80_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     6451 2023-07-24 11:02:44.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyter-notebook_docmanager-extension_lib_index_js-_e4b40.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     6451 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyter-notebook_docmanager-extension_lib_index_js-_e4b41.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     4192 2023-07-24 11:02:44.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyter-notebook_documentsearch-extension_lib_index_js-_32b90.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     4192 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyter-notebook_documentsearch-extension_lib_index_js-_32b91.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     8237 2023-07-24 11:02:44.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyter-notebook_help-extension_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    14218 2023-07-24 11:02:44.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyter-notebook_ui-components_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     4611 2023-07-24 11:02:44.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_cell-toolbar-extension_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    12684 2023-07-24 11:02:44.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_celltags-extension_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    10889 2023-07-24 11:02:44.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_completer-extension_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    10106 2023-07-24 11:02:44.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_htmlviewer-extension_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    16232 2023-07-24 11:02:44.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_htmlviewer_lib_index_js-_f0bb0.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    16232 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_htmlviewer_lib_index_js-_f0bb1.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     9308 2023-07-24 11:02:44.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_hub-extension_lib_index_js-_9dda0.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     9308 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_hub-extension_lib_index_js-_9dda1.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    11638 2023-07-24 11:02:44.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_imageviewer-extension_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    13198 2023-07-24 11:02:44.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_imageviewer_lib_index_js-_afb90.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    13198 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_imageviewer_lib_index_js-_afb91.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     4650 2023-07-24 11:02:44.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_javascript-extension_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     7707 2023-07-24 11:02:44.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_json-extension_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     5553 2023-07-24 11:02:44.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_markedparser-extension_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    10722 2023-07-24 11:02:44.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_mathjax-extension_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     5515 2023-07-24 11:02:44.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_nbformat_lib_index_js-_a6f70.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     5515 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_nbformat_lib_index_js-_a6f71.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     9285 2023-07-24 11:02:44.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_pdf-extension_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    13364 2023-07-24 11:02:44.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_property-inspector_lib_index_js-_90690.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    13364 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_property-inspector_lib_index_js-_90691.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     6978 2023-07-24 11:02:44.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_rendermime-extension_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     1683 2023-07-24 11:02:44.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_rendermime-interfaces_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     3347 2023-07-24 11:02:44.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_theme-dark-extension_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     3360 2023-07-24 11:02:44.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_theme-light-extension_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    11921 2023-07-24 11:02:44.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_tooltip_lib_index_js-_d1c70.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    11921 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_tooltip_lib_index_js-_d1c71.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    11080 2023-07-24 11:02:44.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_translation-extension_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     3267 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_ui-components-extension_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     9222 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_vega5-extension_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     7269 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_lumino_disposable_dist_index_es6_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     8242 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_lumino_keyboard_dist_index_es6_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     7598 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_lumino_properties_dist_index_es6_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     9215 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_mathjax-full_js_mathjax_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    10388 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_mathjax-full_js_util_Options_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     6629 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_process_browser_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     6660 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/packages_application-extension_lib_index_js-_90450.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     6660 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/packages_application-extension_lib_index_js-_90451.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   170833 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_autocomplete_dist_index_js-node_modules_lezer_lr_dist_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    88348 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_commands_dist_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   111075 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_lang-cpp_dist_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    35592 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_lang-css_dist_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    56584 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_lang-html_dist_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    46770 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_lang-java_dist_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   102602 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_lang-javascript_dist_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   108950 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_lang-markdown_dist_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   107893 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_lang-php_dist_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    71985 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_lang-python_dist_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    77183 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_lang-rust_dist_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    45059 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_lang-sql_dist_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    25029 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_lang-xml_dist_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   108331 2023-07-24 11:02:44.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_language_dist_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    42827 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_clike_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    19460 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_clojure_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    13265 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_crystal_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    44777 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_css_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    19531 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_erlang_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    13733 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_gherkin_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    18343 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_haxe_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    15522 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_idl_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    41098 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_javascript_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    12430 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_julia_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    14518 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_nsis_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    31649 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_perl_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    13593 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_powershell_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    16191 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_python_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    15221 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_sas_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    13562 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_scheme_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    49821 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_sql_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    44130 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_stylus_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    14413 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_textile_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    14803 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_vbscript_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    24045 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_verilog_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    17016 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_xquery_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    57618 2023-07-24 11:02:44.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_search_dist_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   585046 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_view_dist_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    66298 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_fast-deep-equal_index_js-node_modules_json-schema-traverse_index_js-node-057f3c.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    46184 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyter-notebook_application-extension_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)  1039276 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyter-notebook_application-extension_style_index_js-node_modules_jupyt-7c11f7.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    42632 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyter-notebook_application_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    24589 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyter-notebook_notebook-extension_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    87145 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyter_ydoc_lib_index_js-node_modules_process_browser_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    65325 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_application-extension_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   117692 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_application_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    35930 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_application_lib_mimerenderers_js-node_modules_jupyterlab_appl-fdcfe8.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   146227 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_apputils-extension_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   684647 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_apputils_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    21206 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_cell-toolbar_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   155086 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_cells_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    44736 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_codeeditor_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    20938 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_codemirror-extension_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   404138 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_codemirror_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   106502 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_completer_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    62765 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_console_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    95087 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_coreutils_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    47796 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_debugger-extension_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   255058 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_debugger_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   419423 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_debugger_lib_panels_variables_gridpanel_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    52170 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_docmanager-extension_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    80126 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_docmanager_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   106978 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_docregistry_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    15457 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_documentsearch-extension_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    69870 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_documentsearch_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    58595 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_filebrowser-extension_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   189164 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_filebrowser_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    88266 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_fileeditor-extension_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    59831 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_fileeditor_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   284183 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_json-extension_lib_component_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    18242 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_launcher_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    34884 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_logconsole_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    33781 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_lsp-extension_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   360406 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_lsp_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    35395 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_mainmenu-extension_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    38403 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_mainmenu_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    15817 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_metadataform-extension_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    29514 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_metadataform_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   161641 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_notebook-extension_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   408495 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_notebook_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    47339 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_observables_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    59675 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_outputarea_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   111820 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_rendermime_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    17290 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_running_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   312806 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_services_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   400161 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_settingregistry_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    82326 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_shortcuts-extension_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    27185 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_statedb_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    28515 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_statusbar_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    15306 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_toc-extension_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    54057 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_toc_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    16126 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_tooltip-extension_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    36200 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_translation_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   705900 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_ui-components_lib_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    79999 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_lezer_common_dist_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    30691 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_lezer_highlight_dist_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   114787 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_lib0_buffer_js-node_modules_lib0_encoding_js-node_modules_lib0_observabl-50dfe2.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   198998 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_lodash-es__baseClone_js-node_modules_lodash-es_get_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    49615 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_lodash-es_has_js-node_modules_lodash-es_hasIn_js-node_modules_lodash-es_-930c1c.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    83073 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_lumino_algorithm_dist_index_es6_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    80996 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_lumino_application_dist_index_es6_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    40333 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_lumino_commands_dist_index_es6_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    19970 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_lumino_coreutils_dist_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    17562 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_lumino_domutils_dist_index_es6_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    37389 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_lumino_dragdrop_dist_index_es6_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    32321 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_lumino_messaging_dist_index_es6_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    20949 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_lumino_polling_dist_index_es6_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    21540 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_lumino_signaling_dist_index_es6_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    27016 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_lumino_virtualdom_dist_index_es6_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   551610 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_lumino_widgets_dist_index_es6_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    84092 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_marked_lib_marked_esm_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    27354 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_a11y_assistive-mml_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    17105 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_adaptors_browserAdaptor_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   118351 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_core_MathItem_js-node_modules_mathjax-full_js_core_MmlTr-144bb4.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    32398 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_core_MmlTree_MmlFactory_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   129649 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_core_MmlTree_MmlNodes_mo_js-node_modules_mathjax-full_js-e92534.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    89680 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_handlers_html_HTMLHandler_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   450064 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_input_tex_AllPackages_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   126224 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_input_tex_Configuration_js-node_modules_mathjax-full_js_-8c4c26.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   154837 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_input_tex_ParseOptions_js-node_modules_mathjax-full_js_i-0c5d92.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    37081 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_input_tex_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    33875 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_input_tex_require_RequireConfiguration_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   234379 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_output_chtml_fonts_tex_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   465381 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_output_chtml_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    33543 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_ui_safe_SafeHandler_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)  1078623 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_react-dom_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    21903 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_react-toastify_dist_react-toastify_esm_mjs.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    92046 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_react_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   327447 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_regexp-match-indices_index_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   575730 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_rjsf_utils_dist_utils_esm_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   320313 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_rjsf_validator-ajv8_dist_validator-ajv8_esm_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)  3384152 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_vega-embed_build_vega-embed_module_js.bundle.js
+-rw-r--r--   0 jitse     (1000) jitse     (1000)   366817 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_yjs_dist_yjs_mjs.bundle.js
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-24 11:02:46.260125 spyder-notebook-0.5.1/spyder_notebook/tests/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)      817 2023-04-29 21:10:29.000000 spyder-notebook-0.5.1/spyder_notebook/tests/test_config.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     8125 2023-07-23 21:35:45.000000 spyder-notebook-0.5.1/spyder_notebook/tests/test_plugin.py
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-24 11:02:46.260125 spyder-notebook-0.5.1/spyder_notebook/utils/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)      350 2023-02-05 14:13:01.000000 spyder-notebook-0.5.1/spyder_notebook/utils/__init__.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)      241 2023-02-05 14:13:44.000000 spyder-notebook-0.5.1/spyder_notebook/utils/localization.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    14226 2023-06-29 13:39:07.000000 spyder-notebook-0.5.1/spyder_notebook/utils/servermanager.py
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-24 11:02:46.260125 spyder-notebook-0.5.1/spyder_notebook/utils/templates/
+-rwxr-xr-x   0 jitse     (1000) jitse     (1000)    16050 2023-06-29 13:39:07.000000 spyder-notebook-0.5.1/spyder_notebook/utils/templates/welcome-dark.html
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    15935 2023-06-29 13:39:07.000000 spyder-notebook-0.5.1/spyder_notebook/utils/templates/welcome.html
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-24 11:02:46.260125 spyder-notebook-0.5.1/spyder_notebook/utils/tests/
+-rwxr-xr-x   0 jitse     (1000) jitse     (1000)     9910 2023-06-29 13:39:07.000000 spyder-notebook-0.5.1/spyder_notebook/utils/tests/test_servermanager.py
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-24 11:02:46.260125 spyder-notebook-0.5.1/spyder_notebook/widgets/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)      348 2023-02-05 14:13:01.000000 spyder-notebook-0.5.1/spyder_notebook/widgets/__init__.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    16346 2023-06-29 13:39:07.000000 spyder-notebook-0.5.1/spyder_notebook/widgets/client.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     2049 2023-02-11 22:17:54.000000 spyder-notebook-0.5.1/spyder_notebook/widgets/dom.py
+-rwxr-xr-x   0 jitse     (1000) jitse     (1000)     3942 2023-02-05 14:13:44.000000 spyder-notebook-0.5.1/spyder_notebook/widgets/example_app.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    13830 2023-07-23 21:35:45.000000 spyder-notebook-0.5.1/spyder_notebook/widgets/main_widget.py
+-rwxr-xr-x   0 jitse     (1000) jitse     (1000)    17725 2023-07-22 23:29:27.000000 spyder-notebook-0.5.1/spyder_notebook/widgets/notebooktabwidget.py
+-rwxr-xr-x   0 jitse     (1000) jitse     (1000)     4344 2023-02-05 14:13:44.000000 spyder-notebook-0.5.1/spyder_notebook/widgets/serverinfo.py
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-24 11:02:46.260125 spyder-notebook-0.5.1/spyder_notebook/widgets/tests/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     4079 2023-06-29 13:39:07.000000 spyder-notebook-0.5.1/spyder_notebook/widgets/tests/test_client.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     9534 2023-06-29 13:39:11.000000 spyder-notebook-0.5.1/spyder_notebook/widgets/tests/test_main_widget.py
+-rwxr-xr-x   0 jitse     (1000) jitse     (1000)     7927 2023-07-22 23:29:27.000000 spyder-notebook-0.5.1/spyder_notebook/widgets/tests/test_notebooktabwidget.py
+-rwxr-xr-x   0 jitse     (1000) jitse     (1000)     2511 2023-06-29 13:39:07.000000 spyder-notebook-0.5.1/spyder_notebook/widgets/tests/test_serverinfo.py
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-24 11:02:46.232125 spyder-notebook-0.5.1/spyder_notebook.egg-info/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     4705 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook.egg-info/PKG-INFO
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    28935 2023-07-24 11:02:46.000000 spyder-notebook-0.5.1/spyder_notebook.egg-info/SOURCES.txt
+-rw-r--r--   0 jitse     (1000) jitse     (1000)        1 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook.egg-info/dependency_links.txt
+-rw-r--r--   0 jitse     (1000) jitse     (1000)       74 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook.egg-info/entry_points.txt
+-rw-r--r--   0 jitse     (1000) jitse     (1000)       84 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook.egg-info/requires.txt
+-rw-r--r--   0 jitse     (1000) jitse     (1000)       33 2023-07-24 11:02:45.000000 spyder-notebook-0.5.1/spyder_notebook.egg-info/top_level.txt
```

### Comparing `spyder-notebook-0.5.0/CHANGELOG.md` & `spyder-notebook-0.5.1/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-## Version 0.5.0 (2023/07/24)
+## Version 0.5.1 (2023/07/24)
 
 This version is based on version 7 of Jupyter Notebook and version 4 of Jupyter Lab, thus profiting of many years of progress in Jupyter.
 
-### Mew Feature
+Version 0.5.0 was uploaded incorrectly.
+
+### New Feature
 
 * Base the plugin on Jupyter Notebook v7 ([Issue 330](https://github.com/spyder-ide/spyder-notebook/issues/330), [Issue 400](https://github.com/spyder-ide/spyder-notebook/issues/400), [Issue 401](https://github.com/spyder-ide/spyder-notebook/issues/401), [Issue 402](https://github.com/spyder-ide/spyder-notebook/issues/402), [Issue 414](https://github.com/spyder-ide/spyder-notebook/issues/414), [PR 396](https://github.com/spyder-ide/spyder-notebook/pull/396), [PR 415](https://github.com/spyder-ide/spyder-notebook/pull/415), [PR 419](https://github.com/spyder-ide/spyder-notebook/pull/419), [PR 420](https://github.com/spyder-ide/spyder-notebook/pull/420), [PR 429](https://github.com/spyder-ide/spyder-notebook/pull/429))
 
 ### Bug Fixes
 
 * Handle NotJSONError when closing a notebook tab ([Issue 432](https://github.com/spyder-ide/spyder-notebook/issues/432), [PR 437](https://github.com/spyder-ide/spyder-notebook/pull/437))
 * Ensure that the precise connection file is used when opening a console ([Issue 421](https://github.com/spyder-ide/spyder-notebook/issues/421), [PR 422](https://github.com/spyder-ide/spyder-notebook/pull/422))
```

### Comparing `spyder-notebook-0.5.0/LICENSE` & `spyder-notebook-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/PKG-INFO` & `spyder-notebook-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spyder-notebook
-Version: 0.5.0
+Version: 0.5.1
 Summary: Jupyter notebook integration with Spyder
 Home-page: https://github.com/spyder-ide/spyder-notebook
 Author: Spyder Development Team
 License: MIT
 Keywords: spyder jupyter notebook
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Jupyter
```

### Comparing `spyder-notebook-0.5.0/README.md` & `spyder-notebook-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/runtests.py` & `spyder-notebook-0.5.1/runtests.py`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/setup.py` & `spyder-notebook-0.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     def list2cmdline(cmd_list):
         """Convert list of arguments to a command line string."""
         return ' '.join(map(pipes.quote, cmd_list))
 
 
 HERE = os.path.abspath(os.path.dirname(__file__))
 SERVER_DIR = osp.join(HERE, 'spyder_notebook', 'server')
-BUILD_DIR = osp.join(SERVER_DIR, 'build')
+BUILD_DIR = osp.join(SERVER_DIR, 'static')
 
 
 def run(cmd, *args, **kwargs):
     """Echo a command before running it."""
     distutils.log.info('> ' + list2cmdline(cmd))
     kwargs['shell'] = (sys.platform == 'win32')
     return subprocess.check_call(cmd, *args, **kwargs)
```

### Comparing `spyder-notebook-0.5.0/spyder_notebook/__init__.py` & `spyder-notebook-0.5.1/spyder_notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/config.py` & `spyder-notebook-0.5.1/spyder_notebook/config.py`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/confpage.py` & `spyder-notebook-0.5.1/spyder_notebook/confpage.py`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/locale/de/LC_MESSAGES/spyder_notebook.mo` & `spyder-notebook-0.5.1/spyder_notebook/locale/de/LC_MESSAGES/spyder_notebook.mo`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/locale/es/LC_MESSAGES/spyder_notebook.mo` & `spyder-notebook-0.5.1/spyder_notebook/locale/es/LC_MESSAGES/spyder_notebook.mo`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/locale/fr/LC_MESSAGES/spyder_notebook.mo` & `spyder-notebook-0.5.1/spyder_notebook/locale/fr/LC_MESSAGES/spyder_notebook.mo`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/locale/hr/LC_MESSAGES/spyder_notebook.mo` & `spyder-notebook-0.5.1/spyder_notebook/locale/hr/LC_MESSAGES/spyder_notebook.mo`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/locale/hu/LC_MESSAGES/spyder_notebook.mo` & `spyder-notebook-0.5.1/spyder_notebook/locale/hu/LC_MESSAGES/spyder_notebook.mo`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/locale/ja/LC_MESSAGES/spyder_notebook.mo` & `spyder-notebook-0.5.1/spyder_notebook/locale/ja/LC_MESSAGES/spyder_notebook.mo`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/locale/pl/LC_MESSAGES/spyder_notebook.mo` & `spyder-notebook-0.5.1/spyder_notebook/locale/pl/LC_MESSAGES/spyder_notebook.mo`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/locale/pt_BR/LC_MESSAGES/spyder_notebook.mo` & `spyder-notebook-0.5.1/spyder_notebook/locale/pt_BR/LC_MESSAGES/spyder_notebook.mo`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/locale/ru/LC_MESSAGES/spyder_notebook.mo` & `spyder-notebook-0.5.1/spyder_notebook/locale/ru/LC_MESSAGES/spyder_notebook.mo`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/locale/zh_CN/LC_MESSAGES/spyder_notebook.mo` & `spyder-notebook-0.5.1/spyder_notebook/locale/zh_CN/LC_MESSAGES/spyder_notebook.mo`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/notebookplugin.py` & `spyder-notebook-0.5.1/spyder_notebook/notebookplugin.py`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/app/build/themes/@jupyterlab/theme-dark-extension/index.css` & `spyder-notebook-0.5.1/spyder_notebook/server/app/build/themes/@jupyterlab/theme-dark-extension/index.css`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/app/build/themes/@jupyterlab/theme-light-extension/index.css` & `spyder-notebook-0.5.1/spyder_notebook/server/app/build/themes/@jupyterlab/theme-light-extension/index.css`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/main.py` & `spyder-notebook-0.5.1/spyder_notebook/server/main.py`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/notebook-template.html` & `spyder-notebook-0.5.1/spyder_notebook/server/notebook-template.html`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/1cb1c39ea642f26a4dfe.woff` & `spyder-notebook-0.5.1/spyder_notebook/server/static/1cb1c39ea642f26a4dfe.woff`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/26683bf201fb258a2237.woff` & `spyder-notebook-0.5.1/spyder_notebook/server/static/26683bf201fb258a2237.woff`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/30e889b58cbc51adfbb0.woff` & `spyder-notebook-0.5.1/spyder_notebook/server/static/30e889b58cbc51adfbb0.woff`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/32792104b5ef69eded90.woff` & `spyder-notebook-0.5.1/spyder_notebook/server/static/32792104b5ef69eded90.woff`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/355254db9ca10a09a3b5.woff` & `spyder-notebook-0.5.1/spyder_notebook/server/static/355254db9ca10a09a3b5.woff`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/36e0d72d8a7afc696a3e.woff` & `spyder-notebook-0.5.1/spyder_notebook/server/static/36e0d72d8a7afc696a3e.woff`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/373c04fd2418f5c77eea.eot` & `spyder-notebook-0.5.1/spyder_notebook/server/static/373c04fd2418f5c77eea.eot`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/3bc6ecaae7ecf6f8d7f8.woff` & `spyder-notebook-0.5.1/spyder_notebook/server/static/3bc6ecaae7ecf6f8d7f8.woff`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/3de784d07b9fa8f104c1.woff` & `spyder-notebook-0.5.1/spyder_notebook/server/static/3de784d07b9fa8f104c1.woff`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/3f6d3488cf65374f6f67.woff` & `spyder-notebook-0.5.1/spyder_notebook/server/static/3f6d3488cf65374f6f67.woff`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/481e39042508ae313a60.woff` & `spyder-notebook-0.5.1/spyder_notebook/server/static/481e39042508ae313a60.woff`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/5cda41563a095bd70c78.woff` & `spyder-notebook-0.5.1/spyder_notebook/server/static/5cda41563a095bd70c78.woff`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/721921bab0d001ebff02.woff` & `spyder-notebook-0.5.1/spyder_notebook/server/static/721921bab0d001ebff02.woff`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/72bc573386dd1d48c5bb.woff` & `spyder-notebook-0.5.1/spyder_notebook/server/static/72bc573386dd1d48c5bb.woff`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/79d088064beb3826054f.eot` & `spyder-notebook-0.5.1/spyder_notebook/server/static/79d088064beb3826054f.eot`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/870673df72e70f87c91a.woff` & `spyder-notebook-0.5.1/spyder_notebook/server/static/870673df72e70f87c91a.woff`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/88b98cad3688915e50da.woff` & `spyder-notebook-0.5.1/spyder_notebook/server/static/88b98cad3688915e50da.woff`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/8ea8791754915a898a31.woff2` & `spyder-notebook-0.5.1/spyder_notebook/server/static/8ea8791754915a898a31.woff2`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/8ea8dbb1b02e6f730f55.woff` & `spyder-notebook-0.5.1/spyder_notebook/server/static/8ea8dbb1b02e6f730f55.woff`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/9674eb1bd55047179038.svg` & `spyder-notebook-0.5.1/spyder_notebook/server/static/9674eb1bd55047179038.svg`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/9834b82ad26e2a37583d.woff2` & `spyder-notebook-0.5.1/spyder_notebook/server/static/9834b82ad26e2a37583d.woff2`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/_8883-_5fa1-_1b46-_2abd-_0836.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/_8883-_5fa1-_1b46-_2abd-_0836.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/a009bea404f7a500ded4.woff` & `spyder-notebook-0.5.1/spyder_notebook/server/static/a009bea404f7a500ded4.woff`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/a3b9817780214caf01e8.svg` & `spyder-notebook-0.5.1/spyder_notebook/server/static/a3b9817780214caf01e8.svg`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/af04542b29eaac04550a.woff` & `spyder-notebook-0.5.1/spyder_notebook/server/static/af04542b29eaac04550a.woff`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/af6397503fcefbd61397.ttf` & `spyder-notebook-0.5.1/spyder_notebook/server/static/af6397503fcefbd61397.ttf`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/af96f67d7accf5fd2a4a.woff` & `spyder-notebook-0.5.1/spyder_notebook/server/static/af96f67d7accf5fd2a4a.woff`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/b418136e3b384baaadec.woff` & `spyder-notebook-0.5.1/spyder_notebook/server/static/b418136e3b384baaadec.woff`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/be0a084962d8066884f7.svg` & `spyder-notebook-0.5.1/spyder_notebook/server/static/be0a084962d8066884f7.svg`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/build_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/build_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/c49810b53ecc0d87d802.woff` & `spyder-notebook-0.5.1/spyder_notebook/server/static/c49810b53ecc0d87d802.woff`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/c56da8d69f1a0208b8e0.woff` & `spyder-notebook-0.5.1/spyder_notebook/server/static/c56da8d69f1a0208b8e0.woff`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/cb9e9e693192413cde2b.woff` & `spyder-notebook-0.5.1/spyder_notebook/server/static/cb9e9e693192413cde2b.woff`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/cda59d6efffa685830fd.ttf` & `spyder-notebook-0.5.1/spyder_notebook/server/static/cda59d6efffa685830fd.ttf`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/e4299464e7b012968eed.eot` & `spyder-notebook-0.5.1/spyder_notebook/server/static/e4299464e7b012968eed.eot`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/e42a88444448ac3d6054.woff2` & `spyder-notebook-0.5.1/spyder_notebook/server/static/e42a88444448ac3d6054.woff2`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/e8711bbb871afd8e9dea.ttf` & `spyder-notebook-0.5.1/spyder_notebook/server/static/e8711bbb871afd8e9dea.ttf`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/f9217f66874b0c01cd8c.woff` & `spyder-notebook-0.5.1/spyder_notebook/server/static/f9217f66874b0c01cd8c.woff`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/fc6ddf5df402b263cfb1.woff` & `spyder-notebook-0.5.1/spyder_notebook/server/static/fc6ddf5df402b263cfb1.woff`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_lang-json_dist_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_lang-json_dist_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_lang-wast_dist_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_lang-wast_dist_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_apl_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_apl_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_asciiarmor_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_asciiarmor_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_asn1_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_asn1_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_asterisk_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_asterisk_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_brainfuck_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_brainfuck_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_cmake_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_cmake_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_cobol_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_cobol_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_coffeescript_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_coffeescript_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_commonlisp_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_commonlisp_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_cypher_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_cypher_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_d_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_d_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_diff_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_diff_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_dockerfile_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_dockerfile_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_dtd_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_dtd_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_dylan_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_dylan_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_ebnf_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_ebnf_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_ecl_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_ecl_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_eiffel_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_eiffel_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_elm_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_elm_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_factor_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_factor_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_fcl_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_fcl_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_forth_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_forth_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_fortran_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_fortran_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_gas_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_gas_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_go_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_go_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_groovy_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_groovy_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_haskell_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_haskell_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_http_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_http_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_jinja2_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_jinja2_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_livescript_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_livescript_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_lua_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_lua_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_mathematica_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_mathematica_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_mbox_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_mbox_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_mirc_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_mirc_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_mllike_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_mllike_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_modelica_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_modelica_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_mscgen_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_mscgen_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_mumps_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_mumps_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_nginx_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_nginx_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_ntriples_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_ntriples_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_octave_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_octave_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_oz_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_oz_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_pascal_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_pascal_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_pig_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_pig_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_properties_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_properties_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_protobuf_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_protobuf_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_puppet_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_puppet_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_q_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_q_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_r_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_r_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_rpm_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_rpm_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_ruby_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_ruby_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_shell_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_shell_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_sieve_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_sieve_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_smalltalk_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_smalltalk_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_solr_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_solr_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_sparql_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_sparql_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_spreadsheet_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_spreadsheet_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_stex_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_stex_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_swift_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_swift_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_tcl_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_tcl_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_tiddlywiki_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_tiddlywiki_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_tiki_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_tiki_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_toml_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_toml_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_troff_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_troff_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_ttcn-cfg_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_ttcn-cfg_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_ttcn_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_ttcn_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_turtle_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_turtle_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_vb_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_vb_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_velocity_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_velocity_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_vhdl_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_vhdl_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_webidl_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_webidl_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_yacas_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_yacas_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_yaml_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_yaml_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_z80_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_codemirror_legacy-modes_mode_z80_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyter-notebook_docmanager-extension_lib_index_js-_e4b40.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyter-notebook_docmanager-extension_lib_index_js-_e4b40.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyter-notebook_docmanager-extension_lib_index_js-_e4b41.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyter-notebook_docmanager-extension_lib_index_js-_e4b41.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyter-notebook_documentsearch-extension_lib_index_js-_32b90.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyter-notebook_documentsearch-extension_lib_index_js-_32b90.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyter-notebook_documentsearch-extension_lib_index_js-_32b91.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyter-notebook_documentsearch-extension_lib_index_js-_32b91.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyter-notebook_help-extension_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyter-notebook_help-extension_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyter-notebook_ui-components_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyter-notebook_ui-components_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_cell-toolbar-extension_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_cell-toolbar-extension_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_celltags-extension_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_celltags-extension_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_completer-extension_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_completer-extension_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_htmlviewer-extension_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_htmlviewer-extension_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_htmlviewer_lib_index_js-_f0bb0.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_htmlviewer_lib_index_js-_f0bb0.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_htmlviewer_lib_index_js-_f0bb1.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_htmlviewer_lib_index_js-_f0bb1.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_hub-extension_lib_index_js-_9dda0.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_hub-extension_lib_index_js-_9dda0.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_hub-extension_lib_index_js-_9dda1.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_hub-extension_lib_index_js-_9dda1.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_imageviewer-extension_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_imageviewer-extension_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_imageviewer_lib_index_js-_afb90.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_imageviewer_lib_index_js-_afb90.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_imageviewer_lib_index_js-_afb91.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_imageviewer_lib_index_js-_afb91.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_javascript-extension_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_javascript-extension_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_json-extension_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_json-extension_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_markedparser-extension_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_markedparser-extension_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_mathjax-extension_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_mathjax-extension_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_nbformat_lib_index_js-_a6f70.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_nbformat_lib_index_js-_a6f70.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_nbformat_lib_index_js-_a6f71.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_nbformat_lib_index_js-_a6f71.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_pdf-extension_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_pdf-extension_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_property-inspector_lib_index_js-_90690.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_property-inspector_lib_index_js-_90690.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_property-inspector_lib_index_js-_90691.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_property-inspector_lib_index_js-_90691.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_rendermime-extension_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_rendermime-extension_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_rendermime-interfaces_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_rendermime-interfaces_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_theme-dark-extension_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_theme-dark-extension_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_theme-light-extension_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_theme-light-extension_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_tooltip_lib_index_js-_d1c70.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_tooltip_lib_index_js-_d1c70.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_tooltip_lib_index_js-_d1c71.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_tooltip_lib_index_js-_d1c71.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_translation-extension_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_translation-extension_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_ui-components-extension_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_ui-components-extension_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_jupyterlab_vega5-extension_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_jupyterlab_vega5-extension_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_lumino_disposable_dist_index_es6_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_lumino_disposable_dist_index_es6_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_lumino_keyboard_dist_index_es6_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_lumino_keyboard_dist_index_es6_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_lumino_properties_dist_index_es6_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_lumino_properties_dist_index_es6_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_mathjax-full_js_mathjax_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_mathjax-full_js_mathjax_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_mathjax-full_js_util_Options_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_mathjax-full_js_util_Options_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/node_modules_process_browser_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/node_modules_process_browser_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/packages_application-extension_lib_index_js-_90450.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/packages_application-extension_lib_index_js-_90450.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/packages_application-extension_lib_index_js-_90451.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/packages_application-extension_lib_index_js-_90451.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_autocomplete_dist_index_js-node_modules_lezer_lr_dist_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_autocomplete_dist_index_js-node_modules_lezer_lr_dist_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_commands_dist_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_commands_dist_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_lang-cpp_dist_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_lang-cpp_dist_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_lang-css_dist_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_lang-css_dist_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_lang-html_dist_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_lang-html_dist_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_lang-java_dist_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_lang-java_dist_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_lang-javascript_dist_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_lang-javascript_dist_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_lang-markdown_dist_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_lang-markdown_dist_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_lang-php_dist_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_lang-php_dist_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_lang-python_dist_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_lang-python_dist_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_lang-rust_dist_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_lang-rust_dist_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_lang-sql_dist_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_lang-sql_dist_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_lang-xml_dist_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_lang-xml_dist_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_language_dist_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_language_dist_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_clike_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_clike_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_clojure_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_clojure_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_crystal_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_crystal_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_css_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_css_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_erlang_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_erlang_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_gherkin_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_gherkin_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_haxe_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_haxe_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_idl_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_idl_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_javascript_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_javascript_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_julia_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_julia_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_nsis_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_nsis_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_perl_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_perl_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_powershell_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_powershell_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_python_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_python_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_sas_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_sas_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_scheme_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_scheme_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_sql_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_sql_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_stylus_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_stylus_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_textile_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_textile_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_vbscript_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_vbscript_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_verilog_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_verilog_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_xquery_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_legacy-modes_mode_xquery_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_search_dist_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_search_dist_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_codemirror_view_dist_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_codemirror_view_dist_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_fast-deep-equal_index_js-node_modules_json-schema-traverse_index_js-node-057f3c.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_fast-deep-equal_index_js-node_modules_json-schema-traverse_index_js-node-057f3c.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyter-notebook_application-extension_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyter-notebook_application-extension_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyter-notebook_application-extension_style_index_js-node_modules_jupyt-7c11f7.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyter-notebook_application-extension_style_index_js-node_modules_jupyt-7c11f7.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyter-notebook_application_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyter-notebook_application_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyter-notebook_notebook-extension_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyter-notebook_notebook-extension_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyter_ydoc_lib_index_js-node_modules_process_browser_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyter_ydoc_lib_index_js-node_modules_process_browser_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_application-extension_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_application-extension_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_application_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_application_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_application_lib_mimerenderers_js-node_modules_jupyterlab_appl-fdcfe8.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_application_lib_mimerenderers_js-node_modules_jupyterlab_appl-fdcfe8.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_apputils-extension_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_apputils-extension_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_apputils_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_apputils_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_cell-toolbar_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_cell-toolbar_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_cells_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_cells_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_codeeditor_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_codeeditor_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_codemirror-extension_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_codemirror-extension_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_codemirror_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_codemirror_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_completer_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_completer_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_console_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_console_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_coreutils_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_coreutils_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_debugger-extension_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_debugger-extension_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_debugger_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_debugger_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_debugger_lib_panels_variables_gridpanel_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_debugger_lib_panels_variables_gridpanel_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_docmanager-extension_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_docmanager-extension_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_docmanager_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_docmanager_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_docregistry_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_docregistry_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_documentsearch-extension_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_documentsearch-extension_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_documentsearch_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_documentsearch_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_filebrowser-extension_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_filebrowser-extension_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_filebrowser_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_filebrowser_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_fileeditor-extension_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_fileeditor-extension_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_fileeditor_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_fileeditor_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_json-extension_lib_component_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_json-extension_lib_component_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_launcher_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_launcher_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_logconsole_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_logconsole_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_lsp-extension_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_lsp-extension_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_lsp_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_lsp_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_mainmenu-extension_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_mainmenu-extension_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_mainmenu_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_mainmenu_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_metadataform-extension_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_metadataform-extension_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_metadataform_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_metadataform_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_notebook-extension_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_notebook-extension_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_notebook_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_notebook_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_observables_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_observables_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_outputarea_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_outputarea_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_rendermime_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_rendermime_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_running_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_running_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_services_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_services_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_settingregistry_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_settingregistry_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_shortcuts-extension_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_shortcuts-extension_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_statedb_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_statedb_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_statusbar_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_statusbar_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_toc-extension_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_toc-extension_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_toc_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_toc_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_tooltip-extension_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_tooltip-extension_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_translation_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_translation_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_jupyterlab_ui-components_lib_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_jupyterlab_ui-components_lib_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_lezer_common_dist_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_lezer_common_dist_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_lezer_highlight_dist_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_lezer_highlight_dist_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_lib0_buffer_js-node_modules_lib0_encoding_js-node_modules_lib0_observabl-50dfe2.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_lib0_buffer_js-node_modules_lib0_encoding_js-node_modules_lib0_observabl-50dfe2.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_lodash-es__baseClone_js-node_modules_lodash-es_get_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_lodash-es__baseClone_js-node_modules_lodash-es_get_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_lodash-es_has_js-node_modules_lodash-es_hasIn_js-node_modules_lodash-es_-930c1c.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_lodash-es_has_js-node_modules_lodash-es_hasIn_js-node_modules_lodash-es_-930c1c.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_lumino_algorithm_dist_index_es6_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_lumino_algorithm_dist_index_es6_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_lumino_application_dist_index_es6_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_lumino_application_dist_index_es6_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_lumino_commands_dist_index_es6_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_lumino_commands_dist_index_es6_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_lumino_coreutils_dist_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_lumino_coreutils_dist_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_lumino_domutils_dist_index_es6_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_lumino_domutils_dist_index_es6_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_lumino_dragdrop_dist_index_es6_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_lumino_dragdrop_dist_index_es6_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_lumino_messaging_dist_index_es6_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_lumino_messaging_dist_index_es6_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_lumino_polling_dist_index_es6_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_lumino_polling_dist_index_es6_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_lumino_signaling_dist_index_es6_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_lumino_signaling_dist_index_es6_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_lumino_virtualdom_dist_index_es6_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_lumino_virtualdom_dist_index_es6_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_lumino_widgets_dist_index_es6_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_lumino_widgets_dist_index_es6_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_marked_lib_marked_esm_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_marked_lib_marked_esm_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_a11y_assistive-mml_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_a11y_assistive-mml_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_adaptors_browserAdaptor_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_adaptors_browserAdaptor_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_core_MathItem_js-node_modules_mathjax-full_js_core_MmlTr-144bb4.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_core_MathItem_js-node_modules_mathjax-full_js_core_MmlTr-144bb4.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_core_MmlTree_MmlFactory_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_core_MmlTree_MmlFactory_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_core_MmlTree_MmlNodes_mo_js-node_modules_mathjax-full_js-e92534.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_core_MmlTree_MmlNodes_mo_js-node_modules_mathjax-full_js-e92534.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_handlers_html_HTMLHandler_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_handlers_html_HTMLHandler_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_input_tex_AllPackages_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_input_tex_AllPackages_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_input_tex_Configuration_js-node_modules_mathjax-full_js_-8c4c26.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_input_tex_Configuration_js-node_modules_mathjax-full_js_-8c4c26.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_input_tex_ParseOptions_js-node_modules_mathjax-full_js_i-0c5d92.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_input_tex_ParseOptions_js-node_modules_mathjax-full_js_i-0c5d92.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_input_tex_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_input_tex_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_input_tex_require_RequireConfiguration_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_input_tex_require_RequireConfiguration_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_output_chtml_fonts_tex_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_output_chtml_fonts_tex_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_output_chtml_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_output_chtml_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_ui_safe_SafeHandler_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_mathjax-full_js_ui_safe_SafeHandler_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_react-dom_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_react-dom_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_react-toastify_dist_react-toastify_esm_mjs.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_react-toastify_dist_react-toastify_esm_mjs.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_react_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_react_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_regexp-match-indices_index_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_regexp-match-indices_index_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_rjsf_utils_dist_utils_esm_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_rjsf_utils_dist_utils_esm_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_rjsf_validator-ajv8_dist_validator-ajv8_esm_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_rjsf_validator-ajv8_dist_validator-ajv8_esm_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_vega-embed_build_vega-embed_module_js.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_vega-embed_build_vega-embed_module_js.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/server/static/vendors-node_modules_yjs_dist_yjs_mjs.bundle.js` & `spyder-notebook-0.5.1/spyder_notebook/server/static/vendors-node_modules_yjs_dist_yjs_mjs.bundle.js`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/tests/test_config.py` & `spyder-notebook-0.5.1/spyder_notebook/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/tests/test_plugin.py` & `spyder-notebook-0.5.1/spyder_notebook/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/utils/servermanager.py` & `spyder-notebook-0.5.1/spyder_notebook/utils/servermanager.py`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/utils/templates/welcome-dark.html` & `spyder-notebook-0.5.1/spyder_notebook/utils/templates/welcome-dark.html`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/utils/templates/welcome.html` & `spyder-notebook-0.5.1/spyder_notebook/utils/templates/welcome.html`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/utils/tests/test_servermanager.py` & `spyder-notebook-0.5.1/spyder_notebook/utils/tests/test_servermanager.py`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/widgets/client.py` & `spyder-notebook-0.5.1/spyder_notebook/widgets/client.py`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/widgets/dom.py` & `spyder-notebook-0.5.1/spyder_notebook/widgets/dom.py`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/widgets/example_app.py` & `spyder-notebook-0.5.1/spyder_notebook/widgets/example_app.py`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/widgets/main_widget.py` & `spyder-notebook-0.5.1/spyder_notebook/widgets/main_widget.py`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/widgets/notebooktabwidget.py` & `spyder-notebook-0.5.1/spyder_notebook/widgets/notebooktabwidget.py`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/widgets/serverinfo.py` & `spyder-notebook-0.5.1/spyder_notebook/widgets/serverinfo.py`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/widgets/tests/test_client.py` & `spyder-notebook-0.5.1/spyder_notebook/widgets/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/widgets/tests/test_main_widget.py` & `spyder-notebook-0.5.1/spyder_notebook/widgets/tests/test_main_widget.py`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/widgets/tests/test_notebooktabwidget.py` & `spyder-notebook-0.5.1/spyder_notebook/widgets/tests/test_notebooktabwidget.py`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook/widgets/tests/test_serverinfo.py` & `spyder-notebook-0.5.1/spyder_notebook/widgets/tests/test_serverinfo.py`

 * *Files identical despite different names*

### Comparing `spyder-notebook-0.5.0/spyder_notebook.egg-info/PKG-INFO` & `spyder-notebook-0.5.1/spyder_notebook.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spyder-notebook
-Version: 0.5.0
+Version: 0.5.1
 Summary: Jupyter notebook integration with Spyder
 Home-page: https://github.com/spyder-ide/spyder-notebook
 Author: Spyder Development Team
 License: MIT
 Keywords: spyder jupyter notebook
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Jupyter
```

### Comparing `spyder-notebook-0.5.0/spyder_notebook.egg-info/SOURCES.txt` & `spyder-notebook-0.5.1/spyder_notebook.egg-info/SOURCES.txt`

 * *Files identical despite different names*

