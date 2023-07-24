# Comparing `tmp/bw_processing-0.8.2.tar.gz` & `tmp/bw-processing-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bw_processing-0.8.2.tar", last modified: Thu Sep 15 09:46:35 2022, max compression
+gzip compressed data, was "bw-processing-0.8.3.tar", last modified: Mon Jul 24 18:14:42 2023, max compression
```

## Comparing `bw_processing-0.8.2.tar` & `bw-processing-0.8.3.tar`

### file list

```diff
@@ -1,115 +1,42 @@
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-09-15 09:46:35.375630 bw_processing-0.8.2/
--rw-r--r--   0 cmutel     (501) staff       (20)     1203 2019-10-16 09:08:39.000000 bw_processing-0.8.2/.gitignore
--rw-r--r--   0 cmutel     (501) staff       (20)      429 2021-10-06 03:30:05.000000 bw_processing-0.8.2/.pre-commit-config.yaml
--rw-r--r--   0 cmutel     (501) staff       (20)     2182 2022-09-15 09:38:57.000000 bw_processing-0.8.2/CHANGELOG.md
--rw-r--r--   0 cmutel     (501) staff       (20)     5226 2020-09-25 13:17:00.000000 bw_processing-0.8.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 cmutel     (501) staff       (20)     1511 2019-10-16 09:21:28.000000 bw_processing-0.8.2/LICENSE
--rw-r--r--   0 cmutel     (501) staff       (20)       43 2019-10-16 09:08:39.000000 bw_processing-0.8.2/MANIFEST.in
--rw-r--r--   0 cmutel     (501) staff       (20)    15017 2022-09-15 09:46:35.375449 bw_processing-0.8.2/PKG-INFO
--rw-r--r--   0 cmutel     (501) staff       (20)    13939 2021-11-24 12:57:21.000000 bw_processing-0.8.2/README.md
--rw-r--r--   0 cmutel     (501) staff       (20)     6573 2022-04-11 10:04:52.000000 bw_processing-0.8.2/azure-pipelines.yml
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-09-15 09:46:35.363240 bw_processing-0.8.2/bw_processing/
--rw-r--r--   0 cmutel     (501) staff       (20)     1344 2022-09-15 09:38:35.000000 bw_processing-0.8.2/bw_processing/__init__.py
--rw-r--r--   0 cmutel     (501) staff       (20)     5839 2021-10-06 03:26:26.000000 bw_processing-0.8.2/bw_processing/array_creation.py
--rw-r--r--   0 cmutel     (501) staff       (20)      916 2021-10-06 03:26:26.000000 bw_processing-0.8.2/bw_processing/constants.py
--rw-r--r--   0 cmutel     (501) staff       (20)    37578 2022-09-15 09:38:35.000000 bw_processing-0.8.2/bw_processing/datapackage.py
--rw-r--r--   0 cmutel     (501) staff       (20)     1395 2021-10-29 21:47:27.000000 bw_processing-0.8.2/bw_processing/errors.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-09-15 09:46:35.364104 bw_processing-0.8.2/bw_processing/examples/
--rw-r--r--   0 cmutel     (501) staff       (20)       73 2020-09-25 13:57:42.000000 bw_processing-0.8.2/bw_processing/examples/__init__.py
--rw-r--r--   0 cmutel     (501) staff       (20)      602 2021-02-02 15:32:53.000000 bw_processing-0.8.2/bw_processing/examples/interfaces.py
--rw-r--r--   0 cmutel     (501) staff       (20)      772 2020-09-25 14:01:54.000000 bw_processing-0.8.2/bw_processing/examples/simple.zip
--rw-r--r--   0 cmutel     (501) staff       (20)     1632 2021-10-06 03:26:26.000000 bw_processing-0.8.2/bw_processing/filesystem.py
--rw-r--r--   0 cmutel     (501) staff       (20)     5612 2021-10-06 03:26:26.000000 bw_processing-0.8.2/bw_processing/indexing.py
--rw-r--r--   0 cmutel     (501) staff       (20)     2915 2022-09-15 09:32:21.000000 bw_processing-0.8.2/bw_processing/io_helpers.py
--rw-r--r--   0 cmutel     (501) staff       (20)     6291 2022-06-24 07:47:52.000000 bw_processing-0.8.2/bw_processing/merging.py
--rw-r--r--   0 cmutel     (501) staff       (20)      484 2021-10-04 13:16:47.000000 bw_processing-0.8.2/bw_processing/proxies.py
--rw-r--r--   0 cmutel     (501) staff       (20)     3819 2021-10-06 03:26:26.000000 bw_processing-0.8.2/bw_processing/unique_fields.py
--rw-r--r--   0 cmutel     (501) staff       (20)     2948 2022-04-11 09:34:06.000000 bw_processing-0.8.2/bw_processing/utils.py
--rw-r--r--   0 cmutel     (501) staff       (20)       20 2022-09-15 09:39:03.000000 bw_processing-0.8.2/bw_processing/version.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-09-15 09:46:35.363750 bw_processing-0.8.2/bw_processing.egg-info/
--rw-r--r--   0 cmutel     (501) staff       (20)    15017 2022-09-15 09:46:35.000000 bw_processing-0.8.2/bw_processing.egg-info/PKG-INFO
--rw-r--r--   0 cmutel     (501) staff       (20)     3069 2022-09-15 09:46:35.000000 bw_processing-0.8.2/bw_processing.egg-info/SOURCES.txt
--rw-r--r--   0 cmutel     (501) staff       (20)        1 2022-09-15 09:46:35.000000 bw_processing-0.8.2/bw_processing.egg-info/dependency_links.txt
--rw-r--r--   0 cmutel     (501) staff       (20)       16 2022-09-15 09:46:35.000000 bw_processing-0.8.2/bw_processing.egg-info/requires.txt
--rw-r--r--   0 cmutel     (501) staff       (20)       14 2022-09-15 09:46:35.000000 bw_processing-0.8.2/bw_processing.egg-info/top_level.txt
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-09-15 09:46:35.364445 bw_processing-0.8.2/ci/
--rw-r--r--   0 cmutel     (501) staff       (20)      386 2019-10-16 10:13:54.000000 bw_processing-0.8.2/ci/conda_upload.sh
--rw-r--r--   0 cmutel     (501) staff       (20)      576 2020-04-20 09:33:31.000000 bw_processing-0.8.2/ci/meta.yaml
--rw-r--r--   0 cmutel     (501) staff       (20)      590 2021-01-29 14:01:40.000000 bw_processing-0.8.2/conftest.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-09-15 09:46:35.365430 bw_processing-0.8.2/dev/
--rw-r--r--   0 cmutel     (501) staff       (20)    15465 2020-09-25 07:45:25.000000 bw_processing-0.8.2/dev/Presamples generator example.ipynb
--rw-r--r--   0 cmutel     (501) staff       (20)     6528 2020-09-21 12:42:34.000000 bw_processing-0.8.2/dev/calculation_package.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-09-15 09:46:35.365806 bw_processing-0.8.2/dev/generator_metadata/
--rw-r--r--   0 cmutel     (501) staff       (20)      949 2021-01-04 10:17:37.000000 bw_processing-0.8.2/dev/generator_metadata/datapackage.json
--rw-r--r--   0 cmutel     (501) staff       (20)      224 2020-09-25 07:11:38.000000 bw_processing-0.8.2/dev/generator_metadata/infinite-data-indices.npy
--rw-r--r--   0 cmutel     (501) staff       (20)       47 2020-09-25 07:13:28.000000 bw_processing-0.8.2/dev/generator_metadata/infinite-data-meta.csv
--rw-r--r--   0 cmutel     (501) staff       (20)     4240 2021-01-04 10:17:38.000000 bw_processing-0.8.2/dev/loading.py
--rw-r--r--   0 cmutel     (501) staff       (20)     9654 2021-01-04 10:17:38.000000 bw_processing-0.8.2/dev/processed_package.py
--rw-r--r--   0 cmutel     (501) staff       (20)      741 2021-01-04 10:17:38.000000 bw_processing-0.8.2/dev/resources.py
--rw-r--r--   0 cmutel     (501) staff       (20)     1195 2020-10-02 12:58:54.000000 bw_processing-0.8.2/dev/speed_tests.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-09-15 09:46:35.366668 bw_processing-0.8.2/docs/
--rw-r--r--   0 cmutel     (501) staff       (20)      634 2020-04-16 13:55:43.000000 bw_processing-0.8.2/docs/Makefile
--rw-r--r--   0 cmutel     (501) staff       (20)     1968 2020-09-25 13:18:47.000000 bw_processing-0.8.2/docs/conf.py
--rw-r--r--   0 cmutel     (501) staff       (20)      364 2020-04-16 14:04:40.000000 bw_processing-0.8.2/docs/index.rst
--rw-r--r--   0 cmutel     (501) staff       (20)       88 2020-04-16 14:25:35.000000 bw_processing-0.8.2/docs/loading.rst
--rw-r--r--   0 cmutel     (501) staff       (20)      795 2020-04-16 13:55:43.000000 bw_processing-0.8.2/docs/make.bat
--rw-r--r--   0 cmutel     (501) staff       (20)      300 2020-09-21 12:42:37.000000 bw_processing-0.8.2/docs/saving.rst
--rw-r--r--   0 cmutel     (501) staff       (20)      893 2021-01-04 10:16:20.000000 bw_processing-0.8.2/docs/utilities.rst
--rw-r--r--   0 cmutel     (501) staff       (20)       82 2019-10-16 09:08:39.000000 bw_processing-0.8.2/pytest.ini
--rw-r--r--   0 cmutel     (501) staff       (20)       16 2021-01-29 14:01:40.000000 bw_processing-0.8.2/requirements.txt
--rw-r--r--   0 cmutel     (501) staff       (20)       38 2022-09-15 09:46:35.375673 bw_processing-0.8.2/setup.cfg
--rw-r--r--   0 cmutel     (501) staff       (20)     1485 2021-01-29 14:01:40.000000 bw_processing-0.8.2/setup.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-09-15 09:46:35.369611 bw_processing-0.8.2/tests/
--rw-r--r--   0 cmutel     (501) staff       (20)      269 2020-10-15 11:30:34.000000 bw_processing-0.8.2/tests/array_creation.py
--rw-r--r--   0 cmutel     (501) staff       (20)     4191 2020-09-25 10:40:43.000000 bw_processing-0.8.2/tests/calculation_package.py
--rw-r--r--   0 cmutel     (501) staff       (20)    16329 2022-09-15 09:38:35.000000 bw_processing-0.8.2/tests/datapackage.py
--rw-r--r--   0 cmutel     (501) staff       (20)     1063 2021-11-24 11:33:04.000000 bw_processing-0.8.2/tests/filesystem.py
--rw-r--r--   0 cmutel     (501) staff       (20)     4654 2021-11-26 07:17:32.000000 bw_processing-0.8.2/tests/filtered_datapackage.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-09-15 09:46:35.370256 bw_processing-0.8.2/tests/fixtures/
--rw-r--r--   0 cmutel     (501) staff       (20)      928 2021-02-03 22:47:04.000000 bw_processing-0.8.2/tests/fixtures/array.npy
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-09-15 09:46:35.372343 bw_processing-0.8.2/tests/fixtures/indexing/
--rw-r--r--   0 cmutel     (501) staff       (20)       69 2021-05-18 13:12:19.000000 bw_processing-0.8.2/tests/fixtures/indexing/array-csv-both.csv
--rw-r--r--   0 cmutel     (501) staff       (20)       69 2021-05-18 13:12:19.000000 bw_processing-0.8.2/tests/fixtures/indexing/array-csv-rows.csv
--rw-r--r--   0 cmutel     (501) staff       (20)      224 2021-05-18 13:12:19.000000 bw_processing-0.8.2/tests/fixtures/indexing/array.data.npy
--rw-r--r--   0 cmutel     (501) staff       (20)      131 2021-05-18 13:12:19.000000 bw_processing-0.8.2/tests/fixtures/indexing/array.flip.npy
--rw-r--r--   0 cmutel     (501) staff       (20)      152 2021-05-18 13:12:19.000000 bw_processing-0.8.2/tests/fixtures/indexing/array.indices.npy
--rw-r--r--   0 cmutel     (501) staff       (20)       69 2021-05-18 13:12:19.000000 bw_processing-0.8.2/tests/fixtures/indexing/csv-multiple.csv
--rw-r--r--   0 cmutel     (501) staff       (20)     3838 2021-05-18 13:17:12.000000 bw_processing-0.8.2/tests/fixtures/indexing/datapackage.json
--rw-r--r--   0 cmutel     (501) staff       (20)       69 2021-05-18 13:12:19.000000 bw_processing-0.8.2/tests/fixtures/indexing/vector-csv-both.csv
--rw-r--r--   0 cmutel     (501) staff       (20)       69 2021-05-18 13:12:19.000000 bw_processing-0.8.2/tests/fixtures/indexing/vector-csv-cols.csv
--rw-r--r--   0 cmutel     (501) staff       (20)       69 2021-05-18 13:12:19.000000 bw_processing-0.8.2/tests/fixtures/indexing/vector-csv-rows.csv
--rw-r--r--   0 cmutel     (501) staff       (20)      152 2021-05-18 13:12:19.000000 bw_processing-0.8.2/tests/fixtures/indexing/vector.data.npy
--rw-r--r--   0 cmutel     (501) staff       (20)      131 2021-05-18 13:12:19.000000 bw_processing-0.8.2/tests/fixtures/indexing/vector.flip.npy
--rw-r--r--   0 cmutel     (501) staff       (20)      152 2021-05-18 13:12:19.000000 bw_processing-0.8.2/tests/fixtures/indexing/vector.indices.npy
--rw-r--r--   0 cmutel     (501) staff       (20)      446 2021-02-03 12:37:56.000000 bw_processing-0.8.2/tests/fixtures/lorem.txt
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-09-15 09:46:35.372888 bw_processing-0.8.2/tests/fixtures/merging/
--rw-r--r--   0 cmutel     (501) staff       (20)     1222 2022-04-11 08:58:51.000000 bw_processing-0.8.2/tests/fixtures/merging/merging_first.zip
--rw-r--r--   0 cmutel     (501) staff       (20)     1161 2022-04-11 08:58:51.000000 bw_processing-0.8.2/tests/fixtures/merging/merging_same_1.zip
--rw-r--r--   0 cmutel     (501) staff       (20)      982 2022-04-11 08:58:51.000000 bw_processing-0.8.2/tests/fixtures/merging/merging_same_2.zip
--rw-r--r--   0 cmutel     (501) staff       (20)     1020 2022-04-11 08:58:51.000000 bw_processing-0.8.2/tests/fixtures/merging/merging_second.zip
--rw-r--r--   0 cmutel     (501) staff       (20)     4075 2021-10-29 21:46:22.000000 bw_processing-0.8.2/tests/fixtures/test-fixture.zip
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-09-15 09:46:35.375200 bw_processing-0.8.2/tests/fixtures/tfd/
--rw-r--r--   0 cmutel     (501) staff       (20)     5785 2021-10-29 21:47:26.000000 bw_processing-0.8.2/tests/fixtures/tfd/datapackage.json
--rw-r--r--   0 cmutel     (501) staff       (20)      152 2021-10-29 21:46:22.000000 bw_processing-0.8.2/tests/fixtures/tfd/sa-array-interface.indices.npy
--rw-r--r--   0 cmutel     (501) staff       (20)       38 2021-10-29 21:47:26.000000 bw_processing-0.8.2/tests/fixtures/tfd/sa-data-array-json-metadata.json
--rw-r--r--   0 cmutel     (501) staff       (20)       19 2021-10-29 21:47:26.000000 bw_processing-0.8.2/tests/fixtures/tfd/sa-data-array-json-parameters.json
--rw-r--r--   0 cmutel     (501) staff       (20)      224 2021-10-29 21:46:22.000000 bw_processing-0.8.2/tests/fixtures/tfd/sa-data-array.data.npy
--rw-r--r--   0 cmutel     (501) staff       (20)      131 2021-10-29 21:46:22.000000 bw_processing-0.8.2/tests/fixtures/tfd/sa-data-array.flip.npy
--rw-r--r--   0 cmutel     (501) staff       (20)      152 2021-10-29 21:46:22.000000 bw_processing-0.8.2/tests/fixtures/tfd/sa-data-array.indices.npy
--rw-r--r--   0 cmutel     (501) staff       (20)       36 2021-10-29 21:46:22.000000 bw_processing-0.8.2/tests/fixtures/tfd/sa-data-vector-csv-metadata.csv
--rw-r--r--   0 cmutel     (501) staff       (20)      136 2021-10-29 21:46:22.000000 bw_processing-0.8.2/tests/fixtures/tfd/sa-data-vector-from-dict.data.npy
--rw-r--r--   0 cmutel     (501) staff       (20)      300 2021-10-29 21:46:22.000000 bw_processing-0.8.2/tests/fixtures/tfd/sa-data-vector-from-dict.distributions.npy
--rw-r--r--   0 cmutel     (501) staff       (20)      130 2021-10-29 21:46:22.000000 bw_processing-0.8.2/tests/fixtures/tfd/sa-data-vector-from-dict.flip.npy
--rw-r--r--   0 cmutel     (501) staff       (20)      144 2021-10-29 21:46:22.000000 bw_processing-0.8.2/tests/fixtures/tfd/sa-data-vector-from-dict.indices.npy
--rw-r--r--   0 cmutel     (501) staff       (20)      152 2021-10-29 21:46:22.000000 bw_processing-0.8.2/tests/fixtures/tfd/sa-data-vector.data.npy
--rw-r--r--   0 cmutel     (501) staff       (20)      131 2021-10-29 21:46:22.000000 bw_processing-0.8.2/tests/fixtures/tfd/sa-data-vector.flip.npy
--rw-r--r--   0 cmutel     (501) staff       (20)      152 2021-10-29 21:46:22.000000 bw_processing-0.8.2/tests/fixtures/tfd/sa-data-vector.indices.npy
--rw-r--r--   0 cmutel     (501) staff       (20)      152 2021-10-29 21:46:22.000000 bw_processing-0.8.2/tests/fixtures/tfd/sa-vector-interface.indices.npy
--rw-r--r--   0 cmutel     (501) staff       (20)    12276 2021-10-29 21:47:28.000000 bw_processing-0.8.2/tests/indexing.py
--rw-r--r--   0 cmutel     (501) staff       (20)    13438 2021-10-29 21:47:28.000000 bw_processing-0.8.2/tests/integration.py
--rw-r--r--   0 cmutel     (501) staff       (20)     3562 2021-11-24 11:34:46.000000 bw_processing-0.8.2/tests/interfaces.py
--rw-r--r--   0 cmutel     (501) staff       (20)     2001 2020-09-27 08:12:37.000000 bw_processing-0.8.2/tests/loading.py
--rw-r--r--   0 cmutel     (501) staff       (20)    12562 2022-06-24 07:47:52.000000 bw_processing-0.8.2/tests/merging.py
--rw-r--r--   0 cmutel     (501) staff       (20)      643 2021-11-24 11:33:04.000000 bw_processing-0.8.2/tests/proxies.py
--rw-r--r--   0 cmutel     (501) staff       (20)     6724 2021-11-24 14:12:50.000000 bw_processing-0.8.2/tests/test_utils.py
--rw-r--r--   0 cmutel     (501) staff       (20)     3680 2021-11-24 11:33:04.000000 bw_processing-0.8.2/tests/unique_fields.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-07-24 18:14:42.045572 bw-processing-0.8.3/
+-rw-r--r--   0 cmutel     (501) staff       (20)     1456 2023-07-24 17:35:22.000000 bw-processing-0.8.3/LICENSE
+-rw-r--r--   0 cmutel     (501) staff       (20)       96 2023-07-24 18:05:46.000000 bw-processing-0.8.3/MANIFEST.in
+-rw-r--r--   0 cmutel     (501) staff       (20)    15927 2023-07-24 18:14:42.045636 bw-processing-0.8.3/PKG-INFO
+-rw-r--r--   0 cmutel     (501) staff       (20)    14848 2023-07-24 17:41:45.000000 bw-processing-0.8.3/README.md
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-07-24 18:14:42.044525 bw-processing-0.8.3/bw_processing/
+-rw-r--r--   0 cmutel     (501) staff       (20)        6 2023-07-24 17:56:31.000000 bw-processing-0.8.3/bw_processing/VERSION
+-rw-r--r--   0 cmutel     (501) staff       (20)     1373 2023-07-24 17:37:49.000000 bw-processing-0.8.3/bw_processing/__init__.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     5839 2021-10-06 03:26:26.000000 bw-processing-0.8.3/bw_processing/array_creation.py
+-rw-r--r--   0 cmutel     (501) staff       (20)      916 2021-10-06 03:26:26.000000 bw-processing-0.8.3/bw_processing/constants.py
+-rw-r--r--   0 cmutel     (501) staff       (20)    37578 2022-09-15 09:38:35.000000 bw-processing-0.8.3/bw_processing/datapackage.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     1395 2021-10-29 21:47:27.000000 bw-processing-0.8.3/bw_processing/errors.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-07-24 18:14:42.045346 bw-processing-0.8.3/bw_processing/examples/
+-rw-r--r--   0 cmutel     (501) staff       (20)       73 2020-09-25 13:57:42.000000 bw-processing-0.8.3/bw_processing/examples/__init__.py
+-rw-r--r--   0 cmutel     (501) staff       (20)      602 2021-02-02 15:32:53.000000 bw-processing-0.8.3/bw_processing/examples/interfaces.py
+-rw-r--r--   0 cmutel     (501) staff       (20)      772 2020-09-25 14:01:54.000000 bw-processing-0.8.3/bw_processing/examples/simple.zip
+-rw-r--r--   0 cmutel     (501) staff       (20)     1632 2021-10-06 03:26:26.000000 bw-processing-0.8.3/bw_processing/filesystem.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     5612 2021-10-06 03:26:26.000000 bw-processing-0.8.3/bw_processing/indexing.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     2915 2022-09-15 09:32:21.000000 bw-processing-0.8.3/bw_processing/io_helpers.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     6291 2022-06-24 07:47:52.000000 bw-processing-0.8.3/bw_processing/merging.py
+-rw-r--r--   0 cmutel     (501) staff       (20)      484 2021-10-04 13:16:47.000000 bw-processing-0.8.3/bw_processing/proxies.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     3819 2021-10-06 03:26:26.000000 bw-processing-0.8.3/bw_processing/unique_fields.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     3372 2023-07-24 17:37:17.000000 bw-processing-0.8.3/bw_processing/utils.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-07-24 18:14:42.045246 bw-processing-0.8.3/bw_processing.egg-info/
+-rw-r--r--   0 cmutel     (501) staff       (20)    15927 2023-07-24 18:14:42.000000 bw-processing-0.8.3/bw_processing.egg-info/PKG-INFO
+-rw-r--r--   0 cmutel     (501) staff       (20)      902 2023-07-24 18:14:42.000000 bw-processing-0.8.3/bw_processing.egg-info/SOURCES.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)        1 2023-07-24 18:14:42.000000 bw-processing-0.8.3/bw_processing.egg-info/dependency_links.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)        1 2023-07-24 17:56:05.000000 bw-processing-0.8.3/bw_processing.egg-info/not-zip-safe
+-rw-r--r--   0 cmutel     (501) staff       (20)      113 2023-07-24 18:14:42.000000 bw-processing-0.8.3/bw_processing.egg-info/requires.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)       34 2023-07-24 18:14:42.000000 bw-processing-0.8.3/bw_processing.egg-info/top_level.txt
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-07-24 18:14:42.044170 bw-processing-0.8.3/dev/
+-rw-r--r--   0 cmutel     (501) staff       (20)     6528 2020-09-21 12:42:34.000000 bw-processing-0.8.3/dev/calculation_package.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     4240 2021-01-04 10:17:38.000000 bw-processing-0.8.3/dev/loading.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     9654 2021-01-04 10:17:38.000000 bw-processing-0.8.3/dev/processed_package.py
+-rw-r--r--   0 cmutel     (501) staff       (20)      741 2021-01-04 10:17:38.000000 bw-processing-0.8.3/dev/resources.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     1195 2020-10-02 12:58:54.000000 bw-processing-0.8.3/dev/speed_tests.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-07-24 18:14:42.044304 bw-processing-0.8.3/docs/
+-rw-r--r--   0 cmutel     (501) staff       (20)     1151 2023-07-24 17:35:22.000000 bw-processing-0.8.3/docs/conf.py
+-rw-r--r--   0 cmutel     (501) staff       (20)       87 2023-07-24 17:35:22.000000 bw-processing-0.8.3/pyproject.toml
+-rw-r--r--   0 cmutel     (501) staff       (20)     1660 2023-07-24 18:14:42.046009 bw-processing-0.8.3/setup.cfg
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-07-24 18:14:42.045481 bw-processing-0.8.3/tests/
+-rw-r--r--   0 cmutel     (501) staff       (20)     6724 2021-11-24 14:12:50.000000 bw-processing-0.8.3/tests/test_utils.py
```

### Comparing `bw_processing-0.8.2/LICENSE` & `bw-processing-0.8.3/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,11 @@
-BSD 3-Clause License
+Copyright 2023 Chris Mutel
 
