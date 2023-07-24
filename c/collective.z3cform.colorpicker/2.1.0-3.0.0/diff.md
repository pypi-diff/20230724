# Comparing `tmp/collective.z3cform.colorpicker-2.1.0.tar.gz` & `tmp/collective.z3cform.colorpicker-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/collective.z3cform.colorpicker-2.1.0.tar", last modified: Fri Sep 17 08:20:10 2021, max compression
+gzip compressed data, was "collective.z3cform.colorpicker-3.0.0.tar", last modified: Mon Jul 24 13:51:17 2023, max compression
```

## Comparing `collective.z3cform.colorpicker-2.1.0.tar` & `collective.z3cform.colorpicker-3.0.0.tar`

### file list

```diff
@@ -1,110 +1,53 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-09-17 08:20:10.000000 collective.z3cform.colorpicker-2.1.0/
--rw-r--r--   0 maurits    (501) staff       (20)     6235 2021-09-17 08:20:10.000000 collective.z3cform.colorpicker-2.1.0/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      188 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/MANIFEST.in
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    12282 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)     1390 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/docs/INSTALL.txt
--rw-r--r--   0 maurits    (501) staff       (20)      761 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/docs/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1824 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/setup.py
--rw-r--r--   0 maurits    (501) staff       (20)      173 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/CONTRIBUTORS.rst
--rw-r--r--   0 maurits    (501) staff       (20)       94 2021-09-17 08:20:10.000000 collective.z3cform.colorpicker-2.1.0/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1550 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1919 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/CHANGES.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-09-17 08:20:10.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-09-17 08:20:10.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/demo/
--rw-r--r--   0 maurits    (501) staff       (20)      358 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/demo/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)        0 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/demo/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1152 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/demo/browser.py
--rw-r--r--   0 maurits    (501) staff       (20)     2611 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1599 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/colorpickeralpha_input.pt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-09-17 08:20:10.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/locales/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/locales/it/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-09-17 08:20:10.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/locales/it/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)      852 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/locales/it/LC_MESSAGES/collective.z3cform.colorpicker.po
--rw-r--r--   0 maurits    (501) staff       (20)      591 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/locales/it/LC_MESSAGES/collective.z3cform.colorpicker.mo
--rwxr-xr-x   0 maurits    (501) staff       (20)     1322 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/locales/rebuild.sh
--rw-r--r--   0 maurits    (501) staff       (20)      828 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/locales/collective.z3cform.colorpicker.pot
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/locales/nl/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-09-17 08:20:10.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/locales/nl/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)      909 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/locales/nl/LC_MESSAGES/collective.z3cform.colorpicker.po
--rw-r--r--   0 maurits    (501) staff       (20)      692 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/locales/nl/LC_MESSAGES/collective.z3cform.colorpicker.mo
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/locales/es/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-09-17 08:20:10.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/locales/es/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)     1082 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/locales/es/LC_MESSAGES/collective.z3cform.colorpicker.po
--rw-r--r--   0 maurits    (501) staff       (20)      777 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/locales/es/LC_MESSAGES/collective.z3cform.colorpicker.mo
--rw-r--r--   0 maurits    (501) staff       (20)      314 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/fields.py
--rw-r--r--   0 maurits    (501) staff       (20)      793 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/colorpicker.py
--rw-r--r--   0 maurits    (501) staff       (20)     1598 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/colorpicker_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      163 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-09-17 08:20:10.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/
--rw-r--r--   0 maurits    (501) staff       (20)      807 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/Gruntfile.js
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-09-17 08:20:10.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/less/
--rw-r--r--   0 maurits    (501) staff       (20)     1278 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/less/colorpicker.less
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/bower_components/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-09-17 08:20:10.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/bower_components/mjolnic-bootstrap-colorpicker/
--rw-r--r--   0 maurits    (501) staff       (20)      552 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/bower_components/mjolnic-bootstrap-colorpicker/LICENSE
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/bower_components/mjolnic-bootstrap-colorpicker/dist/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-09-17 08:20:10.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/bower_components/mjolnic-bootstrap-colorpicker/dist/css/
--rw-r--r--   0 maurits    (501) staff       (20)     3853 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/bower_components/mjolnic-bootstrap-colorpicker/dist/css/bootstrap-colorpicker.min.css
--rw-r--r--   0 maurits    (501) staff       (20)     4599 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/bower_components/mjolnic-bootstrap-colorpicker/dist/css/bootstrap-colorpicker.css
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-09-17 08:20:10.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/bower_components/mjolnic-bootstrap-colorpicker/dist/js/
--rw-r--r--   0 maurits    (501) staff       (20)    18278 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/bower_components/mjolnic-bootstrap-colorpicker/dist/js/bootstrap-colorpicker.min.js
--rw-r--r--   0 maurits    (501) staff       (20)    34100 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/bower_components/mjolnic-bootstrap-colorpicker/dist/js/bootstrap-colorpicker.js
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/bower_components/mjolnic-bootstrap-colorpicker/dist/img/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-09-17 08:20:10.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/bower_components/mjolnic-bootstrap-colorpicker/dist/img/bootstrap-colorpicker/
--rw-r--r--   0 maurits    (501) staff       (20)     2972 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/bower_components/mjolnic-bootstrap-colorpicker/dist/img/bootstrap-colorpicker/hue.png
--rw-r--r--   0 maurits    (501) staff       (20)     3635 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/bower_components/mjolnic-bootstrap-colorpicker/dist/img/bootstrap-colorpicker/alpha-horizontal.png
--rw-r--r--   0 maurits    (501) staff       (20)     3271 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/bower_components/mjolnic-bootstrap-colorpicker/dist/img/bootstrap-colorpicker/alpha.png
--rw-r--r--   0 maurits    (501) staff       (20)     2837 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/bower_components/mjolnic-bootstrap-colorpicker/dist/img/bootstrap-colorpicker/hue-horizontal.png
--rw-r--r--   0 maurits    (501) staff       (20)     8817 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/bower_components/mjolnic-bootstrap-colorpicker/dist/img/bootstrap-colorpicker/saturation.png
--rw-r--r--   0 maurits    (501) staff       (20)      363 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/bower_components/mjolnic-bootstrap-colorpicker/bower.json
--rw-r--r--   0 maurits    (501) staff       (20)     1051 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/bower_components/mjolnic-bootstrap-colorpicker/README.md
--rw-r--r--   0 maurits    (501) staff       (20)     1875 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/bower_components/mjolnic-bootstrap-colorpicker/CONTRIBUTING.md
--rw-r--r--   0 maurits    (501) staff       (20)      716 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/bower_components/mjolnic-bootstrap-colorpicker/.bower.json
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/js/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-09-17 08:20:10.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/js/patterns/
--rw-r--r--   0 maurits    (501) staff       (20)     1360 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/js/patterns/colorpicker.js
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-09-17 08:20:10.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/js/bundles/
--rw-r--r--   0 maurits    (501) staff       (20)      741 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/js/bundles/colorpicker.js
--rw-r--r--   0 maurits    (501) staff       (20)      872 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/Makefile
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-09-17 08:20:10.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/tests/
--rw-r--r--   0 maurits    (501) staff       (20)     1876 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/tests/pattern-colorpicker-test.js
--rw-r--r--   0 maurits    (501) staff       (20)      807 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/tests/config.js
--rw-r--r--   0 maurits    (501) staff       (20)      569 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/.jshintrc
--rw-r--r--   0 maurits    (501) staff       (20)      237 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/bower.json
--rw-r--r--   0 maurits    (501) staff       (20)     1049 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/config.js
--rw-r--r--   0 maurits    (501) staff       (20)      173 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/.editorconfig
--rw-r--r--   0 maurits    (501) staff       (20)      109 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/README.md
--rw-r--r--   0 maurits    (501) staff       (20)     1449 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/package.json
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-09-17 08:20:10.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/dev/
--rw-r--r--   0 maurits    (501) staff       (20)     2543 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/dev/dev.html
--rw-r--r--   0 maurits    (501) staff       (20)     1921 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/dev/dev.js
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-09-17 08:20:10.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/build/
--rw-r--r--   0 maurits    (501) staff       (20)   202134 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/build/colorpicker.min.js
--rw-r--r--   0 maurits    (501) staff       (20)      976 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/build/colorpicker.min.css
--rw-r--r--   0 maurits    (501) staff       (20)    25383 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/build/colorpicker.dev.js
--rw-r--r--   0 maurits    (501) staff       (20)   425438 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/build/colorpicker.js
--rw-r--r--   0 maurits    (501) staff       (20)   204053 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/build/colorpicker.min.map
--rw-r--r--   0 maurits    (501) staff       (20)    25720 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/static/build/colorpicker.dev.map
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-09-17 08:20:10.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)     1811 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/profiles/default/registry.xml
--rw-r--r--   0 maurits    (501) staff       (20)      166 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)      901 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/colorpickeralpha_display.pt
--rw-r--r--   0 maurits    (501) staff       (20)      824 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/colorpickeralpha.py
--rw-r--r--   0 maurits    (501) staff       (20)     1254 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/z3cform_colorpicker.js
--rw-r--r--   0 maurits    (501) staff       (20)      901 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/colorpicker_display.pt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective.z3cform.colorpicker.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)     6235 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective.z3cform.colorpicker.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)        1 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective.z3cform.colorpicker.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)       30 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective.z3cform.colorpicker.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)     5117 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective.z3cform.colorpicker.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)       82 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective.z3cform.colorpicker.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)       46 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective.z3cform.colorpicker.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)       11 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective.z3cform.colorpicker.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2021-09-17 08:20:09.000000 collective.z3cform.colorpicker-2.1.0/src/collective.z3cform.colorpicker.egg-info/dependency_links.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-24 13:51:17.176240 collective.z3cform.colorpicker-3.0.0/
+-rw-r--r--   0 maurits    (501) staff       (20)     2086 2023-07-24 13:51:16.000000 collective.z3cform.colorpicker-3.0.0/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      173 2023-07-24 13:51:16.000000 collective.z3cform.colorpicker-3.0.0/CONTRIBUTORS.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      188 2023-07-24 13:51:16.000000 collective.z3cform.colorpicker-3.0.0/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)     4473 2023-07-24 13:51:17.176335 collective.z3cform.colorpicker-3.0.0/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1271 2023-07-24 13:51:16.000000 collective.z3cform.colorpicker-3.0.0/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-24 13:51:17.168830 collective.z3cform.colorpicker-3.0.0/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)     1390 2023-07-24 13:51:16.000000 collective.z3cform.colorpicker-3.0.0/docs/INSTALL.txt
+-rw-r--r--   0 maurits    (501) staff       (20)    12282 2023-07-24 13:51:16.000000 collective.z3cform.colorpicker-3.0.0/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      761 2023-07-24 13:51:16.000000 collective.z3cform.colorpicker-3.0.0/docs/LICENSE.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       94 2023-07-24 13:51:17.176791 collective.z3cform.colorpicker-3.0.0/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     1665 2023-07-24 13:51:16.000000 collective.z3cform.colorpicker-3.0.0/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-24 13:51:17.165006 collective.z3cform.colorpicker-3.0.0/src/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-24 13:51:17.169221 collective.z3cform.colorpicker-3.0.0/src/collective/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-07-24 13:51:16.000000 collective.z3cform.colorpicker-3.0.0/src/collective/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-24 13:51:17.171754 collective.z3cform.colorpicker-3.0.0/src/collective/z3cform/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-07-24 13:51:16.000000 collective.z3cform.colorpicker-3.0.0/src/collective/z3cform/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-24 13:51:17.173365 collective.z3cform.colorpicker-3.0.0/src/collective/z3cform/colorpicker/
+-rw-r--r--   0 maurits    (501) staff       (20)       74 2023-07-24 13:51:16.000000 collective.z3cform.colorpicker-3.0.0/src/collective/z3cform/colorpicker/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      762 2023-07-24 13:51:16.000000 collective.z3cform.colorpicker-3.0.0/src/collective/z3cform/colorpicker/colorpicker.py
+-rw-r--r--   0 maurits    (501) staff       (20)      901 2023-07-24 13:51:16.000000 collective.z3cform.colorpicker-3.0.0/src/collective/z3cform/colorpicker/colorpicker_display.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1483 2023-07-24 13:51:16.000000 collective.z3cform.colorpicker-3.0.0/src/collective/z3cform/colorpicker/colorpicker_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1649 2023-07-24 13:51:16.000000 collective.z3cform.colorpicker-3.0.0/src/collective/z3cform/colorpicker/configure.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-24 13:51:17.174274 collective.z3cform.colorpicker-3.0.0/src/collective/z3cform/colorpicker/demo/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-24 13:51:16.000000 collective.z3cform.colorpicker-3.0.0/src/collective/z3cform/colorpicker/demo/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      898 2023-07-24 13:51:16.000000 collective.z3cform.colorpicker-3.0.0/src/collective/z3cform/colorpicker/demo/browser.py
+-rw-r--r--   0 maurits    (501) staff       (20)      358 2023-07-24 13:51:16.000000 collective.z3cform.colorpicker-3.0.0/src/collective/z3cform/colorpicker/demo/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      208 2023-07-24 13:51:16.000000 collective.z3cform.colorpicker-3.0.0/src/collective/z3cform/colorpicker/fields.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-24 13:51:17.174797 collective.z3cform.colorpicker-3.0.0/src/collective/z3cform/colorpicker/locales/
+-rw-r--r--   0 maurits    (501) staff       (20)      828 2023-07-24 13:51:16.000000 collective.z3cform.colorpicker-3.0.0/src/collective/z3cform/colorpicker/locales/collective.z3cform.colorpicker.pot
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-24 13:51:17.165707 collective.z3cform.colorpicker-3.0.0/src/collective/z3cform/colorpicker/locales/es/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-24 13:51:17.175055 collective.z3cform.colorpicker-3.0.0/src/collective/z3cform/colorpicker/locales/es/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)     1082 2023-07-24 13:51:16.000000 collective.z3cform.colorpicker-3.0.0/src/collective/z3cform/colorpicker/locales/es/LC_MESSAGES/collective.z3cform.colorpicker.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-24 13:51:17.165895 collective.z3cform.colorpicker-3.0.0/src/collective/z3cform/colorpicker/locales/it/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-24 13:51:17.175283 collective.z3cform.colorpicker-3.0.0/src/collective/z3cform/colorpicker/locales/it/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)      852 2023-07-24 13:51:16.000000 collective.z3cform.colorpicker-3.0.0/src/collective/z3cform/colorpicker/locales/it/LC_MESSAGES/collective.z3cform.colorpicker.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-24 13:51:17.166081 collective.z3cform.colorpicker-3.0.0/src/collective/z3cform/colorpicker/locales/nl/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-24 13:51:17.175509 collective.z3cform.colorpicker-3.0.0/src/collective/z3cform/colorpicker/locales/nl/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)      909 2023-07-24 13:51:16.000000 collective.z3cform.colorpicker-3.0.0/src/collective/z3cform/colorpicker/locales/nl/LC_MESSAGES/collective.z3cform.colorpicker.po
+-rwxr-xr-x   0 maurits    (501) staff       (20)     1322 2023-07-24 13:51:16.000000 collective.z3cform.colorpicker-3.0.0/src/collective/z3cform/colorpicker/locales/rebuild.sh
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-24 13:51:17.166272 collective.z3cform.colorpicker-3.0.0/src/collective/z3cform/colorpicker/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-24 13:51:17.176088 collective.z3cform.colorpicker-3.0.0/src/collective/z3cform/colorpicker/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)      166 2023-07-24 13:51:16.000000 collective.z3cform.colorpicker-3.0.0/src/collective/z3cform/colorpicker/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-24 13:51:16.000000 collective.z3cform.colorpicker-3.0.0/src/collective/z3cform/colorpicker/profiles/default/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-24 13:51:17.171424 collective.z3cform.colorpicker-3.0.0/src/collective.z3cform.colorpicker.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)     4473 2023-07-24 13:51:17.000000 collective.z3cform.colorpicker-3.0.0/src/collective.z3cform.colorpicker.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1659 2023-07-24 13:51:17.000000 collective.z3cform.colorpicker-3.0.0/src/collective.z3cform.colorpicker.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-24 13:51:17.000000 collective.z3cform.colorpicker-3.0.0/src/collective.z3cform.colorpicker.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2023-07-24 13:51:17.000000 collective.z3cform.colorpicker-3.0.0/src/collective.z3cform.colorpicker.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       30 2023-07-24 13:51:17.000000 collective.z3cform.colorpicker-3.0.0/src/collective.z3cform.colorpicker.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-24 13:51:17.000000 collective.z3cform.colorpicker-3.0.0/src/collective.z3cform.colorpicker.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)       46 2023-07-24 13:51:17.000000 collective.z3cform.colorpicker-3.0.0/src/collective.z3cform.colorpicker.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       11 2023-07-24 13:51:17.000000 collective.z3cform.colorpicker-3.0.0/src/collective.z3cform.colorpicker.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `collective.z3cform.colorpicker-2.1.0/docs/LICENSE.GPL` & `collective.z3cform.colorpicker-3.0.0/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.z3cform.colorpicker-2.1.0/docs/INSTALL.txt` & `collective.z3cform.colorpicker-3.0.0/docs/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `collective.z3cform.colorpicker-2.1.0/docs/LICENSE.txt` & `collective.z3cform.colorpicker-3.0.0/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `collective.z3cform.colorpicker-2.1.0/setup.py` & `collective.z3cform.colorpicker-3.0.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = '2.1.0'
+version = '3.0.0'
 
 long_description = (
     open('README.rst').read()
     + '\n' +
     'Contributors\n'
     '============\n'
     + '\n' +
@@ -19,26 +19,22 @@
     version=version,
     description="Colorpicker widget for Plone",
     long_description=long_description,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
-        "Framework :: Plone :: 4.3",
-        "Framework :: Plone :: 5.0",
-        "Framework :: Plone :: 5.1",
-        "Framework :: Plone :: 5.2",
+        "Framework :: Plone :: 6.0",
         "Intended Audience :: End Users/Desktop",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2.7",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Topic :: Internet",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     keywords='plone z3cform colorpicker widget',
     author='Giorgio Borelli',
     author_email='giorgio@giorgioborelli.it',
     url='http://www.giorgioborelli.it',
```

