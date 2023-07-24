# Comparing `tmp/google-cloud-datastream-1.6.1.tar.gz` & `tmp/google-cloud-datastream-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-datastream-1.6.1.tar", last modified: Wed Jul  5 15:52:24 2023, max compression
+gzip compressed data, was "google-cloud-datastream-1.7.0.tar", last modified: Mon Jul 24 20:57:07 2023, max compression
```

## Comparing `google-cloud-datastream-1.6.1.tar` & `google-cloud-datastream-1.7.0.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:24.085279 google-cloud-datastream-1.6.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4649 2023-07-05 15:52:24.085279 google-cloud-datastream-1.6.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3722 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:24.069279 google-cloud-datastream-1.6.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:24.073279 google-cloud-datastream-1.6.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:24.073279 google-cloud-datastream-1.6.1/google/cloud/datastream/
--rw-rw-r--   0 root         (0)     1003     5078 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       84 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:24.073279 google-cloud-datastream-1.6.1/google/cloud/datastream_v1/
--rw-rw-r--   0 root         (0)     1003     4916 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    10384 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       84 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:24.073279 google-cloud-datastream-1.6.1/google/cloud/datastream_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:24.077279 google-cloud-datastream-1.6.1/google/cloud/datastream_v1/services/datastream/
--rw-rw-r--   0 root         (0)     1003      753 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1/services/datastream/__init__.py
--rw-rw-r--   0 root         (0)     1003   141667 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1/services/datastream/async_client.py
--rw-rw-r--   0 root         (0)     1003   157494 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1/services/datastream/client.py
--rw-rw-r--   0 root         (0)     1003    31348 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1/services/datastream/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:24.077279 google-cloud-datastream-1.6.1/google/cloud/datastream_v1/services/datastream/transports/
--rw-rw-r--   0 root         (0)     1003     1344 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1/services/datastream/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    19242 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1/services/datastream/transports/base.py
--rw-rw-r--   0 root         (0)     1003    46386 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1/services/datastream/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    47307 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1/services/datastream/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   160708 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1/services/datastream/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:24.077279 google-cloud-datastream-1.6.1/google/cloud/datastream_v1/types/
--rw-rw-r--   0 root         (0)     1003     4661 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    44898 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1/types/datastream.py
--rw-rw-r--   0 root         (0)     1003    64096 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1/types/datastream_resources.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:24.077279 google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/
--rw-rw-r--   0 root         (0)     1003     4154 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/__init__.py
--rw-rw-r--   0 root         (0)     1003     8809 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       84 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:24.077279 google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:24.081279 google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/services/datastream/
--rw-rw-r--   0 root         (0)     1003      753 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/services/datastream/__init__.py
--rw-rw-r--   0 root         (0)     1003   111056 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/services/datastream/async_client.py
--rw-rw-r--   0 root         (0)     1003   125201 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/services/datastream/client.py
--rw-rw-r--   0 root         (0)     1003    26460 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/services/datastream/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:24.081279 google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/services/datastream/transports/
--rw-rw-r--   0 root         (0)     1003     1344 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/services/datastream/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    15616 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/services/datastream/transports/base.py
--rw-rw-r--   0 root         (0)     1003    36520 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/services/datastream/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    37308 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/services/datastream/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   116775 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/services/datastream/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:24.081279 google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/types/
--rw-rw-r--   0 root         (0)     1003     3893 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    38294 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/types/datastream.py
--rw-rw-r--   0 root         (0)     1003    40603 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/types/datastream_resources.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:24.085279 google-cloud-datastream-1.6.1/google_cloud_datastream.egg-info/
--rw-r--r--   0 root         (0)     1003     4649 2023-07-05 15:52:24.000000 google-cloud-datastream-1.6.1/google_cloud_datastream.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2747 2023-07-05 15:52:24.000000 google-cloud-datastream-1.6.1/google_cloud_datastream.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:52:24.000000 google-cloud-datastream-1.6.1/google_cloud_datastream.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:52:24.000000 google-cloud-datastream-1.6.1/google_cloud_datastream.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:52:24.000000 google-cloud-datastream-1.6.1/google_cloud_datastream.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-07-05 15:52:24.000000 google-cloud-datastream-1.6.1/google_cloud_datastream.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:52:24.000000 google-cloud-datastream-1.6.1/google_cloud_datastream.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:52:24.085279 google-cloud-datastream-1.6.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2982 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:24.085279 google-cloud-datastream-1.6.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:24.085279 google-cloud-datastream-1.6.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:24.085279 google-cloud-datastream-1.6.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:24.085279 google-cloud-datastream-1.6.1/tests/unit/gapic/datastream_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/tests/unit/gapic/datastream_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   654590 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/tests/unit/gapic/datastream_v1/test_datastream.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:24.085279 google-cloud-datastream-1.6.1/tests/unit/gapic/datastream_v1alpha1/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/tests/unit/gapic/datastream_v1alpha1/__init__.py
--rw-rw-r--   0 root         (0)     1003   510931 2023-07-05 15:46:58.000000 google-cloud-datastream-1.6.1/tests/unit/gapic/datastream_v1alpha1/test_datastream.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:07.002594 google-cloud-datastream-1.7.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4649 2023-07-24 20:57:07.002594 google-cloud-datastream-1.7.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3722 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:06.986594 google-cloud-datastream-1.7.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:06.986594 google-cloud-datastream-1.7.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:06.990594 google-cloud-datastream-1.7.0/google/cloud/datastream/
+-rw-rw-r--   0 root         (0)     1003     5078 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/google/cloud/datastream/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/google/cloud/datastream/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       84 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/google/cloud/datastream/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:06.990594 google-cloud-datastream-1.7.0/google/cloud/datastream_v1/
+-rw-rw-r--   0 root         (0)     1003     4916 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/google/cloud/datastream_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10384 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/google/cloud/datastream_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/google/cloud/datastream_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       84 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/google/cloud/datastream_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:06.990594 google-cloud-datastream-1.7.0/google/cloud/datastream_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/google/cloud/datastream_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:06.990594 google-cloud-datastream-1.7.0/google/cloud/datastream_v1/services/datastream/
+-rw-rw-r--   0 root         (0)     1003      753 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/google/cloud/datastream_v1/services/datastream/__init__.py
+-rw-rw-r--   0 root         (0)     1003   141667 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/google/cloud/datastream_v1/services/datastream/async_client.py
+-rw-rw-r--   0 root         (0)     1003   157494 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/google/cloud/datastream_v1/services/datastream/client.py
+-rw-rw-r--   0 root         (0)     1003    31348 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/google/cloud/datastream_v1/services/datastream/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:06.990594 google-cloud-datastream-1.7.0/google/cloud/datastream_v1/services/datastream/transports/
+-rw-rw-r--   0 root         (0)     1003     1344 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/google/cloud/datastream_v1/services/datastream/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    19242 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/google/cloud/datastream_v1/services/datastream/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    46386 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/google/cloud/datastream_v1/services/datastream/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    47307 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/google/cloud/datastream_v1/services/datastream/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   160708 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/google/cloud/datastream_v1/services/datastream/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:06.994594 google-cloud-datastream-1.7.0/google/cloud/datastream_v1/types/
+-rw-rw-r--   0 root         (0)     1003     4661 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/google/cloud/datastream_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    44898 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/google/cloud/datastream_v1/types/datastream.py
+-rw-rw-r--   0 root         (0)     1003    64353 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/google/cloud/datastream_v1/types/datastream_resources.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:06.994594 google-cloud-datastream-1.7.0/google/cloud/datastream_v1alpha1/
+-rw-rw-r--   0 root         (0)     1003     4154 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/google/cloud/datastream_v1alpha1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8809 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/google/cloud/datastream_v1alpha1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/google/cloud/datastream_v1alpha1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       84 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/google/cloud/datastream_v1alpha1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:06.994594 google-cloud-datastream-1.7.0/google/cloud/datastream_v1alpha1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/google/cloud/datastream_v1alpha1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:06.994594 google-cloud-datastream-1.7.0/google/cloud/datastream_v1alpha1/services/datastream/
+-rw-rw-r--   0 root         (0)     1003      753 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/google/cloud/datastream_v1alpha1/services/datastream/__init__.py
+-rw-rw-r--   0 root         (0)     1003   111056 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/google/cloud/datastream_v1alpha1/services/datastream/async_client.py
+-rw-rw-r--   0 root         (0)     1003   125201 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/google/cloud/datastream_v1alpha1/services/datastream/client.py
+-rw-rw-r--   0 root         (0)     1003    26460 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/google/cloud/datastream_v1alpha1/services/datastream/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:06.994594 google-cloud-datastream-1.7.0/google/cloud/datastream_v1alpha1/services/datastream/transports/
+-rw-rw-r--   0 root         (0)     1003     1344 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/google/cloud/datastream_v1alpha1/services/datastream/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    15616 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/google/cloud/datastream_v1alpha1/services/datastream/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    36520 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/google/cloud/datastream_v1alpha1/services/datastream/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    37308 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/google/cloud/datastream_v1alpha1/services/datastream/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   116775 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/google/cloud/datastream_v1alpha1/services/datastream/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:06.998594 google-cloud-datastream-1.7.0/google/cloud/datastream_v1alpha1/types/
+-rw-rw-r--   0 root         (0)     1003     3893 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/google/cloud/datastream_v1alpha1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    38294 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/google/cloud/datastream_v1alpha1/types/datastream.py
+-rw-rw-r--   0 root         (0)     1003    40604 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/google/cloud/datastream_v1alpha1/types/datastream_resources.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:06.998594 google-cloud-datastream-1.7.0/google_cloud_datastream.egg-info/
+-rw-r--r--   0 root         (0)     1003     4649 2023-07-24 20:57:06.000000 google-cloud-datastream-1.7.0/google_cloud_datastream.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2747 2023-07-24 20:57:06.000000 google-cloud-datastream-1.7.0/google_cloud_datastream.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-24 20:57:06.000000 google-cloud-datastream-1.7.0/google_cloud_datastream.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-24 20:57:06.000000 google-cloud-datastream-1.7.0/google_cloud_datastream.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-24 20:57:06.000000 google-cloud-datastream-1.7.0/google_cloud_datastream.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-07-24 20:57:06.000000 google-cloud-datastream-1.7.0/google_cloud_datastream.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-24 20:57:06.000000 google-cloud-datastream-1.7.0/google_cloud_datastream.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-24 20:57:07.002594 google-cloud-datastream-1.7.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2982 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:06.998594 google-cloud-datastream-1.7.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:06.998594 google-cloud-datastream-1.7.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:06.998594 google-cloud-datastream-1.7.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:06.998594 google-cloud-datastream-1.7.0/tests/unit/gapic/datastream_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/tests/unit/gapic/datastream_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   655070 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/tests/unit/gapic/datastream_v1/test_datastream.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:06.998594 google-cloud-datastream-1.7.0/tests/unit/gapic/datastream_v1alpha1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/tests/unit/gapic/datastream_v1alpha1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   510931 2023-07-24 20:53:51.000000 google-cloud-datastream-1.7.0/tests/unit/gapic/datastream_v1alpha1/test_datastream.py
```

### Comparing `google-cloud-datastream-1.6.1/LICENSE` & `google-cloud-datastream-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.6.1/MANIFEST.in` & `google-cloud-datastream-1.7.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.6.1/PKG-INFO` & `google-cloud-datastream-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-datastream
-Version: 1.6.1
+Version: 1.7.0
 Summary: Google Cloud Datastream API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-datastream-1.6.1/README.rst` & `google-cloud-datastream-1.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.6.1/google/cloud/datastream/__init__.py` & `google-cloud-datastream-1.7.0/google/cloud/datastream/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-datastream-1.6.1/google/cloud/datastream/gapic_version.py` & `google-cloud-datastream-1.7.0/google/cloud/datastream/gapic_version.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.6.1"  # {x-release-please-version}
