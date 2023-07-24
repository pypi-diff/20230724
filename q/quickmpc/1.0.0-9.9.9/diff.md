# Comparing `tmp/quickmpc-1.0.0.tar.gz` & `tmp/quickmpc-9.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/QuickMPC/QuickMPC/packages/client/libclient-py/dist/.tmp-vpxq77ha/quickmpc-1.0.0.tar", last modified: Fri Jul 21 11:55:04 2023, max compression
+gzip compressed data, was "/home/runner/work/QuickMPC/QuickMPC/packages/client/libclient-py/dist/.tmp-tx9v318i/quickmpc-9.9.9.tar", last modified: Mon Jul 24 06:37:23 2023, max compression
```

## Comparing `quickmpc-1.0.0.tar` & `quickmpc-9.9.9.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:55:04.000000 quickmpc-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-21 11:54:49.000000 quickmpc-1.0.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-21 11:54:49.000000 quickmpc-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-21 11:54:49.000000 quickmpc-1.0.0/.isort.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:55:04.000000 quickmpc-1.0.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-21 11:54:49.000000 quickmpc-1.0.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-21 11:54:49.000000 quickmpc-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-21 11:54:49.000000 quickmpc-1.0.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-21 11:55:04.000000 quickmpc-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-21 11:54:49.000000 quickmpc-1.0.0/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    38439 2023-07-21 11:54:49.000000 quickmpc-1.0.0/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-21 11:54:49.000000 quickmpc-1.0.0/README-ja.md
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-21 11:54:49.000000 quickmpc-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-21 11:54:49.000000 quickmpc-1.0.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-21 11:54:49.000000 quickmpc-1.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:55:04.000000 quickmpc-1.0.0/quickmpc/
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-21 11:55:04.000000 quickmpc-1.0.0/quickmpc/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:55:04.000000 quickmpc-1.0.0/quickmpc/pandas/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/pandas/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/pandas/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/pandas/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8643 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/pandas/share_data_frame.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:55:04.000000 quickmpc-1.0.0/quickmpc/proto/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/proto/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/proto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:55:04.000000 quickmpc-1.0.0/quickmpc/proto/common_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/proto/common_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/proto/common_types/common_types_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9351 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/proto/common_types/common_types_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12847 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/proto/libc_to_manage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13511 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/proto/libc_to_manage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17455 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/proto/libc_to_manage_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/proto/libc_to_manage_pb2_grpc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/qmpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/qmpc_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:55:04.000000 quickmpc-1.0.0/quickmpc/request/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19239 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/request/qmpc_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/request/qmpc_request_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/request/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:55:04.000000 quickmpc-1.0.0/quickmpc/share/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/share/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/share/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/share/restore.py
--rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/share/share.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:55:04.000000 quickmpc-1.0.0/quickmpc/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/utils/if_present.py
--rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/utils/make_pieces.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/utils/overload_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:55:04.000000 quickmpc-1.0.0/quickmpc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-21 11:55:04.000000 quickmpc-1.0.0/quickmpc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-07-21 11:55:04.000000 quickmpc-1.0.0/quickmpc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 11:55:04.000000 quickmpc-1.0.0/quickmpc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-21 11:55:04.000000 quickmpc-1.0.0/quickmpc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-21 11:55:04.000000 quickmpc-1.0.0/quickmpc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-21 11:55:04.000000 quickmpc-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-21 11:54:49.000000 quickmpc-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:55:04.000000 quickmpc-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:55:04.000000 quickmpc-1.0.0/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/local_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:55:04.000000 quickmpc-1.0.0/tests/unit_tests/pandas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/pandas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:55:04.000000 quickmpc-1.0.0/tests/unit_tests/pandas/test_files/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/pandas/test_files/bitvector.csv
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/pandas/test_files/diff_col.csv
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/pandas/test_files/edge_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/pandas/test_files/empty.csv
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/pandas/test_files/none.csv
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/pandas/test_files/normal.csv
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/pandas/test_files/not_csv.csv
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/pandas/test_files/over_number.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/pandas/test_files/string_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/pandas/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/pandas/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/pandas/test_share_data_frame.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:55:04.000000 quickmpc-1.0.0/tests/unit_tests/request/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6565 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/request/test_qmpc_request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:55:04.000000 quickmpc-1.0.0/tests/unit_tests/share/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/share/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/share/test_random.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/share/test_restore.py
--rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/share/test_share_recons.py
--rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/share/test_share_sharize.py
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/test_qmpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:55:04.000000 quickmpc-1.0.0/tests/unit_tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/utils/test_make_pieces.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/utils/test_over_load.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:37:23.000000 quickmpc-9.9.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-24 06:36:55.000000 quickmpc-9.9.9/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-24 06:36:55.000000 quickmpc-9.9.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-24 06:36:55.000000 quickmpc-9.9.9/.isort.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:37:23.000000 quickmpc-9.9.9/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-24 06:36:55.000000 quickmpc-9.9.9/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-24 06:36:55.000000 quickmpc-9.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-24 06:36:55.000000 quickmpc-9.9.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-24 06:37:23.000000 quickmpc-9.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-24 06:36:55.000000 quickmpc-9.9.9/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    38439 2023-07-24 06:36:55.000000 quickmpc-9.9.9/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-24 06:36:55.000000 quickmpc-9.9.9/README-ja.md
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-24 06:36:55.000000 quickmpc-9.9.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-24 06:36:55.000000 quickmpc-9.9.9/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-24 06:36:55.000000 quickmpc-9.9.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:37:23.000000 quickmpc-9.9.9/quickmpc/
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-24 06:36:55.000000 quickmpc-9.9.9/quickmpc/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-24 06:36:55.000000 quickmpc-9.9.9/quickmpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-24 06:37:23.000000 quickmpc-9.9.9/quickmpc/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-24 06:36:55.000000 quickmpc-9.9.9/quickmpc/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:37:23.000000 quickmpc-9.9.9/quickmpc/pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-24 06:36:55.000000 quickmpc-9.9.9/quickmpc/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-07-24 06:36:55.000000 quickmpc-9.9.9/quickmpc/pandas/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-24 06:36:55.000000 quickmpc-9.9.9/quickmpc/pandas/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-24 06:36:55.000000 quickmpc-9.9.9/quickmpc/pandas/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8643 2023-07-24 06:36:55.000000 quickmpc-9.9.9/quickmpc/pandas/share_data_frame.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:37:23.000000 quickmpc-9.9.9/quickmpc/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-24 06:36:55.000000 quickmpc-9.9.9/quickmpc/proto/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-24 06:36:55.000000 quickmpc-9.9.9/quickmpc/proto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:37:23.000000 quickmpc-9.9.9/quickmpc/proto/common_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 06:36:55.000000 quickmpc-9.9.9/quickmpc/proto/common_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-07-24 06:36:55.000000 quickmpc-9.9.9/quickmpc/proto/common_types/common_types_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9351 2023-07-24 06:36:55.000000 quickmpc-9.9.9/quickmpc/proto/common_types/common_types_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12847 2023-07-24 06:36:55.000000 quickmpc-9.9.9/quickmpc/proto/libc_to_manage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13511 2023-07-24 06:36:55.000000 quickmpc-9.9.9/quickmpc/proto/libc_to_manage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17455 2023-07-24 06:36:55.000000 quickmpc-9.9.9/quickmpc/proto/libc_to_manage_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-07-24 06:36:55.000000 quickmpc-9.9.9/quickmpc/proto/libc_to_manage_pb2_grpc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-07-24 06:36:55.000000 quickmpc-9.9.9/quickmpc/qmpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-24 06:36:55.000000 quickmpc-9.9.9/quickmpc/qmpc_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:37:23.000000 quickmpc-9.9.9/quickmpc/request/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-24 06:36:55.000000 quickmpc-9.9.9/quickmpc/request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19239 2023-07-24 06:36:55.000000 quickmpc-9.9.9/quickmpc/request/qmpc_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-07-24 06:36:55.000000 quickmpc-9.9.9/quickmpc/request/qmpc_request_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-24 06:36:55.000000 quickmpc-9.9.9/quickmpc/request/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:37:23.000000 quickmpc-9.9.9/quickmpc/share/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-24 06:36:55.000000 quickmpc-9.9.9/quickmpc/share/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-07-24 06:36:55.000000 quickmpc-9.9.9/quickmpc/share/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-24 06:36:55.000000 quickmpc-9.9.9/quickmpc/share/restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-07-24 06:36:55.000000 quickmpc-9.9.9/quickmpc/share/share.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:37:23.000000 quickmpc-9.9.9/quickmpc/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-24 06:36:55.000000 quickmpc-9.9.9/quickmpc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-24 06:36:55.000000 quickmpc-9.9.9/quickmpc/utils/if_present.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-07-24 06:36:55.000000 quickmpc-9.9.9/quickmpc/utils/make_pieces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-07-24 06:36:55.000000 quickmpc-9.9.9/quickmpc/utils/overload_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-24 06:36:55.000000 quickmpc-9.9.9/quickmpc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:37:23.000000 quickmpc-9.9.9/quickmpc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-24 06:37:23.000000 quickmpc-9.9.9/quickmpc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-07-24 06:37:23.000000 quickmpc-9.9.9/quickmpc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 06:37:23.000000 quickmpc-9.9.9/quickmpc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-24 06:37:23.000000 quickmpc-9.9.9/quickmpc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-24 06:37:23.000000 quickmpc-9.9.9/quickmpc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-24 06:37:23.000000 quickmpc-9.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-24 06:36:55.000000 quickmpc-9.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:37:23.000000 quickmpc-9.9.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 06:36:55.000000 quickmpc-9.9.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:37:23.000000 quickmpc-9.9.9/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-24 06:36:55.000000 quickmpc-9.9.9/tests/unit_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-24 06:36:55.000000 quickmpc-9.9.9/tests/unit_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-07-24 06:36:55.000000 quickmpc-9.9.9/tests/unit_tests/local_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:37:23.000000 quickmpc-9.9.9/tests/unit_tests/pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 06:36:55.000000 quickmpc-9.9.9/tests/unit_tests/pandas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:37:23.000000 quickmpc-9.9.9/tests/unit_tests/pandas/test_files/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-24 06:36:55.000000 quickmpc-9.9.9/tests/unit_tests/pandas/test_files/bitvector.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-24 06:36:55.000000 quickmpc-9.9.9/tests/unit_tests/pandas/test_files/diff_col.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-24 06:36:55.000000 quickmpc-9.9.9/tests/unit_tests/pandas/test_files/edge_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-24 06:36:55.000000 quickmpc-9.9.9/tests/unit_tests/pandas/test_files/empty.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-24 06:36:55.000000 quickmpc-9.9.9/tests/unit_tests/pandas/test_files/none.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-24 06:36:55.000000 quickmpc-9.9.9/tests/unit_tests/pandas/test_files/normal.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-24 06:36:55.000000 quickmpc-9.9.9/tests/unit_tests/pandas/test_files/not_csv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-24 06:36:55.000000 quickmpc-9.9.9/tests/unit_tests/pandas/test_files/over_number.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-24 06:36:55.000000 quickmpc-9.9.9/tests/unit_tests/pandas/test_files/string_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-07-24 06:36:55.000000 quickmpc-9.9.9/tests/unit_tests/pandas/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-24 06:36:55.000000 quickmpc-9.9.9/tests/unit_tests/pandas/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-07-24 06:36:55.000000 quickmpc-9.9.9/tests/unit_tests/pandas/test_share_data_frame.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:37:23.000000 quickmpc-9.9.9/tests/unit_tests/request/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 06:36:55.000000 quickmpc-9.9.9/tests/unit_tests/request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6565 2023-07-24 06:36:55.000000 quickmpc-9.9.9/tests/unit_tests/request/test_qmpc_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:37:23.000000 quickmpc-9.9.9/tests/unit_tests/share/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 06:36:55.000000 quickmpc-9.9.9/tests/unit_tests/share/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-24 06:36:55.000000 quickmpc-9.9.9/tests/unit_tests/share/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-24 06:36:55.000000 quickmpc-9.9.9/tests/unit_tests/share/test_restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-07-24 06:36:55.000000 quickmpc-9.9.9/tests/unit_tests/share/test_share_recons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-07-24 06:36:55.000000 quickmpc-9.9.9/tests/unit_tests/share/test_share_sharize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-07-24 06:36:55.000000 quickmpc-9.9.9/tests/unit_tests/test_qmpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:37:23.000000 quickmpc-9.9.9/tests/unit_tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 06:36:55.000000 quickmpc-9.9.9/tests/unit_tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-07-24 06:36:55.000000 quickmpc-9.9.9/tests/unit_tests/utils/test_make_pieces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-24 06:36:55.000000 quickmpc-9.9.9/tests/unit_tests/utils/test_over_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-24 06:36:55.000000 quickmpc-9.9.9/tox.ini
```

### Comparing `quickmpc-1.0.0/.vscode/settings.json` & `quickmpc-9.9.9/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `quickmpc-1.0.0/LICENSE` & `quickmpc-9.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `quickmpc-1.0.0/Pipfile.lock` & `quickmpc-9.9.9/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `quickmpc-1.0.0/README-ja.md` & `quickmpc-9.9.9/README-ja.md`

 * *Files identical despite different names*