-Copyright (c) 2019, Chris Mutel
-All rights reserved.
+Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
+1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 
-* Redistributions of source code must retain the above copyright notice, this
-  list of conditions and the following disclaimer.
+2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 
-* Redistributions in binary form must reproduce the above copyright notice,
-  this list of conditions and the following disclaimer in the documentation
-  and/or other materials provided with the distribution.
+3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 
-* Neither the name of the copyright holder nor the names of its
-  contributors may be used to endorse or promote products derived from
-  this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `bw_processing-0.8.2/PKG-INFO` & `bw-processing-0.8.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,29 @@
-Metadata-Version: 2.1
-Name: bw_processing
-Version: 0.8.2
-Summary: Tools to create structured arrays in a common format
-Home-page: https://github.com/brightway-lca/bw_processing
-Author: Chris Mutel
-Author-email: cmutel@gmail.com
-License: BSD 3-clause
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Scientific/Engineering :: Visualization
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# bw_processing
+# bw-processing
 
 Library for storing numeric data for use in matrix-based calculations. Designed for use with the [Brightway life cycle assessment framework](https://brightway.dev/).
 
-[![Azure Status](https://dev.azure.com/mutel/Brightway%20CI/_apis/build/status/brightway-lca.bw_processing?branchName=master)](https://dev.azure.com/mutel/Brightway%20CI/_build/latest?definitionId=7&branchName=master) [![Travis Status](https://travis-ci.org/brightway-lca/bw_processing.svg?branch=master)](https://travis-ci.org/brightway-lca/bw_processing) [![Coverage Status](https://coveralls.io/repos/github/brightway-lca/bw_processing/badge.svg?branch=master)](https://coveralls.io/github/brightway-lca/bw_processing?branch=master) [![Documentation](https://readthedocs.org/projects/bw-processing/badge/?version=latest)](https://bw-processing.readthedocs.io/en/latest/)
+[![PyPI](https://img.shields.io/pypi/v/bw-processing.svg)][pypi status]
+[![Status](https://img.shields.io/pypi/status/bw-processing.svg)][pypi status]
+[![Python Version](https://img.shields.io/pypi/pyversions/bw-processing)][pypi status]
+[![License](https://img.shields.io/pypi/l/bw-processing)][license]
+
+[![Read the documentation at https://bw-processing.readthedocs.io/](https://img.shields.io/readthedocs/bw-processing/latest.svg?label=Read%20the%20Docs)][read the docs]
+[![Tests](https://github.com/brightway-lca/bw-processing/actions/workflows/python-test.yml/badge.svg)][tests]
+[![Codecov](https://codecov.io/gh/brightway-lca/bw-processing/branch/main/graph/badge.svg)][codecov]
+
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]
+[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
+
+[pypi status]: https://pypi.org/project/bw-processing/
+[read the docs]: https://bw-processing.readthedocs.io/
+[tests]: https://github.com/brightway-lca/bw-processing/actions?workflow=Tests
+[codecov]: https://app.codecov.io/gh/brightway-lca/bw-processing
+[pre-commit]: https://github.com/pre-commit/pre-commit
+[black]: https://github.com/psf/black
 
 ## Table of Contents
 
 - [Background](#background)
 - [Concepts](#concepts)
 - [Install](#install)
 - [Usage](#usage)
@@ -225,7 +216,14 @@
 ## Maintainers
 
 * [Chris Mutel](https://github.com/cmutel/)
 
 ## License
 
 [BSD-3-Clause](https://github.com/brightway-lca/bw_processing/blob/master/LICENSE). Copyright 2020 Chris Mutel.
+
+<!-- github-only -->
+
+[command-line reference]: https://bw-processing.readthedocs.io/en/latest/usage.html
+[License]: https://github.com/brightway-lca/bw-processing/blob/main/LICENSE
+[Contributor Guide]: https://github.com/brightway-lca/bw-processing/blob/main/CONTRIBUTING.md
+[Issue Tracker]: https://github.com/brightway-lca/bw-processing/issues
```