### Comparing `collective.z3cform.colorpicker-2.1.0/README.rst` & `collective.z3cform.colorpicker-3.0.0/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,64 +1,61 @@
 .. contents::
 
 Introduction
 ============
 
-collective.z3cform.colorpicker provides a color picker widget for
-z3c.form based `bootstrap-colopicker`_.
+collective.z3cform.colorpicker provides a color picker widget, which uses the Browser native color input.
 
 .. image:: https://raw.githubusercontent.com/collective/collective.z3cform.colorpicker/master/screenshot.png
 
 
 Requirements
 ============
 
 * Plone >= 5.0
 * plone.app.z3cform
 
-
 For previous Plone versions use a version collective.z3cform.colorpicker
 less than 2.x
 
 
 Installation
 ============
 
-This addon can be installed has any other addons, please follow official
-documentation_.
+Install collective.z3cform.colorpicker by adding it to your buildout::
+
+    [buildout]
+
+    ...
+
+    eggs =
+        collective.z3cform.colorpicker
+
+
+and then running ``bin/buildout``
+
+or installing it via ``pip install collective.z3cform.colorpicker``
 
 
 Usage
 =====
 
 You can use this widget setting the "widgetFactory" property of a form field:
 ::
 
         from z3c.form import form, field
         from collective.z3cform.colorpicker import Color