### Comparing `quickmpc-1.0.0/README.md` & `quickmpc-9.9.9/README.md`

 * *Files identical despite different names*

### Comparing `quickmpc-1.0.0/mypy.ini` & `quickmpc-9.9.9/mypy.ini`

 * *Files identical despite different names*

### Comparing `quickmpc-1.0.0/quickmpc/README.md` & `quickmpc-9.9.9/quickmpc/README.md`

 * *Files identical despite different names*

### Comparing `quickmpc-1.0.0/quickmpc/pandas/parser.py` & `quickmpc-9.9.9/quickmpc/pandas/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,19 +71,20 @@
     try:
         return float(val)
     except ValueError:
         # k,m are constants used in the comparison operation
         # Due to the limitation of comparison operation,
         # k bits are taken out and divided by 2^m.
         k: int = 48
-        m: int = 20
+        # m: int = 20
         hs: str = sha512(val.encode()).hexdigest()
         val_int: int = int(hs[:(k >> 2)], 16)
-        val_float: float = val_int / pow(2, m)
-        return val_float
+        # val_float: float = val_int / pow(2, m)
+        # return val_float
+        return val_int
 
 
 def to_int(val: str, encoding='utf-8') -> int:
     encoded = val.encode(encoding)
     return int.from_bytes(encoded, byteorder='big')