### Comparing `bw_processing-0.8.2/README.md` & `bw-processing-0.8.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,58 @@
-# bw_processing
+Metadata-Version: 2.1
+Name: bw-processing
+Version: 0.8.3
+Summary: Tools to create structured arrays in a common format
+Home-page: https://github.com/brightway-lca/bw_processing
+Author: Chris Mutel
+Author-email: <cmutel@gmail.com>
+Maintainer: Chris Mutel
+Maintainer-email: <cmutel@gmail.com>
+License: BSD-3-Clause
+Project-URL: source, https://github.com/brightway-lca/bw_processing
+Project-URL: homepage, https://github.com/brightway-lca/bw_processing
+Project-URL: tracker, https://github.com/brightway-lca/bw_processing/issues
+Keywords: "brightway","development"
+Platform: any
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown; charset=UTF-8
+Provides-Extra: testing
+Provides-Extra: dev
+Provides-Extra: docs
+License-File: LICENSE
+
+# bw-processing
 
 Library for storing numeric data for use in matrix-based calculations. Designed for use with the [Brightway life cycle assessment framework](https://brightway.dev/).
 
-[![Azure Status](https://dev.azure.com/mutel/Brightway%20CI/_apis/build/status/brightway-lca.bw_processing?branchName=master)](https://dev.azure.com/mutel/Brightway%20CI/_build/latest?definitionId=7&branchName=master) [![Travis Status](https://travis-ci.org/brightway-lca/bw_processing.svg?branch=master)](https://travis-ci.org/brightway-lca/bw_processing) [![Coverage Status](https://coveralls.io/repos/github/brightway-lca/bw_processing/badge.svg?branch=master)](https://coveralls.io/github/brightway-lca/bw_processing?branch=master) [![Documentation](https://readthedocs.org/projects/bw-processing/badge/?version=latest)](https://bw-processing.readthedocs.io/en/latest/)
+[![PyPI](https://img.shields.io/pypi/v/bw-processing.svg)][pypi status]
+[![Status](https://img.shields.io/pypi/status/bw-processing.svg)][pypi status]
+[![Python Version](https://img.shields.io/pypi/pyversions/bw-processing)][pypi status]
+[![License](https://img.shields.io/pypi/l/bw-processing)][license]
+
+[![Read the documentation at https://bw-processing.readthedocs.io/](https://img.shields.io/readthedocs/bw-processing/latest.svg?label=Read%20the%20Docs)][read the docs]
+[![Tests](https://github.com/brightway-lca/bw-processing/actions/workflows/python-test.yml/badge.svg)][tests]
+[![Codecov](https://codecov.io/gh/brightway-lca/bw-processing/branch/main/graph/badge.svg)][codecov]
+
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]
+[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
+
+[pypi status]: https://pypi.org/project/bw-processing/
+[read the docs]: https://bw-processing.readthedocs.io/
+[tests]: https://github.com/brightway-lca/bw-processing/actions?workflow=Tests
+[codecov]: https://app.codecov.io/gh/brightway-lca/bw-processing
+[pre-commit]: https://github.com/pre-commit/pre-commit
+[black]: https://github.com/psf/black
 
 ## Table of Contents
 
 - [Background](#background)
 - [Concepts](#concepts)
 - [Install](#install)
 - [Usage](#usage)
@@ -199,7 +245,14 @@
 ## Maintainers
 
 * [Chris Mutel](https://github.com/cmutel/)
 
 ## License
 
 [BSD-3-Clause](https://github.com/brightway-lca/bw_processing/blob/master/LICENSE). Copyright 2020 Chris Mutel.
+
+<!-- github-only -->
+
+[command-line reference]: https://bw-processing.readthedocs.io/en/latest/usage.html
+[License]: https://github.com/brightway-lca/bw-processing/blob/main/LICENSE
+[Contributor Guide]: https://github.com/brightway-lca/bw-processing/blob/main/CONTRIBUTING.md
+[Issue Tracker]: https://github.com/brightway-lca/bw-processing/issues
```

### Comparing `bw_processing-0.8.2/bw_processing/__init__.py` & `bw-processing-0.8.3/bw_processing/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     "reset_index",
     "safe_filename",
     "simple_graph",
     "UNCERTAINTY_DTYPE",
     "UndefinedInterface",
 )
 
+
 from .array_creation import create_array, create_structured_array
 from .constants import DEFAULT_LICENSES, INDICES_DTYPE, UNCERTAINTY_DTYPE
 from .datapackage import (
     Datapackage,
     DatapackageBase,
     FilteredDatapackage,
     create_datapackage,
@@ -38,8 +39,10 @@
 from .examples import examples_dir
 from .filesystem import clean_datapackage_name, md5, safe_filename
 from .indexing import reindex, reset_index
 from .io_helpers import generic_directory_filesystem, generic_zipfile_filesystem
 from .merging import merge_datapackages_with_mask
 from .proxies import UndefinedInterface
 from .unique_fields import as_unique_attributes, as_unique_attributes_dataframe
-from .version import version as __version__
+
+from .utils import get_version_tuple
+__version__ = get_version_tuple()
```

### Comparing `bw_processing-0.8.2/bw_processing/array_creation.py` & `bw-processing-0.8.3/bw_processing/array_creation.py`

 * *Files identical despite different names*

### Comparing `bw_processing-0.8.2/bw_processing/constants.py` & `bw-processing-0.8.3/bw_processing/constants.py`

 * *Files identical despite different names*

### Comparing `bw_processing-0.8.2/bw_processing/datapackage.py` & `bw-processing-0.8.3/bw_processing/datapackage.py`

 * *Files identical despite different names*

### Comparing `bw_processing-0.8.2/bw_processing/errors.py` & `bw-processing-0.8.3/bw_processing/errors.py`

 * *Files identical despite different names*

### Comparing `bw_processing-0.8.2/bw_processing/examples/interfaces.py` & `bw-processing-0.8.3/bw_processing/examples/interfaces.py`

 * *Files identical despite different names*

### Comparing `bw_processing-0.8.2/bw_processing/examples/simple.zip` & `bw-processing-0.8.3/bw_processing/examples/simple.zip`

 * *Files identical despite different names*

### Comparing `bw_processing-0.8.2/bw_processing/filesystem.py` & `bw-processing-0.8.3/bw_processing/filesystem.py`

 * *Files identical despite different names*

### Comparing `bw_processing-0.8.2/bw_processing/indexing.py` & `bw-processing-0.8.3/bw_processing/indexing.py`

 * *Files identical despite different names*

### Comparing `bw_processing-0.8.2/bw_processing/io_helpers.py` & `bw-processing-0.8.3/bw_processing/io_helpers.py`

 * *Files identical despite different names*

### Comparing `bw_processing-0.8.2/bw_processing/merging.py` & `bw-processing-0.8.3/bw_processing/merging.py`

 * *Files identical despite different names*

### Comparing `bw_processing-0.8.2/bw_processing/unique_fields.py` & `bw-processing-0.8.3/bw_processing/unique_fields.py`

 * *Files identical despite different names*

### Comparing `bw_processing-0.8.2/bw_processing/utils.py` & `bw-processing-0.8.3/bw_processing/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,37 @@
 from io import BytesIO
 from pathlib import Path
 from typing import Any, Union
+import importlib.metadata
 
 import numpy as np
 from numpy.lib.recfunctions import repack_fields
 
 from .array_creation import create_structured_array
 from .constants import INDICES_DTYPE, NAME_RE, UNCERTAINTY_DTYPE
 from .errors import InvalidName
 
 
+def get_version_tuple() -> tuple:
+    """Returns version as (major, minor, micro)."""
+
+    def as_integer(version_str: str) -> Union[int, str]:
+        try:
+            return int(version_str)
+        except ValueError:
+            return version_str
+
+    return tuple(
+        as_integer(v)
+        for v in importlib.metadata.version("bw_processing")
+        .strip()
+        .split(".")
+    )
+
+
 def load_bytes(obj: Any) -> Any:
     if isinstance(obj, BytesIO):
         try:
             # Go to the beginning of content
             obj.seek(0)
             return np.load(obj, allow_pickle=False)
         except ValueError:
```

### Comparing `bw_processing-0.8.2/bw_processing.egg-info/PKG-INFO` & `bw-processing-0.8.3/bw_processing.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,58 @@
 Metadata-Version: 2.1
 Name: bw-processing
-Version: 0.8.2
+Version: 0.8.3
 Summary: Tools to create structured arrays in a common format
 Home-page: https://github.com/brightway-lca/bw_processing
 Author: Chris Mutel
-Author-email: cmutel@gmail.com
-License: BSD 3-clause
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
+Author-email: <cmutel@gmail.com>
+Maintainer: Chris Mutel
+Maintainer-email: <cmutel@gmail.com>
+License: BSD-3-Clause
+Project-URL: source, https://github.com/brightway-lca/bw_processing
+Project-URL: homepage, https://github.com/brightway-lca/bw_processing
+Project-URL: tracker, https://github.com/brightway-lca/bw_processing/issues
+Keywords: "brightway","development"
+Platform: any
+Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Scientific/Engineering :: Visualization
-Description-Content-Type: text/markdown
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown; charset=UTF-8
+Provides-Extra: testing
+Provides-Extra: dev
+Provides-Extra: docs
 License-File: LICENSE
 
-# bw_processing
+# bw-processing
 
 Library for storing numeric data for use in matrix-based calculations. Designed for use with the [Brightway life cycle assessment framework](https://brightway.dev/).
 
-[![Azure Status](https://dev.azure.com/mutel/Brightway%20CI/_apis/build/status/brightway-lca.bw_processing?branchName=master)](https://dev.azure.com/mutel/Brightway%20CI/_build/latest?definitionId=7&branchName=master) [![Travis Status](https://travis-ci.org/brightway-lca/bw_processing.svg?branch=master)](https://travis-ci.org/brightway-lca/bw_processing) [![Coverage Status](https://coveralls.io/repos/github/brightway-lca/bw_processing/badge.svg?branch=master)](https://coveralls.io/github/brightway-lca/bw_processing?branch=master) [![Documentation](https://readthedocs.org/projects/bw-processing/badge/?version=latest)](https://bw-processing.readthedocs.io/en/latest/)
+[![PyPI](https://img.shields.io/pypi/v/bw-processing.svg)][pypi status]
+[![Status](https://img.shields.io/pypi/status/bw-processing.svg)][pypi status]
+[![Python Version](https://img.shields.io/pypi/pyversions/bw-processing)][pypi status]
+[![License](https://img.shields.io/pypi/l/bw-processing)][license]
+
+[![Read the documentation at https://bw-processing.readthedocs.io/](https://img.shields.io/readthedocs/bw-processing/latest.svg?label=Read%20the%20Docs)][read the docs]
+[![Tests](https://github.com/brightway-lca/bw-processing/actions/workflows/python-test.yml/badge.svg)][tests]
+[![Codecov](https://codecov.io/gh/brightway-lca/bw-processing/branch/main/graph/badge.svg)][codecov]
+
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]
+[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
+
+[pypi status]: https://pypi.org/project/bw-processing/
+[read the docs]: https://bw-processing.readthedocs.io/
+[tests]: https://github.com/brightway-lca/bw-processing/actions?workflow=Tests
+[codecov]: https://app.codecov.io/gh/brightway-lca/bw-processing
+[pre-commit]: https://github.com/pre-commit/pre-commit
+[black]: https://github.com/psf/black
 
 ## Table of Contents
 
 - [Background](#background)
 - [Concepts](#concepts)
 - [Install](#install)
 - [Usage](#usage)
@@ -225,7 +245,14 @@
 ## Maintainers
 
 * [Chris Mutel](https://github.com/cmutel/)
 
 ## License
 
 [BSD-3-Clause](https://github.com/brightway-lca/bw_processing/blob/master/LICENSE). Copyright 2020 Chris Mutel.
+
+<!-- github-only -->
+
+[command-line reference]: https://bw-processing.readthedocs.io/en/latest/usage.html
+[License]: https://github.com/brightway-lca/bw-processing/blob/main/LICENSE
+[Contributor Guide]: https://github.com/brightway-lca/bw-processing/blob/main/CONTRIBUTING.md
+[Issue Tracker]: https://github.com/brightway-lca/bw-processing/issues
```

### Comparing `bw_processing-0.8.2/dev/calculation_package.py` & `bw-processing-0.8.3/dev/calculation_package.py`

 * *Files identical despite different names*

### Comparing `bw_processing-0.8.2/dev/loading.py` & `bw-processing-0.8.3/dev/loading.py`

 * *Files identical despite different names*

### Comparing `bw_processing-0.8.2/dev/processed_package.py` & `bw-processing-0.8.3/dev/processed_package.py`

 * *Files identical despite different names*

### Comparing `bw_processing-0.8.2/dev/resources.py` & `bw-processing-0.8.3/dev/resources.py`

 * *Files identical despite different names*

### Comparing `bw_processing-0.8.2/dev/speed_tests.py` & `bw-processing-0.8.3/dev/speed_tests.py`

 * *Files identical despite different names*

### Comparing `bw_processing-0.8.2/tests/test_utils.py` & `bw-processing-0.8.3/tests/test_utils.py`

 * *Files identical despite different names*