-        from collective.z3cform.colorpicker import ColorAlpha
 
         class IColorForm(interface.Interface):
             color = Color(
                 title=u"Color",
                 description=u"",
                 required=False,
                 default="#ff0000"
             )
-            alphacolor = ColorAlpha(
-                title=u"Color with alpha layer support",
-                description=u"",
-                required=False,
-                default=u"rgba(104,191,144,0.55)"
-            )
 
 
         class ColorForm(form.Form):
             fields = field.Fields(IColorForm)
             ...
 
 for more information see demo directory in the package sources.
-
-
-
-.. _documentation: http://plone.org/documentation/kb/installing-add-ons-quick-how-to
-.. _bootstrap-colopicker: http://mjolnic.com/bootstrap-colorpicker/
```

### Comparing `collective.z3cform.colorpicker-2.1.0/CHANGES.rst` & `collective.z3cform.colorpicker-3.0.0/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 Changelog
 =========
 
+3.0.0 (2023-07-24)
+------------------
+
+- Move to native input color field, which is supported by all moderns browsers
+  [MrTango]
+
+- Plone compatibility
+  [MrTango]
+
+
 2.1.0 (2021-09-17)
 ------------------
 
 - Python 3 support.  [espen]
 
 
 2.0 (2017-12-21)
```

### Comparing `collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/demo/browser.py` & `collective.z3cform.colorpicker-3.0.0/src/collective/z3cform/colorpicker/demo/browser.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,30 @@
 from plone.z3cform.layout import wrap_form
 from z3c.form import form, field, button
 from zope.interface import Interface
 from collective.z3cform.colorpicker import Color