```

### Comparing `quickmpc-1.0.0/quickmpc/pandas/progress.py` & `quickmpc-9.9.9/quickmpc/pandas/progress.py`

 * *Files identical despite different names*

### Comparing `quickmpc-1.0.0/quickmpc/pandas/readers.py` & `quickmpc-9.9.9/quickmpc/pandas/readers.py`

 * *Files identical despite different names*

### Comparing `quickmpc-1.0.0/quickmpc/pandas/share_data_frame.py` & `quickmpc-9.9.9/quickmpc/pandas/share_data_frame.py`

 * *Files identical despite different names*

### Comparing `quickmpc-1.0.0/quickmpc/proto/common_types/common_types_pb2.py` & `quickmpc-9.9.9/quickmpc/proto/common_types/common_types_pb2.py`

 * *Files identical despite different names*

### Comparing `quickmpc-1.0.0/quickmpc/proto/common_types/common_types_pb2.pyi` & `quickmpc-9.9.9/quickmpc/proto/common_types/common_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `quickmpc-1.0.0/quickmpc/proto/libc_to_manage_pb2.py` & `quickmpc-9.9.9/quickmpc/proto/libc_to_manage_pb2.py`

 * *Files identical despite different names*

### Comparing `quickmpc-1.0.0/quickmpc/proto/libc_to_manage_pb2.pyi` & `quickmpc-9.9.9/quickmpc/proto/libc_to_manage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `quickmpc-1.0.0/quickmpc/proto/libc_to_manage_pb2_grpc.py` & `quickmpc-9.9.9/quickmpc/proto/libc_to_manage_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `quickmpc-1.0.0/quickmpc/proto/libc_to_manage_pb2_grpc.pyi` & `quickmpc-9.9.9/quickmpc/proto/libc_to_manage_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `quickmpc-1.0.0/quickmpc/qmpc.py` & `quickmpc-9.9.9/quickmpc/qmpc.py`

 * *Files identical despite different names*

