# Comparing `tmp/treepoem-3.8.0.tar.gz` & `tmp/treepoem-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/chainz/Documents/Projects/treepoem/dist/tmp4rwh07a0/treepoem-3.8.0.tar", last modified: Wed Dec 30 12:28:43 2020, max compression
+gzip compressed data, was "treepoem-3.9.0.tar", last modified: Mon Mar 22 11:03:32 2021, max compression
```

## Comparing `treepoem-3.8.0.tar` & `treepoem-3.9.0.tar`

### file list

```diff
@@ -1,61 +1,28 @@
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2020-12-30 12:28:43.560426 treepoem-3.8.0/
--rw-r--r--   0 chainz     (501) staff       (20)     6097 2020-12-30 12:28:33.000000 treepoem-3.8.0/HISTORY.rst
--rw-r--r--   0 chainz     (501) staff       (20)     1067 2020-09-21 19:14:48.000000 treepoem-3.8.0/LICENSE
--rw-r--r--   0 chainz     (501) staff       (20)      299 2020-07-22 14:59:39.000000 treepoem-3.8.0/MANIFEST.in
--rw-r--r--   0 chainz     (501) staff       (20)     8118 2020-12-30 12:28:43.560826 treepoem-3.8.0/PKG-INFO
--rw-r--r--   0 chainz     (501) staff       (20)     5580 2020-12-30 12:28:21.000000 treepoem-3.8.0/README.rst
--rw-r--r--   0 chainz     (501) staff       (20)      172 2020-12-04 19:49:33.000000 treepoem-3.8.0/pyproject.toml
--rw-r--r--   0 chainz     (501) staff       (20)     1416 2020-12-30 12:28:43.565643 treepoem-3.8.0/setup.cfg
--rw-r--r--   0 chainz     (501) staff       (20)       38 2020-07-11 12:16:52.000000 treepoem-3.8.0/setup.py
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2020-12-30 12:28:43.496391 treepoem-3.8.0/src/
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2020-12-30 12:28:43.506262 treepoem-3.8.0/src/treepoem/
--rw-r--r--   0 chainz     (501) staff       (20)     3871 2020-06-20 17:50:18.000000 treepoem-3.8.0/src/treepoem/__init__.py
--rw-r--r--   0 chainz     (501) staff       (20)     1948 2020-06-20 17:50:18.000000 treepoem-3.8.0/src/treepoem/__main__.py
--rw-r--r--   0 chainz     (501) staff       (20)     7682 2020-12-30 12:22:33.000000 treepoem-3.8.0/src/treepoem/data.py
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2020-12-30 12:28:43.513852 treepoem-3.8.0/src/treepoem/postscriptbarcode/
--rw-r--r--   0 chainz     (501) staff       (20)    41980 2020-12-30 12:22:33.000000 treepoem-3.8.0/src/treepoem/postscriptbarcode/CHANGES
--rw-r--r--   0 chainz     (501) staff       (20)     1074 2020-12-28 02:51:02.000000 treepoem-3.8.0/src/treepoem/postscriptbarcode/LICENSE
--rw-r--r--   0 chainz     (501) staff       (20)     2119 2020-12-30 12:18:11.000000 treepoem-3.8.0/src/treepoem/postscriptbarcode/README
--rw-r--r--   0 chainz     (501) staff       (20)  1020524 2020-12-30 12:22:33.000000 treepoem-3.8.0/src/treepoem/postscriptbarcode/barcode.ps
--rw-r--r--   0 chainz     (501) staff       (20)  1025204 2020-12-30 12:22:33.000000 treepoem-3.8.0/src/treepoem/postscriptbarcode/barcode_with_sample.ps
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2020-12-30 12:28:43.508911 treepoem-3.8.0/src/treepoem.egg-info/
--rw-r--r--   0 chainz     (501) staff       (20)     8118 2020-12-30 12:28:43.000000 treepoem-3.8.0/src/treepoem.egg-info/PKG-INFO
--rw-r--r--   0 chainz     (501) staff       (20)     1966 2020-12-30 12:28:43.000000 treepoem-3.8.0/src/treepoem.egg-info/SOURCES.txt
--rw-r--r--   0 chainz     (501) staff       (20)        1 2020-12-30 12:28:43.000000 treepoem-3.8.0/src/treepoem.egg-info/dependency_links.txt
--rw-r--r--   0 chainz     (501) staff       (20)       53 2020-12-30 12:28:43.000000 treepoem-3.8.0/src/treepoem.egg-info/entry_points.txt
--rw-r--r--   0 chainz     (501) staff       (20)        1 2020-12-30 12:28:43.000000 treepoem-3.8.0/src/treepoem.egg-info/not-zip-safe
--rw-r--r--   0 chainz     (501) staff       (20)        7 2020-12-30 12:28:43.000000 treepoem-3.8.0/src/treepoem.egg-info/requires.txt
--rw-r--r--   0 chainz     (501) staff       (20)        9 2020-12-30 12:28:43.000000 treepoem-3.8.0/src/treepoem.egg-info/top_level.txt
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2020-12-30 12:28:43.520082 treepoem-3.8.0/tests/
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2020-12-30 12:28:43.553349 treepoem-3.8.0/tests/__pycache__/
--rw-------   0 chainz     (501) staff       (20)     1085 2019-03-18 13:59:31.000000 treepoem-3.8.0/tests/__pycache__/conftest.cpython-27-PYTEST.pyc
--rw-------   0 chainz     (501) staff       (20)      785 2019-05-13 19:19:28.000000 treepoem-3.8.0/tests/__pycache__/conftest.cpython-35-PYTEST.pyc
--rw-------   0 chainz     (501) staff       (20)      727 2019-05-13 19:19:42.000000 treepoem-3.8.0/tests/__pycache__/conftest.cpython-36-PYTEST.pyc
--rw-------   0 chainz     (501) staff       (20)      731 2019-06-19 10:20:03.000000 treepoem-3.8.0/tests/__pycache__/conftest.cpython-37-PYTEST.pyc
--rw-------   0 chainz     (501) staff       (20)      731 2019-10-21 09:19:49.000000 treepoem-3.8.0/tests/__pycache__/conftest.cpython-37-pytest-5.2.1.pyc
--rw-------   0 chainz     (501) staff       (20)      743 2019-11-11 21:25:58.000000 treepoem-3.8.0/tests/__pycache__/conftest.cpython-38-pytest-5.2.2.pyc
--rw-r--r--   0 chainz     (501) staff       (20)      743 2020-07-27 09:42:53.000000 treepoem-3.8.0/tests/__pycache__/conftest.cpython-38-pytest-5.4.3.pyc
--rw-------   0 chainz     (501) staff       (20)    12993 2019-03-18 13:59:31.000000 treepoem-3.8.0/tests/__pycache__/test_main.cpython-27-PYTEST.pyc
--rw-------   0 chainz     (501) staff       (20)    11020 2019-05-13 19:19:28.000000 treepoem-3.8.0/tests/__pycache__/test_main.cpython-35-PYTEST.pyc
--rw-------   0 chainz     (501) staff       (20)     9564 2019-05-13 19:19:42.000000 treepoem-3.8.0/tests/__pycache__/test_main.cpython-36-PYTEST.pyc
--rw-------   0 chainz     (501) staff       (20)     9485 2019-06-19 10:20:03.000000 treepoem-3.8.0/tests/__pycache__/test_main.cpython-37-PYTEST.pyc
--rw-------   0 chainz     (501) staff       (20)     9485 2019-10-21 09:22:27.000000 treepoem-3.8.0/tests/__pycache__/test_main.cpython-37-pytest-5.2.1.pyc
--rw-------   0 chainz     (501) staff       (20)     8085 2019-11-11 21:25:58.000000 treepoem-3.8.0/tests/__pycache__/test_main.cpython-38-pytest-5.2.2.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     6486 2020-07-27 09:42:54.000000 treepoem-3.8.0/tests/__pycache__/test_main.cpython-38-pytest-5.4.3.pyc
--rw-------   0 chainz     (501) staff       (20)     9529 2019-03-18 13:59:31.000000 treepoem-3.8.0/tests/__pycache__/test_treepoem.cpython-27-PYTEST.pyc
--rw-------   0 chainz     (501) staff       (20)     7546 2019-05-13 19:19:28.000000 treepoem-3.8.0/tests/__pycache__/test_treepoem.cpython-35-PYTEST.pyc
--rw-------   0 chainz     (501) staff       (20)     6723 2019-05-13 19:19:42.000000 treepoem-3.8.0/tests/__pycache__/test_treepoem.cpython-36-PYTEST.pyc
--rw-------   0 chainz     (501) staff       (20)     6555 2019-06-19 10:20:03.000000 treepoem-3.8.0/tests/__pycache__/test_treepoem.cpython-37-PYTEST.pyc
--rw-------   0 chainz     (501) staff       (20)     6555 2019-10-21 09:22:27.000000 treepoem-3.8.0/tests/__pycache__/test_treepoem.cpython-37-pytest-5.2.1.pyc
--rw-------   0 chainz     (501) staff       (20)     5975 2019-11-11 21:25:58.000000 treepoem-3.8.0/tests/__pycache__/test_treepoem.cpython-38-pytest-5.2.2.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     5012 2020-07-27 09:42:54.000000 treepoem-3.8.0/tests/__pycache__/test_treepoem.cpython-38-pytest-5.4.3.pyc
--rw-r--r--   0 chainz     (501) staff       (20)      445 2020-06-20 17:50:18.000000 treepoem-3.8.0/tests/conftest.py
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2020-12-30 12:28:43.559867 treepoem-3.8.0/tests/fixtures/
--rw-r--r--   0 chainz     (501) staff       (20)      434 2020-06-20 17:50:18.000000 treepoem-3.8.0/tests/fixtures/azteccode.png
--rw-r--r--   0 chainz     (501) staff       (20)      757 2020-06-20 17:50:18.000000 treepoem-3.8.0/tests/fixtures/code128.png
--rw-r--r--   0 chainz     (501) staff       (20)      853 2020-06-20 17:50:18.000000 treepoem-3.8.0/tests/fixtures/code39.png
--rw-r--r--   0 chainz     (501) staff       (20)      500 2020-06-20 17:50:18.000000 treepoem-3.8.0/tests/fixtures/interleaved2of5.png
--rw-r--r--   0 chainz     (501) staff       (20)      577 2020-06-20 17:50:18.000000 treepoem-3.8.0/tests/fixtures/pdf417.png
--rw-r--r--   0 chainz     (501) staff       (20)      637 2020-06-20 17:50:18.000000 treepoem-3.8.0/tests/fixtures/qrcode.png
--rw-r--r--   0 chainz     (501) staff       (20)     2512 2020-06-20 17:50:18.000000 treepoem-3.8.0/tests/test_main.py
--rw-r--r--   0 chainz     (501) staff       (20)     2503 2020-06-20 17:50:18.000000 treepoem-3.8.0/tests/test_treepoem.py
+drwxr-xr-x   0 chainz     (501) staff       (20)        0 2021-03-22 11:03:32.137558 treepoem-3.9.0/
+-rw-r--r--   0 chainz     (501) staff       (20)     6489 2021-03-22 11:03:24.000000 treepoem-3.9.0/HISTORY.rst
+-rw-r--r--   0 chainz     (501) staff       (20)     1067 2021-02-07 17:51:29.000000 treepoem-3.9.0/LICENSE
+-rw-r--r--   0 chainz     (501) staff       (20)      299 2021-03-19 11:45:23.000000 treepoem-3.9.0/MANIFEST.in
+-rw-r--r--   0 chainz     (501) staff       (20)     8114 2021-03-22 11:03:32.137808 treepoem-3.9.0/PKG-INFO
+-rw-r--r--   0 chainz     (501) staff       (20)     5578 2021-02-07 17:53:16.000000 treepoem-3.9.0/README.rst
+-rw-r--r--   0 chainz     (501) staff       (20)      172 2021-02-07 17:51:29.000000 treepoem-3.9.0/pyproject.toml
+-rw-r--r--   0 chainz     (501) staff       (20)     1414 2021-03-22 11:03:32.138604 treepoem-3.9.0/setup.cfg
+-rw-r--r--   0 chainz     (501) staff       (20)       38 2021-02-07 17:51:29.000000 treepoem-3.9.0/setup.py
+drwxr-xr-x   0 chainz     (501) staff       (20)        0 2021-03-22 11:03:32.125499 treepoem-3.9.0/src/
+drwxr-xr-x   0 chainz     (501) staff       (20)        0 2021-03-22 11:03:32.130393 treepoem-3.9.0/src/treepoem/
+-rw-r--r--   0 chainz     (501) staff       (20)     3871 2021-02-07 17:51:29.000000 treepoem-3.9.0/src/treepoem/__init__.py
+-rw-r--r--   0 chainz     (501) staff       (20)     1948 2021-02-07 17:51:29.000000 treepoem-3.9.0/src/treepoem/__main__.py
+-rw-r--r--   0 chainz     (501) staff       (20)     7682 2021-03-22 11:00:44.000000 treepoem-3.9.0/src/treepoem/data.py
+drwxr-xr-x   0 chainz     (501) staff       (20)        0 2021-03-22 11:03:32.135734 treepoem-3.9.0/src/treepoem/postscriptbarcode/
+-rw-r--r--   0 chainz     (501) staff       (20)    42238 2021-03-22 11:02:56.000000 treepoem-3.9.0/src/treepoem/postscriptbarcode/CHANGES
+-rw-r--r--   0 chainz     (501) staff       (20)     1074 2021-03-22 11:02:56.000000 treepoem-3.9.0/src/treepoem/postscriptbarcode/LICENSE
+-rw-r--r--   0 chainz     (501) staff       (20)     2119 2021-03-22 11:00:43.000000 treepoem-3.9.0/src/treepoem/postscriptbarcode/README
+-rw-r--r--   0 chainz     (501) staff       (20)  1042784 2021-03-22 11:02:56.000000 treepoem-3.9.0/src/treepoem/postscriptbarcode/barcode.ps
+-rw-r--r--   0 chainz     (501) staff       (20)  1047464 2021-03-22 11:02:56.000000 treepoem-3.9.0/src/treepoem/postscriptbarcode/barcode_with_sample.ps
+drwxr-xr-x   0 chainz     (501) staff       (20)        0 2021-03-22 11:03:32.132732 treepoem-3.9.0/src/treepoem.egg-info/
+-rw-r--r--   0 chainz     (501) staff       (20)     8114 2021-03-22 11:03:32.000000 treepoem-3.9.0/src/treepoem.egg-info/PKG-INFO
+-rw-r--r--   0 chainz     (501) staff       (20)      612 2021-03-22 11:03:32.000000 treepoem-3.9.0/src/treepoem.egg-info/SOURCES.txt
+-rw-r--r--   0 chainz     (501) staff       (20)        1 2021-03-22 11:03:32.000000 treepoem-3.9.0/src/treepoem.egg-info/dependency_links.txt
+-rw-r--r--   0 chainz     (501) staff       (20)       53 2021-03-22 11:03:32.000000 treepoem-3.9.0/src/treepoem.egg-info/entry_points.txt
+-rw-r--r--   0 chainz     (501) staff       (20)        1 2021-03-22 11:03:31.000000 treepoem-3.9.0/src/treepoem.egg-info/not-zip-safe
+-rw-r--r--   0 chainz     (501) staff       (20)        7 2021-03-22 11:03:32.000000 treepoem-3.9.0/src/treepoem.egg-info/requires.txt
+-rw-r--r--   0 chainz     (501) staff       (20)        9 2021-03-22 11:03:32.000000 treepoem-3.9.0/src/treepoem.egg-info/top_level.txt
```

### Comparing `treepoem-3.8.0/HISTORY.rst` & `treepoem-3.9.0/HISTORY.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,68 +1,79 @@
 =======
 History
 =======
 
+3.9.0 (2021-03-22)
+------------------
+
+* Upgrade vendored BWIPP to its 2021-02-06 release. You can read its changelog
+  in the `treepoem repo
+  <https://github.com/adamchainz/treepoem/blob/main/src/treepoem/postscriptbarcode/CHANGES>`__.
+
+* Stop distributing tests to reduce package size. Tests are not intended to be
+  run outside of the tox setup in the repository. Repackagers can use GitHub's
+  tarballs per tag.
+
 3.8.0 (2020-12-30)
 ------------------
 
 * Upgrade vendored BWIPP to its 2020-12-28 release. You can read its changelog
   in the `treepoem repo
-  <https://github.com/adamchainz/treepoem/blob/master/src/treepoem/postscriptbarcode/CHANGES>`__.
+  <https://github.com/adamchainz/treepoem/blob/main/src/treepoem/postscriptbarcode/CHANGES>`__.
 
 3.7.0 (2020-12-13)
 ------------------
 
 * Drop Python 3.5 support.
 * Support Python 3.9.
 
 3.6.0 (2020-10-11)
 ------------------
 
 * Upgrade BWIPP from 2020-09-13 to 2020-10-11. This has a few bug fixes and
   performance improvements. You can read its changelog in the vendored copy in
   the `treepoem repo
-  <https://github.com/adamchainz/treepoem/blob/master/src/treepoem/postscriptbarcode/CHANGES>`__.
+  <https://github.com/adamchainz/treepoem/blob/main/src/treepoem/postscriptbarcode/CHANGES>`__.
 
 3.5.0 (2020-09-21)
 ------------------
 
 * Upgrade BWIPP from 2020-04-01 to 2020-09-13. This has a few bug fixes and
   performance improvements. You can read its changelog in the vendored copy in
   the `treepoem repo
-  <https://github.com/adamchainz/treepoem/blob/master/src/treepoem/postscriptbarcode/CHANGES>`__.
+  <https://github.com/adamchainz/treepoem/blob/main/src/treepoem/postscriptbarcode/CHANGES>`__.
 
 3.4.0 (2020-06-21)
 ------------------
 
 * Upgrade BWIPP from 2019-11-08 to 2020-04-01. This has a few bug fixes and
   performance improvements. You can read its changelog in the vendored copy in
   the `treepoem repo
-  <https://github.com/adamchainz/treepoem/blob/master/src/treepoem/postscriptbarcode/CHANGES>`__.
+  <https://github.com/adamchainz/treepoem/blob/main/src/treepoem/postscriptbarcode/CHANGES>`__.
 
 3.3.1 (2020-02-04)
 ------------------
 
 * Update allowed barcode list to add missing types from new versions of BWIPP.
 
 3.3.0 (2019-12-21)
 ------------------
 
 * Upgrade BWIPP from 2019-08-05 to 2019-11-08. This has a few bug fixes and
   performance improvements. You can read its changelog in the vendored copy in
   the `treepoem repo
-  <https://github.com/adamchainz/treepoem/blob/master/src/treepoem/postscriptbarcode/CHANGES>`__.
+  <https://github.com/adamchainz/treepoem/blob/main/src/treepoem/postscriptbarcode/CHANGES>`__.
 
 3.2.0 (2019-12-19)
 ------------------
 
 * Upgrade BWIPP from 2019-04-24 to 2019-08-05. This has a few bug fixes and
   performance improvements. You can read its changelog in the vendored copy in
   the `treepoem repo
-  <https://github.com/adamchainz/treepoem/blob/master/treepoem/postscriptbarcode/CHANGES>`__.
+  <https://github.com/adamchainz/treepoem/blob/main/treepoem/postscriptbarcode/CHANGES>`__.
 * Converted setuptools metadata to configuration file. This meant removing the
   ``__version__`` attribute from the package. If you want to inspect the
   installed version, use
   ``importlib.metadata.version("treepoem")``
   (`docs <https://docs.python.org/3.8/library/importlib.metadata.html#distribution-versions>`__ /
   `backport <https://pypi.org/project/importlib-metadata/>`__).
 * Update Python support to 3.5-3.8.
@@ -70,24 +81,24 @@
 3.1.0 (2019-06-25)
 ------------------
 
 * Update Python support to 3.5-3.7, as 3.4 has reached its end of life.
 * Upgrade BWIPP from 2017-07-27 to 2019-04-24. This has a few bug fixes and
   performance improvements. You can read its changelog in the vendored copy in
   the `treepoem repo
-  <https://github.com/adamchainz/treepoem/blob/master/treepoem/postscriptbarcode/CHANGES>`__.
+  <https://github.com/adamchainz/treepoem/blob/main/treepoem/postscriptbarcode/CHANGES>`__.
 
 3.0.0 (2019-05-08)
 ------------------
 
 * Drop Python 2 support, only Python 3.4+ is supported now.
 * Upgrade BWIPP from 2017-05-20 to 2018-07-27. This has a few bug fixes and
   performance improvements. You can read its changelog in the vendored copy in
   the `treepoem repo
-  <https://github.com/adamchainz/treepoem/blob/master/treepoem/postscriptbarcode/CHANGES>`__.
+  <https://github.com/adamchainz/treepoem/blob/main/treepoem/postscriptbarcode/CHANGES>`__.
 
 2.0.0 (2018-08-04)
 ------------------
 
 * Support binary barcode data - if ``bytes`` (``str`` on Python 2) is passed
   as data, it's not encoded. This has introduced a dependency on ``six``. This
   may be backwards incompatible, depending on what type of data you're passing
@@ -95,54 +106,54 @@
 * Make ``treepoem.barcode_types`` a ``dict`` mapping the BWIPP encoder
   names to a custom type containing a human-readable ``description``. This is
   backwards incompatible if you're relying on ``barcode_types`` which
   previously was a ``set`` of the encoder names.
 * Upgrade BWIPP from 2017-10-19 to 2018-05-20. This has a few bug fixes and
   performance improvements. You can read its changelog in the vendored copy in
   the `treepoem repo
-  <https://github.com/adamchainz/treepoem/blob/master/treepoem/postscriptbarcode/CHANGES>`__.
+  <https://github.com/adamchainz/treepoem/blob/main/treepoem/postscriptbarcode/CHANGES>`__.
 
 1.4.1 (2018-05-01)
 ------------------
 
 * Fix formatting bug in CLI output.
 
 1.4.0 (2018-05-01)
 ------------------
 
 * Make the ``options`` argument to ``generate_barcode`` optional.
 * Add a CLI ``treepoem``.
 * Upgrade BWIPP from 2017-07-10 to 2017-10-19. This has a few bug fixes and
   performance improvements. You can read its changelog in the vendored copy in
   the `treepoem repo
-  <https://github.com/adamchainz/treepoem/blob/master/treepoem/postscriptbarcode/CHANGES>`__.
+  <https://github.com/adamchainz/treepoem/blob/main/treepoem/postscriptbarcode/CHANGES>`__.
 
 1.3.2 (2017-10-22)
 ------------------
 
 * Upgrade BWIPP from 2017-07-10 to 2017-10-19. This has a few bug fixes. You
   can read its changelog in the vendored copy in the `treepoem repo
-  <https://github.com/adamchainz/treepoem/blob/master/treepoem/postscriptbarcode/CHANGES>`__.
+  <https://github.com/adamchainz/treepoem/blob/main/treepoem/postscriptbarcode/CHANGES>`__.
 
 1.3.1 (2017-08-24)
 ------------------
 
 * Upgrade BWIPP from 2017-06-20 to 2017-07-10. This has a few bug fixes. You
   can read its changelog in the vendored copy in the `treepoem repo
-  <https://github.com/adamchainz/treepoem/blob/master/treepoem/postscriptbarcode/CHANGES>`__.
+  <https://github.com/adamchainz/treepoem/blob/main/treepoem/postscriptbarcode/CHANGES>`__.
 
 1.3.0 (2017-06-21)
 ------------------
 
 * Upgrade BWIPP from 2015-11-24 to 2017-06-20. This has a number of bug fixes,
   and supports more barcode types. It has also changed the pixel-for-pixel
   output of some formats, although they still encode the same information -
   notably QR codes, which are tested in ``treepoem``\'s test suite. You can
   read its changelog in the `vendored copy in the treepoem repo
-  <https://github.com/adamchainz/treepoem/blob/master/treepoem/postscriptbarcode/CHANGES>`__.
+  <https://github.com/adamchainz/treepoem/blob/main/treepoem/postscriptbarcode/CHANGES>`__.
 
 1.2.0 (2017-06-21)
 ------------------
 
 * Add ``treepoem.barcode_types``, a set of all the names of supported barcode
   types, and error if asked to generate a barcode of an unknown type.
```

### Comparing `treepoem-3.8.0/LICENSE` & `treepoem-3.9.0/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2016-2020 YPlan
+Copyright (c) 2016-2021 YPlan
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `treepoem-3.8.0/PKG-INFO` & `treepoem-3.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: treepoem
-Version: 3.8.0
+Version: 3.9.0
 Summary: Barcode rendering for Python supporting QRcode, Aztec, PDF417, I25, Code128, Code39 and many more types.
 Home-page: https://github.com/adamchainz/treepoem
 Author: Christian Muirhead
 Author-email: xtian@babbageclunk.com
 Maintainer: Adam Johnson
 Maintainer-email: me@adamj.eu
 License: MIT
-Project-URL: Changelog, https://github.com/adamchainz/treepoem/blob/master/HISTORY.rst
+Project-URL: Changelog, https://github.com/adamchainz/treepoem/blob/main/HISTORY.rst
 Project-URL: Twitter, https://twitter.com/adamchainz
 Description: ========
         Treepoem
         ========
         
-        .. image:: https://img.shields.io/github/workflow/status/adamchainz/treepoem/CI/master?style=for-the-badge
+        .. image:: https://img.shields.io/github/workflow/status/adamchainz/treepoem/CI/main?style=for-the-badge
            :target: https://github.com/adamchainz/treepoem/actions?workflow=CI
         
         .. image:: https://img.shields.io/pypi/v/treepoem.svg?style=for-the-badge
            :target: https://pypi.org/project/treepoem/
         
         .. image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge
            :target: https://github.com/psf/black
```

### Comparing `treepoem-3.8.0/README.rst` & `treepoem-3.9.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ========
 Treepoem
 ========
 
-.. image:: https://img.shields.io/github/workflow/status/adamchainz/treepoem/CI/master?style=for-the-badge
+.. image:: https://img.shields.io/github/workflow/status/adamchainz/treepoem/CI/main?style=for-the-badge
    :target: https://github.com/adamchainz/treepoem/actions?workflow=CI
 
 .. image:: https://img.shields.io/pypi/v/treepoem.svg?style=for-the-badge
    :target: https://pypi.org/project/treepoem/
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge
    :target: https://github.com/psf/black
```

### Comparing `treepoem-3.8.0/setup.cfg` & `treepoem-3.9.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [metadata]
 name = treepoem
-version = 3.8.0
+version = 3.9.0
 description = Barcode rendering for Python supporting QRcode, Aztec, PDF417, I25, Code128, Code39 and many more types.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Christian Muirhead
 author_email = xtian@babbageclunk.com
 maintainer = Adam Johnson
 maintainer_email = me@adamj.eu
 url = https://github.com/adamchainz/treepoem
 project_urls = 
-	Changelog = https://github.com/adamchainz/treepoem/blob/master/HISTORY.rst
+	Changelog = https://github.com/adamchainz/treepoem/blob/main/HISTORY.rst
 	Twitter = https://twitter.com/adamchainz
 license = MIT
 keywords = barcode bwipp postscript ghostscript qr qrcode aztec azteccode pdf417 interleaved2of5 i25 code128 code39
 classifiers = 
 	Development Status :: 3 - Alpha
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
```

### Comparing `treepoem-3.8.0/src/treepoem/__init__.py` & `treepoem-3.9.0/src/treepoem/__init__.py`

 * *Files identical despite different names*

### Comparing `treepoem-3.8.0/src/treepoem/__main__.py` & `treepoem-3.9.0/src/treepoem/__main__.py`

 * *Files identical despite different names*

### Comparing `treepoem-3.8.0/src/treepoem/data.py` & `treepoem-3.9.0/src/treepoem/data.py`

 * *Files identical despite different names*

### Comparing `treepoem-3.8.0/src/treepoem/postscriptbarcode/CHANGES` & `treepoem-3.9.0/src/treepoem/postscriptbarcode/CHANGES`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+2021-02-06
+
+* Linting of GS1 AI (4308) was fixed.
+* Linting of the check character pair for AI (8013) was added.
+
+
+2021-01-15
+
+* Linting for GS1 coupon AIs (8110) and (8112) was added.
+
+
+2021-01-05
+
+* Linting for GS1 AI syntax data was expanded and fixed.
+
+
 2020-12-28
 
 * A convenience encoder for GS1 DotCode was added.
 
 
 2020-12-26
```

### Comparing `treepoem-3.8.0/src/treepoem/postscriptbarcode/LICENSE` & `treepoem-3.9.0/src/treepoem/postscriptbarcode/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2004-2019 Terry Burton
+Copyright (c) 2004-2021 Terry Burton
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `treepoem-3.8.0/src/treepoem/postscriptbarcode/README` & `treepoem-3.9.0/src/treepoem/postscriptbarcode/README`

 * *Files identical despite different names*

### Comparing `treepoem-3.8.0/src/treepoem/postscriptbarcode/barcode.ps` & `treepoem-3.9.0/src/treepoem/postscriptbarcode/barcode.ps`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 %!PS
 
-% Barcode Writer in Pure PostScript - Version 2020-12-28
+% Barcode Writer in Pure PostScript - Version 2021-02-06
 % https://bwipp.terryburton.co.uk
 %
-% Copyright (c) 2004-2019 Terry Burton
+% Copyright (c) 2004-2021 Terry Burton
 %
 % Permission is hereby granted, free of charge, to any
 % person obtaining a copy of this software and associated
 % documentation files (the "Software"), to deal in the
 % Software without restriction, including without
 % limitation the rights to use, copy, modify, merge,
 % publish, distribute, sublicense, and/or sell copies of
@@ -28,29 +28,29 @@
 % CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 % CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
 % IN THE SOFTWARE.
 
 % --BEGIN TEMPLATE--
 
 % --BEGIN RESOURCE preamble--
-%%BeginResource: Category uk.co.terryburton.bwipp 0.0 2020122800 29629 32838
+%%BeginResource: Category uk.co.terryburton.bwipp 0.0 2021020600 29629 32838
 %%BeginData:          6 ASCII Lines
 currentglobal
 true setglobal
 /Generic /Category findresource dup length 1 add dict copy dup
 /InstanceType /setpacking where {pop /packedarraytype} {/arraytype} ifelse put
 /uk.co.terryburton.bwipp exch /Category defineresource pop
 setglobal
 %%EndData
 %%EndResource
 % --END RESOURCE preamble--
 
 % --BEGIN RESOURCE raiseerror--
 % --REQUIRES preamble--