-from collective.z3cform.colorpicker import ColorAlpha
 
 
 class IColorForm(Interface):
     color = Color(
         title=u"Color",
         description=u"",
         required=False,
         default=u"#6298c9")
 
-    alphacolor = ColorAlpha(
-        title=u"Color with alpha layer support",
-        description=u"",
-        required=False,
-        default=u"rgba(104,191,144,0.55)")
-
 
 class ColorDemoForm(form.Form):
     """Example color picker form"""
 
     fields = field.Fields(IColorForm)
     ignoreContext = True
 
     label = u"Colopicker Demo"
     description = (
-        u"Color picker widget based on "
-        u"http://mjolnic.com/bootstrap-colorpicker/"
+        u"Color picker widget using native color input support."
     )
 
     def __init__(self, context, request):
         super(ColorDemoForm, self).__init__(context, request)
         self.request.set('disable_border', True)
 
     @button.buttonAndHandler(u'Save')
```

### Comparing `collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/configure.zcml` & `collective.z3cform.colorpicker-3.0.0/src/collective/z3cform/colorpicker/configure.zcml`

 * *Files 18% similar despite different names*

```diff
@@ -3,56 +3,25 @@
     xmlns:z3c="http://namespaces.zope.org/z3c"
     xmlns:browser="http://namespaces.zope.org/browser"
     xmlns:i18n="http://namespaces.zope.org/i18n"
     xmlns:plone="http://namespaces.plone.org/plone"
     xmlns:genericsetup="http://namespaces.zope.org/genericsetup"
     i18n_domain="collective.z3cform.colorpicker">
 