### Comparing `quickmpc-1.0.0/quickmpc/request/qmpc_request.py` & `quickmpc-9.9.9/quickmpc/request/qmpc_request.py`

 * *Files identical despite different names*

### Comparing `quickmpc-1.0.0/quickmpc/request/qmpc_request_interface.py` & `quickmpc-9.9.9/quickmpc/request/qmpc_request_interface.py`

 * *Files identical despite different names*

### Comparing `quickmpc-1.0.0/quickmpc/request/response.py` & `quickmpc-9.9.9/quickmpc/request/response.py`

 * *Files identical despite different names*

### Comparing `quickmpc-1.0.0/quickmpc/share/random.py` & `quickmpc-9.9.9/quickmpc/share/random.py`

 * *Files 18% similar despite different names*

```diff
@@ -42,17 +42,22 @@
         byte_val: bytes = random(interval_byte)
         int_val = int.from_bytes(byte_val, "big")
         return int_val % (b - a) + a
 
     @get.register(Decimal)
     def __get_decimal(self, a: Decimal, b: Decimal) -> Decimal:
         # 256bit整数を取り出して[a,b]に正規化する
+        # self.__exception_check(a, b)
+        # val: int = self.get(self.mn, self.mx)
+        # return Decimal(val-self.mn)/(self.mx-self.mn)*(b-a)+a
         self.__exception_check(a, b)
-        val: int = self.get(self.mn, self.mx)
-        return Decimal(val-self.mn)/(self.mx-self.mn)*(b-a)+a
+        interval_byte = self.__get_byte_size(b-a)
+        byte_val: bytes = random(interval_byte)
+        int_val = int.from_bytes(byte_val, "big")
+        return int_val % (b - a) + a
 
     @methoddispatch()
     def get_list(self, a, b, size: int):
         raise ArgumentError(
             "乱数の閾値はどちらもintもしくはdecimalでなければなりません．"
             f"a is {type(a)}, b is {type(b)}")
 
@@ -67,18 +72,25 @@
                     for i in range(0, len(bytes_list), byte_size)]
         return [x % (b-a)+a for x in int_list]
 
     @get_list.register(Decimal)
     def __get_list_decimal(self, a: Decimal, b: Decimal, size: int) \
             -> List[Decimal]:
         # 128bit整数を取り出して[a,b]に正規化する
+        # self.__exception_check(a, b)
+        # valList: List[int] = self.get_list(self.mn, self.mx, size)
+        # return [Decimal(val-self.mn)/(self.mx-self.mn)*(b-a)+a
+        #         for val in valList]
+        byte_size: int = self.__get_byte_size(b-a)
         self.__exception_check(a, b)
-        valList: List[int] = self.get_list(self.mn, self.mx, size)
-        return [Decimal(val-self.mn)/(self.mx-self.mn)*(b-a)+a
-                for val in valList]
+        seed: bytes = self.__get_32byte()
+        bytes_list: bytes = randombytes_deterministic(size*byte_size, seed)
+        int_list = [int.from_bytes(bytes_list[i:i+byte_size], "big")
+                    for i in range(0, len(bytes_list), byte_size)]
+        return [Decimal(int(x) % int(b-a))+a for x in int_list]
 
     def __get_byte_size(self, x: int) -> int:
         # 整数の byte サイズを取得
         return max(math.ceil(math.log2(x))//8 + 1, 32)
 
     def __get_32byte(self) -> bytes:
         return random()
```