+__version__ = "1.7.0"  # {x-release-please-version}
```

### Comparing `google-cloud-datastream-1.6.1/google/cloud/datastream_v1/__init__.py` & `google-cloud-datastream-1.7.0/google/cloud/datastream_v1/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-datastream-1.6.1/google/cloud/datastream_v1/gapic_metadata.json` & `google-cloud-datastream-1.7.0/google/cloud/datastream_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.6.1/google/cloud/datastream_v1/gapic_version.py` & `google-cloud-datastream-1.7.0/google/cloud/datastream_v1/gapic_version.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.6.1"  # {x-release-please-version}
+__version__ = "1.7.0"  # {x-release-please-version}
```

### Comparing `google-cloud-datastream-1.6.1/google/cloud/datastream_v1/services/__init__.py` & `google-cloud-datastream-1.7.0/google/cloud/datastream_v1/services/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-datastream-1.6.1/google/cloud/datastream_v1/services/datastream/__init__.py` & `google-cloud-datastream-1.7.0/google/cloud/datastream_v1/services/datastream/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-datastream-1.6.1/google/cloud/datastream_v1/services/datastream/async_client.py` & `google-cloud-datastream-1.7.0/google/cloud/datastream_v1/services/datastream/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-datastream-1.6.1/google/cloud/datastream_v1/services/datastream/client.py` & `google-cloud-datastream-1.7.0/google/cloud/datastream_v1/services/datastream/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-datastream-1.6.1/google/cloud/datastream_v1/services/datastream/pagers.py` & `google-cloud-datastream-1.7.0/google/cloud/datastream_v1/services/datastream/pagers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-datastream-1.6.1/google/cloud/datastream_v1/services/datastream/transports/__init__.py` & `google-cloud-datastream-1.7.0/google/cloud/datastream_v1/services/datastream/transports/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-datastream-1.6.1/google/cloud/datastream_v1/services/datastream/transports/base.py` & `google-cloud-datastream-1.7.0/google/cloud/datastream_v1/services/datastream/transports/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-datastream-1.6.1/google/cloud/datastream_v1/services/datastream/transports/grpc.py` & `google-cloud-datastream-1.7.0/google/cloud/datastream_v1/services/datastream/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-datastream-1.6.1/google/cloud/datastream_v1/services/datastream/transports/grpc_asyncio.py` & `google-cloud-datastream-1.7.0/google/cloud/datastream_v1/services/datastream/transports/grpc_asyncio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-datastream-1.6.1/google/cloud/datastream_v1/services/datastream/transports/rest.py` & `google-cloud-datastream-1.7.0/google/cloud/datastream_v1/services/datastream/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-datastream-1.6.1/google/cloud/datastream_v1/types/__init__.py` & `google-cloud-datastream-1.7.0/google/cloud/datastream_v1/types/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-datastream-1.6.1/google/cloud/datastream_v1/types/datastream.py` & `google-cloud-datastream-1.7.0/google/cloud/datastream_v1/types/datastream.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-datastream-1.6.1/google/cloud/datastream_v1/types/datastream_resources.py` & `google-cloud-datastream-1.7.0/google/cloud/datastream_v1/types/datastream_resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -1024,28 +1024,33 @@
 
     Attributes:
         column (str):
             Column name.
         data_type (str):
             The MySQL data type. Full data types list can
             be found here:
