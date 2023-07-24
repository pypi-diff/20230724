# Comparing `tmp/xinference-0.0.5.tar.gz` & `tmp/xinference-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xinference-0.0.5.tar", last modified: Wed Jul 19 11:33:37 2023, max compression
+gzip compressed data, was "xinference-0.0.6.tar", last modified: Mon Jul 24 07:06:26 2023, max compression
```

## Comparing `xinference-0.0.5.tar` & `xinference-0.0.6.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:33:37.533058 xinference-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-19 11:33:27.000000 xinference-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-19 11:33:27.000000 xinference-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9837 2023-07-19 11:33:37.533058 xinference-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-07-19 11:33:27.000000 xinference-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-19 11:33:27.000000 xinference-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-07-19 11:33:37.537058 xinference-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-07-19 11:33:27.000000 xinference-0.0.5/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83780 2023-07-19 11:33:27.000000 xinference-0.0.5/versioneer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:33:37.537058 xinference-0.0.5/xinference/
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-19 11:33:37.537058 xinference-0.0.5/xinference/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    14201 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:33:37.529058 xinference-0.0.5/xinference/core/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/core/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    15762 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/core/gradio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/core/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/core/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    20673 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/core/restful_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12956 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/core/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:33:37.533058 xinference-0.0.5/xinference/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/deploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/deploy/cmdline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/deploy/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/deploy/supervisor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:33:37.533058 xinference-0.0.5/xinference/deploy/test/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/deploy/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/deploy/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/deploy/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/isolation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:33:37.533058 xinference-0.0.5/xinference/locale/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/locale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/locale/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/locale/zh_CN.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:33:37.533058 xinference-0.0.5/xinference/model/
--rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:33:37.533058 xinference-0.0.5/xinference/model/llm/
--rw-r--r--   0 runner    (1001) docker     (123)    10432 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/model/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/model/llm/chatglm.py
--rw-r--r--   0 runner    (1001) docker     (123)     8940 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/model/llm/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/model/llm/llama2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/model/llm/orca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:33:37.533058 xinference-0.0.5/xinference/model/llm/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/model/llm/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/model/llm/pytorch/baichuan.py
--rw-r--r--   0 runner    (1001) docker     (123)    10004 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/model/llm/pytorch/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    10552 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/model/llm/pytorch/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/model/llm/pytorch/vicuna.py
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/model/llm/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/model/llm/vicuna.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/model/llm/wizardlm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:33:37.529058 xinference-0.0.5/xinference.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9837 2023-07-19 11:33:37.000000 xinference-0.0.5/xinference.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-19 11:33:37.000000 xinference-0.0.5/xinference.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 11:33:37.000000 xinference-0.0.5/xinference.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-19 11:33:37.000000 xinference-0.0.5/xinference.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 11:33:37.000000 xinference-0.0.5/xinference.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-19 11:33:37.000000 xinference-0.0.5/xinference.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-19 11:33:37.000000 xinference-0.0.5/xinference.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:06:26.973025 xinference-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-24 07:06:18.000000 xinference-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-24 07:06:18.000000 xinference-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9977 2023-07-24 07:06:26.973025 xinference-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-07-24 07:06:18.000000 xinference-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-24 07:06:18.000000 xinference-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-24 07:06:26.973025 xinference-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-07-24 07:06:18.000000 xinference-0.0.6/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83780 2023-07-24 07:06:18.000000 xinference-0.0.6/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:06:26.973025 xinference-0.0.6/xinference/
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-24 07:06:26.973025 xinference-0.0.6/xinference/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14201 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:06:26.969025 xinference-0.0.6/xinference/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/core/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15505 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/core/gradio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/core/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/core/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20685 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/core/restful_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13391 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/core/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:06:26.969025 xinference-0.0.6/xinference/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/deploy/cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/deploy/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/deploy/supervisor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:06:26.969025 xinference-0.0.6/xinference/deploy/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/deploy/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/deploy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/deploy/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/isolation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:06:26.969025 xinference-0.0.6/xinference/locale/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/locale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/locale/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/locale/zh_CN.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:06:26.969025 xinference-0.0.6/xinference/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:06:26.973025 xinference-0.0.6/xinference/model/llm/
+-rw-r--r--   0 runner    (1001) docker     (123)    14677 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/model/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/model/llm/chatglm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9000 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/model/llm/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/model/llm/llama2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/model/llm/orca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:06:26.973025 xinference-0.0.6/xinference/model/llm/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/model/llm/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/model/llm/pytorch/baichuan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10357 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/model/llm/pytorch/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10811 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/model/llm/pytorch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/model/llm/pytorch/vicuna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/model/llm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/model/llm/vicuna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/model/llm/wizardlm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:06:26.969025 xinference-0.0.6/xinference.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9977 2023-07-24 07:06:26.000000 xinference-0.0.6/xinference.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-24 07:06:26.000000 xinference-0.0.6/xinference.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 07:06:26.000000 xinference-0.0.6/xinference.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-24 07:06:26.000000 xinference-0.0.6/xinference.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 07:06:26.000000 xinference-0.0.6/xinference.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-24 07:06:26.000000 xinference-0.0.6/xinference.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-24 07:06:26.000000 xinference-0.0.6/xinference.egg-info/top_level.txt
```

### Comparing `xinference-0.0.5/LICENSE` & `xinference-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xinference-0.0.5/PKG-INFO` & `xinference-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xinference
-Version: 0.0.5
+Version: 0.0.6
 Summary: Model Serving Made Easy
 Home-page: https://github.com/xorbitsai/inference
 Author: Qin Xuye
 Author-email: qinxuye@xprobe.io
 Maintainer: Qin Xuye
 Maintainer-email: qinxuye@xprobe.io
 License: Apache License 2.0