### Comparing `quickmpc-1.0.0/quickmpc/share/restore.py` & `quickmpc-9.9.9/quickmpc/share/restore.py`

 * *Files identical despite different names*

### Comparing `quickmpc-1.0.0/quickmpc/share/share.py` & `quickmpc-9.9.9/quickmpc/share/share.py`

 * *Files identical despite different names*

### Comparing `quickmpc-1.0.0/quickmpc/utils/make_pieces.py` & `quickmpc-9.9.9/quickmpc/utils/make_pieces.py`

 * *Files identical despite different names*

### Comparing `quickmpc-1.0.0/quickmpc/utils/overload_tools.py` & `quickmpc-9.9.9/quickmpc/utils/overload_tools.py`

 * *Files identical despite different names*

### Comparing `quickmpc-1.0.0/quickmpc.egg-info/SOURCES.txt` & `quickmpc-9.9.9/quickmpc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quickmpc-1.0.0/tests/unit_tests/conftest.py` & `quickmpc-9.9.9/tests/unit_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `quickmpc-1.0.0/tests/unit_tests/local_server.py` & `quickmpc-9.9.9/tests/unit_tests/local_server.py`

 * *Files identical despite different names*

### Comparing `quickmpc-1.0.0/tests/unit_tests/pandas/test_files/edge_data.csv` & `quickmpc-9.9.9/tests/unit_tests/pandas/test_files/edge_data.csv`

 * *Files identical despite different names*