-    <includeDependencies package="." />
+    <include package="plone.app.z3cform" />
     <i18n:registerTranslations directory="locales" />
 
     <genericsetup:registerProfile
       name="default"
       title="Collective colorpicker"
       directory="profiles/default"
       description="Installs the collective.z3cform.colorpicker package"
       provides="Products.GenericSetup.interfaces.EXTENSION"
       />
 
-    <plone:static
-        directory="static"
-        type="plone"
-        name="colorpicker.static"
-        />
-
-    <class class=".colorpickeralpha.ColorpickerAlphaWidget">
-      <require
-          permission="zope.Public"
-          interface="collective.z3cform.colorpicker.colorpickeralpha.IColorpickerAlphaWidget" />
-    </class>
-
-    <z3c:widgetTemplate
-        mode="display"
-        widget="collective.z3cform.colorpicker.colorpickeralpha.IColorpickerAlphaWidget"
-        layer="z3c.form.interfaces.IFormLayer"
-        template="colorpickeralpha_display.pt" />
-
-    <z3c:widgetTemplate
-        mode="input"
-        widget="collective.z3cform.colorpicker.colorpickeralpha.IColorpickerAlphaWidget"
-        layer="z3c.form.interfaces.IFormLayer"
-        template="colorpickeralpha_input.pt" />
-
-
-    <adapter
-        factory=".colorpickeralpha.ColorpickerAlphaFieldWidget"
-        for=".fields.IColorAlpha
-             z3c.form.interfaces.IFormLayer"
-        />
-
     <class class=".colorpicker.ColorpickerWidget">
       <require
           permission="zope.Public"
           interface="collective.z3cform.colorpicker.colorpicker.IColorpickerWidget" />
     </class>
 
     <z3c:widgetTemplate