+
             https://dev.mysql.com/doc/refman/8.0/en/data-types.html
         length (int):
             Column length.
         collation (str):
             Column collation.
         primary_key (bool):
             Whether or not the column represents a
             primary key.
         nullable (bool):
             Whether or not the column can accept a null
             value.
         ordinal_position (int):
             The ordinal position of the column in the
             table.
+        precision (int):
+            Column precision.
+        scale (int):
+            Column scale.
     """
 
     column: str = proto.Field(
         proto.STRING,
         number=1,
     )
     data_type: str = proto.Field(
@@ -1068,14 +1073,22 @@
         proto.BOOL,
         number=6,
     )
     ordinal_position: int = proto.Field(
         proto.INT32,
         number=7,
     )
+    precision: int = proto.Field(
+        proto.INT32,
+        number=8,
+    )
+    scale: int = proto.Field(
+        proto.INT32,
+        number=9,
+    )
 
 
 class MysqlTable(proto.Message):
     r"""MySQL table.
 
     Attributes:
         table (str):
```

### Comparing `google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/__init__.py` & `google-cloud-datastream-1.7.0/google/cloud/datastream_v1alpha1/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/gapic_metadata.json` & `google-cloud-datastream-1.7.0/google/cloud/datastream_v1alpha1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/gapic_version.py` & `google-cloud-datastream-1.7.0/google/cloud/datastream_v1alpha1/gapic_version.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.6.1"  # {x-release-please-version}
+__version__ = "1.7.0"  # {x-release-please-version}
```

### Comparing `google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/services/__init__.py` & `google-cloud-datastream-1.7.0/google/cloud/datastream_v1alpha1/services/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/services/datastream/__init__.py` & `google-cloud-datastream-1.7.0/google/cloud/datastream_v1alpha1/services/datastream/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/services/datastream/async_client.py` & `google-cloud-datastream-1.7.0/google/cloud/datastream_v1alpha1/services/datastream/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/services/datastream/client.py` & `google-cloud-datastream-1.7.0/google/cloud/datastream_v1alpha1/services/datastream/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/services/datastream/pagers.py` & `google-cloud-datastream-1.7.0/google/cloud/datastream_v1alpha1/services/datastream/pagers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/services/datastream/transports/__init__.py` & `google-cloud-datastream-1.7.0/google/cloud/datastream_v1alpha1/services/datastream/transports/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/services/datastream/transports/base.py` & `google-cloud-datastream-1.7.0/google/cloud/datastream_v1alpha1/services/datastream/transports/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/services/datastream/transports/grpc.py` & `google-cloud-datastream-1.7.0/google/cloud/datastream_v1alpha1/services/datastream/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/services/datastream/transports/grpc_asyncio.py` & `google-cloud-datastream-1.7.0/google/cloud/datastream_v1alpha1/services/datastream/transports/grpc_asyncio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/services/datastream/transports/rest.py` & `google-cloud-datastream-1.7.0/google/cloud/datastream_v1alpha1/services/datastream/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/types/__init__.py` & `google-cloud-datastream-1.7.0/google/cloud/datastream_v1alpha1/types/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/types/datastream.py` & `google-cloud-datastream-1.7.0/google/cloud/datastream_v1alpha1/types/datastream.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-datastream-1.6.1/google/cloud/datastream_v1alpha1/types/datastream_resources.py` & `google-cloud-datastream-1.7.0/google/cloud/datastream_v1alpha1/types/datastream_resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -762,14 +762,15 @@
 
     Attributes:
         column_name (str):
             Column name.
         data_type (str):
             The MySQL data type. Full data types list can
             be found here:
+
             https://dev.mysql.com/doc/refman/8.0/en/data-types.html
         length (int):
             Column length.
         collation (str):
             Column collation.
         primary_key (bool):
             Whether or not the column represents a
```

### Comparing `google-cloud-datastream-1.6.1/google_cloud_datastream.egg-info/PKG-INFO` & `google-cloud-datastream-1.7.0/google_cloud_datastream.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-datastream
-Version: 1.6.1
+Version: 1.7.0
 Summary: Google Cloud Datastream API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-datastream-1.6.1/google_cloud_datastream.egg-info/SOURCES.txt` & `google-cloud-datastream-1.7.0/google_cloud_datastream.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-datastream-1.6.1/setup.py` & `google-cloud-datastream-1.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-datastream-1.6.1/tests/__init__.py` & `google-cloud-datastream-1.7.0/tests/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-datastream-1.6.1/tests/unit/__init__.py` & `google-cloud-datastream-1.7.0/tests/unit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-datastream-1.6.1/tests/unit/gapic/__init__.py` & `google-cloud-datastream-1.7.0/tests/unit/gapic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-datastream-1.6.1/tests/unit/gapic/datastream_v1/__init__.py` & `google-cloud-datastream-1.7.0/tests/unit/gapic/datastream_v1/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-datastream-1.6.1/tests/unit/gapic/datastream_v1/test_datastream.py` & `google-cloud-datastream-1.7.0/tests/unit/gapic/datastream_v1/test_datastream.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10416,14 +10416,16 @@
                                             "column": "column_value",
                                             "data_type": "data_type_value",
                                             "length": 642,
                                             "collation": "collation_value",
                                             "primary_key": True,
                                             "nullable": True,
                                             "ordinal_position": 1725,