### Comparing `quickmpc-1.0.0/tests/unit_tests/pandas/test_files/string_data.csv` & `quickmpc-9.9.9/tests/unit_tests/pandas/test_files/string_data.csv`

 * *Files identical despite different names*

### Comparing `quickmpc-1.0.0/tests/unit_tests/pandas/test_parser.py` & `quickmpc-9.9.9/tests/unit_tests/pandas/test_parser.py`

 * *Files identical despite different names*

### Comparing `quickmpc-1.0.0/tests/unit_tests/pandas/test_reader.py` & `quickmpc-9.9.9/tests/unit_tests/pandas/test_reader.py`

 * *Files identical despite different names*

### Comparing `quickmpc-1.0.0/tests/unit_tests/pandas/test_share_data_frame.py` & `quickmpc-9.9.9/tests/unit_tests/pandas/test_share_data_frame.py`

 * *Files identical despite different names*

### Comparing `quickmpc-1.0.0/tests/unit_tests/request/test_qmpc_request.py` & `quickmpc-9.9.9/tests/unit_tests/request/test_qmpc_request.py`

 * *Files identical despite different names*

### Comparing `quickmpc-1.0.0/tests/unit_tests/share/test_random.py` & `quickmpc-9.9.9/tests/unit_tests/share/test_random.py`

 * *Files identical despite different names*

### Comparing `quickmpc-1.0.0/tests/unit_tests/share/test_restore.py` & `quickmpc-9.9.9/tests/unit_tests/share/test_restore.py`

 * *Files identical despite different names*

### Comparing `quickmpc-1.0.0/tests/unit_tests/share/test_share_recons.py` & `quickmpc-9.9.9/tests/unit_tests/share/test_share_recons.py`

 * *Files identical despite different names*

### Comparing `quickmpc-1.0.0/tests/unit_tests/share/test_share_sharize.py` & `quickmpc-9.9.9/tests/unit_tests/share/test_share_sharize.py`

 * *Files identical despite different names*

### Comparing `quickmpc-1.0.0/tests/unit_tests/test_qmpc.py` & `quickmpc-9.9.9/tests/unit_tests/test_qmpc.py`

 * *Files identical despite different names*

### Comparing `quickmpc-1.0.0/tests/unit_tests/utils/test_make_pieces.py` & `quickmpc-9.9.9/tests/unit_tests/utils/test_make_pieces.py`

 * *Files identical despite different names*

### Comparing `quickmpc-1.0.0/tests/unit_tests/utils/test_over_load.py` & `quickmpc-9.9.9/tests/unit_tests/utils/test_over_load.py`

 * *Files identical despite different names*