@@ -30,15 +30,15 @@
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/xinference.svg?style=for-the-badge)](https://pypi.org/project/xinference/)
 [![License](https://img.shields.io/pypi/l/xinference.svg?style=for-the-badge)](https://github.com/xorbitsai/inference/blob/main/LICENSE)
 [![Build Status](https://img.shields.io/github/actions/workflow/status/xorbitsai/inference/python.yaml?branch=main&style=for-the-badge&label=GITHUB%20ACTIONS&logo=github)](https://actions-badge.atrox.dev/xorbitsai/inference/goto?ref=main)
 [![Slack](https://img.shields.io/badge/join_Slack-781FF5.svg?logo=slack&style=for-the-badge)](https://join.slack.com/t/xorbitsio/shared_invite/zt-1o3z9ucdh-RbfhbPVpx7prOVdM1CAuxg)
 [![Twitter](https://img.shields.io/twitter/follow/xorbitsio?logo=twitter&style=for-the-badge)](https://twitter.com/xorbitsio)
 
-English | [中文介绍](README_zh_CN.md)
+English | [中文介绍](README_zh_CN.md) | [日本語](README_ja_JP.md)
 </div>
 <br />
 
 
 Xorbits Inference(Xinference) is a powerful and versatile library designed to serve language, 
 speech recognition, and multimodal models. With Xorbits Inference, you can effortlessly deploy 
 and serve your or state-of-the-art built-in models using just a single command. Whether you are a 
@@ -199,14 +199,15 @@
 | orca          | SFT Model        | en       | ggmlv3  | 3, 7, 13           | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0'  |
 
 
 **NOTE**:
 - Xinference will download models automatically for you, and by default the models will be saved under `${USER}/.xinference/cache`.
 - Foundation models only provide interface `generate`.
 - RLHF and SFT models provide both `generate` and `chat`.
+- If you want to use Apple Metal GPU for acceleration, please choose the q4_0 and q4_1 quantization methods.
 
 ## Roadmap
 Xinference is currently under active development. Here's a roadmap outlining our planned 
 developments for the next few weeks:
 
 ### PyTorch Support
 With PyTorch integration, users will be able to seamlessly utilize PyTorch models from Hugging Face
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xinference Version: 0.0.5 Summary: Model Serving
+Metadata-Version: 2.1 Name: xinference Version: 0.0.6 Summary: Model Serving
 Made Easy Home-page: https://github.com/xorbitsai/inference Author: Qin Xuye
 Author-email: qinxuye@xprobe.io Maintainer: Qin Xuye Maintainer-email:
 qinxuye@xprobe.io License: Apache License 2.0 Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
@@ -18,15 +18,15 @@
   workflow/status/xorbitsai/inference/python.yaml?branch=main&style=for-the-
   badge&label=GITHUB%20ACTIONS&logo=github)](https://actions-badge.atrox.dev/
   xorbitsai/inference/goto?ref=main) [![Slack](https://img.shields.io/badge/
 join_Slack-781FF5.svg?logo=slack&style=for-the-badge)](https://join.slack.com/
   t/xorbitsio/shared_invite/zt-1o3z9ucdh-RbfhbPVpx7prOVdM1CAuxg) [![Twitter]
  (https://img.shields.io/twitter/follow/xorbitsio?logo=twitter&style=for-the-
         badge)](https://twitter.com/xorbitsio) English | [ä¸­æä»ç»]
-                               (README_zh_CN.md)
+               (README_zh_CN.md) | [æ¥æ¬èª](README_ja_JP.md)
 
 Xorbits Inference(Xinference) is a powerful and versatile library designed to
 serve language, speech recognition, and multimodal models. With Xorbits
 Inference, you can effortlessly deploy and serve your or state-of-the-art
 built-in models using just a single command. Whether you are a researcher,
 developer, or data scientist, Xorbits Inference empowers you to unleash the
 full potential of cutting-edge AI models. ![demo](assets/demo.gif)
@@ -112,13 +112,15 @@
 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' | | wizardlm-v1.1 | SFT Model | en |
 ggmlv3 | 13 | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' | | vicuna-v1.3 | SFT
 Model | en | ggmlv3 | 7, 13 | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' | | orca |
 SFT Model | en | ggmlv3 | 3, 7, 13 | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0' |
 **NOTE**: - Xinference will download models automatically for you, and by
 default the models will be saved under `${USER}/.xinference/cache`. -
 Foundation models only provide interface `generate`. - RLHF and SFT models
-provide both `generate` and `chat`. ## Roadmap Xinference is currently under
-active development. Here's a roadmap outlining our planned developments for the
-next few weeks: ### PyTorch Support With PyTorch integration, users will be
-able to seamlessly utilize PyTorch models from Hugging Face within Xinference.
-### Langchain & LlamaIndex integration With Xinference, it will be much easier
-for users to use these libraries and build applications with LLMs.
+provide both `generate` and `chat`. - If you want to use Apple Metal GPU for
+acceleration, please choose the q4_0 and q4_1 quantization methods. ## Roadmap
+Xinference is currently under active development. Here's a roadmap outlining
+our planned developments for the next few weeks: ### PyTorch Support With
+PyTorch integration, users will be able to seamlessly utilize PyTorch models
+from Hugging Face within Xinference. ### Langchain & LlamaIndex integration
+With Xinference, it will be much easier for users to use these libraries and
+build applications with LLMs.
```

### Comparing `xinference-0.0.5/README.md` & `xinference-0.0.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/xinference.svg?style=for-the-badge)](https://pypi.org/project/xinference/)
 [![License](https://img.shields.io/pypi/l/xinference.svg?style=for-the-badge)](https://github.com/xorbitsai/inference/blob/main/LICENSE)
 [![Build Status](https://img.shields.io/github/actions/workflow/status/xorbitsai/inference/python.yaml?branch=main&style=for-the-badge&label=GITHUB%20ACTIONS&logo=github)](https://actions-badge.atrox.dev/xorbitsai/inference/goto?ref=main)
 [![Slack](https://img.shields.io/badge/join_Slack-781FF5.svg?logo=slack&style=for-the-badge)](https://join.slack.com/t/xorbitsio/shared_invite/zt-1o3z9ucdh-RbfhbPVpx7prOVdM1CAuxg)
 [![Twitter](https://img.shields.io/twitter/follow/xorbitsio?logo=twitter&style=for-the-badge)](https://twitter.com/xorbitsio)
 
-English | [中文介绍](README_zh_CN.md)
+English | [中文介绍](README_zh_CN.md) | [日本語](README_ja_JP.md)
 </div>
 <br />
 
 
 Xorbits Inference(Xinference) is a powerful and versatile library designed to serve language, 
 speech recognition, and multimodal models. With Xorbits Inference, you can effortlessly deploy 
 and serve your or state-of-the-art built-in models using just a single command. Whether you are a 
@@ -174,14 +174,15 @@
 | orca          | SFT Model        | en       | ggmlv3  | 3, 7, 13           | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0'  |
 
 
 **NOTE**:
 - Xinference will download models automatically for you, and by default the models will be saved under `${USER}/.xinference/cache`.
 - Foundation models only provide interface `generate`.
 - RLHF and SFT models provide both `generate` and `chat`.
+- If you want to use Apple Metal GPU for acceleration, please choose the q4_0 and q4_1 quantization methods.
 
 ## Roadmap
 Xinference is currently under active development. Here's a roadmap outlining our planned 
 developments for the next few weeks:
 
 ### PyTorch Support
 With PyTorch integration, users will be able to seamlessly utilize PyTorch models from Hugging Face
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
   workflow/status/xorbitsai/inference/python.yaml?branch=main&style=for-the-
   badge&label=GITHUB%20ACTIONS&logo=github)](https://actions-badge.atrox.dev/
   xorbitsai/inference/goto?ref=main) [![Slack](https://img.shields.io/badge/
 join_Slack-781FF5.svg?logo=slack&style=for-the-badge)](https://join.slack.com/
   t/xorbitsio/shared_invite/zt-1o3z9ucdh-RbfhbPVpx7prOVdM1CAuxg) [![Twitter]
  (https://img.shields.io/twitter/follow/xorbitsio?logo=twitter&style=for-the-
         badge)](https://twitter.com/xorbitsio) English | [ä¸­æä»ç»]
-                               (README_zh_CN.md)
+               (README_zh_CN.md) | [æ¥æ¬èª](README_ja_JP.md)
 
 Xorbits Inference(Xinference) is a powerful and versatile library designed to
 serve language, speech recognition, and multimodal models. With Xorbits
 Inference, you can effortlessly deploy and serve your or state-of-the-art
 built-in models using just a single command. Whether you are a researcher,
 developer, or data scientist, Xorbits Inference empowers you to unleash the
 full potential of cutting-edge AI models. ![demo](assets/demo.gif)
@@ -100,13 +100,15 @@
 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' | | wizardlm-v1.1 | SFT Model | en |
 ggmlv3 | 13 | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' | | vicuna-v1.3 | SFT
 Model | en | ggmlv3 | 7, 13 | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' | | orca |
 SFT Model | en | ggmlv3 | 3, 7, 13 | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0' |
 **NOTE**: - Xinference will download models automatically for you, and by
 default the models will be saved under `${USER}/.xinference/cache`. -
 Foundation models only provide interface `generate`. - RLHF and SFT models
-provide both `generate` and `chat`. ## Roadmap Xinference is currently under
-active development. Here's a roadmap outlining our planned developments for the
-next few weeks: ### PyTorch Support With PyTorch integration, users will be
-able to seamlessly utilize PyTorch models from Hugging Face within Xinference.
-### Langchain & LlamaIndex integration With Xinference, it will be much easier
-for users to use these libraries and build applications with LLMs.
+provide both `generate` and `chat`. - If you want to use Apple Metal GPU for
+acceleration, please choose the q4_0 and q4_1 quantization methods. ## Roadmap
+Xinference is currently under active development. Here's a roadmap outlining
+our planned developments for the next few weeks: ### PyTorch Support With
+PyTorch integration, users will be able to seamlessly utilize PyTorch models
+from Hugging Face within Xinference. ### Langchain & LlamaIndex integration
+With Xinference, it will be much easier for users to use these libraries and
+build applications with LLMs.
```

### Comparing `xinference-0.0.5/setup.cfg` & `xinference-0.0.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires = 
 	xoscar
 	xorbits
-	gradio
+	gradio>=3.35.0
 	click
 	tqdm
 	tabulate
 	requests
 	pydantic
 	fastapi
 	uvicorn
@@ -61,15 +61,15 @@
 	chatglm-cpp
 	llama-cpp-python
 	transformers
 	torch
 	accelerate
 	sentencepiece
 	transformers_stream_generator
-	cpm_kernels
+	cpm_kernels; platform_system != "Darwin"
 doc = 
 	ipython>=6.5.0
 	sphinx>=3.0.0,<5.0.0
 	pydata-sphinx-theme>=0.3.0
 	sphinx-intl>=0.9.9
 
 [options.entry_points]
```

### Comparing `xinference-0.0.5/setup.py` & `xinference-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.5/versioneer.py` & `xinference-0.0.6/versioneer.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.5/xinference/__init__.py` & `xinference-0.0.6/xinference/__init__.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.5/xinference/client.py` & `xinference-0.0.6/xinference/client.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.5/xinference/constants.py` & `xinference-0.0.6/xinference/constants.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.5/xinference/core/__init__.py` & `xinference-0.0.6/xinference/core/__init__.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.5/xinference/core/api.py` & `xinference-0.0.6/xinference/core/api.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.5/xinference/core/gradio.py` & `xinference-0.0.6/xinference/core/gradio.py`

 * *Files 2% similar despite different names*

```diff
@@ -265,41 +265,36 @@
             _model_name: str,
             _model_format: str,
             _model_size_in_billions: str,
             _quantization: str,
             progress=gr.Progress(),
         ):
             model_family = MODEL_TO_FAMILIES[_model_name]
-            cache_path, meta_path = model_family.generate_cache_path(
+            cache_path = model_family.generate_cache_path(
                 int(_model_size_in_billions), _quantization
             )
-            if not (os.path.exists(cache_path) and os.path.exists(meta_path)):
+            if not (os.path.exists(cache_path)):
                 if os.path.exists(cache_path):
                     os.remove(cache_path)
                 url = model_family.url_generator(
                     int(_model_size_in_billions), _quantization
                 )
-                full_name = (
-                    f"{str(model_family)}-{_model_size_in_billions}b-{_quantization}"
-                )
                 try:
                     urllib.request.urlretrieve(
                         url,
                         cache_path,
                         reporthook=lambda block_num, block_size, total_size: progress(
                             block_num * block_size / total_size,
                             desc=self._locale("Downloading"),
                         ),
                     )
-                    # write a meta file to record if download finished
-                    with open(meta_path, "w") as f:
-                        f.write(full_name)
                 except:
                     if os.path.exists(cache_path):
                         os.remove(cache_path)
+                    raise gr.Error(self._locale(f"Download failed, please retry."))
 
             model_uid = self._create_model(
                 _model_name, int(_model_size_in_billions), _model_format, _quantization
             )
             return gr.Chatbot.update(
                 label="-".join(
                     [_model_name, _model_size_in_billions, _model_format, _quantization]
```

### Comparing `xinference-0.0.5/xinference/core/model.py` & `xinference-0.0.6/xinference/core/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,14 +55,32 @@
 
 
 class ModelActor(xo.Actor):
     @classmethod
     def gen_uid(cls, model: "Model"):
         return f"{model.__class__}-model-actor"
 
+    async def __pre_destroy__(self):
+        if self._model.model_spec.model_format == "pytorch":
+            try:
+                import gc
+
+                import torch
+            except ImportError:
+                error_message = "Failed to import module 'torch'"
+                installation_guide = [
+                    "Please make sure 'torch' is installed.\n",
+                ]
+
+                raise ImportError(f"{error_message}\n\n{''.join(installation_guide)}")
+
+            del self._model
+            gc.collect()
+            torch.cuda.empty_cache()
+
     def __init__(self, model: "Model"):
         super().__init__()
         self._model = model
         self._generator: Optional[Iterator] = None
 
     def load(self):
         self._model.load()
```

### Comparing `xinference-0.0.5/xinference/core/resource.py` & `xinference-0.0.6/xinference/core/resource.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.5/xinference/core/restful_api.py` & `xinference-0.0.6/xinference/core/restful_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,15 +181,15 @@
     )
     max_tokens: int = max_tokens_field
     temperature: float = temperature_field
     top_p: float = top_p_field
     mirostat_mode: int = mirostat_mode_field
     mirostat_tau: float = mirostat_tau_field
     mirostat_eta: float = mirostat_eta_field
-    stop: Optional[List[str]] = stop_field
+    stop: Optional[Union[str, List[str]]] = stop_field
     stream: bool = stream_field
     presence_penalty: Optional[float] = presence_penalty_field
     frequency_penalty: Optional[float] = frequency_penalty_field
     logit_bias: Optional[Dict[str, float]] = Field(None)
 
     model: str
     n: Optional[int] = 1
```

### Comparing `xinference-0.0.5/xinference/core/service.py` & `xinference-0.0.6/xinference/core/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import asyncio
+import platform
 import time
 from dataclasses import dataclass
 from logging import getLogger
 from typing import Callable, Dict, List, Optional, Set, Tuple
 
 import xoscar as xo
 
@@ -242,25 +243,33 @@
                 target_subpool_address,
                 min_running_model_count,
             )
             return target_subpool_address
 
         raise RuntimeError("No available slot found")
 
+    def _check_model_is_valid(self, model_name):
+        # baichuan-base and baichuan-chat depend on `cpm_kernels` module,
+        # but `cpm_kernels` cannot run on Darwin system.
+        if platform.system() == "Darwin":
+            if model_name in ["baichuan-base", "baichuan-chat"]:
+                raise ValueError(f"{model_name} model can't run on Darwin system.")
+
     @log
     async def launch_builtin_model(
         self,
         model_uid: str,
         model_name: str,
         model_size_in_billions: Optional[int],
         model_format: Optional[str],
         quantization: Optional[str],
         **kwargs,
     ) -> xo.ActorRefType["ModelActor"]:
         assert model_uid not in self._model_uid_to_model
+        self._check_model_is_valid(model_name)
 
         from ..model import MODEL_FAMILIES
 
         for model_family in MODEL_FAMILIES:
             model_spec = model_family.match(
                 model_name=model_name,
                 model_format=model_format,
```

### Comparing `xinference-0.0.5/xinference/deploy/__init__.py` & `xinference-0.0.6/xinference/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.5/xinference/deploy/cmdline.py` & `xinference-0.0.6/xinference/deploy/cmdline.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.5/xinference/deploy/local.py` & `xinference-0.0.6/xinference/deploy/local.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.5/xinference/deploy/supervisor.py` & `xinference-0.0.6/xinference/deploy/supervisor.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.5/xinference/deploy/test/__init__.py` & `xinference-0.0.6/xinference/deploy/test/__init__.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.5/xinference/deploy/utils.py` & `xinference-0.0.6/xinference/deploy/utils.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.5/xinference/deploy/worker.py` & `xinference-0.0.6/xinference/deploy/worker.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.5/xinference/isolation.py` & `xinference-0.0.6/xinference/isolation.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.5/xinference/locale/__init__.py` & `xinference-0.0.6/xinference/locale/__init__.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.5/xinference/locale/utils.py` & `xinference-0.0.6/xinference/locale/utils.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.5/xinference/locale/zh_CN.json` & `xinference-0.0.6/xinference/locale/zh_CN.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333334%*

 * *Differences: {"'Download failed, please retry.'": "'下载失败，请重新下载'"}*

```diff
@@ -1,10 +1,11 @@
 {
     "Arena": "\u89d2\u6597\u573a",
     "Chat": "\u804a\u5929",
+    "Download failed, please retry.": "\u4e0b\u8f7d\u5931\u8d25\uff0c\u8bf7\u91cd\u65b0\u4e0b\u8f7d",
     "Downloading": "\u4e0b\u8f7d\u4e2d",
     "Input": "\u8f93\u5165",
     "Max tokens": "\u6700\u5927 token \u6570\u91cf",
     "Parameters": "\u53c2\u6570\u8c03\u6574",
     "Please create model first": "\u8bf7\u5148\u521b\u5efa\u6a21\u578b",
     "Show stop reason": "\u5c55\u793a\u505c\u6b62\u539f\u56e0",
     "Temperature": "\u6e29\u5ea6\u53c2\u6570",
```

### Comparing `xinference-0.0.5/xinference/model/__init__.py` & `xinference-0.0.6/xinference/model/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,16 +11,19 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
 import os
 import urllib.request
+import warnings
 from typing import Callable, List, Optional, Type
 
+import requests
+from requests import RequestException
 from tqdm import tqdm
 
 from ..constants import XINFERENCE_CACHE_DIR
 
 logger = logging.getLogger(__name__)
 
 
@@ -28,20 +31,22 @@
     def __init__(
         self,
         model_name: str,
         model_format: str,
         model_size_in_billions: int,
         quantization: str,
         url: str,
+        rp_url: Optional[str] = None,
     ):
         self.model_name = model_name
         self.model_format = model_format
         self.model_size_in_billions = model_size_in_billions
         self.quantization = quantization
         self.url = url
+        self.rp_url = rp_url
 
     def __str__(self):
         return (
             f"{self.model_name}-{self.model_format}-{self.model_size_in_billions}b"
             f"-{self.quantization}"
         )
 
@@ -67,21 +72,23 @@
     def __init__(
         self,
         model_name: str,
         model_format: str,
         model_sizes_in_billions: List[int],
         quantizations: List[str],
         url_generator: Callable[[int, str], str],
+        rp_url_generator: Callable[[int, str], str],
         cls: Type,
     ):
         self.model_name = model_name
         self.model_sizes_in_billions = model_sizes_in_billions
         self.model_format = model_format
         self.quantizations = quantizations
         self.url_generator = url_generator
+        self.rp_url_generator = rp_url_generator
         self.cls = cls
 
     def __str__(self):
         return f"{self.model_name}-{self.model_format}"
 
     def __iter__(self):
         model_specs = []
@@ -90,14 +97,15 @@
                 model_specs.append(
                     ModelSpec(
                         model_name=self.model_name,
                         model_size_in_billions=model_size,
                         model_format=self.model_format,
                         quantization=quantization,
                         url=self.url_generator(model_size, quantization),
+                        rp_url=self.rp_url_generator(model_size, quantization),
                     )
                 )
         return iter(model_specs)
 
     def match(
         self,
         model_name: str,
@@ -121,41 +129,67 @@
         quantization: Optional[str] = None,
     ):
         full_name = f"{str(self)}-{model_size_in_billions}b-{quantization}"
         save_dir = os.path.join(XINFERENCE_CACHE_DIR, full_name)
         if not os.path.exists(save_dir):
             os.makedirs(save_dir, exist_ok=True)
         save_path = os.path.join(save_dir, "model.bin")
-        meta_path = os.path.join(save_dir, "meta")
-        return save_path, meta_path
+        return save_path
 
     def cache(
         self,
         model_size_in_billions: Optional[int] = None,
         quantization: Optional[str] = None,
     ) -> str:
         # by default, choose the smallest size.
         model_size_in_billions = (
             model_size_in_billions or self.model_sizes_in_billions[0]
         )
         # by default, choose the most coarse-grained quantization.
         quantization = quantization or self.quantizations[0]
 
         url = self.url_generator(model_size_in_billions, quantization)
+        rp_url = self.rp_url_generator(model_size_in_billions, quantization)
+
+        try:
+            rp_fetch = requests.get(rp_url)
+        except RequestException:
+            raise RuntimeError(
+                f"Failed to download raw pointer file for integrity verification from {rp_url}"
+            )
+
+        res_content = rp_fetch.content
+        expected_size = -1
+        splitted_res_content = res_content.split()
+        for index in range(len(splitted_res_content)):
+            item = str(splitted_res_content[index], encoding="utf-8")
+            if item == "size":
+                expected_size = int(
+                    str(splitted_res_content[index + 1], encoding="utf-8")
+                )
 
         if self.model_format == "pytorch":
             return url
 
         full_name = f"{str(self)}-{model_size_in_billions}b-{quantization}"
-        save_path, meta_path = self.generate_cache_path(
-            model_size_in_billions, quantization
-        )
-        if os.path.exists(meta_path) and os.path.exists(save_path):
-            # TODO: verify the integrity.
-            return save_path
+        save_path = self.generate_cache_path(model_size_in_billions, quantization)
+
+        if os.path.exists(save_path):
+            if os.path.getsize(save_path) == expected_size:
+                return save_path
+            else:
+                warnings.warn(
+                    "Model size doesn't match, try to update it...", RuntimeWarning
+                )
+
+        save_dir = os.path.join(XINFERENCE_CACHE_DIR, full_name)
+        if not os.path.exists(save_dir):
+            os.makedirs(save_dir, exist_ok=True)
+
+        save_path = os.path.join(save_dir, "model.bin")
 
         try:
             if os.path.exists(save_path):
                 os.remove(save_path)
             with tqdm(
                 unit="B",
                 unit_scale=True,
@@ -166,18 +200,19 @@
                 urllib.request.urlretrieve(
                     url,
                     save_path,
                     reporthook=lambda blocknum, blocksize, totalsize: progress.update(
                         blocksize
                     ),
                 )
-            # write a meta file to record if download finished
-            with open(meta_path, "w") as f:
-                f.write(full_name)
-            # TODO: verify the integrity.
+
+            # verify the integrity.
+            if os.path.getsize(save_path) != expected_size:
+                os.remove(save_path)
+                raise RuntimeError(f"Failed to download {full_name} from {url}")
         except:
             if os.path.exists(save_path):
                 os.remove(save_path)
             raise RuntimeError(f"Failed to download {full_name} from {url}")
 
         return save_path
```

### Comparing `xinference-0.0.5/xinference/model/llm/__init__.py` & `xinference-0.0.6/xinference/model/llm/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -24,14 +24,20 @@
     from .vicuna import VicunaCensoredGgml
     from .wizardlm import WizardlmGgml
 
     baichuan_url_generator = lambda model_size, quantization: (
         f"https://huggingface.co/TheBloke/baichuan-llama-{model_size}B-GGML/resolve/main/"
         f"baichuan-llama-{model_size}b.ggmlv3.{quantization}.bin"
     )
+
+    baichuan_url_raw_generator = lambda model_size, quantization: (
+        f"https://huggingface.co/TheBloke/baichuan-llama-{model_size}B-GGML/raw/main/"
+        f"baichuan-llama-{model_size}b.ggmlv3.{quantization}.bin"
+    )
+
     MODEL_FAMILIES.append(
         ModelFamily(
             model_name="baichuan",
             model_format="ggmlv3",
             model_sizes_in_billions=[7],
             quantizations=[
                 "q2_K",
@@ -46,22 +52,66 @@
                 "q5_1",
                 "q5_K_M",
                 "q5_K_S",
                 "q6_K",
                 "q8_0",
             ],
             url_generator=baichuan_url_generator,
+            rp_url_generator=baichuan_url_raw_generator,
             cls=LlamaCppModel,
         )
     )
 
+    baichuan_chat_url_generator = lambda model_size, quantization: (
+        f"https://huggingface.co/TheBloke/baichuan-vicuna-{model_size}B-GGML/resolve/main/"
+        f"baichuan-vicuna-{model_size}b.ggmlv3.{quantization}.bin"
+    )
+
+    baichuan_chat_url_raw_generator = lambda model_size, quantization: (
+        f"https://huggingface.co/TheBloke/baichuan-vicuna-{model_size}B-GGML/raw/main/"
+        f"baichuan-vicuna-{model_size}b.ggmlv3.{quantization}.bin"
+    )
+
+    MODEL_FAMILIES.append(
+        ModelFamily(
+            model_name="baichuan-chat",
+            model_format="ggmlv3",
+            model_sizes_in_billions=[7],
+            quantizations=[
+                "q2_K",
+                "q3_K_L",
+                "q3_K_M",
+                "q3_K_S",
+                "q4_0",
+                "q4_1",
+                "q4_K_M",
+                "q4_K_S",
+                "q5_0",
+                "q5_1",
+                "q5_K_M",
+                "q5_K_S",
+                "q6_K",
+                "q8_0",
+            ],
+            url_generator=baichuan_chat_url_generator,
+            rp_url_generator=baichuan_chat_url_raw_generator,
+            cls=VicunaCensoredGgml,
+        )
+    )
+
     wizardlm_v1_0_url_generator = lambda model_size, quantization: (
         f"https://huggingface.co/TheBloke/WizardLM-{model_size}B-V1.0-Uncensored-GGML/resolve/main/"
         f"wizardlm-{model_size}b-v1.0-uncensored.ggmlv3.{quantization}.bin"
     )
+
+    wizardlm_v1_0_url_raw_generator = lambda model_size, quantization: (
+        f"https://huggingface.co/TheBloke/WizardLM-{model_size}B-V1.0-Uncensored-GGML/raw/main/"
+        f"wizardlm-{model_size}b-v1.0-uncensored.ggmlv3.{quantization}.bin"
+    )
+
     MODEL_FAMILIES.append(
         ModelFamily(
             model_name="wizardlm-v1.0",
             model_sizes_in_billions=[7, 13, 33],
             model_format="ggmlv3",
             quantizations=[
                 "q2_K",
@@ -76,22 +126,27 @@
                 "q5_1",
                 "q5_K_M",
                 "q5_K_S",
                 "q6_K",
                 "q8_0",
             ],
             url_generator=wizardlm_v1_0_url_generator,
+            rp_url_generator=wizardlm_v1_0_url_raw_generator,
             cls=WizardlmGgml,
         ),
     )
 
     wizardlm_v1_1_url_generator = lambda model_size, quantization: (
         f"https://huggingface.co/TheBloke/WizardLM-{model_size}B-V1.1-GGML/resolve/main/"
         f"wizardlm-{model_size}b-v1.1.ggmlv3.{quantization}.bin"
     )
+    wizardlm_v1_1_url_raw_generator = lambda model_size, quantization: (
+        f"https://huggingface.co/TheBloke/WizardLM-{model_size}B-V1.1-GGML/raw/main/"
+        f"wizardlm-{model_size}b-v1.1.ggmlv3.{quantization}.bin"
+    )
     MODEL_FAMILIES.append(
         ModelFamily(
             model_name="wizardlm-v1.1",
             model_sizes_in_billions=[13],
             model_format="ggmlv3",
             quantizations=[
                 "q2_K",
@@ -106,14 +161,15 @@
                 "q5_1",
                 "q5_K_M",
                 "q5_K_S",
                 "q6_K",
                 "q8_0",
             ],
             url_generator=wizardlm_v1_1_url_generator,
+            rp_url_generator=wizardlm_v1_1_url_raw_generator,
             cls=VicunaCensoredGgml,  # according to https://huggingface.co/TheBloke/WizardLM-13B-V1.1-GGML
         ),
     )
 
     vicuna_v1_3_url_generator = lambda model_size, quantization: (
         "https://huggingface.co/TheBloke/vicuna-7B-v1.3-GGML/resolve/main/"
         f"vicuna-7b-v1.3.ggmlv3.{quantization}.bin"
@@ -121,14 +177,25 @@
         else (
             "https://huggingface.co/TheBloke/vicuna-13b-v1.3.0-GGML/resolve/main/"
             f"vicuna-13b-v1.3.0.ggmlv3.{quantization}.bin"
             if model_size == 13
             else f"https://huggingface.co/TheBloke/vicuna-33B-GGML/resolve/main/vicuna-33b.ggmlv3.{quantization}.bin"
         )
     )
+
+    vicuna_v1_3__url_raw_generator = lambda model_size, quantization: (
+        "https://huggingface.co/TheBloke/vicuna-7B-v1.3-GGML/raw/main/"
+        f"vicuna-7b-v1.3.ggmlv3.{quantization}.bin"
+        if model_size == 7
+        else (
+            "https://huggingface.co/TheBloke/vicuna-13b-v1.3.0-GGML/raw/main/"
+            f"vicuna-13b-v1.3.0.ggmlv3.{quantization}.bin"
+        )
+    )
+
     MODEL_FAMILIES.append(
         ModelFamily(
             model_name="vicuna-v1.3",
             model_sizes_in_billions=[7, 13, 33],
             model_format="ggmlv3",
             quantizations=[
                 "q2_K",
@@ -143,85 +210,106 @@
                 "q5_1",
                 "q5_K_M",
                 "q5_K_S",
                 "q6_K",
                 "q8_0",
             ],
             url_generator=vicuna_v1_3_url_generator,
+            rp_url_generator=vicuna_v1_3__url_raw_generator,
             cls=VicunaCensoredGgml,
         ),
     )
 
     orca_url_generator = lambda model_size, quantization: (
         f"https://huggingface.co/TheBloke/orca_mini_{model_size}B-GGML/resolve/main/orca-mini-"
         f"{model_size}b.ggmlv3.{quantization}.bin"
     )
+    orca_url_raw_generator = lambda model_size, quantization: (
+        f"https://huggingface.co/TheBloke/orca_mini_{model_size}B-GGML/raw/main/orca-mini-"
+        f"{model_size}b.ggmlv3.{quantization}.bin"
+    )
+
     MODEL_FAMILIES.append(
         ModelFamily(
             model_name="orca",
             model_sizes_in_billions=[3, 7, 13],
             model_format="ggmlv3",
             quantizations=[
                 "q4_0",
                 "q4_1",
                 "q5_0",
                 "q5_1",
                 "q8_0",
             ],
             url_generator=orca_url_generator,
+            rp_url_generator=orca_url_raw_generator,
             cls=OrcaMiniGgml,
         )
     )
 
     chatglm_url_generator = lambda model_size, quantization: (
         f"https://huggingface.co/Xorbits/chatglm-{model_size}B-GGML/resolve/main/"
         f"chatglm-ggml-{quantization}.bin"
     )
+    chatglm_url_raw_generator = lambda model_size, quantization: (
+        f"https://huggingface.co/Xorbits/chatglm-{model_size}B-GGML/raw/main/"
+        f"chatglm-ggml-{quantization}.bin"
+    )
     MODEL_FAMILIES.append(
         ModelFamily(
             model_name="chatglm",
             model_sizes_in_billions=[6],
             model_format="ggmlv3",
             quantizations=[
                 "q4_0",
                 "q4_1",
                 "q5_0",
                 "q5_1",
                 "q8_0",
             ],
             url_generator=chatglm_url_generator,
+            rp_url_generator=chatglm_url_raw_generator,
             cls=ChatglmCppChatModel,
         )
     )
 
     chatglm2_url_generator = lambda model_size, quantization: (
         f"https://huggingface.co/Xorbits/chatglm2-{model_size}B-GGML/resolve/main/"
         f"chatglm2-ggml-{quantization}.bin"
     )
+    chatglm2_url_raw_generator = lambda model_size, quantization: (
+        f"https://huggingface.co/Xorbits/chatglm2-{model_size}B-GGML/raw/main/"
+        f"chatglm2-ggml-{quantization}.bin"
+    )
     MODEL_FAMILIES.append(
         ModelFamily(
             model_name="chatglm2",
             model_sizes_in_billions=[6],
             model_format="ggmlv3",
             quantizations=[
                 "q4_0",
                 "q4_1",
                 "q5_0",
                 "q5_1",
                 "q8_0",
             ],
             url_generator=chatglm2_url_generator,
+            rp_url_generator=chatglm2_url_raw_generator,
             cls=ChatglmCppChatModel,
         )
     )
 
     llama2_chat_url_generator = lambda model_size, quantization: (
         f"https://huggingface.co/TheBloke/Llama-2-{model_size}B-chat-GGML/resolve/main/llama-2-"
         f"{model_size}b-chat.ggmlv3.{quantization}.bin"
     )
+    llama2_chat_url_raw_generator = lambda model_size, quantization: (
+        f"https://huggingface.co/TheBloke/Llama-2-{model_size}B-chat-GGML/raw/main/llama-2-"
+        f"{model_size}b-chat.ggmlv3.{quantization}.bin"
+    )
     MODEL_FAMILIES.append(
         ModelFamily(
             model_name="llama-2-chat",
             model_sizes_in_billions=[7, 13],
             model_format="ggmlv3",
             quantizations=[
                 "q2_K",
@@ -236,22 +324,27 @@
                 "q5_1",
                 "q5_K_M",
                 "q5_K_S",
                 "q6_K",
                 "q8_0",
             ],
             url_generator=llama2_chat_url_generator,
+            rp_url_generator=llama2_chat_url_raw_generator,
             cls=Llama2ChatGgml,
         )
     )
 
     llama2_url_generator = lambda model_size, quantization: (
         f"https://huggingface.co/TheBloke/Llama-2-{model_size}B-GGML/resolve/main/llama-2-"
         f"{model_size}b.ggmlv3.{quantization}.bin"
     )
+    llama2_url_raw_generator = lambda model_size, quantization: (
+        f"https://huggingface.co/TheBloke/Llama-2-{model_size}B-GGML/raw/main/llama-2-"
+        f"{model_size}b.ggmlv3.{quantization}.bin"
+    )
     MODEL_FAMILIES.append(
         ModelFamily(
             model_name="llama-2",
             model_sizes_in_billions=[7, 13],
             model_format="ggmlv3",
             quantizations=[
                 "q2_K",
@@ -266,66 +359,74 @@
                 "q5_1",
                 "q5_K_M",
                 "q5_K_S",
                 "q6_K",
                 "q8_0",
             ],
             url_generator=llama2_url_generator,
+            rp_url_generator=llama2_chat_url_raw_generator,
             cls=LlamaCppModel,
         )
     )
 
     pytorch_baichuan_name_generator = lambda model_size, quantization: (
         f"baichuan-inc/Baichuan-{model_size}B"
     )
     MODEL_FAMILIES.append(
         ModelFamily(
             model_name="baichuan",
             model_sizes_in_billions=[7],
             model_format="pytorch",
             quantizations=["none"],
             url_generator=pytorch_baichuan_name_generator,
+            rp_url_generator=lambda model_size, quantization: "",
             cls=BaichuanPytorch,
         ),
     )
 
     pytorch_baichuan_base_name_generator = lambda model_size, quantization: (
         f"baichuan-inc/Baichuan-{model_size}B-Base"
     )
     MODEL_FAMILIES.append(
         ModelFamily(
             model_name="baichuan-base",
             model_sizes_in_billions=[13],
             model_format="pytorch",
             quantizations=["int4", "int8", "none"],
             url_generator=pytorch_baichuan_base_name_generator,
+            rp_url_generator=lambda model_size, quantization: "",
             cls=BaichuanPytorch,
         ),
     )
 
     pytorch_baichuan_chat_name_generator = lambda model_size, quantization: (
         f"baichuan-inc/Baichuan-{model_size}B-Chat"
     )
     MODEL_FAMILIES.append(
         ModelFamily(
             model_name="baichuan-chat",
             model_sizes_in_billions=[13],
             model_format="pytorch",
             quantizations=["int4", "int8", "none"],
             url_generator=pytorch_baichuan_chat_name_generator,
+            rp_url_generator=lambda model_size, quantization: "",
             cls=BaichuanPytorchChat,
         ),
     )
 
+    """
+    # ggmlv3 model has the same model_name as pytorch model, comment it out in temporary
     pytorch_vicuna_v1_3_name_generator = lambda model_size, quantization: (
         f"lmsys/vicuna-{model_size}b-v1.3"
     )
     MODEL_FAMILIES.append(
         ModelFamily(
             model_name="vicuna-v1.3",
             model_sizes_in_billions=[7, 13],
             model_format="pytorch",
             quantizations=["none"],
             url_generator=pytorch_vicuna_v1_3_name_generator,
+            rp_url_generator=lambda model_size, quantization: "",
             cls=VicunaCensoredPytorch,
         ),
     )
+    """
```

### Comparing `xinference-0.0.5/xinference/model/llm/chatglm.py` & `xinference-0.0.6/xinference/model/llm/chatglm.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.5/xinference/model/llm/core.py` & `xinference-0.0.6/xinference/model/llm/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,14 +141,15 @@
         if llamacpp_model_config is None:
             llamacpp_model_config = LlamaCppModelConfig()
         if platform.system() == "Windows":
             llamacpp_model_config.setdefault("n_ctx", 512)
         else:
             llamacpp_model_config.setdefault("n_ctx", 2048)
 
+        llamacpp_model_config.setdefault("embedding", True)
         llamacpp_model_config.setdefault("use_mmap", False)
         llamacpp_model_config.setdefault("use_mlock", True)
 
         if self._is_darwin_and_apple_silicon() and self._can_apply_metal():
             llamacpp_model_config.setdefault("n_gpu_layers", 1)
         elif self._is_linux() and self._can_apply_cublas():
             llamacpp_model_config.setdefault("n_gpu_layers", self._gpu_layers)
```

### Comparing `xinference-0.0.5/xinference/model/llm/llama2.py` & `xinference-0.0.6/xinference/model/llm/llama2.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.5/xinference/model/llm/orca.py` & `xinference-0.0.6/xinference/model/llm/orca.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.5/xinference/model/llm/pytorch/__init__.py` & `xinference-0.0.6/xinference/model/llm/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.5/xinference/model/llm/pytorch/baichuan.py` & `xinference-0.0.6/xinference/model/llm/pytorch/baichuan.py`

 * *Files 14% similar despite different names*

```diff
@@ -61,22 +61,19 @@
             cache_dir=XINFERENCE_CACHE_DIR,
             **kwargs,
         )
         return model, tokenizer
 
 
 class BaichuanPytorchChat(PytorchChatModel):
-    _system_prompt = (
-        "A chat between a curious user and an artificial intelligence assistant. "
-        "The assistant gives helpful, detailed, and polite answers to the user's questions."
-    )
-    _sep = "\n###"
-    _user_name = "User"
-    _assistant_name = "Assistant"
-    _stop = "###"
+    _system_prompt = ""
+    _sep = "\n"
+    _user_name = " <reserved_102> "
+    _assistant_name = " <reserved_103> "
+    _stop_token_ids = [2, 195]
 
     def __init__(
         self,
         model_uid: str,
         model_spec: "ModelSpec",
         model_path: str,
         pytorch_model_config: Optional[PytorchModelConfig] = None,
@@ -85,15 +82,15 @@
             model_uid,
             model_spec,
             model_path,
             system_prompt=self._system_prompt,
             sep=self._sep,
             user_name=self._user_name,
             assistant_name=self._assistant_name,
-            stop=self._stop,
+            stop_token_ids=self._stop_token_ids,
             pytorch_model_config=pytorch_model_config,
         )
         self._use_fast_tokenizer = False
 
     def _load_model(self, kwargs: dict):
         try:
             from transformers import AutoModelForCausalLM, AutoTokenizer
```

### Comparing `xinference-0.0.5/xinference/model/llm/pytorch/core.py` & `xinference-0.0.6/xinference/model/llm/pytorch/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -225,32 +225,39 @@
         model_spec: "ModelSpec",
         model_path: str,
         system_prompt: str,
         sep: str,
         user_name: str,
         assistant_name: str,
         stop: Optional[Union[str, List[str]]] = None,
+        stop_token_ids: Optional[Union[int, List[int]]] = None,
         pytorch_model_config: Optional[PytorchModelConfig] = None,
     ):
         super().__init__(model_uid, model_spec, model_path, pytorch_model_config)
         self._system_prompt: str = system_prompt
         self._sep: str = sep
         self._user_name: str = user_name
         self._assistant_name: str = assistant_name
         self._stop: Optional[Union[str, List[str]]] = stop
+        self._stop_token_ids: Optional[Union[int, List[int]]] = stop_token_ids
 
     def _sanitize_generate_config(
         self,
         pytorch_generate_config: Optional[PytorchGenerateConfig],
     ) -> PytorchGenerateConfig:
         pytorch_generate_config = super()._sanitize_generate_config(
             pytorch_generate_config
         )
         if "stop" not in pytorch_generate_config and self._stop is not None:
             pytorch_generate_config["stop"] = self._stop
+        if (
+            "stop_token_ids" not in pytorch_generate_config
+            and self._stop_token_ids is not None
+        ):
+            pytorch_generate_config["stop_token_ids"] = self._stop_token_ids
 
         return pytorch_generate_config
 
     def chat(
         self,
         prompt: str,
         system_prompt: Optional[str] = None,
```

### Comparing `xinference-0.0.5/xinference/model/llm/pytorch/utils.py` & `xinference-0.0.6/xinference/model/llm/pytorch/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,23 +78,24 @@
     prompt,
     device,
     generate_config,
     judge_sent_end=False,
 ) -> Iterator[Tuple[CompletionChunk, CompletionUsage]]:
     context_len = get_context_length(model.config)
     stream_interval = generate_config.get("stream_interval", 2)
+    stream = generate_config.get("stream", False)
 
     len_prompt = len(prompt)
 
     temperature = float(generate_config.get("temperature", 1.0))
     repetition_penalty = float(generate_config.get("repetition_penalty", 1.0))
     top_p = float(generate_config.get("top_p", 1.0))
     top_k = int(generate_config.get("top_k", -1))  # -1 means disable
     max_new_tokens = int(generate_config.get("max_new_tokens", 256))
-    echo = bool(generate_config.get("echo", True))
+    echo = bool(generate_config.get("echo", False))
     stop_str = generate_config.get("stop", None)
     stop_token_ids = generate_config.get("stop_token_ids", None) or []
     stop_token_ids.append(tokenizer.eos_token_id)
 
     logits_processor = prepare_logits_processor(
         temperature, repetition_penalty, top_p, top_k
     )
@@ -119,14 +120,15 @@
             dtype=torch.int64,
             device=device,
         )
 
     past_key_values = out = None
     sent_interrupt = False
     token = None
+    last_output_length = 0
     for i in range(max_new_tokens):
         if i == 0:
             if model.config.is_encoder_decoder:
                 out = model.decoder(
                     input_ids=start_ids,
                     encoder_hidden_states=encoder_output,
                     use_cache=True,
@@ -199,14 +201,15 @@
 
             output = tokenizer.decode(
                 tmp_output_ids,
                 skip_special_tokens=True,
                 spaces_between_special_tokens=False,
                 clean_up_tokenization_spaces=True,
             )
+
             # TODO: For the issue of incomplete sentences interrupting output, apply a patch and others can also modify it to a more elegant way
             if judge_sent_end and stopped and not is_sentence_complete(output):
                 if len(tokens) > 1:
                     token = tokens[1]
                     output_ids[-1] = token
                 else:
                     output_ids.pop()
@@ -232,14 +235,19 @@
                         else:
                             partially_stopped = is_partial_stop(output, each_stop)
                             if partially_stopped:
                                 break
                 else:
                     raise ValueError("Invalid stop field type.")
 
+            if stream:
+                tmp_output_length = len(output)
+                output = output[last_output_length:]
+                last_output_length = tmp_output_length
+
             # prevent yielding partial stop sequence
             if not partially_stopped:
                 completion_choice = CompletionChoice(
                     text=output, index=0, logprobs=None, finish_reason=None
                 )
                 completion_chunk = CompletionChunk(
                     id=str(uuid.uuid1()),
```

### Comparing `xinference-0.0.5/xinference/model/llm/pytorch/vicuna.py` & `xinference-0.0.6/xinference/model/llm/pytorch/vicuna.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.5/xinference/model/llm/utils.py` & `xinference-0.0.6/xinference/model/llm/utils.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.5/xinference/model/llm/vicuna.py` & `xinference-0.0.6/xinference/model/llm/vicuna.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.5/xinference/model/llm/wizardlm.py` & `xinference-0.0.6/xinference/model/llm/wizardlm.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.5/xinference/types.py` & `xinference-0.0.6/xinference/types.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.5/xinference.egg-info/PKG-INFO` & `xinference-0.0.6/xinference.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xinference
-Version: 0.0.5
+Version: 0.0.6
 Summary: Model Serving Made Easy
 Home-page: https://github.com/xorbitsai/inference
 Author: Qin Xuye
 Author-email: qinxuye@xprobe.io
 Maintainer: Qin Xuye
 Maintainer-email: qinxuye@xprobe.io
 License: Apache License 2.0
@@ -30,15 +30,15 @@
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/xinference.svg?style=for-the-badge)](https://pypi.org/project/xinference/)
 [![License](https://img.shields.io/pypi/l/xinference.svg?style=for-the-badge)](https://github.com/xorbitsai/inference/blob/main/LICENSE)
 [![Build Status](https://img.shields.io/github/actions/workflow/status/xorbitsai/inference/python.yaml?branch=main&style=for-the-badge&label=GITHUB%20ACTIONS&logo=github)](https://actions-badge.atrox.dev/xorbitsai/inference/goto?ref=main)
 [![Slack](https://img.shields.io/badge/join_Slack-781FF5.svg?logo=slack&style=for-the-badge)](https://join.slack.com/t/xorbitsio/shared_invite/zt-1o3z9ucdh-RbfhbPVpx7prOVdM1CAuxg)
 [![Twitter](https://img.shields.io/twitter/follow/xorbitsio?logo=twitter&style=for-the-badge)](https://twitter.com/xorbitsio)
 
-English | [中文介绍](README_zh_CN.md)
+English | [中文介绍](README_zh_CN.md) | [日本語](README_ja_JP.md)
 </div>
 <br />
 
 
 Xorbits Inference(Xinference) is a powerful and versatile library designed to serve language, 
 speech recognition, and multimodal models. With Xorbits Inference, you can effortlessly deploy 
 and serve your or state-of-the-art built-in models using just a single command. Whether you are a 
@@ -199,14 +199,15 @@
 | orca          | SFT Model        | en       | ggmlv3  | 3, 7, 13           | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0'  |
 
 
 **NOTE**:
 - Xinference will download models automatically for you, and by default the models will be saved under `${USER}/.xinference/cache`.
 - Foundation models only provide interface `generate`.
 - RLHF and SFT models provide both `generate` and `chat`.
+- If you want to use Apple Metal GPU for acceleration, please choose the q4_0 and q4_1 quantization methods.
 
 ## Roadmap
 Xinference is currently under active development. Here's a roadmap outlining our planned 
 developments for the next few weeks:
 
 ### PyTorch Support
 With PyTorch integration, users will be able to seamlessly utilize PyTorch models from Hugging Face
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xinference Version: 0.0.5 Summary: Model Serving
+Metadata-Version: 2.1 Name: xinference Version: 0.0.6 Summary: Model Serving
 Made Easy Home-page: https://github.com/xorbitsai/inference Author: Qin Xuye
 Author-email: qinxuye@xprobe.io Maintainer: Qin Xuye Maintainer-email:
 qinxuye@xprobe.io License: Apache License 2.0 Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
@@ -18,15 +18,15 @@
   workflow/status/xorbitsai/inference/python.yaml?branch=main&style=for-the-
   badge&label=GITHUB%20ACTIONS&logo=github)](https://actions-badge.atrox.dev/
   xorbitsai/inference/goto?ref=main) [![Slack](https://img.shields.io/badge/
 join_Slack-781FF5.svg?logo=slack&style=for-the-badge)](https://join.slack.com/
   t/xorbitsio/shared_invite/zt-1o3z9ucdh-RbfhbPVpx7prOVdM1CAuxg) [![Twitter]
  (https://img.shields.io/twitter/follow/xorbitsio?logo=twitter&style=for-the-
         badge)](https://twitter.com/xorbitsio) English | [ä¸­æä»ç»]
-                               (README_zh_CN.md)
+               (README_zh_CN.md) | [æ¥æ¬èª](README_ja_JP.md)
 
 Xorbits Inference(Xinference) is a powerful and versatile library designed to
 serve language, speech recognition, and multimodal models. With Xorbits
 Inference, you can effortlessly deploy and serve your or state-of-the-art
 built-in models using just a single command. Whether you are a researcher,
 developer, or data scientist, Xorbits Inference empowers you to unleash the
 full potential of cutting-edge AI models. ![demo](assets/demo.gif)
@@ -112,13 +112,15 @@
 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' | | wizardlm-v1.1 | SFT Model | en |
 ggmlv3 | 13 | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' | | vicuna-v1.3 | SFT
 Model | en | ggmlv3 | 7, 13 | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' | | orca |
 SFT Model | en | ggmlv3 | 3, 7, 13 | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0' |
 **NOTE**: - Xinference will download models automatically for you, and by
 default the models will be saved under `${USER}/.xinference/cache`. -
 Foundation models only provide interface `generate`. - RLHF and SFT models
-provide both `generate` and `chat`. ## Roadmap Xinference is currently under
-active development. Here's a roadmap outlining our planned developments for the
-next few weeks: ### PyTorch Support With PyTorch integration, users will be
-able to seamlessly utilize PyTorch models from Hugging Face within Xinference.
-### Langchain & LlamaIndex integration With Xinference, it will be much easier
-for users to use these libraries and build applications with LLMs.
+provide both `generate` and `chat`. - If you want to use Apple Metal GPU for
+acceleration, please choose the q4_0 and q4_1 quantization methods. ## Roadmap
+Xinference is currently under active development. Here's a roadmap outlining
+our planned developments for the next few weeks: ### PyTorch Support With
+PyTorch integration, users will be able to seamlessly utilize PyTorch models
+from Hugging Face within Xinference. ### Langchain & LlamaIndex integration
+With Xinference, it will be much easier for users to use these libraries and
+build applications with LLMs.
```

### Comparing `xinference-0.0.5/xinference.egg-info/SOURCES.txt` & `xinference-0.0.6/xinference.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `xinference-0.0.5/xinference.egg-info/requires.txt` & `xinference-0.0.6/xinference.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 xoscar
 xorbits
-gradio
+gradio>=3.35.0
 click
 tqdm
 tabulate
 requests
 pydantic
 fastapi
 uvicorn
@@ -14,14 +14,16 @@
 chatglm-cpp
 llama-cpp-python
 transformers
 torch
 accelerate
 sentencepiece
 transformers_stream_generator
+
+[all:platform_system != "Darwin"]
 cpm_kernels
 
 [dev]
 cython>=0.29
 pytest>=3.5.0
 pytest-cov>=2.5.0
 pytest-timeout>=1.2.0
```