-%%BeginResource: uk.co.terryburton.bwipp raiseerror 0.0 2020122800 39041 38872
+%%BeginResource: uk.co.terryburton.bwipp raiseerror 0.0 2021020600 39041 38872
 %%BeginData:         15 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 begin
 /raiseerror {
   $error exch /errorinfo exch put
   $error exch /errorname exch put
@@ -65,15 +65,15 @@
 /setpacking where {pop setpacking} if
 %%EndData
 %%EndResource
 % --END RESOURCE raiseerror--
 
 % --BEGIN RESOURCE parseinput--
 % --REQUIRES preamble raiseerror--
-%%BeginResource: uk.co.terryburton.bwipp parseinput 0.0 2020122800 58305 58180
+%%BeginResource: uk.co.terryburton.bwipp parseinput 0.0 2021020600 58305 58204
 %%BeginData:        129 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 4 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 begin
 /parseinput {
 
@@ -202,16 +202,16 @@
 /setpacking where {pop setpacking} if
 %%EndData
 %%EndResource
 % --END RESOURCE parseinput--
 
 % --BEGIN RESOURCE gs1lint--
 % --REQUIRES preamble raiseerror--
-%%BeginResource: uk.co.terryburton.bwipp gs1lint 0.0 2020122800 247873 257453
-%%BeginData:       1235 ASCII Lines
+%%BeginResource: uk.co.terryburton.bwipp gs1lint 0.0 2021020600 360967 368615
+%%BeginData:       1674 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 2 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 begin
 /gs1lint {
 
     20 dict begin
@@ -264,28 +264,169 @@
         mark exch
         dup length 2 mod 0 eq {3} {1} ifelse
         exch { 48 sub 1 index mul exch 4 exch sub } forall pop
         0 counttomark 1 sub {add} repeat exch pop
         10 mod 0 ne { pop /bwipp.GS1badChecksum (Bad checksum) false exit } if
     } bind def
 
+    /cset82 <<
+        0 (!"%&'\(\)*+,-./0123456789:;<=>?ABCDEFGHIJKLMNOPQRSTUVWXYZ_abcdefghijklmnopqrstuvwxyz)
+        { exch dup 1 add } forall pop
+    >> def
+
+    /cset32 <<
+        0 (23456789ABCDEFGHJKLMNPQRSTUVWXYZ)
+        { exch dup 1 add } forall pop
+    >> def
+
+    /lintcsumalpha {
+        dup length 2 lt { pop pop /bwipp.GS1alphaTooShort (Alphanumeric string is too short to check) false exit} if
+        dup length 2 sub
+        2 copy
+        0 exch getinterval mark exch {
+            dup cset82 exch known { cset82 exch get } { -1 exit } ifelse
+        } forall
+        dup -1 eq { cleartomark pop pop pop /bwipp.GS1UnknownCSET82Character (Unknown CSET 82 character) false exit} if
+        counttomark array astore exch pop
+        3 1 roll
+        2 getinterval mark exch {
+            dup cset32 exch known { cset32 exch get } { -1 exit } ifelse
+        } forall
+        dup -1 eq { cleartomark pop pop /bwipp.GS1UnknownCSET32Character (Unknown CSET 32 character) false exit} if
+        counttomark array astore exch pop
+        dup 0 get 5 bitshift exch 1 get add exch
+        [ 2 3 5 7 11 13 17 19 23 29 31 37 41 43 47 53 59 61 67 71 73 79 83 ]
+        1 index length
+        dup 2 index length gt { pop pop pop pop pop /bwipp.GS1alphaTooLong (Alphanumeric string is too long to check) false exit} if
+        0 exch getinterval {exch} forall
+        0 exch { 3 -1 roll exch mul add } forall 1021 mod
+        ne { pop /bwipp.GS1badAlphaCheckCharacters (Bad alphanumeric check characters) false exit} if
+    } bind def
+
+    /iso3166 << [
+        /004 /008 /010 /012 /016 /020 /024 /028 /031 /032 /036 /040 /044 /048
+        /050 /051 /052 /056 /060 /064 /068 /070 /072 /074 /076 /084 /086 /090 /092 /096
+        /100 /104 /108 /112 /116 /120 /124 /132 /136 /140 /144 /148
+        /152 /156 /158 /162 /166 /170 /174 /175 /178 /180 /184 /188 /191 /192 /196
+        /203 /204 /208 /212 /214 /218 /222 /226 /231 /232 /233 /234 /238 /239 /242 /246 /248
+        /250 /254 /258 /260 /262 /266 /268 /270 /275 /276 /288 /292 /296
+        /300 /304 /308 /312 /316 /320 /324 /328 /332 /334 /336 /340 /344 /348
+        /352 /356 /360 /364 /368 /372 /376 /380 /384 /388 /392 /398
+        /400 /404 /408 /410 /414 /417 /418 /422 /426 /428 /430 /434 /438 /440 /442 /446
+        /450 /454 /458 /462 /466 /470 /474 /478 /480 /484 /492 /496 /498 /499
+        /500 /504 /508 /512 /516 /520 /524 /528 /531 /533 /534 /535 /540 /548
+        /554 /558 /562 /566 /570 /574 /578 /580 /581 /583 /584 /585 /586 /591 /598
+        /600 /604 /608 /612 /616 /620 /624 /626 /630 /634 /638 /642 /643 /646
+        /652 /654 /659 /660 /662 /663 /666 /670 /674 /678 /682 /686 /688 /690 /694
+        /702 /703 /704 /705 /706 /710 /716 /724 /728 /729 /732 /740 /744 /748
+        /752 /756 /760 /762 /764 /768 /772 /776 /780 /784 /788 /792 /795 /796 /798
+        /800 /804 /807 /818 /826 /831 /832 /833 /834 /840
+        /850 /854 /858 /860 /862 /876 /882 /887 /894
+    ] {dup} forall >> def
+
+    /lintiso3166 {
+        iso3166 exch known not { pop /bwipp.GS1UnknownCountry (Unknown country code) false exit } if
+    } bind def
+
+    /lintiso3166999 {
+        dup /999 ne {
+            iso3166 exch known not { pop /bwipp.GS1UnknownCountryOr999 (Unknown country code or not 999) false exit } if
+        } {
+            pop
+        } ifelse
+    } bind def
+
+    /lintiso3166list {
+        dup length 3 mod 0 ne {
+            pop pop /bwipp.GS1BadCountryListLength (Not a group of three-digit country codes) false exit
+        } if
+        true
+        0 3 3 index length 1 sub {
+            2 index exch 3 getinterval
+            iso3166 exch known not { pop pop false exit } if
+        } for
+        not { pop /bwipp.GS1UnknownCountry (Unknown country code) false exit } if
+        pop
+    } bind def
+
+    /iso3166alpha2 << [
+        /AD /AE /AF /AG /AI /AL /AM /AO /AQ /AR /AS /AT /AU /AW /AX /AZ
+        /BA /BB /BD /BE /BF /BG /BH /BI /BJ /BL /BM /BN /BO /BQ /BR /BS /BT /BV /BW /BY /BZ
+        /CA /CC /CD /CF /CG /CH /CI /CK /CL /CM /CN /CO /CR /CU /CV /CW /CX /CY /CZ
+        /DE /DJ /DK /DM /DO /DZ
+        /EC /EE /EG /EH /ER /ES /ET
+        /FI /FJ /FK /FM /FO /FR
+        /GA /GB /GD /GE /GF /GG /GH /GI /GL /GM /GN /GP /GQ /GR /GS /GT /GU /GW /GY
+        /HK /HM /HN /HR /HT /HU
+        /ID /IE /IL /IM /IN /IO /IQ /IR /IS /IT /JE /JM /JO /JP
+        /KE /KG /KH /KI /KM /KN /KP /KR /KW /KY /KZ
+        /LA /LB /LC /LI /LK /LR /LS /LT /LU /LV /LY
+        /MA /MC /MD /ME /MF /MG /MH /MK /ML /MM /MN /MO /MP /MQ /MR /MS /MT /MU /MV /MW /MX /MY /MZ
+        /NA /NC /NE /NF /NG /NI /NL /NO /NP /NR /NU /NZ
+        /OM
+        /PA /PE /PF /PG /PH /PK /PL /PM /PN /PR /PS /PT /PW /PY
+        /QA
+        /RE /RO /RS /RU /RW
+        /SA /SB /SC /SD /SE /SG /SH /SI /SJ /SK /SL /SM /SN /SO /SR /SS /ST /SV /SX /SY /SZ
+        /TC /TD /TF /TG /TH /TJ /TK /TL /TM /TN /TO /TR /TT /TV /TW /TZ
+        /UA /UG /UM /US /UY /UZ
+        /VA /VC /VE /VG /VI /VN /VU
+        /WF /WS
+        /YE /YT
+        /ZA /ZM /ZW
+    ] {dup} forall >> def
+
+    /lintiso3166alpha2 {
+        iso3166alpha2 exch known not { pop /bwipp.GS1UnknownCountryAlpha (Unknown country alpha code) false exit } if
+    } bind def
+
+    /iso4217 << [
+        /008 /012 /032 /036 /044 /048
+        /050 /051 /052 /060 /064 /068 /072 /084 /090 /096
+        /104 /108 /116 /124 /132 /136 /144
+        /152 /156 /170 /174 /188 /191 /192
+        /203 /208 /214 /222 /230 /232 /238 /242 /262 /270 /292
+        /320 /324 /328 /332 /340 /344 /348
+        /352 /356 /360 /364 /368 /376 /388 /392 /398
+        /400 /404 /408 /410 /414 /417 /418
+        /422 /426 /430 /434 /446
+        /454 /458 /462 /480 /484 /496 /498
+        /504 /512 /516 /524 /532 /533 /548
+        /554 /558 /566 /578 /586 /590 /598
+        /600 /604 /608 /634 /643 /646 /654 /682 /690 /694
+        /702 /704 /706 /710 /728 /748
+        /752 /756 /760 /764 /776 /780 /784 /788
+        /800 /807 /818 /826 /834 /840 /858 /860 /882 /886
+        /901 /927 /928 /929 /930 /931 /932 /933 /934 /936 /938
+        /940 /941 /943 /944 /946 /947 /948 /949
+        /950 /951 /952 /953 /955 /956 /957 /958 /959
+        /960 /961 /962 /963 /964 /965 /967 /968 /969
+        /970 /971 /972 /973 /975 /976 /977 /978 /979
+        /980 /981 /984 /985 /986 /990 /994 /997 /999
+    ] {dup} forall >> def
+
+    /lintiso4217 {
+        iso4217 exch known not { pop /bwipp.GS1UnknownCurrency (Unknown currency code) false exit } if
+    } bind def
+
     /lintiban {
         dup length 4 lt { pop pop /bwipp.GS1tooShort (IBAN too short) false exit } if
         dup true exch {
             1 string dup 0 4 -1 roll put
             (0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZ)
             exch search not { pop pop false exit } if
             pop pop pop
         } forall
         not { pop /bwipp.GS1badIBANcharacter (Invalid IBAN character) false exit } if
-        mark exch mark exch {} forall counttomark -4 roll counttomark array astore exch pop {
+        dup mark exch mark exch {} forall counttomark -4 roll counttomark array astore exch pop {
             48 sub dup 9 gt {7 sub dup 10 idiv exch 10 mod} if
         } forall counttomark array astore exch pop
         0 exch {exch 10 mul add 97 mod} forall
-        1 ne { pop /bwipp.GS1badIBANchecksum (IBAN checksum incorrect) false exit } if
+        1 ne { pop pop /bwipp.GS1badIBANchecksum (IBAN checksum incorrect) false exit } if
+        0 2 getinterval lintiso3166alpha2
     } bind def
 
     /lintzero {
         (0) ne { pop /bwipp.GS1zeroRequired (Zero is required) false exit } if
     } bind def
 
     /lintnonzero {
@@ -311,29 +452,32 @@
 
     /lintyymmdd {
         dup length 6 ne { pop /bwipp.GS1badDateLength (Invalid length for date) false exit } if
         dup 4 2 getinterval cvi 1 lt { pop /bwipp.GS1badDay (Invalid day of month) false exit } if
         lintyymmd0
     } bind def
 
+    /lintyymmddhh {
+        dup length 8 ne { pop /bwipp.GS1badYYMMDDHHLength (Invalid length for date with hour) false exit } if
+        dup 6 2 getinterval cvi 23 gt { pop pop /bwipp.GS1badHour (Invalid hour of day) false exit } if
+        0 6 getinterval lintyymmdd
+    } bind def
+
     /linthhmm {
         dup 0 2 getinterval cvi 23 gt { pop pop /bwipp.GS1badHour (Invalid hour of day) false exit } if
         2 2 getinterval cvi 59 gt { pop /bwipp.GS1badMinute (Invalid minute in the hour) false exit } if
     } bind def
 
-    /linthhoptmmss {
-        dup length dup 2 ne exch dup 4 ne exch 6 ne and and {
-            pop /bwipp.GS1badTimeLength (Invalid length for time of day with optional mins and secs) false exit
+    /lintmmoptss {
+        dup length dup 2 ne exch 4 ne and {
+            pop /bwipp.GS1badTimeLength (Invalid length for optional minutes and seconds) false exit
         } if
-        dup 0 2 getinterval cvi 23 gt { pop pop /bwipp.GS1badHour (Invalid hour of day) false exit } if
+        dup 0 2 getinterval cvi 59 gt { pop pop /bwipp.GS1badMinute (Invalid minute in the hour) false exit } if
         dup length 4 ge {
-            dup 2 2 getinterval cvi 59 gt { pop pop /bwipp.GS1badMinute (Invalid minute in the hour) false exit } if
-        } if
-        dup length 6 ge {
-            dup 4 2 getinterval cvi 59 gt { pop pop /bwipp.GS1badSecond (Invalid second in the minute) false exit } if
+            dup 2 2 getinterval cvi 59 gt { pop pop /bwipp.GS1badSecond (Invalid second in the minute) false exit } if
         } if
         pop
     } bind def
 
     /lintyesno {
         dup (0) ne exch (1) ne and {
             pop /bwipp.GS1badBoolean (Neither 0 nor 1 for yes or no) false exit
@@ -365,57 +509,352 @@
                 exch search not { pop pop false exit } if
                 pop pop pop
             } forall
             not { pop pop /bwipp.GS1badPercentChars (Invalid characters for percent encoding) false exit } if
         } loop
     } bind def
 
-    /lintcouponcode {  % TODO
-        pop
-    } bind def
+    /lintcouponcode {
+        dup true exch {
+            dup 48 lt exch 57 gt or { pop false exit } if
+        } forall
+        not { pop pop /bwipp.GS1couponNotNumeric (Coupon not numeric) false exit } if
 
-    /lintcouponposoffer {  % TODO
-        pop
-    } bind def
+        % GCP VLI and value
+        dup length 1 lt {
+            pop pop /bwipp.GS1couponTooShortGCPVLI (Coupon too short: Missing GCP VLI) false exit
+        } if
+        dup 0 1 getinterval cvi dup 6 gt {
+            pop pop /bwipp.GS1couponBadGCPVLI (Coupon GCP length indicator must be 0-6) false exit
+        } if
+        6 add 1 add
+        2 copy exch length gt {
+            pop pop pop /bwipp.GS1couponTooShortGCP (Coupon too short: GCP truncated) false exit
+        } if
+        dup 2 index length exch sub getinterval
 
-    /isocc << [
-        /004 /008 /010 /012 /016 /020 /024 /028 /031 /032 /036 /040 /044 /048
-        /050 /051 /052 /056 /060 /064 /068 /070 /072 /074 /076 /084 /086 /090 /092 /096
-        /100 /104 /108 /112 /116 /120 /124 /132 /136 /140 /144 /148
-        /152 /156 /158 /162 /166 /170 /174 /175 /178 /180 /184 /188 /191 /192 /196
-        /203 /204 /208 /212 /214 /218 /222 /226 /231 /232 /233 /234 /238 /239 /242 /246 /248
-        /250 /254 /258 /260 /262 /266 /268 /270 /275 /276 /288 /292 /296
-        /300 /304 /308 /312 /316 /320 /324 /328 /332 /334 /336 /340 /344 /348
-        /352 /356 /360 /364 /368 /372 /376 /380 /384 /388 /392 /398
-        /400 /404 /408 /410 /414 /417 /418 /422 /426 /428 /430 /434 /438 /440 /442 /446
-        /450 /454 /458 /462 /466 /470 /474 /478 /480 /484 /492 /496 /498 /499
-        /500 /504 /508 /512 /516 /520 /524 /528 /531 /533 /534 /535 /540 /548
-        /554 /558 /562 /566 /570 /574 /578 /580 /581 /583 /584 /585 /586 /591 /598
-        /600 /604 /608 /612 /616 /620 /624 /626 /630 /634 /638 /642 /643 /646
-        /652 /654 /659 /660 /662 /663 /666 /670 /674 /678 /682 /686 /688 /690 /694
-        /702 /703 /704 /705 /706 /710 /716 /724 /728 /729 /732 /740 /744 /748
-        /752 /756 /760 /762 /764 /768 /772 /776 /780 /784 /788 /792 /795 /796 /798
-        /800 /804 /807 /818 /826 /831 /832 /833 /834 /840
-        /850 /854 /858 /860 /862 /876 /882 /887 /894
-    ] {dup} forall >> def
+        % Offer Code
+        dup length 6 lt {
+            pop pop /bwipp.GS1couponTooShortOfferCode (Coupon too short: Offer Code truncated) false exit
+        } if
+        dup length 6 sub 6 exch getinterval
+
+        % Save Value VLI and value
+        dup length 1 lt {
+            pop pop /bwipp.GS1couponTooShortSaveValueVLI (Coupon too short: Missing Save Value VLI) false exit
+        } if
+        dup 0 1 getinterval cvi dup dup 1 lt exch 5 gt or {
+            pop pop /bwipp.GS1couponBadSaveValueVLI (Coupon Save Value length indicator must be 1-5) false exit
+        } if
+        1 add
+        2 copy exch length gt {
+            pop pop pop /bwipp.GS1couponTooShortSaveValue (Coupon too short: Save Value truncated) false exit
+        } if
+        dup 2 index length exch sub getinterval
+
+        % 1st Purchase Requirement VLI and value
+        dup length 1 lt {
+            pop pop /bwipp.GS1couponTooShort1stPurchaseRequirementVLI (Coupon too short: Missing 1st Purchase Requirement VLI) false exit
+        } if
+        dup 0 1 getinterval cvi dup dup 1 lt exch 5 gt or {
+            pop pop /bwipp.GS1couponBad1stPurchaseRequirementVLI (Coupon 1st Purchase Requirement length indicator must be 1-5) false exit
+        } if
+        1 add
+        2 copy exch length gt {
+            pop pop pop /bwipp.GS1couponTooShort1stPurchaseRequirement (Coupon too short: 1st Purchase Requirement truncated) false exit
+        } if
+        dup 2 index length exch sub getinterval
+
+        % 1st Purchase Requirement Code
+        dup length 1 lt {
+            pop pop /bwipp.GS1couponTooShort1stPurchaseRequirementCode (Coupon too short: Missing 1st Purchase Requirement Code) false exit
+        } if
+        dup 0 1 getinterval cvi dup 4 gt exch 9 ne and {
+            pop pop /bwipp.GS1couponBad1stPurchaseRequirementCode (Coupon 1st Purchase Requirement Code must be 0-4 or 9) false exit
+        } if
+        dup length 1 sub 1 exch getinterval
+
+        % 1st Purchase Family Code
+        dup length 3 lt {
+            pop pop /bwipp.GS1couponTooShort1stPurchaseFamilyCode (Coupon too short: 1st Purchase Family Code truncated) false exit
+        } if
+        dup length 3 sub 3 exch getinterval
+
+        % Optional field 1
+        dup length 1 ge { dup 0 1 getinterval cvi 1 eq {
+            1 dup 2 index length exch sub getinterval
+
+            % Additional Purchase Rules Code
+            dup length 1 lt {
+                pop pop /bwipp.GS1couponTooShortAdditionalPurchaseRulesCode (Coupon too short: Missing Additional Purchase Rules Code) false exit
+            } if
+            dup 0 1 getinterval cvi 3 gt {
+                pop pop /bwipp.GS1couponBadAdditionalPurchaseRulesCode (Coupon Additional Purchase Rules Code must be 0-3) false exit
+            } if
+            dup length 1 sub 1 exch getinterval
+
+            % 2nd Purchase RequirementVLI and value
+            dup length 1 lt {
+                pop pop /bwipp.GS1couponTooShort2ndPurchaseRequirementVLI (Coupon too short: Missing 2nd Purchase Requirement VLI) false exit
+            } if
+            dup 0 1 getinterval cvi dup dup 1 lt exch 5 gt or {
+                pop pop /bwipp.GS1couponBad2ndPurchaseRequirementVLI (Coupon 2nd Purchase Requirement length indicator must be 1-5) false exit
+            } if
+            1 add
+            2 copy exch length gt {
+                pop pop pop /bwipp.GS1couponTooShort2ndPurchaseRequirement (Coupon too short: 2nd Purchase Requirement truncated) false exit
+            } if
+            dup 2 index length exch sub getinterval
+
+            % 2nd Purchase Requirement Code
+            dup length 1 lt {
+                pop pop /bwipp.GS1couponTooShort2ndPurchaseRequirementCode (Coupon too short: Missing 2nd Purchase Requirement Code) false exit
+            } if
+            dup 0 1 getinterval cvi dup 4 gt exch 9 ne and {
+                pop pop /bwipp.GS1couponBad2ndPurchaseRequirementCode (Coupon 2nd Purchase Requirement Code must be 0-4 or 9) false exit
+            } if
+            dup length 1 sub 1 exch getinterval
+
+            % 2nd Purchase Family Code
+            dup length 3 lt {
+                pop pop /bwipp.GS1couponTooShort2ndPurchaseFamilyCode (Coupon too short: 2nd Purchase Family Code truncated) false exit
+            } if
+            dup length 3 sub 3 exch getinterval
+
+            % 2nd Purchase GCP VLI and value
+            dup length 1 lt {
+                pop pop /bwipp.GS1couponTooShort2ndPurchaseGCPVLI (Coupon too short: Missing 2nd Purchase GCP VLI) false exit
+            } if
+            dup 0 1 getinterval cvi dup dup 6 gt exch 9 ne and {
+                pop pop /bwipp.GS1couponBad2ndPurchaseGCPVLI (Coupon 2nd Purchase GCP length indicator must be 0-6 or 9) false exit
+            } if
+            dup 9 ne {6 add} {pop 0} ifelse 1 add
+            2 copy exch length gt {
+                pop pop pop /bwipp.GS1couponTooShort2ndPurchaseGCP (Coupon too short: 2nd Purchase GCP truncated) false exit
+            } if
+            dup 2 index length exch sub getinterval
+
+        } if } if
+
+        % Optional field 2
+        dup length 1 ge { dup 0 1 getinterval cvi 2 eq {
+            1 dup 2 index length exch sub getinterval
+
+            % 3rd Purchase RequirementVLI and value
+            dup length 1 lt {
+                pop pop /bwipp.GS1couponTooShort3rdPurchaseRequirementVLI (Coupon too short: Missing 3rd Purchase Requirement VLI) false exit
+            } if
+            dup 0 1 getinterval cvi dup dup 1 lt exch 5 gt or {
+                pop pop /bwipp.GS1couponBad3rdPurchaseRequirementVLI (Coupon 3rd Purchase Requirement length indicator must be 1-5) false exit
+            } if
+            1 add
+            2 copy exch length gt {
+                pop pop pop /bwipp.GS1couponTooShort3rdPurchaseRequirement (Coupon too short: 3rd Purchase Requirement truncated) false exit
+            } if
+            dup 2 index length exch sub getinterval
+
+            % 3rd Purchase Requirement Code
+            dup length 1 lt {
+                pop pop /bwipp.GS1couponTooShort3rdPurchaseRequirementCode (Coupon too short: Missing 3rd Purchase Requirement Code) false exit
+            } if
+            dup 0 1 getinterval cvi dup 4 gt exch 9 ne and {
+                pop pop /bwipp.GS1couponBad3rdPurchaseRequirementCode (Coupon 3rd Purchase Requirement Code must be 0-4 or 9) false exit
+            } if
+            dup length 1 sub 1 exch getinterval
+
+            % 3rd Purchase Family Code
+            dup length 3 lt {
+                pop pop /bwipp.GS1couponTooShort3rdPurchaseFamilyCode (Coupon too short: 3rd Purchase Family Code truncated) false exit
+            } if
+            dup length 3 sub 3 exch getinterval
+
+            % 3rd Purchase GCP VLI and value
+            dup length 1 lt {
+                pop pop /bwipp.GS1couponTooShort3rdPurchaseGCPVLI (Coupon too short: Missing 3rd Purchase GCP VLI) false exit
+            } if
+            dup 0 1 getinterval cvi dup dup 6 gt exch 9 ne and {
+                pop pop /bwipp.GS1couponBad3rdPurchaseGCPVLI (Coupon 3rd Purchase GCP length indicator must be 0-6 or 9) false exit
+            } if
+            dup 9 ne {6 add} {pop 0} ifelse 1 add
+            2 copy exch length gt {
+                pop pop pop /bwipp.GS1couponTooShort3rdPurchaseGCP (Coupon too short: 3rd Purchase GCP truncated) false exit
+            } if
+            dup 2 index length exch sub getinterval
+
+        } if } if
+
+        % Optional field 3
+        /couponexpire -1 def
+        dup length 1 ge { dup 0 1 getinterval cvi 3 eq {
+            1 dup 2 index length exch sub getinterval
+
+            % Expiration date
+            dup length 6 lt {
+                pop pop /bwipp.GS1couponTooShortExpirationDate (Coupon too short: Expiration date) false exit
+            } if
+            dup 2 2 getinterval cvi dup 1 lt exch 12 gt or { pop pop /bwipp.GS1couponExpirationDateBadMonth (Invalid month in expiration date) false exit } if
+            dup 0 2 getinterval cvi dup 21 sub  % Update 20YY periodically for century calculation
+            dup 51 ge {pop 1900 add} { -50 le {2100 add} {2000 add} ifelse} ifelse  % YYYY
+            dup 400 mod 0 eq exch dup 4 mod 0 eq exch 100 mod 0 ne and or           % Leap year?
+            [ 31  3 -1 roll {29} {28} ifelse  31 30 31 30 31 31 30 31 30 31 ]
+            1 index 2 2 getinterval cvi 1 sub get
+            1 index 4 2 getinterval cvi dup 3 1 roll lt
+            exch 1 lt or { pop pop /bwipp.GS1couponExpirationDateBadDay (Invalid day of month in expiration date) false exit } if
+            dup 0 6 getinterval cvi /couponexpire exch def
+            dup length 6 sub 6 exch getinterval
+
+        } if } if
+
+        % Optional field 4
+        dup length 1 ge { dup 0 1 getinterval cvi 4 eq {
+            1 dup 2 index length exch sub getinterval
+
+            % Start date
+            dup length 6 lt {
+                pop pop /bwipp.GS1couponTooShortStartDate (Coupon too short: Start date) false exit
+            } if
+            dup 2 2 getinterval cvi dup 1 lt exch 12 gt or { pop pop /bwipp.GS1couponStartDateBadMonth (Invalid month in start date) false exit } if
+            dup 0 2 getinterval cvi dup 21 sub  % Update 20YY periodically for century calculation
+            dup 51 ge {pop 1900 add} { -50 le {2100 add} {2000 add} ifelse} ifelse  % YYYY
+            dup 400 mod 0 eq exch dup 4 mod 0 eq exch 100 mod 0 ne and or           % Leap year?
+            [ 31  3 -1 roll {29} {28} ifelse  31 30 31 30 31 31 30 31 30 31 ]
+            1 index 2 2 getinterval cvi 1 sub get
+            1 index 4 2 getinterval cvi dup 3 1 roll lt
+            exch 1 lt or { pop pop /bwipp.GS1couponStartDateBadDay (Invalid day of month in start date) false exit } if
+            dup 0 6 getinterval cvi /couponstart exch def
+            couponexpire -1 ne couponexpire couponstart lt and {
+                pop pop /bwipp.GS1couponExpireDateBeforeStartDate (Coupon expires before it starts) false exit
+            } if
+            dup length 6 sub 6 exch getinterval
+
+        } if } if
+
+        % Optional field 5
+        dup length 1 ge { dup 0 1 getinterval cvi 5 eq {
+            1 dup 2 index length exch sub getinterval
+
+            % Serial Number VLI and value
+            dup length 1 lt {
+                pop pop /bwipp.GS1couponTooShortSerialNumberVLI (Coupon too short: Missing Serial Number VLI) false exit
+            } if
+            dup 0 1 getinterval cvi 6 add 1 add
+            2 copy exch length gt {
+                pop pop pop /bwipp.GS1couponTooShortSerialNumber (Coupon too short: Serial Number truncated) false exit
+            } if
+            dup 2 index length exch sub getinterval
+
+        } if } if
+
+        % Optional field 6
+        dup length 1 ge { dup 0 1 getinterval cvi 6 eq {
+            1 dup 2 index length exch sub getinterval
+
+            % Retailer GCP/GLN VLI and value
+            dup length 1 lt {
+                pop pop /bwipp.GS1couponTooShortRetailerGCPGLNVLI (Coupon too short: Missing Retailer GCP/GLN VLI) false exit
+            } if
+            dup 0 1 getinterval cvi dup dup 1 lt exch 7 gt or {
+                pop pop /bwipp.GS1couponBadRetailerGCPGLNVLI (Coupon Retailer GCP/GLN length indicator must be 1-7) false exit
+            } if
+            6 add 1 add
+            2 copy exch length gt {
+                pop pop pop /bwipp.GS1couponTooShortRetailerGCPGLN (Coupon too short: Retailer GCP/GLN truncated) false exit
+            } if
+            dup 2 index length exch sub getinterval
+
+        } if } if
+
+        % Optional field 9
+        dup length 1 ge { dup 0 1 getinterval cvi 9 eq {
+            1 dup 2 index length exch sub getinterval
+
+            % Save Value Code
+            dup length 1 lt {
+                pop pop /bwipp.GS1couponTooShortSaveValueCode (Coupon too short: Missing Save Value Code) false exit
+            } if
+            dup 0 1 getinterval cvi dup 6 gt exch dup 3 eq exch 4 eq or or {
+                pop pop /bwipp.GS1couponBadSaveValueCode (Coupon Save Value Code must be 0,1,2,5 or 6) false exit
+            } if
+            dup length 1 sub 1 exch getinterval
+
+            % Save Value Applies to Item
+            dup length 1 lt {
+                pop pop /bwipp.GS1couponTooShortSaveValueAppliesToItem (Coupon too short: Missing Save Value Applies to Item) false exit
+            } if
+            dup 0 1 getinterval cvi 2 gt {
+                pop pop /bwipp.GS1couponBadSaveValueAppliesToItem (Coupon Save Value Applies to Item must be 0-2) false exit
+            } if
+            dup length 1 sub 1 exch getinterval
+
+            % Store Coupon Flag
+            dup length 1 lt {
+                pop pop /bwipp.GS1couponTooShortStoreCouponFlag (Coupon too short: Missing Store Coupon Flag) false exit
+            } if
+            dup length 1 sub 1 exch getinterval
+
+            % Don't Multiply Flag
+            dup length 1 lt {
+                pop pop /bwipp.GS1couponTooShortDontMultiplyFlag (Coupon too short: Missing Don't Multiply Flag) false exit
+            } if
+            dup 0 1 getinterval cvi 1 gt {
+                pop pop /bwipp.GS1couponBadDontMultiplyFlag (Don't Multiply Flag must be 0 or 1) false exit
+            } if
+            dup length 1 sub 1 exch getinterval
 
-    /lintisocc {
-        isocc exch known not { pop /bwipp.GS1UnknownCountry (Unknown country code) false exit } if
+        } if } if
+
+        dup length 0 ne {
+            pop pop /bwipp.GS1couponUnrecognisedOptionalField (Coupon fields must be 1,2,3,4,5,6 or 9, increasing order) false exit
+        } if
+        pop
     } bind def
 
-    /lintisocclist {
-        dup length 3 mod 0 ne {
-            pop pop /bwipp.GS1BadCountryListLength (Not a group of three-digit country codes) false exit
+    /lintcouponposoffer {
+        dup true exch {
+            dup 48 lt exch 57 gt or { pop false exit } if
+        } forall
+        not { pop pop /bwipp.GS1couponNotNumeric (Coupon not numeric) false exit } if
+        % Format Code
+        dup length 1 lt {
+            pop pop /bwipp.GS1couponTooShortFormatCode (Coupon too short: Missing Format Code) false exit
+        } if
+        dup 0 1 getinterval dup (0) ne exch (1) ne and {
+            pop pop /bwipp.GS1couponBadFormatCode (Coupon format must be 0 or 1) false exit
+        } if
+        dup length 1 sub 1 exch getinterval
+        % Funder ID VLI and Funder ID
+        dup length 1 lt {
+            pop pop /bwipp.GS1couponTooShortFunderVLI (Coupon too short: Missing Funder VLI) false exit
+        } if
+        dup 0 1 getinterval cvi dup 6 gt {
+            pop pop pop /bwipp.GS1couponBadFunderVLI (Coupon Funder length indicator must be 0-6) false exit
+        } if
+        6 add 1 add
+        2 copy exch length gt {
+            pop pop pop /bwipp.GS1couponTooShortFunder (Coupon too short: Truncated Funder ID) false exit
+        } if
+        dup 2 index length exch sub getinterval
+        % Offer Code
+        dup length 6 lt {
+            pop pop /bwipp.GS1couponTooShortOfferCode (Coupon too short: Truncated Offer Code) false exit
+        } if
+        dup length 6 sub 6 exch getinterval
+        % Serial Number VLI and Serial Number
+        dup length 1 lt {
+            pop pop /bwipp.GS1couponTooShortSnVLI (Coupon too short: Missing SN VLI) false exit
+        } if
+        dup 0 1 getinterval cvi
+        6 add 1 add
+        2 copy exch length gt {
+            pop pop pop /bwipp.GS1couponTooShortSn (Coupon too short: Truncated SN) false exit
+        } if
+        dup 2 index length exch sub getinterval
+        dup length 0 ne {
+            pop pop /bwipp.GS1couponTooLong (Coupon too long) false exit
         } if
-        true
-        0 3 3 index length 1 sub {
-            2 index exch 3 getinterval
-            isocc exch known not { pop pop false exit } if
-        } for
-        not { pop /bwipp.GS1UnknownCountry (Unknown country code) false exit } if
         pop
     } bind def
 
     /gs1syntax <<
 
         [
         << /cset /N  /min 18  /max 18  /check [ /lintcsum /lintkey ] >>
@@ -860,15 +1299,15 @@
         (3906) exch dup
         (3907) exch dup
         (3908) exch dup
         (3909) exch dup
         pop
 
         [
-        << /cset /N  /min  3  /max  3  /check [ /lintisocc ] >>
+        << /cset /N  /min  3  /max  3  /check [ /lintiso4217 ] >>
         << /cset /N  /min  1  /max 15  /check [] >>
         ]
         (3910) exch dup
         (3911) exch dup
         (3912) exch dup
         (3913) exch dup
         (3914) exch dup
@@ -891,15 +1330,15 @@
         (3926) exch dup
         (3927) exch dup
         (3928) exch dup
         (3929) exch dup
         pop
 
         [
-        << /cset /N  /min  3  /max  3  /check [ /lintisocc ] >>
+        << /cset /N  /min  3  /max  3  /check [ /lintiso4217 ] >>
         << /cset /N  /min  1  /max 15  /check [] >>
         ]
         (3930) exch dup
         (3931) exch dup
         (3932) exch dup
         (3933) exch dup
         (3934) exch dup
@@ -970,46 +1409,46 @@
         [
         << /cset /X  /min  1  /max 20  /check [] >>
         ]
         (420) exch dup
         pop
 
         [
-        << /cset /N  /min  3  /max  3  /check [ /lintisocc ] >>
+        << /cset /N  /min  3  /max  3  /check [ /lintiso3166 ] >>
         << /cset /X  /min  1  /max  9  /check [] >>
         ]
         (421) exch dup
         pop
 
         [
-        << /cset /N  /min  3  /max  3  /check [ /lintisocc ] >>
+        << /cset /N  /min  3  /max  3  /check [ /lintiso3166 ] >>
         ]
         (422) exch dup
         pop
 
         [
-        << /cset /N  /min  1  /max 15  /check [ /lintisocclist ] >>
+        << /cset /N  /min  1  /max 15  /check [ /lintiso3166list ] >>
         ]
         (423) exch dup
         pop
 
         [
-        << /cset /N  /min  3  /max  3  /check [ /lintisocc ] >>
+        << /cset /N  /min  3  /max  3  /check [ /lintiso3166 ] >>
         ]
         (424) exch dup
         pop
 
         [
-        << /cset /N  /min  1  /max 15  /check [ /lintisocclist ] >>
+        << /cset /N  /min  1  /max 15  /check [ /lintiso3166list ] >>
         ]
         (425) exch dup
         pop
 
         [
-        << /cset /N  /min  3  /max  3  /check [ /lintisocc ] >>
+        << /cset /N  /min  3  /max  3  /check [ /lintiso3166 ] >>
         ]
         (426) exch dup
         pop
 
         [
         << /cset /X  /min  1  /max  3  /check [] >>
         ]
@@ -1030,21 +1469,21 @@
         (4303) exch dup
         (4304) exch dup
         (4305) exch dup
         (4306) exch dup
         pop
 
         [
-        << /cset /X  /min  2  /max  2  /check [] >>
+        << /cset /X  /min  2  /max  2  /check [ /lintiso3166alpha2 ] >>
         ]
         (4307) exch dup
         pop
 
         [
-        << /cset /X  /min  1  /max 30  /check [ /lintpcenc ] >>
+        << /cset /X  /min  1  /max 30  /check [] >>
         ]
         (4308) exch dup
         pop
 
         [
         << /cset /X  /min  1  /max 35  /check [ /lintpcenc ] >>
         ]
@@ -1059,15 +1498,15 @@
         (4313) exch dup
         (4314) exch dup
         (4315) exch dup
         (4316) exch dup
         pop
 
         [
-        << /cset /X  /min  2  /max  2  /check [] >>
+        << /cset /X  /min  2  /max  2  /check [ /lintiso3166alpha2 ] >>
         ]
         (4317) exch dup
         pop
 
         [
         << /cset /X  /min  1  /max 20  /check [] >>
         ]
@@ -1181,15 +1620,15 @@
         [
         << /cset /X  /min  1  /max 30  /check [ /lintkey ] >>
         ]
         (7023) exch dup
         pop
 
         [
-        << /cset /N  /min  3  /max  3  /check [ /lintisocc ] >>
+        << /cset /N  /min  3  /max  3  /check [ /lintiso3166999 ] >>
         << /cset /X  /min  1  /max 27  /check [] >>
         ]
         (7030) exch dup
         (7031) exch dup
         (7032) exch dup
         (7033) exch dup
         (7034) exch dup
@@ -1287,16 +1726,16 @@
         [
         << /cset /X  /min  1  /max 34  /check [ /lintiban ] >>
         ]
         (8007) exch dup
         pop
 
         [
-        << /cset /N  /min  6  /max  6  /check [ /lintyymmdd ] >>
-        << /cset /N  /min  1  /max  6  /check [ /linthhoptmmss ] >>
+        << /cset /N  /min  8  /max  8  /check [ /lintyymmddhh ] >>
+        << /cset /N  /min  0  /max  4  /check [ /lintmmoptss ] >>
         ]
         (8008) exch dup
         pop
 
         [
         << /cset /X  /min  1  /max 50  /check [] >>
         ]
@@ -1318,15 +1757,15 @@
         [
         << /cset /X  /min  1  /max 20  /check [] >>
         ]
         (8012) exch dup
         pop
 
         [
-        << /cset /X  /min  1  /max 30  /check [ /lintkey ] >>
+        << /cset /X  /min  1  /max 25  /check [ /lintcsumalpha /lintkey ] >>
         ]
         (8013) exch dup
         pop
 
         [
         << /cset /N  /min 18  /max 18  /check [ /lintcsum ] >>
         ]
@@ -1445,15 +1884,15 @@
 /setpacking where {pop setpacking} if
 %%EndData
 %%EndResource
 % --END RESOURCE gs1lint--
 
 % --BEGIN RENDERER renlinear--
 % --REQUIRES preamble raiseerror--
-%%BeginResource: uk.co.terryburton.bwipp renlinear 0.0 2020122800 74728 73842
+%%BeginResource: uk.co.terryburton.bwipp renlinear 0.0 2021020600 74728 73842
 %%BeginData:        239 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 begin
 /renlinear {
 
@@ -1692,15 +2131,15 @@
 /setpacking where {pop setpacking} if
 %%EndData
 %%EndResource
 % --END RENDERER renlinear--
 
 % --BEGIN RENDERER renmatrix--
 % --REQUIRES preamble raiseerror--
-%%BeginResource: uk.co.terryburton.bwipp renmatrix 0.0 2020122800 90359 89573
+%%BeginResource: uk.co.terryburton.bwipp renmatrix 0.0 2021020600 90359 89573
 %%BeginData:        306 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 begin
 /renmatrix {
 
@@ -2006,15 +2445,15 @@
 /setpacking where {pop setpacking} if
 %%EndData
 %%EndResource
 % --END RENDERER renmatrix--
 
 % --BEGIN RENDERER renmaximatrix--
 % --REQUIRES preamble raiseerror--
-%%BeginResource: uk.co.terryburton.bwipp renmaximatrix 0.0 2020122800 50046 50044
+%%BeginResource: uk.co.terryburton.bwipp renmaximatrix 0.0 2021020600 50046 50044
 %%BeginData:         81 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 begin
 /renmaximatrix {
 
@@ -2099,15 +2538,15 @@
 
 % --BEGIN ENCODER ean5--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: EAN-5 (5 digit addon)
 % --EXAM: 90200
 % --EXOP: includetext guardwhitespace
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp ean5 0.0 2020122800 58142 57836
+%%BeginResource: uk.co.terryburton.bwipp ean5 0.0 2021020600 58118 57836
 %%BeginData:        137 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /ean5 {
@@ -2248,15 +2687,15 @@
 
 % --BEGIN ENCODER ean2--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: EAN-2 (2 digit addon)
 % --EXAM: 05
 % --EXOP: includetext guardwhitespace
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp ean2 0.0 2020122800 56723 56466
+%%BeginResource: uk.co.terryburton.bwipp ean2 0.0 2021020600 56699 56466
 %%BeginData:        122 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /ean2 {
@@ -2382,15 +2821,15 @@
 
 % --BEGIN ENCODER ean13--
 % --REQUIRES preamble raiseerror renlinear ean5 ean2--
 % --DESC: EAN-13
 % --EXAM: 2112345678900
 % --EXOP: includetext guardwhitespace
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp ean13 0.0 2020122800 81040 77231
+%%BeginResource: uk.co.terryburton.bwipp ean13 0.0 2021020600 80936 77207
 %%BeginData:        217 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /ean2 dup /uk.co.terryburton.bwipp findresource put
 dup /ean5 dup /uk.co.terryburton.bwipp findresource put
@@ -2611,15 +3050,15 @@
 
 % --BEGIN ENCODER ean8--
 % --REQUIRES preamble raiseerror renlinear ean5 ean2--
 % --DESC: EAN-8
 % --EXAM: 02345673
 % --EXOP: includetext guardwhitespace
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp ean8 0.0 2020122800 78158 74434
+%%BeginResource: uk.co.terryburton.bwipp ean8 0.0 2021020600 78158 74434
 %%BeginData:        198 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /ean2 dup /uk.co.terryburton.bwipp findresource put
 dup /ean5 dup /uk.co.terryburton.bwipp findresource put
@@ -2821,15 +3260,15 @@
 
 % --BEGIN ENCODER upca--
 % --REQUIRES preamble raiseerror renlinear ean5 ean2--
 % --DESC: UPC-A
 % --EXAM: 416000336108
 % --EXOP: includetext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp upca 0.0 2020122800 85897 81982
+%%BeginResource: uk.co.terryburton.bwipp upca 0.0 2021020600 86001 81982
 %%BeginData:        250 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /ean2 dup /uk.co.terryburton.bwipp findresource put
 dup /ean5 dup /uk.co.terryburton.bwipp findresource put
@@ -3083,15 +3522,15 @@
 
 % --BEGIN ENCODER upce--
 % --REQUIRES preamble raiseerror renlinear ean5 ean2--
 % --DESC: UPC-E
 % --EXAM: 00123457
 % --EXOP: includetext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp upce 0.0 2020122800 90606 86630
+%%BeginResource: uk.co.terryburton.bwipp upce 0.0 2021020600 90606 86630
 %%BeginData:        289 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /ean2 dup /uk.co.terryburton.bwipp findresource put
 dup /ean5 dup /uk.co.terryburton.bwipp findresource put
@@ -3384,15 +3823,15 @@
 
 % --BEGIN ENCODER isbn--
 % --REQUIRES preamble raiseerror renlinear ean5 ean2 ean13--
 % --DESC: ISBN
 % --EXAM: 978-1-56581-231-4 90000
 % --EXOP: includetext guardwhitespace
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp isbn 0.0 2020122800 86046 88625
+%%BeginResource: uk.co.terryburton.bwipp isbn 0.0 2021020600 86022 88625
 %%BeginData:        254 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /ean13 dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -3650,15 +4089,15 @@
 
 % --BEGIN ENCODER ismn--
 % --REQUIRES preamble raiseerror renlinear ean5 ean2 ean13--
 % --DESC: ISMN
 % --EXAM: 979-0-2605-3211-3
 % --EXOP: includetext guardwhitespace
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp ismn 0.0 2020122800 82722 85314
+%%BeginResource: uk.co.terryburton.bwipp ismn 0.0 2021020600 82594 85418
 %%BeginData:        233 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /ean13 dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -3895,15 +4334,15 @@
 
 % --BEGIN ENCODER issn--
 % --REQUIRES preamble raiseerror renlinear ean2 ean5 ean13--
 % --DESC: ISSN
 % --EXAM: 0311-175X 00 17
 % --EXOP: includetext guardwhitespace
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp issn 0.0 2020122800 74050 77078
+%%BeginResource: uk.co.terryburton.bwipp issn 0.0 2021020600 74026 77078
 %%BeginData:        178 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /ean13 dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -4085,15 +4524,15 @@
 
 % --BEGIN ENCODER code128--
 % --REQUIRES preamble raiseerror parseinput renlinear--
 % --DESC: Code 128
 % --EXAM: Count01234567!
 % --EXOP: includetext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp code128 0.0 2020122800 120207 123267
+%%BeginResource: uk.co.terryburton.bwipp code128 0.0 2021020600 120103 123035
 %%BeginData:        425 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -4522,15 +4961,15 @@
 
 % --BEGIN ENCODER gs1-128--
 % --REQUIRES preamble raiseerror parseinput gs1lint renlinear code128--
 % --DESC: GS1-128
 % --EXAM: (01)95012345678903(3103)000123
 % --EXOP: includetext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp gs1-128 0.0 2020122800 81217 81205
+%%BeginResource: uk.co.terryburton.bwipp gs1-128 0.0 2021020600 84649 81205
 %%BeginData:        156 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /gs1lint dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
@@ -4690,15 +5129,15 @@
 
 % --BEGIN ENCODER ean14--
 % --REQUIRES preamble raiseerror parseinput renlinear code128--
 % --DESC: GS1-14
 % --EXAM: (01) 0 46 01234 56789 3
 % --EXOP: includetext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp ean14 0.0 2020122800 66768 63140
+%%BeginResource: uk.co.terryburton.bwipp ean14 0.0 2021020600 66848 63140
 %%BeginData:        107 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /code128 dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -4809,15 +5248,15 @@
 
 % --BEGIN ENCODER sscc18--
 % --REQUIRES preamble raiseerror parseinput renlinear code128--
 % --DESC: SSCC-18
 % --EXAM: (00) 0 0614141 123456789 0
 % --EXOP: includetext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp sscc18 0.0 2020122800 66780 63147
+%%BeginResource: uk.co.terryburton.bwipp sscc18 0.0 2021020600 66860 63147
 %%BeginData:        107 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /code128 dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -4928,15 +5367,15 @@
 
 % --BEGIN ENCODER code39--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: Code 39
 % --EXAM: THIS IS CODE 39
 % --EXOP: includetext includecheck includecheckintext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp code39 0.0 2020122800 62946 62641
+%%BeginResource: uk.co.terryburton.bwipp code39 0.0 2021020600 62922 62513
 %%BeginData:        143 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /code39 {
@@ -5083,15 +5522,15 @@
 
 % --BEGIN ENCODER code39ext--
 % --REQUIRES preamble raiseerror parseinput renlinear code39--
 % --DESC: Code 39 Extended
 % --EXAM: Code39 Ext!
 % --EXOP: includetext includecheck includecheckintext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp code39ext 0.0 2020122800 65099 61411
+%%BeginResource: uk.co.terryburton.bwipp code39ext 0.0 2021020600 65075 61411
 %%BeginData:        100 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /code39 dup /uk.co.terryburton.bwipp findresource put
@@ -5195,15 +5634,15 @@
 
 % --BEGIN ENCODER code32--
 % --REQUIRES preamble raiseerror renlinear code39--
 % --DESC: Italian Pharmacode
 % --EXAM: 01234567
 % --EXOP: includetext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp code32 0.0 2020122800 58289 61504
+%%BeginResource: uk.co.terryburton.bwipp code32 0.0 2021020600 58289 61504
 %%BeginData:        101 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /code39 dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -5308,15 +5747,15 @@
 
 % --BEGIN ENCODER pzn--
 % --REQUIRES preamble raiseerror renlinear code39--
 % --DESC: Pharmazentralnummer (PZN)
 % --EXAM: 123456
 % --EXOP: includetext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp pzn 0.0 2020122800 58384 61524
+%%BeginResource: uk.co.terryburton.bwipp pzn 0.0 2021020600 58384 61524
 %%BeginData:        102 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /code39 dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -5422,15 +5861,15 @@
 
 % --BEGIN ENCODER code93--
 % --REQUIRES preamble raiseerror parseinput renlinear--
 % --DESC: Code 93
 % --EXAM: THIS IS CODE 93
 % --EXOP: includetext includecheck
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp code93 0.0 2020122800 62124 65325
+%%BeginResource: uk.co.terryburton.bwipp code93 0.0 2021020600 62124 65325
 %%BeginData:        134 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -5568,15 +6007,15 @@
 
 % --BEGIN ENCODER code93ext--
 % --REQUIRES preamble raiseerror parseinput renlinear code93--
 % --DESC: Code 93 Extended
 % --EXAM: Code93 Ext!
 % --EXOP: includetext includecheck
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp code93ext 0.0 2020122800 65429 61772
+%%BeginResource: uk.co.terryburton.bwipp code93ext 0.0 2021020600 65429 61772
 %%BeginData:        104 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /code93 dup /uk.co.terryburton.bwipp findresource put
@@ -5684,15 +6123,15 @@
 
 % --BEGIN ENCODER interleaved2of5--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: Interleaved 2 of 5 (ITF)
 % --EXAM: 2401234567
 % --EXOP: height=0.5 includecheck includetext includecheckintext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp interleaved2of5 0.0 2020122800 61533 61096
+%%BeginResource: uk.co.terryburton.bwipp interleaved2of5 0.0 2021020600 61405 61096
 %%BeginData:        152 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /interleaved2of5 {
@@ -5848,15 +6287,15 @@
 
 % --BEGIN ENCODER itf14--
 % --REQUIRES preamble raiseerror renlinear interleaved2of5--
 % --DESC: ITF-14
 % --EXAM: 0 46 01234 56789 3
 % --EXOP: includetext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp itf14 0.0 2020122800 60879 64093
+%%BeginResource: uk.co.terryburton.bwipp itf14 0.0 2021020600 60983 64117
 %%BeginData:        111 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /interleaved2of5 dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -5971,15 +6410,15 @@
 
 % --BEGIN ENCODER identcode--
 % --REQUIRES preamble raiseerror renlinear interleaved2of5--
 % --DESC: Deutsche Post Identcode
 % --EXAM: 563102430313
 % --EXOP: includetext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp identcode 0.0 2020122800 57310 60628
+%%BeginResource: uk.co.terryburton.bwipp identcode 0.0 2021020600 57310 60628
 %%BeginData:         93 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /interleaved2of5 dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -6076,15 +6515,15 @@
 
 % --BEGIN ENCODER leitcode--
 % --REQUIRES preamble raiseerror renlinear interleaved2of5--
 % --DESC: Deutsche Post Leitcode
 % --EXAM: 21348075016401
 % --EXOP: includetext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp leitcode 0.0 2020122800 57302 60624
+%%BeginResource: uk.co.terryburton.bwipp leitcode 0.0 2021020600 57302 60624
 %%BeginData:         93 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /interleaved2of5 dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -6181,15 +6620,15 @@
 
 % --BEGIN ENCODER databaromni--
 % --REQUIRES preamble raiseerror renlinear renmatrix--
 % --DESC: GS1 DataBar Omnidirectional
 % --EXAM: (01)24012345678905
 % --EXOP:
 % --RNDR: renlinear renmatrix
-%%BeginResource: uk.co.terryburton.bwipp databaromni 0.0 2020122800 105701 108053
+%%BeginResource: uk.co.terryburton.bwipp databaromni 0.0 2021020600 105701 108261
 %%BeginData:        425 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -6618,15 +7057,15 @@
 
 % --BEGIN ENCODER databarstacked--
 % --REQUIRES preamble raiseerror renlinear renmatrix databaromni--
 % --DESC: GS1 DataBar Stacked
 % --EXAM: (01)24012345678905
 % --EXOP:
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp databarstacked 0.0 2020122800 61648 57939
+%%BeginResource: uk.co.terryburton.bwipp databarstacked 0.0 2021020600 61520 58043
 %%BeginData:         75 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 dup /databaromni dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -6705,15 +7144,15 @@
 
 % --BEGIN ENCODER databarstackedomni--
 % --REQUIRES preamble raiseerror renlinear renmatrix databaromni--
 % --DESC: GS1 DataBar Stacked Omnidirectional
 % --EXAM: (01)24012345678905
 % --EXOP:
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp databarstackedomni 0.0 2020122800 61748 58019
+%%BeginResource: uk.co.terryburton.bwipp databarstackedomni 0.0 2021020600 61620 58123
 %%BeginData:         75 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 dup /databaromni dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -6792,15 +7231,15 @@
 
 % --BEGIN ENCODER databartruncated--
 % --REQUIRES preamble raiseerror renlinear renmatrix databaromni--
 % --DESC: GS1 DataBar Truncated
 % --EXAM: (01)24012345678905
 % --EXOP:
 % --RNDR: renlinear renmatrix
-%%BeginResource: uk.co.terryburton.bwipp databartruncated 0.0 2020122800 61674 57955
+%%BeginResource: uk.co.terryburton.bwipp databartruncated 0.0 2021020600 61546 58059
 %%BeginData:         75 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /databaromni dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -6879,15 +7318,15 @@
 
 % --BEGIN ENCODER databarlimited--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: GS1 DataBar Limited
 % --EXAM: (01)15012345678907
 % --EXOP:
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp databarlimited 0.0 2020122800 81204 80353
+%%BeginResource: uk.co.terryburton.bwipp databarlimited 0.0 2021020600 81076 80249
 %%BeginData:        278 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /databarlimited {
@@ -7169,15 +7608,15 @@
 
 % --BEGIN ENCODER databarexpanded--
 % --REQUIRES preamble raiseerror parseinput gs1lint renlinear renmatrix--
 % --DESC: GS1 DataBar Expanded
 % --EXAM: (01)95012345678903(3103)000123
 % --EXOP:
 % --RNDR: renlinear renmatrix
-%%BeginResource: uk.co.terryburton.bwipp databarexpanded 0.0 2020122800 242804 248423
+%%BeginResource: uk.co.terryburton.bwipp databarexpanded 0.0 2021020600 242700 244887
 %%BeginData:        886 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /gs1lint dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
@@ -8067,15 +8506,15 @@
 
 % --BEGIN ENCODER databarexpandedstacked--
 % --REQUIRES preamble raiseerror parseinput gs1lint renlinear renmatrix databarexpanded--
 % --DESC: GS1 DataBar Expanded Stacked
 % --EXAM: (01)95012345678903(3103)000123
 % --EXOP: segments=4
 % --RNDR: renlinear renmatrix
-%%BeginResource: uk.co.terryburton.bwipp databarexpandedstacked 0.0 2020122800 66639 66505
+%%BeginResource: uk.co.terryburton.bwipp databarexpandedstacked 0.0 2021020600 66639 63073
 %%BeginData:         45 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 dup /databarexpanded dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -8124,15 +8563,15 @@
 
 % --BEGIN ENCODER gs1northamericancoupon--
 % --REQUIRES preamble raiseerror parseinput gs1lint renlinear renmatrix databarexpanded databarexpandedstacked--
 % --DESC: GS1 North American Coupon
 % --EXAM: (8110)106141416543213500110000310123196000
 % --EXOP: includetext segments=8
 % --RNDR: renlinear renmatrix
-%%BeginResource: uk.co.terryburton.bwipp gs1northamericancoupon 0.0 2020122800 82792 85943
+%%BeginResource: uk.co.terryburton.bwipp gs1northamericancoupon 0.0 2021020600 82792 82511
 %%BeginData:        131 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /gs1lint dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
@@ -8267,15 +8706,15 @@
 
 % --BEGIN ENCODER pharmacode--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: Pharmaceutical Binary Code
 % --EXAM: 117480
 % --EXOP: showborder
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp pharmacode 0.0 2020122800 55122 54752
+%%BeginResource: uk.co.terryburton.bwipp pharmacode 0.0 2021020600 54994 54752
 %%BeginData:         93 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /pharmacode {
@@ -8372,15 +8811,15 @@
 
 % --BEGIN ENCODER pharmacode2--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: Two-track Pharmacode
 % --EXAM: 117480
 % --EXOP: includetext showborder
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp pharmacode2 0.0 2020122800 55953 55610
+%%BeginResource: uk.co.terryburton.bwipp pharmacode2 0.0 2021020600 55929 55610
 %%BeginData:         98 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /pharmacode2 {
@@ -8482,15 +8921,15 @@
 
 % --BEGIN ENCODER code2of5--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: Code 25
 % --EXAM: 01234567
 % --EXOP: includetext includecheck includecheckintext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp code2of5 0.0 2020122800 63541 62953
+%%BeginResource: uk.co.terryburton.bwipp code2of5 0.0 2021020600 63389 62953
 %%BeginData:        153 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /code2of5 {
@@ -8647,15 +9086,15 @@
 
 % --BEGIN ENCODER industrial2of5--
 % --REQUIRES preamble raiseerror renlinear code2of5--
 % --DESC: Industrial 2 of 5
 % --EXAM: 01234567
 % --EXOP: includetext includecheck includecheckintext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp industrial2of5 0.0 2020122800 51614 55042
+%%BeginResource: uk.co.terryburton.bwipp industrial2of5 0.0 2021020600 51614 55042
 %%BeginData:         57 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /code2of5 dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -8716,15 +9155,15 @@
 
 % --BEGIN ENCODER iata2of5--
 % --REQUIRES preamble raiseerror renlinear code2of5--
 % --DESC: IATA 2 of 5
 % --EXAM: 01234567
 % --EXOP: includetext includecheck includecheckintext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp iata2of5 0.0 2020122800 51584 55018
+%%BeginResource: uk.co.terryburton.bwipp iata2of5 0.0 2021020600 51584 55018
 %%BeginData:         57 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /code2of5 dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -8785,15 +9224,15 @@
 
 % --BEGIN ENCODER matrix2of5--
 % --REQUIRES preamble raiseerror renlinear code2of5--
 % --DESC: Matrix 2 of 5
 % --EXAM: 01234567
 % --EXOP: includetext includecheck includecheckintext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp matrix2of5 0.0 2020122800 51594 55026
+%%BeginResource: uk.co.terryburton.bwipp matrix2of5 0.0 2021020600 51594 55026
 %%BeginData:         57 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /code2of5 dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -8854,15 +9293,15 @@
 
 % --BEGIN ENCODER coop2of5--
 % --REQUIRES preamble raiseerror renlinear code2of5--
 % --DESC: COOP 2 of 5
 % --EXAM: 01234567
 % --EXOP: includetext includecheck includecheckintext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp coop2of5 0.0 2020122800 51584 55018
+%%BeginResource: uk.co.terryburton.bwipp coop2of5 0.0 2021020600 51584 55018
 %%BeginData:         57 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /code2of5 dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -8923,15 +9362,15 @@
 
 % --BEGIN ENCODER datalogic2of5--
 % --REQUIRES preamble raiseerror renlinear code2of5--
 % --DESC: Datalogic 2 of 5
 % --EXAM: 01234567
 % --EXOP: includetext includecheck includecheckintext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp datalogic2of5 0.0 2020122800 51609 55038
+%%BeginResource: uk.co.terryburton.bwipp datalogic2of5 0.0 2021020600 51609 55038
 %%BeginData:         57 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /code2of5 dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -8992,15 +9431,15 @@
 
 % --BEGIN ENCODER code11--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: Code 11
 % --EXAM: 0123456789
 % --EXOP: includetext includecheck includecheckintext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp code11 0.0 2020122800 64947 64410
+%%BeginResource: uk.co.terryburton.bwipp code11 0.0 2021020600 64819 64410
 %%BeginData:        160 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /code11 {
@@ -9164,15 +9603,15 @@
 
 % --BEGIN ENCODER bc412--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: BC412
 % --EXAM: BC412
 % --EXOP: semi includetext includecheckintext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp bc412 0.0 2020122800 60520 60057
+%%BeginResource: uk.co.terryburton.bwipp bc412 0.0 2021020600 60392 60057
 %%BeginData:        150 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /bc412 {
@@ -9326,15 +9765,15 @@
 
 % --BEGIN ENCODER rationalizedCodabar--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: Codabar
 % --EXAM: A0123456789B
 % --EXOP: includetext includecheck includecheckintext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp rationalizedCodabar 0.0 2020122800 65443 64950
+%%BeginResource: uk.co.terryburton.bwipp rationalizedCodabar 0.0 2021020600 65419 64822
 %%BeginData:        158 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /rationalizedCodabar {
@@ -9496,15 +9935,15 @@
 
 % --BEGIN ENCODER onecode--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: USPS Intelligent Mail
 % --EXAM: 0123456709498765432101234567891
 % --EXOP: barcolor=FF0000
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp onecode 0.0 2020122800 99173 98718
+%%BeginResource: uk.co.terryburton.bwipp onecode 0.0 2021020600 99045 98718
 %%BeginData:        337 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /onecode {
@@ -9845,15 +10284,15 @@
 
 % --BEGIN ENCODER postnet--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: USPS POSTNET
 % --EXAM: 01234
 % --EXOP: includetext includecheckintext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp postnet 0.0 2020122800 61318 60891
+%%BeginResource: uk.co.terryburton.bwipp postnet 0.0 2021020600 61190 60891
 %%BeginData:        142 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /postnet {
@@ -9999,15 +10438,15 @@
 
 % --BEGIN ENCODER planet--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: USPS PLANET
 % --EXAM: 01234567890
 % --EXOP: includetext includecheckintext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp planet 0.0 2020122800 61178 60755
+%%BeginResource: uk.co.terryburton.bwipp planet 0.0 2021020600 61050 60755
 %%BeginData:        143 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /planet {
@@ -10154,15 +10593,15 @@
 
 % --BEGIN ENCODER royalmail--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: Royal Mail 4 State Customer Code
 % --EXAM: LE28HS9Z
 % --EXOP: includetext barcolor=FF0000
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp royalmail 0.0 2020122800 61989 61521
+%%BeginResource: uk.co.terryburton.bwipp royalmail 0.0 2021020600 61861 61521
 %%BeginData:        147 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /royalmail {
@@ -10313,15 +10752,15 @@
 
 % --BEGIN ENCODER auspost--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: AusPost 4 State Customer Code
 % --EXAM: 5956439111ABA 9
 % --EXOP: includetext custinfoenc=character
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp auspost 0.0 2020122800 72801 72415
+%%BeginResource: uk.co.terryburton.bwipp auspost 0.0 2021020600 72777 72519
 %%BeginData:        204 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /auspost {
@@ -10529,15 +10968,15 @@
 
 % --BEGIN ENCODER kix--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: Royal Dutch TPG Post KIX
 % --EXAM: 1231FZ13XHS
 % --EXOP: includetext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp kix 0.0 2020122800 57131 56916
+%%BeginResource: uk.co.terryburton.bwipp kix 0.0 2021020600 57107 56916
 %%BeginData:        113 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /kix {
@@ -10654,15 +11093,15 @@
 
 % --BEGIN ENCODER japanpost--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: Japan Post 4 State Customer Code
 % --EXAM: 6540123789-A-K-Z
 % --EXOP: includetext includecheckintext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp japanpost 0.0 2020122800 62150 61757
+%%BeginResource: uk.co.terryburton.bwipp japanpost 0.0 2021020600 62126 61757
 %%BeginData:        164 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /japanpost {
@@ -10830,15 +11269,15 @@
 
 % --BEGIN ENCODER msi--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: MSI Modified Plessey
 % --EXAM: 0123456789
 % --EXOP: includetext includecheck includecheckintext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp msi 0.0 2020122800 67193 66798
+%%BeginResource: uk.co.terryburton.bwipp msi 0.0 2021020600 67169 66798
 %%BeginData:        141 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /msi {
@@ -10983,15 +11422,15 @@
 
 % --BEGIN ENCODER plessey--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: Plessey UK
 % --EXAM: 01234ABCD
 % --EXOP: includetext includecheckintext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp plessey 0.0 2020122800 63687 63197
+%%BeginResource: uk.co.terryburton.bwipp plessey 0.0 2021020600 63559 63197
 %%BeginData:        148 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /plessey {
@@ -11143,15 +11582,15 @@
 
 % --BEGIN ENCODER telepen--
 % --REQUIRES preamble raiseerror parseinput renlinear--
 % --DESC: Telepen
 % --EXAM: ABCDEF
 % --EXOP: includetext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp telepen 0.0 2020122800 65612 68797
+%%BeginResource: uk.co.terryburton.bwipp telepen 0.0 2021020600 65612 68821
 %%BeginData:        165 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -11320,15 +11759,15 @@
 
 % --BEGIN ENCODER telepennumeric--
 % --REQUIRES preamble raiseerror parseinput renlinear telepen--
 % --DESC: Telepen Numeric
 % --EXAM: 01234567
 % --EXOP: includetext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp telepennumeric 0.0 2020122800 57897 54467
+%%BeginResource: uk.co.terryburton.bwipp telepennumeric 0.0 2021020600 57921 54339
 %%BeginData:         57 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /telepen dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -11389,15 +11828,15 @@
 
 % --BEGIN ENCODER posicode--
 % --REQUIRES preamble raiseerror parseinput renlinear--
 % --DESC: PosiCode
 % --EXAM: ABC123
 % --EXOP: version=b inkspread=-0.5 parsefnc includetext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp posicode 0.0 2020122800 107180 110082
+%%BeginResource: uk.co.terryburton.bwipp posicode 0.0 2021020600 107180 110082
 %%BeginData:        390 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -11791,15 +12230,15 @@
 
 % --BEGIN ENCODER codablockf--
 % --REQUIRES preamble raiseerror parseinput renmatrix--
 % --DESC: Codablock F
 % --EXAM: CODABLOCK F 34567890123456789010040digit
 % --EXOP: columns=8
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp codablockf 0.0 2020122800 128823 131632
+%%BeginResource: uk.co.terryburton.bwipp codablockf 0.0 2021020600 128847 131632
 %%BeginData:        488 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -12291,15 +12730,15 @@
 
 % --BEGIN ENCODER code16k--
 % --REQUIRES preamble raiseerror parseinput renmatrix--
 % --DESC: Code 16K
 % --EXAM: Abcd-1234567890-wxyZ
 % --EXOP:
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp code16k 0.0 2020122800 153345 155912
+%%BeginResource: uk.co.terryburton.bwipp code16k 0.0 2021020600 153473 155912
 %%BeginData:        711 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -13014,15 +13453,15 @@
 
 % --BEGIN ENCODER code49--
 % --REQUIRES preamble raiseerror parseinput renmatrix--
 % --DESC: Code 49
 % --EXAM: MULTIPLE ROWS IN CODE 49
 % --EXOP:
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp code49 0.0 2020122800 255438 268416
+%%BeginResource: uk.co.terryburton.bwipp code49 0.0 2021020600 255462 258120
 %%BeginData:       1042 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -14068,15 +14507,15 @@
 
 % --BEGIN ENCODER channelcode--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: Channel Code
 % --EXAM: 3493
 % --EXOP: height=0.5 includetext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp channelcode 0.0 2020122800 125448 124333
+%%BeginResource: uk.co.terryburton.bwipp channelcode 0.0 2021020600 125424 124333
 %%BeginData:        250 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /channelcode {
@@ -14330,15 +14769,15 @@
 
 % --BEGIN ENCODER flattermarken--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: Flattermarken
 % --EXAM: 11099
 % --EXOP: inkspread=-0.25 showborder borderleft=0 borderright=0
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp flattermarken 0.0 2020122800 53933 53728
+%%BeginResource: uk.co.terryburton.bwipp flattermarken 0.0 2021020600 53805 53752
 %%BeginData:         95 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /flattermarken {
@@ -14437,15 +14876,15 @@
 
 % --BEGIN ENCODER raw--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: Custom 1D symbology
 % --EXAM: 331132131313411122131311333213114131131221323
 % --EXOP: height=0.5
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp raw 0.0 2020122800 49535 49415
+%%BeginResource: uk.co.terryburton.bwipp raw 0.0 2021020600 49511 49415
 %%BeginData:         54 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /raw {
@@ -14503,15 +14942,15 @@
 
 % --BEGIN ENCODER daft--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: Custom 4 state symbology
 % --EXAM: FATDAFTDAD
 % --EXOP:
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp daft 0.0 2020122800 52789 52642
+%%BeginResource: uk.co.terryburton.bwipp daft 0.0 2021020600 52765 52642
 %%BeginData:         78 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /daft {
@@ -14593,15 +15032,15 @@
 
 % --BEGIN ENCODER symbol--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: Miscellaneous symbols
 % --EXAM: fima
 % --EXOP: backgroundcolor=DD000011
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp symbol 0.0 2020122800 52393 52217
+%%BeginResource: uk.co.terryburton.bwipp symbol 0.0 2021020600 52369 52217
 %%BeginData:         74 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /symbol {
@@ -14679,15 +15118,15 @@
 
 % --BEGIN ENCODER pdf417--
 % --REQUIRES preamble raiseerror parseinput renmatrix--
 % --DESC: PDF417
 % --EXAM: This is PDF417
 % --EXOP: columns=2
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp pdf417 0.0 2020122800 195817 201631
+%%BeginResource: uk.co.terryburton.bwipp pdf417 0.0 2021020600 195945 198071
 %%BeginData:        893 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -15584,15 +16023,15 @@
 
 % --BEGIN ENCODER pdf417compact--
 % --REQUIRES preamble raiseerror parseinput renmatrix pdf417--
 % --DESC: Compact PDF417
 % --EXAM: This is compact PDF417
 % --EXOP: columns=2
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp pdf417compact 0.0 2020122800 56915 53230
+%%BeginResource: uk.co.terryburton.bwipp pdf417compact 0.0 2021020600 56787 53230
 %%BeginData:         45 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 dup /pdf417 dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -15641,15 +16080,15 @@
 
 % --BEGIN ENCODER micropdf417--
 % --REQUIRES preamble raiseerror parseinput renmatrix--
 % --DESC: MicroPDF417
 % --EXAM: MicroPDF417
 % --EXOP:
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp micropdf417 0.0 2020122800 206979 215991
+%%BeginResource: uk.co.terryburton.bwipp micropdf417 0.0 2021020600 207003 209127
 %%BeginData:        980 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -16633,15 +17072,15 @@
 
 % --BEGIN ENCODER datamatrix--
 % --REQUIRES preamble raiseerror parseinput renmatrix--
 % --DESC: Data Matrix
 % --EXAM: This is Data Matrix!
 % --EXOP:
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp datamatrix 0.0 2020122800 207969 233965
+%%BeginResource: uk.co.terryburton.bwipp datamatrix 0.0 2021020600 208097 216597
 %%BeginData:        917 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -17562,15 +18001,15 @@
 
 % --BEGIN ENCODER datamatrixrectangular--
 % --REQUIRES preamble raiseerror parseinput renmatrix datamatrix--
 % --DESC: Data Matrix Rectangular
 % --EXAM: 1234
 % --EXOP:
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp datamatrixrectangular 0.0 2020122800 56843 53278
+%%BeginResource: uk.co.terryburton.bwipp datamatrixrectangular 0.0 2021020600 56843 53278
 %%BeginData:         45 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 dup /datamatrix dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -17619,15 +18058,15 @@
 
 % --BEGIN ENCODER datamatrixrectangularextension--
 % --REQUIRES preamble raiseerror parseinput renmatrix datamatrix--
 % --DESC: Data Matrix Rectangular Extension
 % --EXAM: 1234
 % --EXOP: version=8x96
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp datamatrixrectangularextension 0.0 2020122800 57622 54152
+%%BeginResource: uk.co.terryburton.bwipp datamatrixrectangularextension 0.0 2021020600 57622 54152
 %%BeginData:         55 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 dup /datamatrix dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -17686,15 +18125,15 @@
 
 % --BEGIN ENCODER mailmark--
 % --REQUIRES preamble raiseerror parseinput renmatrix datamatrix--
 % --DESC: Royal Mail Mailmark
 % --EXAM: JGB 012100123412345678AB19XY1A 0             www.xyz.com
 % --EXOP: type=29
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp mailmark 0.0 2020122800 60327 56712
+%%BeginResource: uk.co.terryburton.bwipp mailmark 0.0 2021020600 60223 56712
 %%BeginData:         80 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 dup /datamatrix dup /uk.co.terryburton.bwipp findresource put
@@ -17778,15 +18217,15 @@
 
 % --BEGIN ENCODER qrcode--
 % --REQUIRES preamble raiseerror parseinput renmatrix--
 % --DESC: QR Code
 % --EXAM: http://goo.gl/0bis
 % --EXOP: eclevel=M
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp qrcode 0.0 2020122800 324078 365813
+%%BeginResource: uk.co.terryburton.bwipp qrcode 0.0 2021020600 313702 355309
 %%BeginData:       1291 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -19081,15 +19520,15 @@
 
 % --BEGIN ENCODER swissqrcode--
 % --REQUIRES preamble raiseerror parseinput renmatrix qrcode--
 % --DESC: Swiss QR Code
 % --EXAM:
 % --EXOP:
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp swissqrcode 0.0 2020122800 65895 58838
+%%BeginResource: uk.co.terryburton.bwipp swissqrcode 0.0 2021020600 62487 58862
 %%BeginData:        127 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 dup /qrcode dup /uk.co.terryburton.bwipp findresource put
@@ -19220,15 +19659,15 @@
 
 % --BEGIN ENCODER microqrcode--
 % --REQUIRES preamble raiseerror parseinput renmatrix qrcode--
 % --DESC: Micro QR Code
 % --EXAM: 1234
 % --EXOP:
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp microqrcode 0.0 2020122800 57155 57010
+%%BeginResource: uk.co.terryburton.bwipp microqrcode 0.0 2021020600 57179 53578
 %%BeginData:         45 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 dup /qrcode dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -19277,15 +19716,15 @@
 
 % --BEGIN ENCODER rectangularmicroqrcode--
 % --REQUIRES preamble raiseerror parseinput renmatrix qrcode--
 % --DESC: Rectangular Micro QR Code
 % --EXAM: 1234
 % --EXOP: version=R17x139
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp rectangularmicroqrcode 0.0 2020122800 57198 57042
+%%BeginResource: uk.co.terryburton.bwipp rectangularmicroqrcode 0.0 2021020600 57222 53610
 %%BeginData:         45 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 dup /qrcode dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -19334,15 +19773,15 @@
 
 % --BEGIN ENCODER maxicode--
 % --REQUIRES preamble raiseerror parseinput renmaximatrix--
 % --DESC: MaxiCode
 % --EXAM: [)>^03001^02996152382802^029840^029001^0291Z00004951^029UPSN^02906X610^029159^0291234567^0291/1^029^029Y^029634 ALPHA DR^029PITTSBURGH^029PA^029^004
 % --EXOP: mode=2 parse
 % --RNDR: renmaximatrix
-%%BeginResource: uk.co.terryburton.bwipp maxicode 0.0 2020122800 126819 129220
+%%BeginResource: uk.co.terryburton.bwipp maxicode 0.0 2021020600 126819 129324
 %%BeginData:        596 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /renmaximatrix dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -19942,15 +20381,15 @@
 
 % --BEGIN ENCODER azteccode--
 % --REQUIRES preamble raiseerror parseinput renmatrix--
 % --DESC: Aztec Code
 % --EXAM: This is Aztec Code
 % --EXOP: format=full
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp azteccode 0.0 2020122800 174547 187059
+%%BeginResource: uk.co.terryburton.bwipp azteccode 0.0 2021020600 174571 176659
 %%BeginData:        714 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -20668,15 +21107,15 @@
 
 % --BEGIN ENCODER azteccodecompact--
 % --REQUIRES preamble raiseerror parseinput renmatrix azteccode--
 % --DESC: Compact Aztec Code
 % --EXAM: 1234
 % --EXOP:
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp azteccodecompact 0.0 2020122800 56819 53259
+%%BeginResource: uk.co.terryburton.bwipp azteccodecompact 0.0 2021020600 56819 53387
 %%BeginData:         45 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 dup /azteccode dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -20725,15 +21164,15 @@
 
 % --BEGIN ENCODER aztecrune--
 % --REQUIRES preamble raiseerror parseinput renmatrix azteccode--
 % --DESC: Aztec Runes
 % --EXAM: 1
 % --EXOP:
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp aztecrune 0.0 2020122800 56788 53235
+%%BeginResource: uk.co.terryburton.bwipp aztecrune 0.0 2021020600 56788 53363
 %%BeginData:         45 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 dup /azteccode dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -20782,16 +21221,16 @@
 
 % --BEGIN ENCODER codeone--
 % --REQUIRES preamble raiseerror parseinput renmatrix--
 % --DESC: Code One
 % --EXAM: Code One
 % --EXOP:
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp codeone 0.0 2020122800 191244 210362
-%%BeginData:        856 ASCII Lines
+%%BeginResource: uk.co.terryburton.bwipp codeone 0.0 2021020600 196386 201586
+%%BeginData:        883 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 begin
 /codeone {
@@ -21144,23 +21583,23 @@
                     } if
                     /char msg i k add get def
                     /ac ac isD {1 2 div add} {isEA {ceiling 2 add} {ceiling 1 add} ifelse} ifelse def
                     /cc cc isC {2 3 div add} {isEA { 8 3 div add } { 4 3 div add } ifelse} ifelse def
                     /tc tc isT {2 3 div add} {isEA { 8 3 div add } { 4 3 div add } ifelse} ifelse def
                     /xc xc isX {2 3 div add} {isEA {13 3 div add } {10 3 div add } ifelse} ifelse def
                     /bc bc isFN {3 add} {1 add} ifelse def
-                    k 3 ge {
+                    k 3 ge {  % Checking after at least 4 characters (cf. Data Matrix), not 3 as in spec Step Q
                         true [ac cc tc xc   ] {bc 1 add exch ceiling le and} forall {B exit} if
                         true [   cc tc xc bc] {ac 1 add exch ceiling le and} forall {A exit} if
-                        true [ac cc    xc bc] {tc 1 add exch ceiling le and} forall {T exit} if
-                        true [ac    tc      ] {cc 1 add exch ceiling le and} forall {
+                        true [ac cc    xc bc] {tc ceiling 1 add exch ceiling le and} forall {T exit} if
+                        true [ac    tc      ] {cc ceiling 1 add exch ceiling le and} forall {
                             cc ceiling xc ceiling lt {C exit} if
                             cc xc eq {i k add 1 add XtermFirst {X exit} {C exit} ifelse} if
                         } if
-                        true [ac cc tc    bc] {xc 1 add exch lt and} forall {X exit} if
+                        true [ac cc tc    bc] {xc ceiling 1 add exch ceiling le and} forall {X exit} if
                     } if
                     /k k 1 add def
                 } loop
             } repeat
         } bind def
 
         /addtocws {
@@ -21232,32 +21671,51 @@
         /encCTX {
             /p 0 def
             /ctxvals 2220 array def
 
             % Lookup the values for each character
             {
                 i msglen eq {exit} if
-                encvals mode get msg i get known not {exit} if
                 p 3 mod 0 eq {
                     numD i get 12 ge {
+                        ctxvals 0 p getinterval CTXvalstocws addtocws
                         [unlcw] addtocws
                         /mode A def
                         exit
                     } if
                     numD i get dup 8 ge exch i add msglen eq and {
-                        [unlcw] addtocws
-                        /mode A def
-                        exit
-                    } if
-                    lookup mode ne {
                         ctxvals 0 p getinterval CTXvalstocws addtocws
                         [unlcw] addtocws
                         /mode A def
                         exit
                     } if
+                    mode X eq {  % Steps E1c, E2
+                        Xvals msg i get known not {
+                            ctxvals 0 p getinterval CTXvalstocws addtocws
+                            % Unlatch to ASCII unless one codeword left and single ASCII to encode
+                            numremcws j get 1 ne msg i get 127 gt or {
+                                [unlcw] addtocws
+                            } if
+                            /mode A def
+                            exit
+                        } if
+                        i 1 add msglen lt {
+                            Xvals msg i 1 add get known not {exit} if
+                            i 2 add msglen lt {
+                                Xvals msg i 2 add get known not {exit} if
+                            } if
+                        } if
+                    } {
+                        lookup mode ne {
+                            ctxvals 0 p getinterval CTXvalstocws addtocws
+                            [unlcw] addtocws
+                            /mode A def
+                            exit
+                        } if
+                    } ifelse
                     msglen i sub 3 le {  % Check end of data conditions
                         /remcws numremcws j p 3 idiv 2 mul add get def
                         /remvals [
                             msg i msglen i sub getinterval {
                                 dup encvals mode get exch known {
                                     encvals mode get exch get aload pop
                                 } {  % Unencodable X12 characters
@@ -21343,19 +21801,25 @@
 
                 numD i get 3 lt {
 
                     /Drem 8 Dbits length 8 mod sub 8 mod def
                     /remcws numremcws j Dbits length 8 idiv add get def
 
                     % Final codeword with no data
-                    numremcws j Dbits length 8 idiv add 1 sub get 1 sub 0 eq
-                    i msglen eq and {exit} if
+                    numremcws j Dbits length 8 idiv add 1 sub get 1 sub 0 eq Drem 0 eq and  % No remaining codewords and no bits
+                    remcws 1 eq Drem 0 ne and or  % Or 1 remaining codeword and some bits
+                    i msglen eq and {
+                        Drem 4 eq Drem 6 eq or { /Dbits [ Dbits aload pop 1 1 1 1 ] def } if
+                        Drem 2 eq Drem 6 eq or { /Dbits [ Dbits aload pop 0 1 ] def } if
+                        exit
+                    } if
 
-                    % Final digit into final codeword as ASCII
+                    % Final digit or double-digit into final codeword as ASCII
                     i msglen 1 sub eq numD i get 1 eq and
+                    i msglen 2 sub eq numD i get 2 eq and or
                     remcws 1 eq and Drem 0 eq and {exit} if
 
                     % Latch to ASCII unless 4 or 6 bits remain in final codeword
                     i msglen 1 sub eq numD i get 1 eq and
                     remcws 1 eq and Drem 4 eq Drem 6 eq or and not {
                       /Dbits [ Dbits aload pop 1 1 1 1 1 1 ] def
                       /Drem 8 Dbits length 8 mod sub 8 mod def
@@ -21457,14 +21921,16 @@
     % Extend cws to ncws codewords by addition of pad characters
     stype not {
         /cws [ cws aload pop dcws cws length sub {129} repeat ] def
     } {
         /cws [ dcws cws length sub {0} repeat cws aload pop ] def
     } ifelse
 
+    options /debugcws known { /bwipp.debugcws cws //raiseerror exec } if
+
     % De-interleave the codewords into blocks
     /cwbs rsbl array def  % Array of data codeword blocks
     /ecbs rsbl array def  % Array of error correction blocks
     0 1 rsbl 1 sub {
         /i exch def
         /cwb dcpb array def
         0 1 dcpb 1 sub {
@@ -21650,15 +22116,15 @@
 
 % --BEGIN ENCODER hanxin--
 % --REQUIRES preamble raiseerror parseinput renmatrix--
 % --DESC: Han Xin Code
 % --EXAM: This is Han Xin
 % --EXOP:
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp hanxin 0.0 2020122800 306050 349404
+%%BeginResource: uk.co.terryburton.bwipp hanxin 0.0 2021020600 299418 335780
 %%BeginData:        852 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -22514,15 +22980,15 @@
 
 % --BEGIN ENCODER dotcode--
 % --REQUIRES preamble raiseerror parseinput renmatrix--
 % --DESC: DotCode
 % --EXAM: This is DotCode
 % --EXOP: inkspread=0.16
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp dotcode 0.0 2020122800 231602 264430
+%%BeginResource: uk.co.terryburton.bwipp dotcode 0.0 2021020600 231730 243734
 %%BeginData:       1035 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -23561,15 +24027,15 @@
 
 % --BEGIN ENCODER ultracode--
 % --REQUIRES preamble raiseerror parseinput renmatrix--
 % --DESC: Ultracode
 % --EXAM: Awesome colours!
 % --EXOP: eclevel=EC2
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp ultracode 0.0 2020122800 84277 87023
+%%BeginResource: uk.co.terryburton.bwipp ultracode 0.0 2021020600 84301 87023
 %%BeginData:        299 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -23872,15 +24338,15 @@
 
 % --BEGIN ENCODER jabcode--
 % --REQUIRES preamble raiseerror parseinput renmatrix--
 % --DESC: JAB Code (Beta)
 % --EXAM: This is JAB Code
 % --EXOP: eclevel=6
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp jabcode 0.0 2020122800 243765 285987
+%%BeginResource: uk.co.terryburton.bwipp jabcode 0.0 2021020600 243685 265291
 %%BeginData:       1132 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -25016,15 +25482,15 @@
 
 % --BEGIN ENCODER gs1-cc--
 % --REQUIRES preamble raiseerror parseinput gs1lint renmatrix micropdf417 pdf417--
 % --DESC: GS1 Composite 2D Component
 % --EXAM: (01)95012345678903(3103)000123
 % --EXOP: ccversion=b cccolumns=4
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp gs1-cc 0.0 2020122800 205183 207592
+%%BeginResource: uk.co.terryburton.bwipp gs1-cc 0.0 2021020600 208615 207592
 %%BeginData:        659 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /gs1lint dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
@@ -25687,15 +26153,15 @@
 
 % --BEGIN ENCODER ean13composite--
 % --REQUIRES preamble raiseerror parseinput gs1lint renlinear renmatrix ean5 ean2 ean13 micropdf417 pdf417 gs1-cc--
 % --DESC: EAN-13 Composite
 % --EXAM: 2112345678900|(99)1234-abcd
 % --EXOP: includetext
 % --RNDR: renlinear renmatrix
-%%BeginResource: uk.co.terryburton.bwipp ean13composite 0.0 2020122800 79583 86527
+%%BeginResource: uk.co.terryburton.bwipp ean13composite 0.0 2021020600 83015 86399
 %%BeginData:         74 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /ean13 dup /uk.co.terryburton.bwipp findresource put
 dup /gs1-cc dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
@@ -25773,15 +26239,15 @@
 
 % --BEGIN ENCODER ean8composite--
 % --REQUIRES preamble raiseerror parseinput gs1lint renlinear renmatrix ean5 ean2 ean8 micropdf417 pdf417 gs1-cc--
 % --DESC: EAN-8 Composite
 % --EXAM: 02345673|(21)A12345678
 % --EXOP: includetext
 % --RNDR: renlinear renmatrix
-%%BeginResource: uk.co.terryburton.bwipp ean8composite 0.0 2020122800 83484 86741
+%%BeginResource: uk.co.terryburton.bwipp ean8composite 0.0 2021020600 83356 86741
 %%BeginData:         77 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /ean8 dup /uk.co.terryburton.bwipp findresource put
 dup /gs1-cc dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
@@ -25862,15 +26328,15 @@
 
 % --BEGIN ENCODER upcacomposite--
 % --REQUIRES preamble raiseerror parseinput gs1lint renlinear renmatrix ean5 ean2 upca micropdf417 pdf417 gs1-cc--
 % --DESC: UPC-A Composite
 % --EXAM: 416000336108|(99)1234-abcd
 % --EXOP: includetext
 % --RNDR: renlinear renmatrix
-%%BeginResource: uk.co.terryburton.bwipp upcacomposite 0.0 2020122800 82993 82946
+%%BeginResource: uk.co.terryburton.bwipp upcacomposite 0.0 2021020600 79561 86378
 %%BeginData:         74 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 2 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /upca dup /uk.co.terryburton.bwipp findresource put
 dup /gs1-cc dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
@@ -25948,15 +26414,15 @@
 
 % --BEGIN ENCODER upcecomposite--
 % --REQUIRES preamble raiseerror parseinput gs1lint renlinear renmatrix ean5 ean2 upce micropdf417 pdf417 gs1-cc--
 % --DESC: UPC-E Composite
 % --EXAM: 00123457|(15)021231
 % --EXOP: includetext
 % --RNDR: renlinear renmatrix
-%%BeginResource: uk.co.terryburton.bwipp upcecomposite 0.0 2020122800 84275 87649
+%%BeginResource: uk.co.terryburton.bwipp upcecomposite 0.0 2021020600 84275 87649
 %%BeginData:         89 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 2 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /upce dup /uk.co.terryburton.bwipp findresource put
 dup /gs1-cc dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
@@ -26049,15 +26515,15 @@
 
 % --BEGIN ENCODER databaromnicomposite--
 % --REQUIRES preamble raiseerror parseinput gs1lint renlinear renmatrix databaromni micropdf417 pdf417 gs1-cc--
 % --DESC: GS1 DataBar Omnidirectional Composite
 % --EXAM: (01)03612345678904|(11)990102
 % --EXOP:
 % --RNDR: renlinear renmatrix
-%%BeginResource: uk.co.terryburton.bwipp databaromnicomposite 0.0 2020122800 87494 83950
+%%BeginResource: uk.co.terryburton.bwipp databaromnicomposite 0.0 2021020600 87598 83950
 %%BeginData:        102 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 2 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /databaromni dup /uk.co.terryburton.bwipp findresource put
 dup /gs1-cc dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
@@ -26163,15 +26629,15 @@
 
 % --BEGIN ENCODER databarstackedcomposite--
 % --REQUIRES preamble raiseerror parseinput gs1lint renlinear renmatrix databaromni databarstacked micropdf417 pdf417 gs1-cc--
 % --DESC: GS1 DataBar Stacked Composite
 % --EXAM: (01)03412345678900|(17)010200
 % --EXOP:
 % --RNDR: renlinear renmatrix
-%%BeginResource: uk.co.terryburton.bwipp databarstackedcomposite 0.0 2020122800 85882 89213
+%%BeginResource: uk.co.terryburton.bwipp databarstackedcomposite 0.0 2021020600 89442 89213
 %%BeginData:         98 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 2 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /databarstacked dup /uk.co.terryburton.bwipp findresource put
 dup /gs1-cc dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
@@ -26273,15 +26739,15 @@
 
 % --BEGIN ENCODER databarstackedomnicomposite--
 % --REQUIRES preamble raiseerror parseinput gs1lint renlinear renmatrix databaromni databarstackedomni micropdf417 pdf417 gs1-cc--
 % --DESC: GS1 DataBar Stacked Omnidirectional Composite
 % --EXAM: (01)03612345678904|(11)990102
 % --EXOP:
 % --RNDR: renlinear renmatrix
-%%BeginResource: uk.co.terryburton.bwipp databarstackedomnicomposite 0.0 2020122800 85910 89237
+%%BeginResource: uk.co.terryburton.bwipp databarstackedomnicomposite 0.0 2021020600 89470 89237
 %%BeginData:         98 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 2 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /databarstackedomni dup /uk.co.terryburton.bwipp findresource put
 dup /gs1-cc dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
@@ -26383,15 +26849,15 @@
 
 % --BEGIN ENCODER databartruncatedcomposite--
 % --REQUIRES preamble raiseerror parseinput gs1lint renlinear renmatrix databaromni databartruncated micropdf417 pdf417 gs1-cc--
 % --DESC: GS1 DataBar Truncated Composite
 % --EXAM: (01)03612345678904|(11)990102
 % --EXOP:
 % --RNDR: renlinear renmatrix
-%%BeginResource: uk.co.terryburton.bwipp databartruncatedcomposite 0.0 2020122800 86952 90267
+%%BeginResource: uk.co.terryburton.bwipp databartruncatedcomposite 0.0 2021020600 90512 90267
 %%BeginData:        102 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 2 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /databartruncated dup /uk.co.terryburton.bwipp findresource put
 dup /gs1-cc dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
@@ -26497,15 +26963,15 @@
 
 % --BEGIN ENCODER databarlimitedcomposite--
 % --REQUIRES preamble raiseerror parseinput gs1lint renlinear renmatrix databarlimited micropdf417 pdf417 gs1-cc--
 % --DESC: GS1 DataBar Limited Composite
 % --EXAM: (01)03512345678907|(21)abcdefghijklmnopqrstuv
 % --EXOP:
 % --RNDR: renlinear renmatrix
-%%BeginResource: uk.co.terryburton.bwipp databarlimitedcomposite 0.0 2020122800 83791 80260
+%%BeginResource: uk.co.terryburton.bwipp databarlimitedcomposite 0.0 2021020600 83919 80260
 %%BeginData:         81 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 2 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /databarlimited dup /uk.co.terryburton.bwipp findresource put
 dup /gs1-cc dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
@@ -26590,15 +27056,15 @@
 
 % --BEGIN ENCODER databarexpandedcomposite--
 % --REQUIRES preamble raiseerror parseinput gs1lint renlinear renmatrix databarexpanded micropdf417 pdf417 gs1-cc--
 % --DESC: GS1 DataBar Expanded Composite
 % --EXAM: (01)93712345678904(3103)001234|(91)1A2B3C4D5E
 % --EXOP:
 % --RNDR: renlinear renmatrix
-%%BeginResource: uk.co.terryburton.bwipp databarexpandedcomposite 0.0 2020122800 83389 83390
+%%BeginResource: uk.co.terryburton.bwipp databarexpandedcomposite 0.0 2021020600 83389 83262
 %%BeginData:        100 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 2 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /databarexpanded dup /uk.co.terryburton.bwipp findresource put
 dup /gs1-cc dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
@@ -26702,15 +27168,15 @@
 
 % --BEGIN ENCODER databarexpandedstackedcomposite--
 % --REQUIRES preamble raiseerror parseinput gs1lint renlinear renmatrix databarexpanded databarexpandedstacked micropdf417 pdf417 gs1-cc--
 % --DESC: GS1 DataBar Expanded Stacked Composite
 % --EXAM: (01)00012345678905(10)ABCDEF|(21)12345678
 % --EXOP: segments=4
 % --RNDR: renmatrix renlinear
-%%BeginResource: uk.co.terryburton.bwipp databarexpandedstackedcomposite 0.0 2020122800 85613 85493
+%%BeginResource: uk.co.terryburton.bwipp databarexpandedstackedcomposite 0.0 2021020600 89173 85493
 %%BeginData:         97 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 2 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /databarexpandedstacked dup /uk.co.terryburton.bwipp findresource put
 dup /gs1-cc dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
@@ -26811,15 +27277,15 @@
 
 % --BEGIN ENCODER gs1-128composite--
 % --REQUIRES preamble raiseerror parseinput gs1lint renlinear renmatrix code128 gs1-128 micropdf417 pdf417 gs1-cc--
 % --DESC: GS1-128 Composite
 % --EXAM: (00)030123456789012340|(02)13012345678909(37)24(10)1234567ABCDEFG
 % --EXOP: ccversion=c
 % --RNDR: renlinear renmatrix
-%%BeginResource: uk.co.terryburton.bwipp gs1-128composite 0.0 2020122800 86500 89809
+%%BeginResource: uk.co.terryburton.bwipp gs1-128composite 0.0 2021020600 90060 89809
 %%BeginData:        102 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 2 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /gs1-128 dup /uk.co.terryburton.bwipp findresource put
 dup /gs1-cc dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
@@ -26925,15 +27391,15 @@
 
 % --BEGIN ENCODER gs1datamatrix--
 % --REQUIRES preamble raiseerror parseinput gs1lint renmatrix datamatrix--
 % --DESC: GS1 Data Matrix
 % --EXAM: (01)03453120000011(17)120508(10)ABCD1234(410)9501101020917
 % --EXOP:
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp gs1datamatrix 0.0 2020122800 77808 77858
+%%BeginResource: uk.co.terryburton.bwipp gs1datamatrix 0.0 2021020600 77808 74426
 %%BeginData:        133 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /gs1lint dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
@@ -27070,15 +27536,15 @@
 
 % --BEGIN ENCODER gs1datamatrixrectangular--
 % --REQUIRES preamble raiseerror parseinput gs1lint renmatrix datamatrix--
 % --DESC: GS1 Data Matrix Rectangular
 % --EXAM: (01)03453120000011(17)120508(10)ABCD1234(410)9501101020917
 % --EXOP:
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp gs1datamatrixrectangular 0.0 2020122800 78011 78026
+%%BeginResource: uk.co.terryburton.bwipp gs1datamatrixrectangular 0.0 2021020600 78011 78026
 %%BeginData:        134 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /gs1lint dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
@@ -27216,15 +27682,15 @@
 
 % --BEGIN ENCODER gs1qrcode--
 % --REQUIRES preamble raiseerror parseinput gs1lint renmatrix qrcode--
 % --DESC: GS1 QR Code
 % --EXAM: (01)03453120000011(8200)http://www.abc.net(10)ABCD1234(410)9501101020917
 % --EXOP:
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp gs1qrcode 0.0 2020122800 77795 77814
+%%BeginResource: uk.co.terryburton.bwipp gs1qrcode 0.0 2021020600 81227 74382
 %%BeginData:        132 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /gs1lint dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 dup /qrcode dup /uk.co.terryburton.bwipp findresource put
@@ -27357,18 +27823,18 @@
 %%EndData
 %%EndResource
 % --END ENCODER gs1qrcode--
 
 % --BEGIN ENCODER gs1dotcode--
 % --REQUIRES preamble raiseerror parseinput gs1lint renmatrix dotcode--
 % --DESC: GS1 DotCode
-% --EXAM: (01)03453120000011(17)120508(10)ABCD1234(410)9501101020917
-% --EXOP:
+% --EXAM: (235)5vBZIF%!<B;?oa%(01)01234567890128(8008)19052001
+% --EXOP: rows=16
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp gs1dotcode 0.0 2020122800 81234 74387
+%%BeginResource: uk.co.terryburton.bwipp gs1dotcode 0.0 2021020600 77802 77819
 %%BeginData:        133 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /gs1lint dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
@@ -27505,15 +27971,15 @@
 
 % --BEGIN ENCODER hibccode39--
 % --REQUIRES preamble raiseerror renlinear code39--
 % --DESC: HIBC Code 39
 % --EXAM: A123BJC5D6E71
 % --EXOP: includetext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp hibccode39 0.0 2020122800 57669 60912
+%%BeginResource: uk.co.terryburton.bwipp hibccode39 0.0 2021020600 57669 61040
 %%BeginData:         94 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /code39 dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -27611,15 +28077,15 @@
 
 % --BEGIN ENCODER hibccode128--
 % --REQUIRES preamble raiseerror parseinput renlinear code128--
 % --DESC: HIBC Code 128
 % --EXAM: A123BJC5D6E71
 % --EXOP: includetext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp hibccode128 0.0 2020122800 63913 60296
+%%BeginResource: uk.co.terryburton.bwipp hibccode128 0.0 2021020600 63889 60320
 %%BeginData:         93 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /code128 dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -27716,15 +28182,15 @@
 
 % --BEGIN ENCODER hibcdatamatrix--
 % --REQUIRES preamble raiseerror parseinput renmatrix datamatrix--
 % --DESC: HIBC Data Matrix
 % --EXAM: A123BJC5D6E71
 % --EXOP:
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp hibcdatamatrix 0.0 2020122800 61356 57634
+%%BeginResource: uk.co.terryburton.bwipp hibcdatamatrix 0.0 2021020600 61356 57634
 %%BeginData:         76 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 dup /datamatrix dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -27804,15 +28270,15 @@
 
 % --BEGIN ENCODER hibcdatamatrixrectangular--
 % --REQUIRES preamble raiseerror parseinput renmatrix datamatrix--
 % --DESC: HIBC Data Matrix Rectangular
 % --EXAM: A123BJC5D6E71
 % --EXOP:
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp hibcdatamatrixrectangular 0.0 2020122800 61709 57954
+%%BeginResource: uk.co.terryburton.bwipp hibcdatamatrixrectangular 0.0 2021020600 61709 57954
 %%BeginData:         77 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 dup /datamatrix dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -27893,15 +28359,15 @@
 
 % --BEGIN ENCODER hibcpdf417--
 % --REQUIRES preamble raiseerror parseinput renmatrix pdf417--
 % --DESC: HIBC PDF417
 % --EXAM: A123BJC5D6E71
 % --EXOP:
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp hibcpdf417 0.0 2020122800 61867 58059
+%%BeginResource: uk.co.terryburton.bwipp hibcpdf417 0.0 2021020600 61739 58059
 %%BeginData:         80 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 dup /pdf417 dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -27985,15 +28451,15 @@
 
 % --BEGIN ENCODER hibcmicropdf417--
 % --REQUIRES preamble raiseerror parseinput renmatrix micropdf417--
 % --DESC: HIBC MicroPDF417
 % --EXAM: A123BJC5D6E71
 % --EXOP:
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp hibcmicropdf417 0.0 2020122800 61685 58118
+%%BeginResource: uk.co.terryburton.bwipp hibcmicropdf417 0.0 2021020600 61789 58094
 %%BeginData:         80 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 dup /micropdf417 dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -28077,15 +28543,15 @@
 
 % --BEGIN ENCODER hibcqrcode--
 % --REQUIRES preamble raiseerror parseinput renmatrix qrcode--
 % --DESC: HIBC QR Code
 % --EXAM: A123BJC5D6E71
 % --EXOP:
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp hibcqrcode 0.0 2020122800 65776 58524
+%%BeginResource: uk.co.terryburton.bwipp hibcqrcode 0.0 2021020600 62368 58652
 %%BeginData:         76 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 dup /qrcode dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -28165,15 +28631,15 @@
 
 % --BEGIN ENCODER hibccodablockf--
 % --REQUIRES preamble raiseerror parseinput renmatrix codablockf--
 % --DESC: HIBC Codablock F
 % --EXAM: A123BJC5D6E71
 % --EXOP:
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp hibccodablockf 0.0 2020122800 61336 57866
+%%BeginResource: uk.co.terryburton.bwipp hibccodablockf 0.0 2021020600 61336 57866
 %%BeginData:         76 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 dup /codablockf dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -28253,15 +28719,15 @@
 
 % --BEGIN ENCODER hibcazteccode--
 % --REQUIRES preamble raiseerror parseinput renmatrix azteccode--
 % --DESC: HIBC Aztec Code
 % --EXAM: A123BJC5D6E71
 % --EXOP:
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp hibcazteccode 0.0 2020122800 61330 57627
+%%BeginResource: uk.co.terryburton.bwipp hibcazteccode 0.0 2021020600 61330 57627
 %%BeginData:         76 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 dup /azteccode dup /uk.co.terryburton.bwipp findresource put
 begin
```

### Comparing `treepoem-3.8.0/src/treepoem/postscriptbarcode/barcode_with_sample.ps` & `treepoem-3.9.0/src/treepoem/postscriptbarcode/barcode_with_sample.ps`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 %!PS
 
-% Barcode Writer in Pure PostScript - Version 2020-12-28
+% Barcode Writer in Pure PostScript - Version 2021-02-06
 % https://bwipp.terryburton.co.uk
 %
-% Copyright (c) 2004-2019 Terry Burton
+% Copyright (c) 2004-2021 Terry Burton
 %
 % Permission is hereby granted, free of charge, to any
 % person obtaining a copy of this software and associated
 % documentation files (the "Software"), to deal in the
 % Software without restriction, including without
 % limitation the rights to use, copy, modify, merge,
 % publish, distribute, sublicense, and/or sell copies of
@@ -28,29 +28,29 @@
 % CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 % CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
 % IN THE SOFTWARE.
 
 % --BEGIN TEMPLATE--
 
 % --BEGIN RESOURCE preamble--
-%%BeginResource: Category uk.co.terryburton.bwipp 0.0 2020122800 29629 32838
+%%BeginResource: Category uk.co.terryburton.bwipp 0.0 2021020600 29629 32838
 %%BeginData:          6 ASCII Lines
 currentglobal
 true setglobal
 /Generic /Category findresource dup length 1 add dict copy dup
 /InstanceType /setpacking where {pop /packedarraytype} {/arraytype} ifelse put
 /uk.co.terryburton.bwipp exch /Category defineresource pop
 setglobal
 %%EndData
 %%EndResource
 % --END RESOURCE preamble--
 
 % --BEGIN RESOURCE raiseerror--
 % --REQUIRES preamble--
-%%BeginResource: uk.co.terryburton.bwipp raiseerror 0.0 2020122800 39041 38872
+%%BeginResource: uk.co.terryburton.bwipp raiseerror 0.0 2021020600 39041 38872
 %%BeginData:         15 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 begin
 /raiseerror {
   $error exch /errorinfo exch put
   $error exch /errorname exch put
@@ -65,15 +65,15 @@
 /setpacking where {pop setpacking} if
 %%EndData
 %%EndResource
 % --END RESOURCE raiseerror--
 
 % --BEGIN RESOURCE parseinput--
 % --REQUIRES preamble raiseerror--
-%%BeginResource: uk.co.terryburton.bwipp parseinput 0.0 2020122800 58305 58180
+%%BeginResource: uk.co.terryburton.bwipp parseinput 0.0 2021020600 58305 58204
 %%BeginData:        129 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 4 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 begin
 /parseinput {
 
@@ -202,16 +202,16 @@
 /setpacking where {pop setpacking} if
 %%EndData
 %%EndResource
 % --END RESOURCE parseinput--
 
 % --BEGIN RESOURCE gs1lint--
 % --REQUIRES preamble raiseerror--
-%%BeginResource: uk.co.terryburton.bwipp gs1lint 0.0 2020122800 247873 257453
-%%BeginData:       1235 ASCII Lines
+%%BeginResource: uk.co.terryburton.bwipp gs1lint 0.0 2021020600 360967 368615
+%%BeginData:       1674 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 2 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 begin
 /gs1lint {
 
     20 dict begin
@@ -264,28 +264,169 @@
         mark exch
         dup length 2 mod 0 eq {3} {1} ifelse
         exch { 48 sub 1 index mul exch 4 exch sub } forall pop
         0 counttomark 1 sub {add} repeat exch pop
         10 mod 0 ne { pop /bwipp.GS1badChecksum (Bad checksum) false exit } if
     } bind def
 
+    /cset82 <<
+        0 (!"%&'\(\)*+,-./0123456789:;<=>?ABCDEFGHIJKLMNOPQRSTUVWXYZ_abcdefghijklmnopqrstuvwxyz)
+        { exch dup 1 add } forall pop
+    >> def
+
+    /cset32 <<
+        0 (23456789ABCDEFGHJKLMNPQRSTUVWXYZ)
+        { exch dup 1 add } forall pop
+    >> def
+
+    /lintcsumalpha {
+        dup length 2 lt { pop pop /bwipp.GS1alphaTooShort (Alphanumeric string is too short to check) false exit} if
+        dup length 2 sub
+        2 copy
+        0 exch getinterval mark exch {
+            dup cset82 exch known { cset82 exch get } { -1 exit } ifelse
+        } forall
+        dup -1 eq { cleartomark pop pop pop /bwipp.GS1UnknownCSET82Character (Unknown CSET 82 character) false exit} if
+        counttomark array astore exch pop
+        3 1 roll
+        2 getinterval mark exch {
+            dup cset32 exch known { cset32 exch get } { -1 exit } ifelse
+        } forall
+        dup -1 eq { cleartomark pop pop /bwipp.GS1UnknownCSET32Character (Unknown CSET 32 character) false exit} if
+        counttomark array astore exch pop
+        dup 0 get 5 bitshift exch 1 get add exch
+        [ 2 3 5 7 11 13 17 19 23 29 31 37 41 43 47 53 59 61 67 71 73 79 83 ]
+        1 index length
+        dup 2 index length gt { pop pop pop pop pop /bwipp.GS1alphaTooLong (Alphanumeric string is too long to check) false exit} if
+        0 exch getinterval {exch} forall
+        0 exch { 3 -1 roll exch mul add } forall 1021 mod
+        ne { pop /bwipp.GS1badAlphaCheckCharacters (Bad alphanumeric check characters) false exit} if
+    } bind def
+
+    /iso3166 << [
+        /004 /008 /010 /012 /016 /020 /024 /028 /031 /032 /036 /040 /044 /048
+        /050 /051 /052 /056 /060 /064 /068 /070 /072 /074 /076 /084 /086 /090 /092 /096
+        /100 /104 /108 /112 /116 /120 /124 /132 /136 /140 /144 /148
+        /152 /156 /158 /162 /166 /170 /174 /175 /178 /180 /184 /188 /191 /192 /196
+        /203 /204 /208 /212 /214 /218 /222 /226 /231 /232 /233 /234 /238 /239 /242 /246 /248
+        /250 /254 /258 /260 /262 /266 /268 /270 /275 /276 /288 /292 /296
+        /300 /304 /308 /312 /316 /320 /324 /328 /332 /334 /336 /340 /344 /348
+        /352 /356 /360 /364 /368 /372 /376 /380 /384 /388 /392 /398
+        /400 /404 /408 /410 /414 /417 /418 /422 /426 /428 /430 /434 /438 /440 /442 /446
+        /450 /454 /458 /462 /466 /470 /474 /478 /480 /484 /492 /496 /498 /499
+        /500 /504 /508 /512 /516 /520 /524 /528 /531 /533 /534 /535 /540 /548
+        /554 /558 /562 /566 /570 /574 /578 /580 /581 /583 /584 /585 /586 /591 /598
+        /600 /604 /608 /612 /616 /620 /624 /626 /630 /634 /638 /642 /643 /646
+        /652 /654 /659 /660 /662 /663 /666 /670 /674 /678 /682 /686 /688 /690 /694
+        /702 /703 /704 /705 /706 /710 /716 /724 /728 /729 /732 /740 /744 /748
+        /752 /756 /760 /762 /764 /768 /772 /776 /780 /784 /788 /792 /795 /796 /798
+        /800 /804 /807 /818 /826 /831 /832 /833 /834 /840
+        /850 /854 /858 /860 /862 /876 /882 /887 /894
+    ] {dup} forall >> def
+
+    /lintiso3166 {
+        iso3166 exch known not { pop /bwipp.GS1UnknownCountry (Unknown country code) false exit } if
+    } bind def
+
+    /lintiso3166999 {
+        dup /999 ne {
+            iso3166 exch known not { pop /bwipp.GS1UnknownCountryOr999 (Unknown country code or not 999) false exit } if
+        } {
+            pop
+        } ifelse
+    } bind def
+
+    /lintiso3166list {
+        dup length 3 mod 0 ne {
+            pop pop /bwipp.GS1BadCountryListLength (Not a group of three-digit country codes) false exit
+        } if
+        true
+        0 3 3 index length 1 sub {
+            2 index exch 3 getinterval
+            iso3166 exch known not { pop pop false exit } if
+        } for
+        not { pop /bwipp.GS1UnknownCountry (Unknown country code) false exit } if
+        pop
+    } bind def
+
+    /iso3166alpha2 << [
+        /AD /AE /AF /AG /AI /AL /AM /AO /AQ /AR /AS /AT /AU /AW /AX /AZ
+        /BA /BB /BD /BE /BF /BG /BH /BI /BJ /BL /BM /BN /BO /BQ /BR /BS /BT /BV /BW /BY /BZ
+        /CA /CC /CD /CF /CG /CH /CI /CK /CL /CM /CN /CO /CR /CU /CV /CW /CX /CY /CZ
+        /DE /DJ /DK /DM /DO /DZ
+        /EC /EE /EG /EH /ER /ES /ET
+        /FI /FJ /FK /FM /FO /FR
+        /GA /GB /GD /GE /GF /GG /GH /GI /GL /GM /GN /GP /GQ /GR /GS /GT /GU /GW /GY
+        /HK /HM /HN /HR /HT /HU
+        /ID /IE /IL /IM /IN /IO /IQ /IR /IS /IT /JE /JM /JO /JP
+        /KE /KG /KH /KI /KM /KN /KP /KR /KW /KY /KZ
+        /LA /LB /LC /LI /LK /LR /LS /LT /LU /LV /LY
+        /MA /MC /MD /ME /MF /MG /MH /MK /ML /MM /MN /MO /MP /MQ /MR /MS /MT /MU /MV /MW /MX /MY /MZ
+        /NA /NC /NE /NF /NG /NI /NL /NO /NP /NR /NU /NZ
+        /OM
+        /PA /PE /PF /PG /PH /PK /PL /PM /PN /PR /PS /PT /PW /PY
+        /QA
+        /RE /RO /RS /RU /RW
+        /SA /SB /SC /SD /SE /SG /SH /SI /SJ /SK /SL /SM /SN /SO /SR /SS /ST /SV /SX /SY /SZ
+        /TC /TD /TF /TG /TH /TJ /TK /TL /TM /TN /TO /TR /TT /TV /TW /TZ
+        /UA /UG /UM /US /UY /UZ
+        /VA /VC /VE /VG /VI /VN /VU
+        /WF /WS
+        /YE /YT
+        /ZA /ZM /ZW
+    ] {dup} forall >> def
+
+    /lintiso3166alpha2 {
+        iso3166alpha2 exch known not { pop /bwipp.GS1UnknownCountryAlpha (Unknown country alpha code) false exit } if
+    } bind def
+
+    /iso4217 << [
+        /008 /012 /032 /036 /044 /048
+        /050 /051 /052 /060 /064 /068 /072 /084 /090 /096
+        /104 /108 /116 /124 /132 /136 /144
+        /152 /156 /170 /174 /188 /191 /192
+        /203 /208 /214 /222 /230 /232 /238 /242 /262 /270 /292
+        /320 /324 /328 /332 /340 /344 /348
+        /352 /356 /360 /364 /368 /376 /388 /392 /398
+        /400 /404 /408 /410 /414 /417 /418
+        /422 /426 /430 /434 /446
+        /454 /458 /462 /480 /484 /496 /498
+        /504 /512 /516 /524 /532 /533 /548
+        /554 /558 /566 /578 /586 /590 /598
+        /600 /604 /608 /634 /643 /646 /654 /682 /690 /694
+        /702 /704 /706 /710 /728 /748
+        /752 /756 /760 /764 /776 /780 /784 /788
+        /800 /807 /818 /826 /834 /840 /858 /860 /882 /886
+        /901 /927 /928 /929 /930 /931 /932 /933 /934 /936 /938
+        /940 /941 /943 /944 /946 /947 /948 /949
+        /950 /951 /952 /953 /955 /956 /957 /958 /959
+        /960 /961 /962 /963 /964 /965 /967 /968 /969
+        /970 /971 /972 /973 /975 /976 /977 /978 /979
+        /980 /981 /984 /985 /986 /990 /994 /997 /999
+    ] {dup} forall >> def
+
+    /lintiso4217 {
+        iso4217 exch known not { pop /bwipp.GS1UnknownCurrency (Unknown currency code) false exit } if
+    } bind def
+
     /lintiban {
         dup length 4 lt { pop pop /bwipp.GS1tooShort (IBAN too short) false exit } if
         dup true exch {
             1 string dup 0 4 -1 roll put
             (0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZ)
             exch search not { pop pop false exit } if
             pop pop pop
         } forall
         not { pop /bwipp.GS1badIBANcharacter (Invalid IBAN character) false exit } if
-        mark exch mark exch {} forall counttomark -4 roll counttomark array astore exch pop {
+        dup mark exch mark exch {} forall counttomark -4 roll counttomark array astore exch pop {
             48 sub dup 9 gt {7 sub dup 10 idiv exch 10 mod} if
         } forall counttomark array astore exch pop
         0 exch {exch 10 mul add 97 mod} forall
-        1 ne { pop /bwipp.GS1badIBANchecksum (IBAN checksum incorrect) false exit } if
+        1 ne { pop pop /bwipp.GS1badIBANchecksum (IBAN checksum incorrect) false exit } if
+        0 2 getinterval lintiso3166alpha2
     } bind def
 
     /lintzero {
         (0) ne { pop /bwipp.GS1zeroRequired (Zero is required) false exit } if
     } bind def
 
     /lintnonzero {
@@ -311,29 +452,32 @@
 
     /lintyymmdd {
         dup length 6 ne { pop /bwipp.GS1badDateLength (Invalid length for date) false exit } if
         dup 4 2 getinterval cvi 1 lt { pop /bwipp.GS1badDay (Invalid day of month) false exit } if
         lintyymmd0
     } bind def
 
+    /lintyymmddhh {
+        dup length 8 ne { pop /bwipp.GS1badYYMMDDHHLength (Invalid length for date with hour) false exit } if
+        dup 6 2 getinterval cvi 23 gt { pop pop /bwipp.GS1badHour (Invalid hour of day) false exit } if
+        0 6 getinterval lintyymmdd
+    } bind def
+
     /linthhmm {
         dup 0 2 getinterval cvi 23 gt { pop pop /bwipp.GS1badHour (Invalid hour of day) false exit } if
         2 2 getinterval cvi 59 gt { pop /bwipp.GS1badMinute (Invalid minute in the hour) false exit } if
     } bind def
 
-    /linthhoptmmss {
-        dup length dup 2 ne exch dup 4 ne exch 6 ne and and {
-            pop /bwipp.GS1badTimeLength (Invalid length for time of day with optional mins and secs) false exit
+    /lintmmoptss {
+        dup length dup 2 ne exch 4 ne and {
+            pop /bwipp.GS1badTimeLength (Invalid length for optional minutes and seconds) false exit
         } if
-        dup 0 2 getinterval cvi 23 gt { pop pop /bwipp.GS1badHour (Invalid hour of day) false exit } if
+        dup 0 2 getinterval cvi 59 gt { pop pop /bwipp.GS1badMinute (Invalid minute in the hour) false exit } if
         dup length 4 ge {
-            dup 2 2 getinterval cvi 59 gt { pop pop /bwipp.GS1badMinute (Invalid minute in the hour) false exit } if
-        } if
-        dup length 6 ge {
-            dup 4 2 getinterval cvi 59 gt { pop pop /bwipp.GS1badSecond (Invalid second in the minute) false exit } if
+            dup 2 2 getinterval cvi 59 gt { pop pop /bwipp.GS1badSecond (Invalid second in the minute) false exit } if
         } if
         pop
     } bind def
 
     /lintyesno {
         dup (0) ne exch (1) ne and {
             pop /bwipp.GS1badBoolean (Neither 0 nor 1 for yes or no) false exit
@@ -365,57 +509,352 @@
                 exch search not { pop pop false exit } if
                 pop pop pop
             } forall
             not { pop pop /bwipp.GS1badPercentChars (Invalid characters for percent encoding) false exit } if
         } loop
     } bind def
 
-    /lintcouponcode {  % TODO
-        pop
-    } bind def
+    /lintcouponcode {
+        dup true exch {
+            dup 48 lt exch 57 gt or { pop false exit } if
+        } forall
+        not { pop pop /bwipp.GS1couponNotNumeric (Coupon not numeric) false exit } if
 
-    /lintcouponposoffer {  % TODO
-        pop
-    } bind def
+        % GCP VLI and value
+        dup length 1 lt {
+            pop pop /bwipp.GS1couponTooShortGCPVLI (Coupon too short: Missing GCP VLI) false exit
+        } if
+        dup 0 1 getinterval cvi dup 6 gt {
+            pop pop /bwipp.GS1couponBadGCPVLI (Coupon GCP length indicator must be 0-6) false exit
+        } if
+        6 add 1 add
+        2 copy exch length gt {
+            pop pop pop /bwipp.GS1couponTooShortGCP (Coupon too short: GCP truncated) false exit
+        } if
+        dup 2 index length exch sub getinterval
 
-    /isocc << [
-        /004 /008 /010 /012 /016 /020 /024 /028 /031 /032 /036 /040 /044 /048
-        /050 /051 /052 /056 /060 /064 /068 /070 /072 /074 /076 /084 /086 /090 /092 /096
-        /100 /104 /108 /112 /116 /120 /124 /132 /136 /140 /144 /148
-        /152 /156 /158 /162 /166 /170 /174 /175 /178 /180 /184 /188 /191 /192 /196
-        /203 /204 /208 /212 /214 /218 /222 /226 /231 /232 /233 /234 /238 /239 /242 /246 /248
-        /250 /254 /258 /260 /262 /266 /268 /270 /275 /276 /288 /292 /296
-        /300 /304 /308 /312 /316 /320 /324 /328 /332 /334 /336 /340 /344 /348
-        /352 /356 /360 /364 /368 /372 /376 /380 /384 /388 /392 /398
-        /400 /404 /408 /410 /414 /417 /418 /422 /426 /428 /430 /434 /438 /440 /442 /446
-        /450 /454 /458 /462 /466 /470 /474 /478 /480 /484 /492 /496 /498 /499
-        /500 /504 /508 /512 /516 /520 /524 /528 /531 /533 /534 /535 /540 /548
-        /554 /558 /562 /566 /570 /574 /578 /580 /581 /583 /584 /585 /586 /591 /598
-        /600 /604 /608 /612 /616 /620 /624 /626 /630 /634 /638 /642 /643 /646
-        /652 /654 /659 /660 /662 /663 /666 /670 /674 /678 /682 /686 /688 /690 /694
-        /702 /703 /704 /705 /706 /710 /716 /724 /728 /729 /732 /740 /744 /748
-        /752 /756 /760 /762 /764 /768 /772 /776 /780 /784 /788 /792 /795 /796 /798
-        /800 /804 /807 /818 /826 /831 /832 /833 /834 /840
-        /850 /854 /858 /860 /862 /876 /882 /887 /894
-    ] {dup} forall >> def
+        % Offer Code
+        dup length 6 lt {
+            pop pop /bwipp.GS1couponTooShortOfferCode (Coupon too short: Offer Code truncated) false exit
+        } if
+        dup length 6 sub 6 exch getinterval
+
+        % Save Value VLI and value
+        dup length 1 lt {
+            pop pop /bwipp.GS1couponTooShortSaveValueVLI (Coupon too short: Missing Save Value VLI) false exit
+        } if
+        dup 0 1 getinterval cvi dup dup 1 lt exch 5 gt or {
+            pop pop /bwipp.GS1couponBadSaveValueVLI (Coupon Save Value length indicator must be 1-5) false exit
+        } if
+        1 add
+        2 copy exch length gt {
+            pop pop pop /bwipp.GS1couponTooShortSaveValue (Coupon too short: Save Value truncated) false exit
+        } if
+        dup 2 index length exch sub getinterval
+
+        % 1st Purchase Requirement VLI and value
+        dup length 1 lt {
+            pop pop /bwipp.GS1couponTooShort1stPurchaseRequirementVLI (Coupon too short: Missing 1st Purchase Requirement VLI) false exit
+        } if
+        dup 0 1 getinterval cvi dup dup 1 lt exch 5 gt or {
+            pop pop /bwipp.GS1couponBad1stPurchaseRequirementVLI (Coupon 1st Purchase Requirement length indicator must be 1-5) false exit
+        } if
+        1 add
+        2 copy exch length gt {
+            pop pop pop /bwipp.GS1couponTooShort1stPurchaseRequirement (Coupon too short: 1st Purchase Requirement truncated) false exit
+        } if
+        dup 2 index length exch sub getinterval
+
+        % 1st Purchase Requirement Code
+        dup length 1 lt {
+            pop pop /bwipp.GS1couponTooShort1stPurchaseRequirementCode (Coupon too short: Missing 1st Purchase Requirement Code) false exit
+        } if
+        dup 0 1 getinterval cvi dup 4 gt exch 9 ne and {
+            pop pop /bwipp.GS1couponBad1stPurchaseRequirementCode (Coupon 1st Purchase Requirement Code must be 0-4 or 9) false exit
+        } if
+        dup length 1 sub 1 exch getinterval
+
+        % 1st Purchase Family Code
+        dup length 3 lt {
+            pop pop /bwipp.GS1couponTooShort1stPurchaseFamilyCode (Coupon too short: 1st Purchase Family Code truncated) false exit
+        } if
+        dup length 3 sub 3 exch getinterval
+
+        % Optional field 1
+        dup length 1 ge { dup 0 1 getinterval cvi 1 eq {
+            1 dup 2 index length exch sub getinterval
+
+            % Additional Purchase Rules Code
+            dup length 1 lt {
+                pop pop /bwipp.GS1couponTooShortAdditionalPurchaseRulesCode (Coupon too short: Missing Additional Purchase Rules Code) false exit
+            } if
+            dup 0 1 getinterval cvi 3 gt {
+                pop pop /bwipp.GS1couponBadAdditionalPurchaseRulesCode (Coupon Additional Purchase Rules Code must be 0-3) false exit
+            } if
+            dup length 1 sub 1 exch getinterval
+
+            % 2nd Purchase RequirementVLI and value
+            dup length 1 lt {
+                pop pop /bwipp.GS1couponTooShort2ndPurchaseRequirementVLI (Coupon too short: Missing 2nd Purchase Requirement VLI) false exit
+            } if
+            dup 0 1 getinterval cvi dup dup 1 lt exch 5 gt or {
+                pop pop /bwipp.GS1couponBad2ndPurchaseRequirementVLI (Coupon 2nd Purchase Requirement length indicator must be 1-5) false exit
+            } if
+            1 add
+            2 copy exch length gt {
+                pop pop pop /bwipp.GS1couponTooShort2ndPurchaseRequirement (Coupon too short: 2nd Purchase Requirement truncated) false exit
+            } if
+            dup 2 index length exch sub getinterval
+
+            % 2nd Purchase Requirement Code
+            dup length 1 lt {
+                pop pop /bwipp.GS1couponTooShort2ndPurchaseRequirementCode (Coupon too short: Missing 2nd Purchase Requirement Code) false exit
+            } if
+            dup 0 1 getinterval cvi dup 4 gt exch 9 ne and {
+                pop pop /bwipp.GS1couponBad2ndPurchaseRequirementCode (Coupon 2nd Purchase Requirement Code must be 0-4 or 9) false exit
+            } if
+            dup length 1 sub 1 exch getinterval
+
+            % 2nd Purchase Family Code
+            dup length 3 lt {
+                pop pop /bwipp.GS1couponTooShort2ndPurchaseFamilyCode (Coupon too short: 2nd Purchase Family Code truncated) false exit
+            } if
+            dup length 3 sub 3 exch getinterval
+
+            % 2nd Purchase GCP VLI and value
+            dup length 1 lt {
+                pop pop /bwipp.GS1couponTooShort2ndPurchaseGCPVLI (Coupon too short: Missing 2nd Purchase GCP VLI) false exit
+            } if
+            dup 0 1 getinterval cvi dup dup 6 gt exch 9 ne and {
+                pop pop /bwipp.GS1couponBad2ndPurchaseGCPVLI (Coupon 2nd Purchase GCP length indicator must be 0-6 or 9) false exit
+            } if
+            dup 9 ne {6 add} {pop 0} ifelse 1 add
+            2 copy exch length gt {
+                pop pop pop /bwipp.GS1couponTooShort2ndPurchaseGCP (Coupon too short: 2nd Purchase GCP truncated) false exit
+            } if
+            dup 2 index length exch sub getinterval
+
+        } if } if
+
+        % Optional field 2
+        dup length 1 ge { dup 0 1 getinterval cvi 2 eq {
+            1 dup 2 index length exch sub getinterval
+
+            % 3rd Purchase RequirementVLI and value
+            dup length 1 lt {
+                pop pop /bwipp.GS1couponTooShort3rdPurchaseRequirementVLI (Coupon too short: Missing 3rd Purchase Requirement VLI) false exit
+            } if
+            dup 0 1 getinterval cvi dup dup 1 lt exch 5 gt or {
+                pop pop /bwipp.GS1couponBad3rdPurchaseRequirementVLI (Coupon 3rd Purchase Requirement length indicator must be 1-5) false exit
+            } if
+            1 add
+            2 copy exch length gt {
+                pop pop pop /bwipp.GS1couponTooShort3rdPurchaseRequirement (Coupon too short: 3rd Purchase Requirement truncated) false exit
+            } if
+            dup 2 index length exch sub getinterval
+
+            % 3rd Purchase Requirement Code
+            dup length 1 lt {
+                pop pop /bwipp.GS1couponTooShort3rdPurchaseRequirementCode (Coupon too short: Missing 3rd Purchase Requirement Code) false exit
+            } if
+            dup 0 1 getinterval cvi dup 4 gt exch 9 ne and {
+                pop pop /bwipp.GS1couponBad3rdPurchaseRequirementCode (Coupon 3rd Purchase Requirement Code must be 0-4 or 9) false exit
+            } if
+            dup length 1 sub 1 exch getinterval
+
+            % 3rd Purchase Family Code
+            dup length 3 lt {
+                pop pop /bwipp.GS1couponTooShort3rdPurchaseFamilyCode (Coupon too short: 3rd Purchase Family Code truncated) false exit
+            } if
+            dup length 3 sub 3 exch getinterval
+
+            % 3rd Purchase GCP VLI and value
+            dup length 1 lt {
+                pop pop /bwipp.GS1couponTooShort3rdPurchaseGCPVLI (Coupon too short: Missing 3rd Purchase GCP VLI) false exit
+            } if
+            dup 0 1 getinterval cvi dup dup 6 gt exch 9 ne and {
+                pop pop /bwipp.GS1couponBad3rdPurchaseGCPVLI (Coupon 3rd Purchase GCP length indicator must be 0-6 or 9) false exit
+            } if
+            dup 9 ne {6 add} {pop 0} ifelse 1 add
+            2 copy exch length gt {
+                pop pop pop /bwipp.GS1couponTooShort3rdPurchaseGCP (Coupon too short: 3rd Purchase GCP truncated) false exit
+            } if
+            dup 2 index length exch sub getinterval
+
+        } if } if
+
+        % Optional field 3
+        /couponexpire -1 def
+        dup length 1 ge { dup 0 1 getinterval cvi 3 eq {
+            1 dup 2 index length exch sub getinterval
+
+            % Expiration date
+            dup length 6 lt {
+                pop pop /bwipp.GS1couponTooShortExpirationDate (Coupon too short: Expiration date) false exit
+            } if
+            dup 2 2 getinterval cvi dup 1 lt exch 12 gt or { pop pop /bwipp.GS1couponExpirationDateBadMonth (Invalid month in expiration date) false exit } if
+            dup 0 2 getinterval cvi dup 21 sub  % Update 20YY periodically for century calculation
+            dup 51 ge {pop 1900 add} { -50 le {2100 add} {2000 add} ifelse} ifelse  % YYYY
+            dup 400 mod 0 eq exch dup 4 mod 0 eq exch 100 mod 0 ne and or           % Leap year?
+            [ 31  3 -1 roll {29} {28} ifelse  31 30 31 30 31 31 30 31 30 31 ]
+            1 index 2 2 getinterval cvi 1 sub get
+            1 index 4 2 getinterval cvi dup 3 1 roll lt
+            exch 1 lt or { pop pop /bwipp.GS1couponExpirationDateBadDay (Invalid day of month in expiration date) false exit } if
+            dup 0 6 getinterval cvi /couponexpire exch def
+            dup length 6 sub 6 exch getinterval
+
+        } if } if
+
+        % Optional field 4
+        dup length 1 ge { dup 0 1 getinterval cvi 4 eq {
+            1 dup 2 index length exch sub getinterval
+
+            % Start date
+            dup length 6 lt {
+                pop pop /bwipp.GS1couponTooShortStartDate (Coupon too short: Start date) false exit
+            } if
+            dup 2 2 getinterval cvi dup 1 lt exch 12 gt or { pop pop /bwipp.GS1couponStartDateBadMonth (Invalid month in start date) false exit } if
+            dup 0 2 getinterval cvi dup 21 sub  % Update 20YY periodically for century calculation
+            dup 51 ge {pop 1900 add} { -50 le {2100 add} {2000 add} ifelse} ifelse  % YYYY
+            dup 400 mod 0 eq exch dup 4 mod 0 eq exch 100 mod 0 ne and or           % Leap year?
+            [ 31  3 -1 roll {29} {28} ifelse  31 30 31 30 31 31 30 31 30 31 ]
+            1 index 2 2 getinterval cvi 1 sub get
+            1 index 4 2 getinterval cvi dup 3 1 roll lt
+            exch 1 lt or { pop pop /bwipp.GS1couponStartDateBadDay (Invalid day of month in start date) false exit } if
+            dup 0 6 getinterval cvi /couponstart exch def
+            couponexpire -1 ne couponexpire couponstart lt and {
+                pop pop /bwipp.GS1couponExpireDateBeforeStartDate (Coupon expires before it starts) false exit
+            } if
+            dup length 6 sub 6 exch getinterval
+
+        } if } if
+
+        % Optional field 5
+        dup length 1 ge { dup 0 1 getinterval cvi 5 eq {
+            1 dup 2 index length exch sub getinterval
+
+            % Serial Number VLI and value
+            dup length 1 lt {
+                pop pop /bwipp.GS1couponTooShortSerialNumberVLI (Coupon too short: Missing Serial Number VLI) false exit
+            } if
+            dup 0 1 getinterval cvi 6 add 1 add
+            2 copy exch length gt {
+                pop pop pop /bwipp.GS1couponTooShortSerialNumber (Coupon too short: Serial Number truncated) false exit
+            } if
+            dup 2 index length exch sub getinterval
+
+        } if } if
+
+        % Optional field 6
+        dup length 1 ge { dup 0 1 getinterval cvi 6 eq {
+            1 dup 2 index length exch sub getinterval
+
+            % Retailer GCP/GLN VLI and value
+            dup length 1 lt {
+                pop pop /bwipp.GS1couponTooShortRetailerGCPGLNVLI (Coupon too short: Missing Retailer GCP/GLN VLI) false exit
+            } if
+            dup 0 1 getinterval cvi dup dup 1 lt exch 7 gt or {
+                pop pop /bwipp.GS1couponBadRetailerGCPGLNVLI (Coupon Retailer GCP/GLN length indicator must be 1-7) false exit
+            } if
+            6 add 1 add
+            2 copy exch length gt {
+                pop pop pop /bwipp.GS1couponTooShortRetailerGCPGLN (Coupon too short: Retailer GCP/GLN truncated) false exit
+            } if
+            dup 2 index length exch sub getinterval
+
+        } if } if
+
+        % Optional field 9
+        dup length 1 ge { dup 0 1 getinterval cvi 9 eq {
+            1 dup 2 index length exch sub getinterval
+
+            % Save Value Code
+            dup length 1 lt {
+                pop pop /bwipp.GS1couponTooShortSaveValueCode (Coupon too short: Missing Save Value Code) false exit
+            } if
+            dup 0 1 getinterval cvi dup 6 gt exch dup 3 eq exch 4 eq or or {
+                pop pop /bwipp.GS1couponBadSaveValueCode (Coupon Save Value Code must be 0,1,2,5 or 6) false exit
+            } if
+            dup length 1 sub 1 exch getinterval
+
+            % Save Value Applies to Item
+            dup length 1 lt {
+                pop pop /bwipp.GS1couponTooShortSaveValueAppliesToItem (Coupon too short: Missing Save Value Applies to Item) false exit
+            } if
+            dup 0 1 getinterval cvi 2 gt {
+                pop pop /bwipp.GS1couponBadSaveValueAppliesToItem (Coupon Save Value Applies to Item must be 0-2) false exit
+            } if
+            dup length 1 sub 1 exch getinterval
+
+            % Store Coupon Flag
+            dup length 1 lt {
+                pop pop /bwipp.GS1couponTooShortStoreCouponFlag (Coupon too short: Missing Store Coupon Flag) false exit
+            } if
+            dup length 1 sub 1 exch getinterval
+
+            % Don't Multiply Flag
+            dup length 1 lt {
+                pop pop /bwipp.GS1couponTooShortDontMultiplyFlag (Coupon too short: Missing Don't Multiply Flag) false exit
+            } if
+            dup 0 1 getinterval cvi 1 gt {
+                pop pop /bwipp.GS1couponBadDontMultiplyFlag (Don't Multiply Flag must be 0 or 1) false exit
+            } if
+            dup length 1 sub 1 exch getinterval
 
-    /lintisocc {
-        isocc exch known not { pop /bwipp.GS1UnknownCountry (Unknown country code) false exit } if
+        } if } if
+
+        dup length 0 ne {
+            pop pop /bwipp.GS1couponUnrecognisedOptionalField (Coupon fields must be 1,2,3,4,5,6 or 9, increasing order) false exit
+        } if
+        pop
     } bind def
 
-    /lintisocclist {
-        dup length 3 mod 0 ne {
-            pop pop /bwipp.GS1BadCountryListLength (Not a group of three-digit country codes) false exit
+    /lintcouponposoffer {
+        dup true exch {
+            dup 48 lt exch 57 gt or { pop false exit } if
+        } forall
+        not { pop pop /bwipp.GS1couponNotNumeric (Coupon not numeric) false exit } if
+        % Format Code
+        dup length 1 lt {
+            pop pop /bwipp.GS1couponTooShortFormatCode (Coupon too short: Missing Format Code) false exit
+        } if
+        dup 0 1 getinterval dup (0) ne exch (1) ne and {
+            pop pop /bwipp.GS1couponBadFormatCode (Coupon format must be 0 or 1) false exit
+        } if
+        dup length 1 sub 1 exch getinterval
+        % Funder ID VLI and Funder ID
+        dup length 1 lt {
+            pop pop /bwipp.GS1couponTooShortFunderVLI (Coupon too short: Missing Funder VLI) false exit
+        } if
+        dup 0 1 getinterval cvi dup 6 gt {
+            pop pop pop /bwipp.GS1couponBadFunderVLI (Coupon Funder length indicator must be 0-6) false exit
+        } if
+        6 add 1 add
+        2 copy exch length gt {
+            pop pop pop /bwipp.GS1couponTooShortFunder (Coupon too short: Truncated Funder ID) false exit
+        } if
+        dup 2 index length exch sub getinterval
+        % Offer Code
+        dup length 6 lt {
+            pop pop /bwipp.GS1couponTooShortOfferCode (Coupon too short: Truncated Offer Code) false exit
+        } if
+        dup length 6 sub 6 exch getinterval
+        % Serial Number VLI and Serial Number
+        dup length 1 lt {
+            pop pop /bwipp.GS1couponTooShortSnVLI (Coupon too short: Missing SN VLI) false exit
+        } if
+        dup 0 1 getinterval cvi
+        6 add 1 add
+        2 copy exch length gt {
+            pop pop pop /bwipp.GS1couponTooShortSn (Coupon too short: Truncated SN) false exit
+        } if
+        dup 2 index length exch sub getinterval
+        dup length 0 ne {
+            pop pop /bwipp.GS1couponTooLong (Coupon too long) false exit
         } if
-        true
-        0 3 3 index length 1 sub {
-            2 index exch 3 getinterval
-            isocc exch known not { pop pop false exit } if
-        } for
-        not { pop /bwipp.GS1UnknownCountry (Unknown country code) false exit } if
         pop
     } bind def
 
     /gs1syntax <<
 
         [
         << /cset /N  /min 18  /max 18  /check [ /lintcsum /lintkey ] >>
@@ -860,15 +1299,15 @@
         (3906) exch dup
         (3907) exch dup
         (3908) exch dup
         (3909) exch dup
         pop
 
         [
-        << /cset /N  /min  3  /max  3  /check [ /lintisocc ] >>
+        << /cset /N  /min  3  /max  3  /check [ /lintiso4217 ] >>
         << /cset /N  /min  1  /max 15  /check [] >>
         ]
         (3910) exch dup
         (3911) exch dup
         (3912) exch dup
         (3913) exch dup
         (3914) exch dup
@@ -891,15 +1330,15 @@
         (3926) exch dup
         (3927) exch dup
         (3928) exch dup
         (3929) exch dup
         pop
 
         [
-        << /cset /N  /min  3  /max  3  /check [ /lintisocc ] >>
+        << /cset /N  /min  3  /max  3  /check [ /lintiso4217 ] >>
         << /cset /N  /min  1  /max 15  /check [] >>
         ]
         (3930) exch dup
         (3931) exch dup
         (3932) exch dup
         (3933) exch dup
         (3934) exch dup
@@ -970,46 +1409,46 @@
         [
         << /cset /X  /min  1  /max 20  /check [] >>
         ]
         (420) exch dup
         pop
 
         [
-        << /cset /N  /min  3  /max  3  /check [ /lintisocc ] >>
+        << /cset /N  /min  3  /max  3  /check [ /lintiso3166 ] >>
         << /cset /X  /min  1  /max  9  /check [] >>
         ]
         (421) exch dup
         pop
 
         [
-        << /cset /N  /min  3  /max  3  /check [ /lintisocc ] >>
+        << /cset /N  /min  3  /max  3  /check [ /lintiso3166 ] >>
         ]
         (422) exch dup
         pop
 
         [
-        << /cset /N  /min  1  /max 15  /check [ /lintisocclist ] >>
+        << /cset /N  /min  1  /max 15  /check [ /lintiso3166list ] >>
         ]
         (423) exch dup
         pop
 
         [
-        << /cset /N  /min  3  /max  3  /check [ /lintisocc ] >>
+        << /cset /N  /min  3  /max  3  /check [ /lintiso3166 ] >>
         ]
         (424) exch dup
         pop
 
         [
-        << /cset /N  /min  1  /max 15  /check [ /lintisocclist ] >>
+        << /cset /N  /min  1  /max 15  /check [ /lintiso3166list ] >>
         ]
         (425) exch dup
         pop
 
         [
-        << /cset /N  /min  3  /max  3  /check [ /lintisocc ] >>
+        << /cset /N  /min  3  /max  3  /check [ /lintiso3166 ] >>
         ]
         (426) exch dup
         pop
 
         [
         << /cset /X  /min  1  /max  3  /check [] >>
         ]
@@ -1030,21 +1469,21 @@
         (4303) exch dup
         (4304) exch dup
         (4305) exch dup
         (4306) exch dup
         pop
 
         [
-        << /cset /X  /min  2  /max  2  /check [] >>
+        << /cset /X  /min  2  /max  2  /check [ /lintiso3166alpha2 ] >>
         ]
         (4307) exch dup
         pop
 
         [
-        << /cset /X  /min  1  /max 30  /check [ /lintpcenc ] >>
+        << /cset /X  /min  1  /max 30  /check [] >>
         ]
         (4308) exch dup
         pop
 
         [
         << /cset /X  /min  1  /max 35  /check [ /lintpcenc ] >>
         ]
@@ -1059,15 +1498,15 @@
         (4313) exch dup
         (4314) exch dup
         (4315) exch dup
         (4316) exch dup
         pop
 
         [
-        << /cset /X  /min  2  /max  2  /check [] >>
+        << /cset /X  /min  2  /max  2  /check [ /lintiso3166alpha2 ] >>
         ]
         (4317) exch dup
         pop
 
         [
         << /cset /X  /min  1  /max 20  /check [] >>
         ]
@@ -1181,15 +1620,15 @@
         [
         << /cset /X  /min  1  /max 30  /check [ /lintkey ] >>
         ]
         (7023) exch dup
         pop
 
         [
-        << /cset /N  /min  3  /max  3  /check [ /lintisocc ] >>
+        << /cset /N  /min  3  /max  3  /check [ /lintiso3166999 ] >>
         << /cset /X  /min  1  /max 27  /check [] >>
         ]
         (7030) exch dup
         (7031) exch dup
         (7032) exch dup
         (7033) exch dup
         (7034) exch dup
@@ -1287,16 +1726,16 @@
         [
         << /cset /X  /min  1  /max 34  /check [ /lintiban ] >>
         ]
         (8007) exch dup
         pop
 
         [
-        << /cset /N  /min  6  /max  6  /check [ /lintyymmdd ] >>
-        << /cset /N  /min  1  /max  6  /check [ /linthhoptmmss ] >>
+        << /cset /N  /min  8  /max  8  /check [ /lintyymmddhh ] >>
+        << /cset /N  /min  0  /max  4  /check [ /lintmmoptss ] >>
         ]
         (8008) exch dup
         pop
 
         [
         << /cset /X  /min  1  /max 50  /check [] >>
         ]
@@ -1318,15 +1757,15 @@
         [
         << /cset /X  /min  1  /max 20  /check [] >>
         ]
         (8012) exch dup
         pop
 
         [
-        << /cset /X  /min  1  /max 30  /check [ /lintkey ] >>
+        << /cset /X  /min  1  /max 25  /check [ /lintcsumalpha /lintkey ] >>
         ]
         (8013) exch dup
         pop
 
         [
         << /cset /N  /min 18  /max 18  /check [ /lintcsum ] >>
         ]
@@ -1445,15 +1884,15 @@
 /setpacking where {pop setpacking} if
 %%EndData
 %%EndResource
 % --END RESOURCE gs1lint--
 
 % --BEGIN RENDERER renlinear--
 % --REQUIRES preamble raiseerror--
-%%BeginResource: uk.co.terryburton.bwipp renlinear 0.0 2020122800 74728 73842
+%%BeginResource: uk.co.terryburton.bwipp renlinear 0.0 2021020600 74728 73842
 %%BeginData:        239 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 begin
 /renlinear {
 
@@ -1692,15 +2131,15 @@
 /setpacking where {pop setpacking} if
 %%EndData
 %%EndResource
 % --END RENDERER renlinear--
 
 % --BEGIN RENDERER renmatrix--
 % --REQUIRES preamble raiseerror--
-%%BeginResource: uk.co.terryburton.bwipp renmatrix 0.0 2020122800 90359 89573
+%%BeginResource: uk.co.terryburton.bwipp renmatrix 0.0 2021020600 90359 89573
 %%BeginData:        306 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 begin
 /renmatrix {
 
@@ -2006,15 +2445,15 @@
 /setpacking where {pop setpacking} if
 %%EndData
 %%EndResource
 % --END RENDERER renmatrix--
 
 % --BEGIN RENDERER renmaximatrix--
 % --REQUIRES preamble raiseerror--
-%%BeginResource: uk.co.terryburton.bwipp renmaximatrix 0.0 2020122800 50046 50044
+%%BeginResource: uk.co.terryburton.bwipp renmaximatrix 0.0 2021020600 50046 50044
 %%BeginData:         81 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 begin
 /renmaximatrix {
 
@@ -2099,15 +2538,15 @@
 
 % --BEGIN ENCODER ean5--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: EAN-5 (5 digit addon)
 % --EXAM: 90200
 % --EXOP: includetext guardwhitespace
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp ean5 0.0 2020122800 58142 57836
+%%BeginResource: uk.co.terryburton.bwipp ean5 0.0 2021020600 58118 57836
 %%BeginData:        137 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /ean5 {
@@ -2248,15 +2687,15 @@
 
 % --BEGIN ENCODER ean2--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: EAN-2 (2 digit addon)
 % --EXAM: 05
 % --EXOP: includetext guardwhitespace
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp ean2 0.0 2020122800 56723 56466
+%%BeginResource: uk.co.terryburton.bwipp ean2 0.0 2021020600 56699 56466
 %%BeginData:        122 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /ean2 {
@@ -2382,15 +2821,15 @@
 
 % --BEGIN ENCODER ean13--
 % --REQUIRES preamble raiseerror renlinear ean5 ean2--
 % --DESC: EAN-13
 % --EXAM: 2112345678900
 % --EXOP: includetext guardwhitespace
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp ean13 0.0 2020122800 81040 77231
+%%BeginResource: uk.co.terryburton.bwipp ean13 0.0 2021020600 80936 77207
 %%BeginData:        217 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /ean2 dup /uk.co.terryburton.bwipp findresource put
 dup /ean5 dup /uk.co.terryburton.bwipp findresource put
@@ -2611,15 +3050,15 @@
 
 % --BEGIN ENCODER ean8--
 % --REQUIRES preamble raiseerror renlinear ean5 ean2--
 % --DESC: EAN-8
 % --EXAM: 02345673
 % --EXOP: includetext guardwhitespace
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp ean8 0.0 2020122800 78158 74434
+%%BeginResource: uk.co.terryburton.bwipp ean8 0.0 2021020600 78158 74434
 %%BeginData:        198 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /ean2 dup /uk.co.terryburton.bwipp findresource put
 dup /ean5 dup /uk.co.terryburton.bwipp findresource put
@@ -2821,15 +3260,15 @@
 
 % --BEGIN ENCODER upca--
 % --REQUIRES preamble raiseerror renlinear ean5 ean2--
 % --DESC: UPC-A
 % --EXAM: 416000336108
 % --EXOP: includetext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp upca 0.0 2020122800 85897 81982
+%%BeginResource: uk.co.terryburton.bwipp upca 0.0 2021020600 86001 81982
 %%BeginData:        250 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /ean2 dup /uk.co.terryburton.bwipp findresource put
 dup /ean5 dup /uk.co.terryburton.bwipp findresource put
@@ -3083,15 +3522,15 @@
 
 % --BEGIN ENCODER upce--
 % --REQUIRES preamble raiseerror renlinear ean5 ean2--
 % --DESC: UPC-E
 % --EXAM: 00123457
 % --EXOP: includetext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp upce 0.0 2020122800 90606 86630
+%%BeginResource: uk.co.terryburton.bwipp upce 0.0 2021020600 90606 86630
 %%BeginData:        289 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /ean2 dup /uk.co.terryburton.bwipp findresource put
 dup /ean5 dup /uk.co.terryburton.bwipp findresource put
@@ -3384,15 +3823,15 @@
 
 % --BEGIN ENCODER isbn--
 % --REQUIRES preamble raiseerror renlinear ean5 ean2 ean13--
 % --DESC: ISBN
 % --EXAM: 978-1-56581-231-4 90000
 % --EXOP: includetext guardwhitespace
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp isbn 0.0 2020122800 86046 88625
+%%BeginResource: uk.co.terryburton.bwipp isbn 0.0 2021020600 86022 88625
 %%BeginData:        254 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /ean13 dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -3650,15 +4089,15 @@
 
 % --BEGIN ENCODER ismn--
 % --REQUIRES preamble raiseerror renlinear ean5 ean2 ean13--
 % --DESC: ISMN
 % --EXAM: 979-0-2605-3211-3
 % --EXOP: includetext guardwhitespace
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp ismn 0.0 2020122800 82722 85314
+%%BeginResource: uk.co.terryburton.bwipp ismn 0.0 2021020600 82594 85418
 %%BeginData:        233 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /ean13 dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -3895,15 +4334,15 @@
 
 % --BEGIN ENCODER issn--
 % --REQUIRES preamble raiseerror renlinear ean2 ean5 ean13--
 % --DESC: ISSN
 % --EXAM: 0311-175X 00 17
 % --EXOP: includetext guardwhitespace
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp issn 0.0 2020122800 74050 77078
+%%BeginResource: uk.co.terryburton.bwipp issn 0.0 2021020600 74026 77078
 %%BeginData:        178 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /ean13 dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -4085,15 +4524,15 @@
 
 % --BEGIN ENCODER code128--
 % --REQUIRES preamble raiseerror parseinput renlinear--
 % --DESC: Code 128
 % --EXAM: Count01234567!
 % --EXOP: includetext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp code128 0.0 2020122800 120207 123267
+%%BeginResource: uk.co.terryburton.bwipp code128 0.0 2021020600 120103 123035
 %%BeginData:        425 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -4522,15 +4961,15 @@
 
 % --BEGIN ENCODER gs1-128--
 % --REQUIRES preamble raiseerror parseinput gs1lint renlinear code128--
 % --DESC: GS1-128
 % --EXAM: (01)95012345678903(3103)000123
 % --EXOP: includetext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp gs1-128 0.0 2020122800 81217 81205
+%%BeginResource: uk.co.terryburton.bwipp gs1-128 0.0 2021020600 84649 81205
 %%BeginData:        156 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /gs1lint dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
@@ -4690,15 +5129,15 @@
 
 % --BEGIN ENCODER ean14--
 % --REQUIRES preamble raiseerror parseinput renlinear code128--
 % --DESC: GS1-14
 % --EXAM: (01) 0 46 01234 56789 3
 % --EXOP: includetext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp ean14 0.0 2020122800 66768 63140
+%%BeginResource: uk.co.terryburton.bwipp ean14 0.0 2021020600 66848 63140
 %%BeginData:        107 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /code128 dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -4809,15 +5248,15 @@
 
 % --BEGIN ENCODER sscc18--
 % --REQUIRES preamble raiseerror parseinput renlinear code128--
 % --DESC: SSCC-18
 % --EXAM: (00) 0 0614141 123456789 0
 % --EXOP: includetext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp sscc18 0.0 2020122800 66780 63147
+%%BeginResource: uk.co.terryburton.bwipp sscc18 0.0 2021020600 66860 63147
 %%BeginData:        107 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /code128 dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -4928,15 +5367,15 @@
 
 % --BEGIN ENCODER code39--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: Code 39
 % --EXAM: THIS IS CODE 39
 % --EXOP: includetext includecheck includecheckintext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp code39 0.0 2020122800 62946 62641
+%%BeginResource: uk.co.terryburton.bwipp code39 0.0 2021020600 62922 62513
 %%BeginData:        143 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /code39 {
@@ -5083,15 +5522,15 @@
 
 % --BEGIN ENCODER code39ext--
 % --REQUIRES preamble raiseerror parseinput renlinear code39--
 % --DESC: Code 39 Extended
 % --EXAM: Code39 Ext!
 % --EXOP: includetext includecheck includecheckintext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp code39ext 0.0 2020122800 65099 61411
+%%BeginResource: uk.co.terryburton.bwipp code39ext 0.0 2021020600 65075 61411
 %%BeginData:        100 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /code39 dup /uk.co.terryburton.bwipp findresource put
@@ -5195,15 +5634,15 @@
 
 % --BEGIN ENCODER code32--
 % --REQUIRES preamble raiseerror renlinear code39--
 % --DESC: Italian Pharmacode
 % --EXAM: 01234567
 % --EXOP: includetext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp code32 0.0 2020122800 58289 61504
+%%BeginResource: uk.co.terryburton.bwipp code32 0.0 2021020600 58289 61504
 %%BeginData:        101 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /code39 dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -5308,15 +5747,15 @@
 
 % --BEGIN ENCODER pzn--
 % --REQUIRES preamble raiseerror renlinear code39--
 % --DESC: Pharmazentralnummer (PZN)
 % --EXAM: 123456
 % --EXOP: includetext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp pzn 0.0 2020122800 58384 61524
+%%BeginResource: uk.co.terryburton.bwipp pzn 0.0 2021020600 58384 61524
 %%BeginData:        102 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /code39 dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -5422,15 +5861,15 @@
 
 % --BEGIN ENCODER code93--
 % --REQUIRES preamble raiseerror parseinput renlinear--
 % --DESC: Code 93
 % --EXAM: THIS IS CODE 93
 % --EXOP: includetext includecheck
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp code93 0.0 2020122800 62124 65325
+%%BeginResource: uk.co.terryburton.bwipp code93 0.0 2021020600 62124 65325
 %%BeginData:        134 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -5568,15 +6007,15 @@
 
 % --BEGIN ENCODER code93ext--
 % --REQUIRES preamble raiseerror parseinput renlinear code93--
 % --DESC: Code 93 Extended
 % --EXAM: Code93 Ext!
 % --EXOP: includetext includecheck
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp code93ext 0.0 2020122800 65429 61772
+%%BeginResource: uk.co.terryburton.bwipp code93ext 0.0 2021020600 65429 61772
 %%BeginData:        104 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /code93 dup /uk.co.terryburton.bwipp findresource put
@@ -5684,15 +6123,15 @@
 
 % --BEGIN ENCODER interleaved2of5--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: Interleaved 2 of 5 (ITF)
 % --EXAM: 2401234567
 % --EXOP: height=0.5 includecheck includetext includecheckintext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp interleaved2of5 0.0 2020122800 61533 61096
+%%BeginResource: uk.co.terryburton.bwipp interleaved2of5 0.0 2021020600 61405 61096
 %%BeginData:        152 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /interleaved2of5 {
@@ -5848,15 +6287,15 @@
 
 % --BEGIN ENCODER itf14--
 % --REQUIRES preamble raiseerror renlinear interleaved2of5--
 % --DESC: ITF-14
 % --EXAM: 0 46 01234 56789 3
 % --EXOP: includetext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp itf14 0.0 2020122800 60879 64093
+%%BeginResource: uk.co.terryburton.bwipp itf14 0.0 2021020600 60983 64117
 %%BeginData:        111 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /interleaved2of5 dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -5971,15 +6410,15 @@
 
 % --BEGIN ENCODER identcode--
 % --REQUIRES preamble raiseerror renlinear interleaved2of5--
 % --DESC: Deutsche Post Identcode
 % --EXAM: 563102430313
 % --EXOP: includetext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp identcode 0.0 2020122800 57310 60628
+%%BeginResource: uk.co.terryburton.bwipp identcode 0.0 2021020600 57310 60628
 %%BeginData:         93 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /interleaved2of5 dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -6076,15 +6515,15 @@
 
 % --BEGIN ENCODER leitcode--
 % --REQUIRES preamble raiseerror renlinear interleaved2of5--
 % --DESC: Deutsche Post Leitcode
 % --EXAM: 21348075016401
 % --EXOP: includetext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp leitcode 0.0 2020122800 57302 60624
+%%BeginResource: uk.co.terryburton.bwipp leitcode 0.0 2021020600 57302 60624
 %%BeginData:         93 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /interleaved2of5 dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -6181,15 +6620,15 @@
 
 % --BEGIN ENCODER databaromni--
 % --REQUIRES preamble raiseerror renlinear renmatrix--
 % --DESC: GS1 DataBar Omnidirectional
 % --EXAM: (01)24012345678905
 % --EXOP:
 % --RNDR: renlinear renmatrix
-%%BeginResource: uk.co.terryburton.bwipp databaromni 0.0 2020122800 105701 108053
+%%BeginResource: uk.co.terryburton.bwipp databaromni 0.0 2021020600 105701 108261
 %%BeginData:        425 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -6618,15 +7057,15 @@
 
 % --BEGIN ENCODER databarstacked--
 % --REQUIRES preamble raiseerror renlinear renmatrix databaromni--
 % --DESC: GS1 DataBar Stacked
 % --EXAM: (01)24012345678905
 % --EXOP:
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp databarstacked 0.0 2020122800 61648 57939
+%%BeginResource: uk.co.terryburton.bwipp databarstacked 0.0 2021020600 61520 58043
 %%BeginData:         75 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 dup /databaromni dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -6705,15 +7144,15 @@
 
 % --BEGIN ENCODER databarstackedomni--
 % --REQUIRES preamble raiseerror renlinear renmatrix databaromni--
 % --DESC: GS1 DataBar Stacked Omnidirectional
 % --EXAM: (01)24012345678905
 % --EXOP:
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp databarstackedomni 0.0 2020122800 61748 58019
+%%BeginResource: uk.co.terryburton.bwipp databarstackedomni 0.0 2021020600 61620 58123
 %%BeginData:         75 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 dup /databaromni dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -6792,15 +7231,15 @@
 
 % --BEGIN ENCODER databartruncated--
 % --REQUIRES preamble raiseerror renlinear renmatrix databaromni--
 % --DESC: GS1 DataBar Truncated
 % --EXAM: (01)24012345678905
 % --EXOP:
 % --RNDR: renlinear renmatrix
-%%BeginResource: uk.co.terryburton.bwipp databartruncated 0.0 2020122800 61674 57955
+%%BeginResource: uk.co.terryburton.bwipp databartruncated 0.0 2021020600 61546 58059
 %%BeginData:         75 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /databaromni dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -6879,15 +7318,15 @@
 
 % --BEGIN ENCODER databarlimited--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: GS1 DataBar Limited
 % --EXAM: (01)15012345678907
 % --EXOP:
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp databarlimited 0.0 2020122800 81204 80353
+%%BeginResource: uk.co.terryburton.bwipp databarlimited 0.0 2021020600 81076 80249
 %%BeginData:        278 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /databarlimited {
@@ -7169,15 +7608,15 @@
 
 % --BEGIN ENCODER databarexpanded--
 % --REQUIRES preamble raiseerror parseinput gs1lint renlinear renmatrix--
 % --DESC: GS1 DataBar Expanded
 % --EXAM: (01)95012345678903(3103)000123
 % --EXOP:
 % --RNDR: renlinear renmatrix
-%%BeginResource: uk.co.terryburton.bwipp databarexpanded 0.0 2020122800 242804 248423
+%%BeginResource: uk.co.terryburton.bwipp databarexpanded 0.0 2021020600 242700 244887
 %%BeginData:        886 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /gs1lint dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
@@ -8067,15 +8506,15 @@
 
 % --BEGIN ENCODER databarexpandedstacked--
 % --REQUIRES preamble raiseerror parseinput gs1lint renlinear renmatrix databarexpanded--
 % --DESC: GS1 DataBar Expanded Stacked
 % --EXAM: (01)95012345678903(3103)000123
 % --EXOP: segments=4
 % --RNDR: renlinear renmatrix
-%%BeginResource: uk.co.terryburton.bwipp databarexpandedstacked 0.0 2020122800 66639 66505
+%%BeginResource: uk.co.terryburton.bwipp databarexpandedstacked 0.0 2021020600 66639 63073
 %%BeginData:         45 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 dup /databarexpanded dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -8124,15 +8563,15 @@
 
 % --BEGIN ENCODER gs1northamericancoupon--
 % --REQUIRES preamble raiseerror parseinput gs1lint renlinear renmatrix databarexpanded databarexpandedstacked--
 % --DESC: GS1 North American Coupon
 % --EXAM: (8110)106141416543213500110000310123196000
 % --EXOP: includetext segments=8
 % --RNDR: renlinear renmatrix
-%%BeginResource: uk.co.terryburton.bwipp gs1northamericancoupon 0.0 2020122800 82792 85943
+%%BeginResource: uk.co.terryburton.bwipp gs1northamericancoupon 0.0 2021020600 82792 82511
 %%BeginData:        131 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /gs1lint dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
@@ -8267,15 +8706,15 @@
 
 % --BEGIN ENCODER pharmacode--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: Pharmaceutical Binary Code
 % --EXAM: 117480
 % --EXOP: showborder
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp pharmacode 0.0 2020122800 55122 54752
+%%BeginResource: uk.co.terryburton.bwipp pharmacode 0.0 2021020600 54994 54752
 %%BeginData:         93 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /pharmacode {
@@ -8372,15 +8811,15 @@
 
 % --BEGIN ENCODER pharmacode2--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: Two-track Pharmacode
 % --EXAM: 117480
 % --EXOP: includetext showborder
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp pharmacode2 0.0 2020122800 55953 55610
+%%BeginResource: uk.co.terryburton.bwipp pharmacode2 0.0 2021020600 55929 55610
 %%BeginData:         98 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /pharmacode2 {
@@ -8482,15 +8921,15 @@
 
 % --BEGIN ENCODER code2of5--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: Code 25
 % --EXAM: 01234567
 % --EXOP: includetext includecheck includecheckintext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp code2of5 0.0 2020122800 63541 62953
+%%BeginResource: uk.co.terryburton.bwipp code2of5 0.0 2021020600 63389 62953
 %%BeginData:        153 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /code2of5 {
@@ -8647,15 +9086,15 @@
 
 % --BEGIN ENCODER industrial2of5--
 % --REQUIRES preamble raiseerror renlinear code2of5--
 % --DESC: Industrial 2 of 5
 % --EXAM: 01234567
 % --EXOP: includetext includecheck includecheckintext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp industrial2of5 0.0 2020122800 51614 55042
+%%BeginResource: uk.co.terryburton.bwipp industrial2of5 0.0 2021020600 51614 55042
 %%BeginData:         57 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /code2of5 dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -8716,15 +9155,15 @@
 
 % --BEGIN ENCODER iata2of5--
 % --REQUIRES preamble raiseerror renlinear code2of5--
 % --DESC: IATA 2 of 5
 % --EXAM: 01234567
 % --EXOP: includetext includecheck includecheckintext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp iata2of5 0.0 2020122800 51584 55018
+%%BeginResource: uk.co.terryburton.bwipp iata2of5 0.0 2021020600 51584 55018
 %%BeginData:         57 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /code2of5 dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -8785,15 +9224,15 @@
 
 % --BEGIN ENCODER matrix2of5--
 % --REQUIRES preamble raiseerror renlinear code2of5--
 % --DESC: Matrix 2 of 5
 % --EXAM: 01234567
 % --EXOP: includetext includecheck includecheckintext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp matrix2of5 0.0 2020122800 51594 55026
+%%BeginResource: uk.co.terryburton.bwipp matrix2of5 0.0 2021020600 51594 55026
 %%BeginData:         57 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /code2of5 dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -8854,15 +9293,15 @@
 
 % --BEGIN ENCODER coop2of5--
 % --REQUIRES preamble raiseerror renlinear code2of5--
 % --DESC: COOP 2 of 5
 % --EXAM: 01234567
 % --EXOP: includetext includecheck includecheckintext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp coop2of5 0.0 2020122800 51584 55018
+%%BeginResource: uk.co.terryburton.bwipp coop2of5 0.0 2021020600 51584 55018
 %%BeginData:         57 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /code2of5 dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -8923,15 +9362,15 @@
 
 % --BEGIN ENCODER datalogic2of5--
 % --REQUIRES preamble raiseerror renlinear code2of5--
 % --DESC: Datalogic 2 of 5
 % --EXAM: 01234567
 % --EXOP: includetext includecheck includecheckintext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp datalogic2of5 0.0 2020122800 51609 55038
+%%BeginResource: uk.co.terryburton.bwipp datalogic2of5 0.0 2021020600 51609 55038
 %%BeginData:         57 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /code2of5 dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -8992,15 +9431,15 @@
 
 % --BEGIN ENCODER code11--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: Code 11
 % --EXAM: 0123456789
 % --EXOP: includetext includecheck includecheckintext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp code11 0.0 2020122800 64947 64410
+%%BeginResource: uk.co.terryburton.bwipp code11 0.0 2021020600 64819 64410
 %%BeginData:        160 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /code11 {
@@ -9164,15 +9603,15 @@
 
 % --BEGIN ENCODER bc412--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: BC412
 % --EXAM: BC412
 % --EXOP: semi includetext includecheckintext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp bc412 0.0 2020122800 60520 60057
+%%BeginResource: uk.co.terryburton.bwipp bc412 0.0 2021020600 60392 60057
 %%BeginData:        150 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /bc412 {
@@ -9326,15 +9765,15 @@
 
 % --BEGIN ENCODER rationalizedCodabar--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: Codabar
 % --EXAM: A0123456789B
 % --EXOP: includetext includecheck includecheckintext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp rationalizedCodabar 0.0 2020122800 65443 64950
+%%BeginResource: uk.co.terryburton.bwipp rationalizedCodabar 0.0 2021020600 65419 64822
 %%BeginData:        158 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /rationalizedCodabar {
@@ -9496,15 +9935,15 @@
 
 % --BEGIN ENCODER onecode--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: USPS Intelligent Mail
 % --EXAM: 0123456709498765432101234567891
 % --EXOP: barcolor=FF0000
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp onecode 0.0 2020122800 99173 98718
+%%BeginResource: uk.co.terryburton.bwipp onecode 0.0 2021020600 99045 98718
 %%BeginData:        337 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /onecode {
@@ -9845,15 +10284,15 @@
 
 % --BEGIN ENCODER postnet--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: USPS POSTNET
 % --EXAM: 01234
 % --EXOP: includetext includecheckintext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp postnet 0.0 2020122800 61318 60891
+%%BeginResource: uk.co.terryburton.bwipp postnet 0.0 2021020600 61190 60891
 %%BeginData:        142 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /postnet {
@@ -9999,15 +10438,15 @@
 
 % --BEGIN ENCODER planet--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: USPS PLANET
 % --EXAM: 01234567890
 % --EXOP: includetext includecheckintext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp planet 0.0 2020122800 61178 60755
+%%BeginResource: uk.co.terryburton.bwipp planet 0.0 2021020600 61050 60755
 %%BeginData:        143 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /planet {
@@ -10154,15 +10593,15 @@
 
 % --BEGIN ENCODER royalmail--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: Royal Mail 4 State Customer Code
 % --EXAM: LE28HS9Z
 % --EXOP: includetext barcolor=FF0000
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp royalmail 0.0 2020122800 61989 61521
+%%BeginResource: uk.co.terryburton.bwipp royalmail 0.0 2021020600 61861 61521
 %%BeginData:        147 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /royalmail {
@@ -10313,15 +10752,15 @@
 
 % --BEGIN ENCODER auspost--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: AusPost 4 State Customer Code
 % --EXAM: 5956439111ABA 9
 % --EXOP: includetext custinfoenc=character
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp auspost 0.0 2020122800 72801 72415
+%%BeginResource: uk.co.terryburton.bwipp auspost 0.0 2021020600 72777 72519
 %%BeginData:        204 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /auspost {
@@ -10529,15 +10968,15 @@
 
 % --BEGIN ENCODER kix--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: Royal Dutch TPG Post KIX
 % --EXAM: 1231FZ13XHS
 % --EXOP: includetext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp kix 0.0 2020122800 57131 56916
+%%BeginResource: uk.co.terryburton.bwipp kix 0.0 2021020600 57107 56916
 %%BeginData:        113 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /kix {
@@ -10654,15 +11093,15 @@
 
 % --BEGIN ENCODER japanpost--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: Japan Post 4 State Customer Code
 % --EXAM: 6540123789-A-K-Z
 % --EXOP: includetext includecheckintext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp japanpost 0.0 2020122800 62150 61757
+%%BeginResource: uk.co.terryburton.bwipp japanpost 0.0 2021020600 62126 61757
 %%BeginData:        164 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /japanpost {
@@ -10830,15 +11269,15 @@
 
 % --BEGIN ENCODER msi--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: MSI Modified Plessey
 % --EXAM: 0123456789
 % --EXOP: includetext includecheck includecheckintext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp msi 0.0 2020122800 67193 66798
+%%BeginResource: uk.co.terryburton.bwipp msi 0.0 2021020600 67169 66798
 %%BeginData:        141 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /msi {
@@ -10983,15 +11422,15 @@
 
 % --BEGIN ENCODER plessey--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: Plessey UK
 % --EXAM: 01234ABCD
 % --EXOP: includetext includecheckintext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp plessey 0.0 2020122800 63687 63197
+%%BeginResource: uk.co.terryburton.bwipp plessey 0.0 2021020600 63559 63197
 %%BeginData:        148 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /plessey {
@@ -11143,15 +11582,15 @@
 
 % --BEGIN ENCODER telepen--
 % --REQUIRES preamble raiseerror parseinput renlinear--
 % --DESC: Telepen
 % --EXAM: ABCDEF
 % --EXOP: includetext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp telepen 0.0 2020122800 65612 68797
+%%BeginResource: uk.co.terryburton.bwipp telepen 0.0 2021020600 65612 68821
 %%BeginData:        165 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -11320,15 +11759,15 @@
 
 % --BEGIN ENCODER telepennumeric--
 % --REQUIRES preamble raiseerror parseinput renlinear telepen--
 % --DESC: Telepen Numeric
 % --EXAM: 01234567
 % --EXOP: includetext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp telepennumeric 0.0 2020122800 57897 54467
+%%BeginResource: uk.co.terryburton.bwipp telepennumeric 0.0 2021020600 57921 54339
 %%BeginData:         57 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /telepen dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -11389,15 +11828,15 @@
 
 % --BEGIN ENCODER posicode--
 % --REQUIRES preamble raiseerror parseinput renlinear--
 % --DESC: PosiCode
 % --EXAM: ABC123
 % --EXOP: version=b inkspread=-0.5 parsefnc includetext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp posicode 0.0 2020122800 107180 110082
+%%BeginResource: uk.co.terryburton.bwipp posicode 0.0 2021020600 107180 110082
 %%BeginData:        390 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -11791,15 +12230,15 @@
 
 % --BEGIN ENCODER codablockf--
 % --REQUIRES preamble raiseerror parseinput renmatrix--
 % --DESC: Codablock F
 % --EXAM: CODABLOCK F 34567890123456789010040digit
 % --EXOP: columns=8
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp codablockf 0.0 2020122800 128823 131632
+%%BeginResource: uk.co.terryburton.bwipp codablockf 0.0 2021020600 128847 131632
 %%BeginData:        488 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -12291,15 +12730,15 @@
 
 % --BEGIN ENCODER code16k--
 % --REQUIRES preamble raiseerror parseinput renmatrix--
 % --DESC: Code 16K
 % --EXAM: Abcd-1234567890-wxyZ
 % --EXOP:
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp code16k 0.0 2020122800 153345 155912
+%%BeginResource: uk.co.terryburton.bwipp code16k 0.0 2021020600 153473 155912
 %%BeginData:        711 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -13014,15 +13453,15 @@
 
 % --BEGIN ENCODER code49--
 % --REQUIRES preamble raiseerror parseinput renmatrix--
 % --DESC: Code 49
 % --EXAM: MULTIPLE ROWS IN CODE 49
 % --EXOP:
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp code49 0.0 2020122800 255438 268416
+%%BeginResource: uk.co.terryburton.bwipp code49 0.0 2021020600 255462 258120
 %%BeginData:       1042 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -14068,15 +14507,15 @@
 
 % --BEGIN ENCODER channelcode--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: Channel Code
 % --EXAM: 3493
 % --EXOP: height=0.5 includetext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp channelcode 0.0 2020122800 125448 124333
+%%BeginResource: uk.co.terryburton.bwipp channelcode 0.0 2021020600 125424 124333
 %%BeginData:        250 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /channelcode {
@@ -14330,15 +14769,15 @@
 
 % --BEGIN ENCODER flattermarken--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: Flattermarken
 % --EXAM: 11099
 % --EXOP: inkspread=-0.25 showborder borderleft=0 borderright=0
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp flattermarken 0.0 2020122800 53933 53728
+%%BeginResource: uk.co.terryburton.bwipp flattermarken 0.0 2021020600 53805 53752
 %%BeginData:         95 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /flattermarken {
@@ -14437,15 +14876,15 @@
 
 % --BEGIN ENCODER raw--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: Custom 1D symbology
 % --EXAM: 331132131313411122131311333213114131131221323
 % --EXOP: height=0.5
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp raw 0.0 2020122800 49535 49415
+%%BeginResource: uk.co.terryburton.bwipp raw 0.0 2021020600 49511 49415
 %%BeginData:         54 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /raw {
@@ -14503,15 +14942,15 @@
 
 % --BEGIN ENCODER daft--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: Custom 4 state symbology
 % --EXAM: FATDAFTDAD
 % --EXOP:
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp daft 0.0 2020122800 52789 52642
+%%BeginResource: uk.co.terryburton.bwipp daft 0.0 2021020600 52765 52642
 %%BeginData:         78 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /daft {
@@ -14593,15 +15032,15 @@
 
 % --BEGIN ENCODER symbol--
 % --REQUIRES preamble raiseerror renlinear--
 % --DESC: Miscellaneous symbols
 % --EXAM: fima
 % --EXOP: backgroundcolor=DD000011
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp symbol 0.0 2020122800 52393 52217
+%%BeginResource: uk.co.terryburton.bwipp symbol 0.0 2021020600 52369 52217
 %%BeginData:         74 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 begin
 /symbol {
@@ -14679,15 +15118,15 @@
 
 % --BEGIN ENCODER pdf417--
 % --REQUIRES preamble raiseerror parseinput renmatrix--
 % --DESC: PDF417
 % --EXAM: This is PDF417
 % --EXOP: columns=2
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp pdf417 0.0 2020122800 195817 201631
+%%BeginResource: uk.co.terryburton.bwipp pdf417 0.0 2021020600 195945 198071
 %%BeginData:        893 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -15584,15 +16023,15 @@
 
 % --BEGIN ENCODER pdf417compact--
 % --REQUIRES preamble raiseerror parseinput renmatrix pdf417--
 % --DESC: Compact PDF417
 % --EXAM: This is compact PDF417
 % --EXOP: columns=2
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp pdf417compact 0.0 2020122800 56915 53230
+%%BeginResource: uk.co.terryburton.bwipp pdf417compact 0.0 2021020600 56787 53230
 %%BeginData:         45 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 dup /pdf417 dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -15641,15 +16080,15 @@
 
 % --BEGIN ENCODER micropdf417--
 % --REQUIRES preamble raiseerror parseinput renmatrix--
 % --DESC: MicroPDF417
 % --EXAM: MicroPDF417
 % --EXOP:
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp micropdf417 0.0 2020122800 206979 215991
+%%BeginResource: uk.co.terryburton.bwipp micropdf417 0.0 2021020600 207003 209127
 %%BeginData:        980 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -16633,15 +17072,15 @@
 
 % --BEGIN ENCODER datamatrix--
 % --REQUIRES preamble raiseerror parseinput renmatrix--
 % --DESC: Data Matrix
 % --EXAM: This is Data Matrix!
 % --EXOP:
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp datamatrix 0.0 2020122800 207969 233965
+%%BeginResource: uk.co.terryburton.bwipp datamatrix 0.0 2021020600 208097 216597
 %%BeginData:        917 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -17562,15 +18001,15 @@
 
 % --BEGIN ENCODER datamatrixrectangular--
 % --REQUIRES preamble raiseerror parseinput renmatrix datamatrix--
 % --DESC: Data Matrix Rectangular
 % --EXAM: 1234
 % --EXOP:
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp datamatrixrectangular 0.0 2020122800 56843 53278
+%%BeginResource: uk.co.terryburton.bwipp datamatrixrectangular 0.0 2021020600 56843 53278
 %%BeginData:         45 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 dup /datamatrix dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -17619,15 +18058,15 @@
 
 % --BEGIN ENCODER datamatrixrectangularextension--
 % --REQUIRES preamble raiseerror parseinput renmatrix datamatrix--
 % --DESC: Data Matrix Rectangular Extension
 % --EXAM: 1234
 % --EXOP: version=8x96
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp datamatrixrectangularextension 0.0 2020122800 57622 54152
+%%BeginResource: uk.co.terryburton.bwipp datamatrixrectangularextension 0.0 2021020600 57622 54152
 %%BeginData:         55 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 dup /datamatrix dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -17686,15 +18125,15 @@
 
 % --BEGIN ENCODER mailmark--
 % --REQUIRES preamble raiseerror parseinput renmatrix datamatrix--
 % --DESC: Royal Mail Mailmark
 % --EXAM: JGB 012100123412345678AB19XY1A 0             www.xyz.com
 % --EXOP: type=29
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp mailmark 0.0 2020122800 60327 56712
+%%BeginResource: uk.co.terryburton.bwipp mailmark 0.0 2021020600 60223 56712
 %%BeginData:         80 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 dup /datamatrix dup /uk.co.terryburton.bwipp findresource put
@@ -17778,15 +18217,15 @@
 
 % --BEGIN ENCODER qrcode--
 % --REQUIRES preamble raiseerror parseinput renmatrix--
 % --DESC: QR Code
 % --EXAM: http://goo.gl/0bis
 % --EXOP: eclevel=M
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp qrcode 0.0 2020122800 324078 365813
+%%BeginResource: uk.co.terryburton.bwipp qrcode 0.0 2021020600 313702 355309
 %%BeginData:       1291 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -19081,15 +19520,15 @@
 
 % --BEGIN ENCODER swissqrcode--
 % --REQUIRES preamble raiseerror parseinput renmatrix qrcode--
 % --DESC: Swiss QR Code
 % --EXAM:
 % --EXOP:
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp swissqrcode 0.0 2020122800 65895 58838
+%%BeginResource: uk.co.terryburton.bwipp swissqrcode 0.0 2021020600 62487 58862
 %%BeginData:        127 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 dup /qrcode dup /uk.co.terryburton.bwipp findresource put
@@ -19220,15 +19659,15 @@
 
 % --BEGIN ENCODER microqrcode--
 % --REQUIRES preamble raiseerror parseinput renmatrix qrcode--
 % --DESC: Micro QR Code
 % --EXAM: 1234
 % --EXOP:
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp microqrcode 0.0 2020122800 57155 57010
+%%BeginResource: uk.co.terryburton.bwipp microqrcode 0.0 2021020600 57179 53578
 %%BeginData:         45 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 dup /qrcode dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -19277,15 +19716,15 @@
 
 % --BEGIN ENCODER rectangularmicroqrcode--
 % --REQUIRES preamble raiseerror parseinput renmatrix qrcode--
 % --DESC: Rectangular Micro QR Code
 % --EXAM: 1234
 % --EXOP: version=R17x139
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp rectangularmicroqrcode 0.0 2020122800 57198 57042
+%%BeginResource: uk.co.terryburton.bwipp rectangularmicroqrcode 0.0 2021020600 57222 53610
 %%BeginData:         45 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 dup /qrcode dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -19334,15 +19773,15 @@
 
 % --BEGIN ENCODER maxicode--
 % --REQUIRES preamble raiseerror parseinput renmaximatrix--
 % --DESC: MaxiCode
 % --EXAM: [)>^03001^02996152382802^029840^029001^0291Z00004951^029UPSN^02906X610^029159^0291234567^0291/1^029^029Y^029634 ALPHA DR^029PITTSBURGH^029PA^029^004
 % --EXOP: mode=2 parse
 % --RNDR: renmaximatrix
-%%BeginResource: uk.co.terryburton.bwipp maxicode 0.0 2020122800 126819 129220
+%%BeginResource: uk.co.terryburton.bwipp maxicode 0.0 2021020600 126819 129324
 %%BeginData:        596 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /renmaximatrix dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -19942,15 +20381,15 @@
 
 % --BEGIN ENCODER azteccode--
 % --REQUIRES preamble raiseerror parseinput renmatrix--
 % --DESC: Aztec Code
 % --EXAM: This is Aztec Code
 % --EXOP: format=full
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp azteccode 0.0 2020122800 174547 187059
+%%BeginResource: uk.co.terryburton.bwipp azteccode 0.0 2021020600 174571 176659
 %%BeginData:        714 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -20668,15 +21107,15 @@
 
 % --BEGIN ENCODER azteccodecompact--
 % --REQUIRES preamble raiseerror parseinput renmatrix azteccode--
 % --DESC: Compact Aztec Code
 % --EXAM: 1234
 % --EXOP:
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp azteccodecompact 0.0 2020122800 56819 53259
+%%BeginResource: uk.co.terryburton.bwipp azteccodecompact 0.0 2021020600 56819 53387
 %%BeginData:         45 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 dup /azteccode dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -20725,15 +21164,15 @@
 
 % --BEGIN ENCODER aztecrune--
 % --REQUIRES preamble raiseerror parseinput renmatrix azteccode--
 % --DESC: Aztec Runes
 % --EXAM: 1
 % --EXOP:
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp aztecrune 0.0 2020122800 56788 53235
+%%BeginResource: uk.co.terryburton.bwipp aztecrune 0.0 2021020600 56788 53363
 %%BeginData:         45 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 dup /azteccode dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -20782,16 +21221,16 @@
 
 % --BEGIN ENCODER codeone--
 % --REQUIRES preamble raiseerror parseinput renmatrix--
 % --DESC: Code One
 % --EXAM: Code One
 % --EXOP:
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp codeone 0.0 2020122800 191244 210362
-%%BeginData:        856 ASCII Lines
+%%BeginResource: uk.co.terryburton.bwipp codeone 0.0 2021020600 196386 201586
+%%BeginData:        883 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 begin
 /codeone {
@@ -21144,23 +21583,23 @@
                     } if
                     /char msg i k add get def
                     /ac ac isD {1 2 div add} {isEA {ceiling 2 add} {ceiling 1 add} ifelse} ifelse def
                     /cc cc isC {2 3 div add} {isEA { 8 3 div add } { 4 3 div add } ifelse} ifelse def
                     /tc tc isT {2 3 div add} {isEA { 8 3 div add } { 4 3 div add } ifelse} ifelse def
                     /xc xc isX {2 3 div add} {isEA {13 3 div add } {10 3 div add } ifelse} ifelse def
                     /bc bc isFN {3 add} {1 add} ifelse def
-                    k 3 ge {
+                    k 3 ge {  % Checking after at least 4 characters (cf. Data Matrix), not 3 as in spec Step Q
                         true [ac cc tc xc   ] {bc 1 add exch ceiling le and} forall {B exit} if
                         true [   cc tc xc bc] {ac 1 add exch ceiling le and} forall {A exit} if
-                        true [ac cc    xc bc] {tc 1 add exch ceiling le and} forall {T exit} if
-                        true [ac    tc      ] {cc 1 add exch ceiling le and} forall {
+                        true [ac cc    xc bc] {tc ceiling 1 add exch ceiling le and} forall {T exit} if
+                        true [ac    tc      ] {cc ceiling 1 add exch ceiling le and} forall {
                             cc ceiling xc ceiling lt {C exit} if
                             cc xc eq {i k add 1 add XtermFirst {X exit} {C exit} ifelse} if
                         } if
-                        true [ac cc tc    bc] {xc 1 add exch lt and} forall {X exit} if
+                        true [ac cc tc    bc] {xc ceiling 1 add exch ceiling le and} forall {X exit} if
                     } if
                     /k k 1 add def
                 } loop
             } repeat
         } bind def
 
         /addtocws {
@@ -21232,32 +21671,51 @@
         /encCTX {
             /p 0 def
             /ctxvals 2220 array def
 
             % Lookup the values for each character
             {
                 i msglen eq {exit} if
-                encvals mode get msg i get known not {exit} if
                 p 3 mod 0 eq {
                     numD i get 12 ge {
+                        ctxvals 0 p getinterval CTXvalstocws addtocws
                         [unlcw] addtocws
                         /mode A def
                         exit
                     } if
                     numD i get dup 8 ge exch i add msglen eq and {
-                        [unlcw] addtocws
-                        /mode A def
-                        exit
-                    } if
-                    lookup mode ne {
                         ctxvals 0 p getinterval CTXvalstocws addtocws
                         [unlcw] addtocws
                         /mode A def
                         exit
                     } if
+                    mode X eq {  % Steps E1c, E2
+                        Xvals msg i get known not {
+                            ctxvals 0 p getinterval CTXvalstocws addtocws
+                            % Unlatch to ASCII unless one codeword left and single ASCII to encode
+                            numremcws j get 1 ne msg i get 127 gt or {
+                                [unlcw] addtocws
+                            } if
+                            /mode A def
+                            exit
+                        } if
+                        i 1 add msglen lt {
+                            Xvals msg i 1 add get known not {exit} if
+                            i 2 add msglen lt {
+                                Xvals msg i 2 add get known not {exit} if
+                            } if
+                        } if
+                    } {
+                        lookup mode ne {
+                            ctxvals 0 p getinterval CTXvalstocws addtocws
+                            [unlcw] addtocws
+                            /mode A def
+                            exit
+                        } if
+                    } ifelse
                     msglen i sub 3 le {  % Check end of data conditions
                         /remcws numremcws j p 3 idiv 2 mul add get def
                         /remvals [
                             msg i msglen i sub getinterval {
                                 dup encvals mode get exch known {
                                     encvals mode get exch get aload pop
                                 } {  % Unencodable X12 characters
@@ -21343,19 +21801,25 @@
 
                 numD i get 3 lt {
 
                     /Drem 8 Dbits length 8 mod sub 8 mod def
                     /remcws numremcws j Dbits length 8 idiv add get def
 
                     % Final codeword with no data
-                    numremcws j Dbits length 8 idiv add 1 sub get 1 sub 0 eq
-                    i msglen eq and {exit} if
+                    numremcws j Dbits length 8 idiv add 1 sub get 1 sub 0 eq Drem 0 eq and  % No remaining codewords and no bits
+                    remcws 1 eq Drem 0 ne and or  % Or 1 remaining codeword and some bits
+                    i msglen eq and {
+                        Drem 4 eq Drem 6 eq or { /Dbits [ Dbits aload pop 1 1 1 1 ] def } if
+                        Drem 2 eq Drem 6 eq or { /Dbits [ Dbits aload pop 0 1 ] def } if
+                        exit
+                    } if
 
-                    % Final digit into final codeword as ASCII
+                    % Final digit or double-digit into final codeword as ASCII
                     i msglen 1 sub eq numD i get 1 eq and
+                    i msglen 2 sub eq numD i get 2 eq and or
                     remcws 1 eq and Drem 0 eq and {exit} if
 
                     % Latch to ASCII unless 4 or 6 bits remain in final codeword
                     i msglen 1 sub eq numD i get 1 eq and
                     remcws 1 eq and Drem 4 eq Drem 6 eq or and not {
                       /Dbits [ Dbits aload pop 1 1 1 1 1 1 ] def
                       /Drem 8 Dbits length 8 mod sub 8 mod def
@@ -21457,14 +21921,16 @@
     % Extend cws to ncws codewords by addition of pad characters
     stype not {
         /cws [ cws aload pop dcws cws length sub {129} repeat ] def
     } {
         /cws [ dcws cws length sub {0} repeat cws aload pop ] def
     } ifelse
 
+    options /debugcws known { /bwipp.debugcws cws //raiseerror exec } if
+
     % De-interleave the codewords into blocks
     /cwbs rsbl array def  % Array of data codeword blocks
     /ecbs rsbl array def  % Array of error correction blocks
     0 1 rsbl 1 sub {
         /i exch def
         /cwb dcpb array def
         0 1 dcpb 1 sub {
@@ -21650,15 +22116,15 @@
 
 % --BEGIN ENCODER hanxin--
 % --REQUIRES preamble raiseerror parseinput renmatrix--
 % --DESC: Han Xin Code
 % --EXAM: This is Han Xin
 % --EXOP:
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp hanxin 0.0 2020122800 306050 349404
+%%BeginResource: uk.co.terryburton.bwipp hanxin 0.0 2021020600 299418 335780
 %%BeginData:        852 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -22514,15 +22980,15 @@
 
 % --BEGIN ENCODER dotcode--
 % --REQUIRES preamble raiseerror parseinput renmatrix--
 % --DESC: DotCode
 % --EXAM: This is DotCode
 % --EXOP: inkspread=0.16
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp dotcode 0.0 2020122800 231602 264430
+%%BeginResource: uk.co.terryburton.bwipp dotcode 0.0 2021020600 231730 243734
 %%BeginData:       1035 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -23561,15 +24027,15 @@
 
 % --BEGIN ENCODER ultracode--
 % --REQUIRES preamble raiseerror parseinput renmatrix--
 % --DESC: Ultracode
 % --EXAM: Awesome colours!
 % --EXOP: eclevel=EC2
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp ultracode 0.0 2020122800 84277 87023
+%%BeginResource: uk.co.terryburton.bwipp ultracode 0.0 2021020600 84301 87023
 %%BeginData:        299 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -23872,15 +24338,15 @@
 
 % --BEGIN ENCODER jabcode--
 % --REQUIRES preamble raiseerror parseinput renmatrix--
 % --DESC: JAB Code (Beta)
 % --EXAM: This is JAB Code
 % --EXOP: eclevel=6
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp jabcode 0.0 2020122800 243765 285987
+%%BeginResource: uk.co.terryburton.bwipp jabcode 0.0 2021020600 243685 265291
 %%BeginData:       1132 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -25016,15 +25482,15 @@
 
 % --BEGIN ENCODER gs1-cc--
 % --REQUIRES preamble raiseerror parseinput gs1lint renmatrix micropdf417 pdf417--
 % --DESC: GS1 Composite 2D Component
 % --EXAM: (01)95012345678903(3103)000123
 % --EXOP: ccversion=b cccolumns=4
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp gs1-cc 0.0 2020122800 205183 207592
+%%BeginResource: uk.co.terryburton.bwipp gs1-cc 0.0 2021020600 208615 207592
 %%BeginData:        659 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /gs1lint dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
@@ -25687,15 +26153,15 @@
 
 % --BEGIN ENCODER ean13composite--
 % --REQUIRES preamble raiseerror parseinput gs1lint renlinear renmatrix ean5 ean2 ean13 micropdf417 pdf417 gs1-cc--
 % --DESC: EAN-13 Composite
 % --EXAM: 2112345678900|(99)1234-abcd
 % --EXOP: includetext
 % --RNDR: renlinear renmatrix
-%%BeginResource: uk.co.terryburton.bwipp ean13composite 0.0 2020122800 79583 86527
+%%BeginResource: uk.co.terryburton.bwipp ean13composite 0.0 2021020600 83015 86399
 %%BeginData:         74 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /ean13 dup /uk.co.terryburton.bwipp findresource put
 dup /gs1-cc dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
@@ -25773,15 +26239,15 @@
 
 % --BEGIN ENCODER ean8composite--
 % --REQUIRES preamble raiseerror parseinput gs1lint renlinear renmatrix ean5 ean2 ean8 micropdf417 pdf417 gs1-cc--
 % --DESC: EAN-8 Composite
 % --EXAM: 02345673|(21)A12345678
 % --EXOP: includetext
 % --RNDR: renlinear renmatrix
-%%BeginResource: uk.co.terryburton.bwipp ean8composite 0.0 2020122800 83484 86741
+%%BeginResource: uk.co.terryburton.bwipp ean8composite 0.0 2021020600 83356 86741
 %%BeginData:         77 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /ean8 dup /uk.co.terryburton.bwipp findresource put
 dup /gs1-cc dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
@@ -25862,15 +26328,15 @@
 
 % --BEGIN ENCODER upcacomposite--
 % --REQUIRES preamble raiseerror parseinput gs1lint renlinear renmatrix ean5 ean2 upca micropdf417 pdf417 gs1-cc--
 % --DESC: UPC-A Composite
 % --EXAM: 416000336108|(99)1234-abcd
 % --EXOP: includetext
 % --RNDR: renlinear renmatrix
-%%BeginResource: uk.co.terryburton.bwipp upcacomposite 0.0 2020122800 82993 82946
+%%BeginResource: uk.co.terryburton.bwipp upcacomposite 0.0 2021020600 79561 86378
 %%BeginData:         74 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 2 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /upca dup /uk.co.terryburton.bwipp findresource put
 dup /gs1-cc dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
@@ -25948,15 +26414,15 @@
 
 % --BEGIN ENCODER upcecomposite--
 % --REQUIRES preamble raiseerror parseinput gs1lint renlinear renmatrix ean5 ean2 upce micropdf417 pdf417 gs1-cc--
 % --DESC: UPC-E Composite
 % --EXAM: 00123457|(15)021231
 % --EXOP: includetext
 % --RNDR: renlinear renmatrix
-%%BeginResource: uk.co.terryburton.bwipp upcecomposite 0.0 2020122800 84275 87649
+%%BeginResource: uk.co.terryburton.bwipp upcecomposite 0.0 2021020600 84275 87649
 %%BeginData:         89 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 2 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /upce dup /uk.co.terryburton.bwipp findresource put
 dup /gs1-cc dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
@@ -26049,15 +26515,15 @@
 
 % --BEGIN ENCODER databaromnicomposite--
 % --REQUIRES preamble raiseerror parseinput gs1lint renlinear renmatrix databaromni micropdf417 pdf417 gs1-cc--
 % --DESC: GS1 DataBar Omnidirectional Composite
 % --EXAM: (01)03612345678904|(11)990102
 % --EXOP:
 % --RNDR: renlinear renmatrix
-%%BeginResource: uk.co.terryburton.bwipp databaromnicomposite 0.0 2020122800 87494 83950
+%%BeginResource: uk.co.terryburton.bwipp databaromnicomposite 0.0 2021020600 87598 83950
 %%BeginData:        102 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 2 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /databaromni dup /uk.co.terryburton.bwipp findresource put
 dup /gs1-cc dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
@@ -26163,15 +26629,15 @@
 
 % --BEGIN ENCODER databarstackedcomposite--
 % --REQUIRES preamble raiseerror parseinput gs1lint renlinear renmatrix databaromni databarstacked micropdf417 pdf417 gs1-cc--
 % --DESC: GS1 DataBar Stacked Composite
 % --EXAM: (01)03412345678900|(17)010200
 % --EXOP:
 % --RNDR: renlinear renmatrix
-%%BeginResource: uk.co.terryburton.bwipp databarstackedcomposite 0.0 2020122800 85882 89213
+%%BeginResource: uk.co.terryburton.bwipp databarstackedcomposite 0.0 2021020600 89442 89213
 %%BeginData:         98 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 2 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /databarstacked dup /uk.co.terryburton.bwipp findresource put
 dup /gs1-cc dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
@@ -26273,15 +26739,15 @@
 
 % --BEGIN ENCODER databarstackedomnicomposite--
 % --REQUIRES preamble raiseerror parseinput gs1lint renlinear renmatrix databaromni databarstackedomni micropdf417 pdf417 gs1-cc--
 % --DESC: GS1 DataBar Stacked Omnidirectional Composite
 % --EXAM: (01)03612345678904|(11)990102
 % --EXOP:
 % --RNDR: renlinear renmatrix
-%%BeginResource: uk.co.terryburton.bwipp databarstackedomnicomposite 0.0 2020122800 85910 89237
+%%BeginResource: uk.co.terryburton.bwipp databarstackedomnicomposite 0.0 2021020600 89470 89237
 %%BeginData:         98 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 2 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /databarstackedomni dup /uk.co.terryburton.bwipp findresource put
 dup /gs1-cc dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
@@ -26383,15 +26849,15 @@
 
 % --BEGIN ENCODER databartruncatedcomposite--
 % --REQUIRES preamble raiseerror parseinput gs1lint renlinear renmatrix databaromni databartruncated micropdf417 pdf417 gs1-cc--
 % --DESC: GS1 DataBar Truncated Composite
 % --EXAM: (01)03612345678904|(11)990102
 % --EXOP:
 % --RNDR: renlinear renmatrix
-%%BeginResource: uk.co.terryburton.bwipp databartruncatedcomposite 0.0 2020122800 86952 90267
+%%BeginResource: uk.co.terryburton.bwipp databartruncatedcomposite 0.0 2021020600 90512 90267
 %%BeginData:        102 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 2 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /databartruncated dup /uk.co.terryburton.bwipp findresource put
 dup /gs1-cc dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
@@ -26497,15 +26963,15 @@
 
 % --BEGIN ENCODER databarlimitedcomposite--
 % --REQUIRES preamble raiseerror parseinput gs1lint renlinear renmatrix databarlimited micropdf417 pdf417 gs1-cc--
 % --DESC: GS1 DataBar Limited Composite
 % --EXAM: (01)03512345678907|(21)abcdefghijklmnopqrstuv
 % --EXOP:
 % --RNDR: renlinear renmatrix
-%%BeginResource: uk.co.terryburton.bwipp databarlimitedcomposite 0.0 2020122800 83791 80260
+%%BeginResource: uk.co.terryburton.bwipp databarlimitedcomposite 0.0 2021020600 83919 80260
 %%BeginData:         81 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 2 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /databarlimited dup /uk.co.terryburton.bwipp findresource put
 dup /gs1-cc dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
@@ -26590,15 +27056,15 @@
 
 % --BEGIN ENCODER databarexpandedcomposite--
 % --REQUIRES preamble raiseerror parseinput gs1lint renlinear renmatrix databarexpanded micropdf417 pdf417 gs1-cc--
 % --DESC: GS1 DataBar Expanded Composite
 % --EXAM: (01)93712345678904(3103)001234|(91)1A2B3C4D5E
 % --EXOP:
 % --RNDR: renlinear renmatrix
-%%BeginResource: uk.co.terryburton.bwipp databarexpandedcomposite 0.0 2020122800 83389 83390
+%%BeginResource: uk.co.terryburton.bwipp databarexpandedcomposite 0.0 2021020600 83389 83262
 %%BeginData:        100 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 2 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /databarexpanded dup /uk.co.terryburton.bwipp findresource put
 dup /gs1-cc dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
@@ -26702,15 +27168,15 @@
 
 % --BEGIN ENCODER databarexpandedstackedcomposite--
 % --REQUIRES preamble raiseerror parseinput gs1lint renlinear renmatrix databarexpanded databarexpandedstacked micropdf417 pdf417 gs1-cc--
 % --DESC: GS1 DataBar Expanded Stacked Composite
 % --EXAM: (01)00012345678905(10)ABCDEF|(21)12345678
 % --EXOP: segments=4
 % --RNDR: renmatrix renlinear
-%%BeginResource: uk.co.terryburton.bwipp databarexpandedstackedcomposite 0.0 2020122800 85613 85493
+%%BeginResource: uk.co.terryburton.bwipp databarexpandedstackedcomposite 0.0 2021020600 89173 85493
 %%BeginData:         97 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 2 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /databarexpandedstacked dup /uk.co.terryburton.bwipp findresource put
 dup /gs1-cc dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
@@ -26811,15 +27277,15 @@
 
 % --BEGIN ENCODER gs1-128composite--
 % --REQUIRES preamble raiseerror parseinput gs1lint renlinear renmatrix code128 gs1-128 micropdf417 pdf417 gs1-cc--
 % --DESC: GS1-128 Composite
 % --EXAM: (00)030123456789012340|(02)13012345678909(37)24(10)1234567ABCDEFG
 % --EXOP: ccversion=c
 % --RNDR: renlinear renmatrix
-%%BeginResource: uk.co.terryburton.bwipp gs1-128composite 0.0 2020122800 86500 89809
+%%BeginResource: uk.co.terryburton.bwipp gs1-128composite 0.0 2021020600 90060 89809
 %%BeginData:        102 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 2 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /gs1-128 dup /uk.co.terryburton.bwipp findresource put
 dup /gs1-cc dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
@@ -26925,15 +27391,15 @@
 
 % --BEGIN ENCODER gs1datamatrix--
 % --REQUIRES preamble raiseerror parseinput gs1lint renmatrix datamatrix--
 % --DESC: GS1 Data Matrix
 % --EXAM: (01)03453120000011(17)120508(10)ABCD1234(410)9501101020917
 % --EXOP:
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp gs1datamatrix 0.0 2020122800 77808 77858
+%%BeginResource: uk.co.terryburton.bwipp gs1datamatrix 0.0 2021020600 77808 74426
 %%BeginData:        133 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /gs1lint dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
@@ -27070,15 +27536,15 @@
 
 % --BEGIN ENCODER gs1datamatrixrectangular--
 % --REQUIRES preamble raiseerror parseinput gs1lint renmatrix datamatrix--
 % --DESC: GS1 Data Matrix Rectangular
 % --EXAM: (01)03453120000011(17)120508(10)ABCD1234(410)9501101020917
 % --EXOP:
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp gs1datamatrixrectangular 0.0 2020122800 78011 78026
+%%BeginResource: uk.co.terryburton.bwipp gs1datamatrixrectangular 0.0 2021020600 78011 78026
 %%BeginData:        134 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /gs1lint dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
@@ -27216,15 +27682,15 @@
 
 % --BEGIN ENCODER gs1qrcode--
 % --REQUIRES preamble raiseerror parseinput gs1lint renmatrix qrcode--
 % --DESC: GS1 QR Code
 % --EXAM: (01)03453120000011(8200)http://www.abc.net(10)ABCD1234(410)9501101020917
 % --EXOP:
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp gs1qrcode 0.0 2020122800 77795 77814
+%%BeginResource: uk.co.terryburton.bwipp gs1qrcode 0.0 2021020600 81227 74382
 %%BeginData:        132 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /gs1lint dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 dup /qrcode dup /uk.co.terryburton.bwipp findresource put
@@ -27357,18 +27823,18 @@
 %%EndData
 %%EndResource
 % --END ENCODER gs1qrcode--
 
 % --BEGIN ENCODER gs1dotcode--
 % --REQUIRES preamble raiseerror parseinput gs1lint renmatrix dotcode--
 % --DESC: GS1 DotCode
-% --EXAM: (01)03453120000011(17)120508(10)ABCD1234(410)9501101020917
-% --EXOP:
+% --EXAM: (235)5vBZIF%!<B;?oa%(01)01234567890128(8008)19052001
+% --EXOP: rows=16
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp gs1dotcode 0.0 2020122800 81234 74387
+%%BeginResource: uk.co.terryburton.bwipp gs1dotcode 0.0 2021020600 77802 77819
 %%BeginData:        133 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /parseinput dup /uk.co.terryburton.bwipp findresource put
 dup /gs1lint dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
@@ -27505,15 +27971,15 @@
 
 % --BEGIN ENCODER hibccode39--
 % --REQUIRES preamble raiseerror renlinear code39--
 % --DESC: HIBC Code 39
 % --EXAM: A123BJC5D6E71
 % --EXOP: includetext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp hibccode39 0.0 2020122800 57669 60912
+%%BeginResource: uk.co.terryburton.bwipp hibccode39 0.0 2021020600 57669 61040
 %%BeginData:         94 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /code39 dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -27611,15 +28077,15 @@
 
 % --BEGIN ENCODER hibccode128--
 % --REQUIRES preamble raiseerror parseinput renlinear code128--
 % --DESC: HIBC Code 128
 % --EXAM: A123BJC5D6E71
 % --EXOP: includetext
 % --RNDR: renlinear
-%%BeginResource: uk.co.terryburton.bwipp hibccode128 0.0 2020122800 63913 60296
+%%BeginResource: uk.co.terryburton.bwipp hibccode128 0.0 2021020600 63889 60320
 %%BeginData:         93 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renlinear dup /uk.co.terryburton.bwipp findresource put
 dup /code128 dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -27716,15 +28182,15 @@
 
 % --BEGIN ENCODER hibcdatamatrix--
 % --REQUIRES preamble raiseerror parseinput renmatrix datamatrix--
 % --DESC: HIBC Data Matrix
 % --EXAM: A123BJC5D6E71
 % --EXOP:
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp hibcdatamatrix 0.0 2020122800 61356 57634
+%%BeginResource: uk.co.terryburton.bwipp hibcdatamatrix 0.0 2021020600 61356 57634
 %%BeginData:         76 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 dup /datamatrix dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -27804,15 +28270,15 @@
 
 % --BEGIN ENCODER hibcdatamatrixrectangular--
 % --REQUIRES preamble raiseerror parseinput renmatrix datamatrix--
 % --DESC: HIBC Data Matrix Rectangular
 % --EXAM: A123BJC5D6E71
 % --EXOP:
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp hibcdatamatrixrectangular 0.0 2020122800 61709 57954
+%%BeginResource: uk.co.terryburton.bwipp hibcdatamatrixrectangular 0.0 2021020600 61709 57954
 %%BeginData:         77 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 dup /datamatrix dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -27893,15 +28359,15 @@
 
 % --BEGIN ENCODER hibcpdf417--
 % --REQUIRES preamble raiseerror parseinput renmatrix pdf417--
 % --DESC: HIBC PDF417
 % --EXAM: A123BJC5D6E71
 % --EXOP:
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp hibcpdf417 0.0 2020122800 61867 58059
+%%BeginResource: uk.co.terryburton.bwipp hibcpdf417 0.0 2021020600 61739 58059
 %%BeginData:         80 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 dup /pdf417 dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -27985,15 +28451,15 @@
 
 % --BEGIN ENCODER hibcmicropdf417--
 % --REQUIRES preamble raiseerror parseinput renmatrix micropdf417--
 % --DESC: HIBC MicroPDF417
 % --EXAM: A123BJC5D6E71
 % --EXOP:
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp hibcmicropdf417 0.0 2020122800 61685 58118
+%%BeginResource: uk.co.terryburton.bwipp hibcmicropdf417 0.0 2021020600 61789 58094
 %%BeginData:         80 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 dup /micropdf417 dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -28077,15 +28543,15 @@
 
 % --BEGIN ENCODER hibcqrcode--
 % --REQUIRES preamble raiseerror parseinput renmatrix qrcode--
 % --DESC: HIBC QR Code
 % --EXAM: A123BJC5D6E71
 % --EXOP:
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp hibcqrcode 0.0 2020122800 65776 58524
+%%BeginResource: uk.co.terryburton.bwipp hibcqrcode 0.0 2021020600 62368 58652
 %%BeginData:         76 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 dup /qrcode dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -28165,15 +28631,15 @@
 
 % --BEGIN ENCODER hibccodablockf--
 % --REQUIRES preamble raiseerror parseinput renmatrix codablockf--
 % --DESC: HIBC Codablock F
 % --EXAM: A123BJC5D6E71
 % --EXOP:
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp hibccodablockf 0.0 2020122800 61336 57866
+%%BeginResource: uk.co.terryburton.bwipp hibccodablockf 0.0 2021020600 61336 57866
 %%BeginData:         76 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 dup /codablockf dup /uk.co.terryburton.bwipp findresource put
 begin
@@ -28253,15 +28719,15 @@
 
 % --BEGIN ENCODER hibcazteccode--
 % --REQUIRES preamble raiseerror parseinput renmatrix azteccode--
 % --DESC: HIBC Aztec Code
 % --EXAM: A123BJC5D6E71
 % --EXOP:
 % --RNDR: renmatrix
-%%BeginResource: uk.co.terryburton.bwipp hibcazteccode 0.0 2020122800 61330 57627
+%%BeginResource: uk.co.terryburton.bwipp hibcazteccode 0.0 2021020600 61330 57627
 %%BeginData:         76 ASCII Lines
 /setpacking where {pop currentpacking true setpacking} if
 1 dict
 dup /raiseerror dup /uk.co.terryburton.bwipp findresource put
 dup /renmatrix dup /uk.co.terryburton.bwipp findresource put
 dup /azteccode dup /uk.co.terryburton.bwipp findresource put
 begin
```

### Comparing `treepoem-3.8.0/src/treepoem.egg-info/PKG-INFO` & `treepoem-3.9.0/src/treepoem.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: treepoem
-Version: 3.8.0
+Version: 3.9.0
 Summary: Barcode rendering for Python supporting QRcode, Aztec, PDF417, I25, Code128, Code39 and many more types.
 Home-page: https://github.com/adamchainz/treepoem
 Author: Christian Muirhead
 Author-email: xtian@babbageclunk.com
 Maintainer: Adam Johnson
 Maintainer-email: me@adamj.eu
 License: MIT
-Project-URL: Changelog, https://github.com/adamchainz/treepoem/blob/master/HISTORY.rst
+Project-URL: Changelog, https://github.com/adamchainz/treepoem/blob/main/HISTORY.rst
 Project-URL: Twitter, https://twitter.com/adamchainz
 Description: ========
         Treepoem
         ========
         
-        .. image:: https://img.shields.io/github/workflow/status/adamchainz/treepoem/CI/master?style=for-the-badge
+        .. image:: https://img.shields.io/github/workflow/status/adamchainz/treepoem/CI/main?style=for-the-badge
            :target: https://github.com/adamchainz/treepoem/actions?workflow=CI
         
         .. image:: https://img.shields.io/pypi/v/treepoem.svg?style=for-the-badge
            :target: https://pypi.org/project/treepoem/
         
         .. image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge
            :target: https://github.com/psf/black
```