+                                            "precision": 972,
+                                            "scale": 520,
                                         }
                                     ],
                                 }
                             ],
                         }
                     ]
                 },
@@ -10764,14 +10766,16 @@
                                             "column": "column_value",
                                             "data_type": "data_type_value",
                                             "length": 642,
                                             "collation": "collation_value",
                                             "primary_key": True,
                                             "nullable": True,
                                             "ordinal_position": 1725,
+                                            "precision": 972,
+                                            "scale": 520,
                                         }
                                     ],
                                 }
                             ],
                         }
                     ]
                 },
@@ -10997,14 +11001,16 @@
                                             "column": "column_value",
                                             "data_type": "data_type_value",
                                             "length": 642,
                                             "collation": "collation_value",
                                             "primary_key": True,
                                             "nullable": True,
                                             "ordinal_position": 1725,
+                                            "precision": 972,
+                                            "scale": 520,
                                         }
                                     ],
                                 }
                             ],
                         }
                     ]
                 },
@@ -11323,14 +11329,16 @@
                                             "column": "column_value",
                                             "data_type": "data_type_value",
                                             "length": 642,
                                             "collation": "collation_value",
                                             "primary_key": True,
                                             "nullable": True,
                                             "ordinal_position": 1725,
+                                            "precision": 972,
+                                            "scale": 520,
                                         }
                                     ],
                                 }
                             ],
                         }
                     ]
                 },
```

### Comparing `google-cloud-datastream-1.6.1/tests/unit/gapic/datastream_v1alpha1/__init__.py` & `google-cloud-datastream-1.7.0/tests/unit/gapic/datastream_v1alpha1/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-datastream-1.6.1/tests/unit/gapic/datastream_v1alpha1/test_datastream.py` & `google-cloud-datastream-1.7.0/tests/unit/gapic/datastream_v1alpha1/test_datastream.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