```

### Comparing `collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/colorpickeralpha_input.pt` & `collective.z3cform.colorpicker-3.0.0/src/collective/z3cform/colorpicker/colorpicker_input.pt`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-<div class="input-group pat-colorpicker"
-     data-pat-colorpicker="format: rgba">
-  <input type="text" id="color" name="" class="" title="" lang="" disabled=""
+<div class="input-group">
+  <input type="color" name="" class="" title="" lang="" disabled=""
        readonly="" alt="" tabindex="" accesskey="" size="" maxlength=""
        tal:attributes="id string:${view/id};
                        name view/name;
                        class string:${view/klass} form-control;
                        style view/style;
                        title view/title;
                        lang view/lang;
@@ -26,9 +25,8 @@
                        onchange view/onchange;
                        readonly view/readonly;
                        alt view/alt;
                        accesskey view/accesskey;
                        onselect view/onselect;
                        size view/size;
                        maxlength view/maxlength" />
-  <span class="input-group-addon"><i></i></span>
 </div>
```

### Comparing `collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/locales/it/LC_MESSAGES/collective.z3cform.colorpicker.po` & `collective.z3cform.colorpicker-3.0.0/src/collective/z3cform/colorpicker/locales/it/LC_MESSAGES/collective.z3cform.colorpicker.po`

 * *Files identical despite different names*

### Comparing `collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/locales/rebuild.sh` & `collective.z3cform.colorpicker-3.0.0/src/collective/z3cform/colorpicker/locales/rebuild.sh`

 * *Files identical despite different names*

### Comparing `collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/locales/collective.z3cform.colorpicker.pot` & `collective.z3cform.colorpicker-3.0.0/src/collective/z3cform/colorpicker/locales/collective.z3cform.colorpicker.pot`

 * *Files identical despite different names*

### Comparing `collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/locales/nl/LC_MESSAGES/collective.z3cform.colorpicker.po` & `collective.z3cform.colorpicker-3.0.0/src/collective/z3cform/colorpicker/locales/nl/LC_MESSAGES/collective.z3cform.colorpicker.po`

 * *Files identical despite different names*

### Comparing `collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/locales/es/LC_MESSAGES/collective.z3cform.colorpicker.po` & `collective.z3cform.colorpicker-3.0.0/src/collective/z3cform/colorpicker/locales/es/LC_MESSAGES/collective.z3cform.colorpicker.po`

 * *Files identical despite different names*

### Comparing `collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/colorpicker.py` & `collective.z3cform.colorpicker-3.0.0/src/collective/z3cform/colorpicker/colorpicker.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 class IColorpickerWidget(IWidget):
     """Colorpicker widget."""
 
 @implementer_only(IColorpickerWidget)
 class ColorpickerWidget(TextWidget):
     maxlength = 7
     size = 8
-    klass = u'pat-colorpicker'
 
 
 @adapter(IField, IFormLayer)
 @implementer(IFieldWidget)
 def ColorpickerFieldWidget(field, request):
     """IFieldWidget factory for ColorpickerWidget."""
     return FieldWidget(field, ColorpickerWidget(request))
```

### Comparing `collective.z3cform.colorpicker-2.1.0/src/collective/z3cform/colorpicker/colorpickeralpha_display.pt` & `collective.z3cform.colorpicker-3.0.0/src/collective/z3cform/colorpicker/colorpicker_display.pt`

 * *Files identical despite different names*

