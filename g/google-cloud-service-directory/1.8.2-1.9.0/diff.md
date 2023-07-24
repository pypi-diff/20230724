# Comparing `tmp/google-cloud-service-directory-1.8.2.tar.gz` & `tmp/google-cloud-service-directory-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-service-directory-1.8.2.tar", last modified: Wed Jul  5 15:55:45 2023, max compression
+gzip compressed data, was "google-cloud-service-directory-1.9.0.tar", last modified: Mon Jul 24 20:57:12 2023, max compression
```

## Comparing `google-cloud-service-directory-1.8.2.tar` & `google-cloud-service-directory-1.9.0.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.209954 google-cloud-service-directory-1.8.2/
--rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4636 2023-07-05 15:55:45.209954 google-cloud-service-directory-1.8.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3695 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.193955 google-cloud-service-directory-1.8.2/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.193955 google-cloud-service-directory-1.8.2/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.197955 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory/
--rw-rw-r--   0 root         (0)     1003     2830 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       91 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.197955 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/
--rw-rw-r--   0 root         (0)     1003     2391 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     8096 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       91 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.197955 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.197955 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/lookup_service/
--rw-rw-r--   0 root         (0)     1003      765 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/lookup_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    13015 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/lookup_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    22993 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/lookup_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.197955 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/lookup_service/transports/
--rw-rw-r--   0 root         (0)     1003     1386 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/lookup_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6097 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/lookup_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    11949 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/lookup_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    12162 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/lookup_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    12672 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/lookup_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.201954 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/registration_service/
--rw-rw-r--   0 root         (0)     1003      789 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/registration_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    97044 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/registration_service/async_client.py
--rw-rw-r--   0 root         (0)     1003   110000 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/registration_service/client.py
--rw-rw-r--   0 root         (0)     1003    16223 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/registration_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.201954 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/registration_service/transports/
--rw-rw-r--   0 root         (0)     1003     1478 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/registration_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    14234 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/registration_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    32351 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/registration_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    33079 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/registration_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   109437 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/registration_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.201954 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/types/
--rw-rw-r--   0 root         (0)     1003     1911 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     3578 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/types/endpoint.py
--rw-rw-r--   0 root         (0)     1003     3222 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/types/lookup_service.py
--rw-rw-r--   0 root         (0)     1003     1773 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/types/namespace.py
--rw-rw-r--   0 root         (0)     1003    20397 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/types/registration_service.py
--rw-rw-r--   0 root         (0)     1003     3593 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/types/service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.201954 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/
--rw-rw-r--   0 root         (0)     1003     2396 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     8106 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       91 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.201954 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.201954 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/
--rw-rw-r--   0 root         (0)     1003      765 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    13214 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    23671 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.205954 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/
--rw-rw-r--   0 root         (0)     1003     1386 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6107 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    11972 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    12185 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    12692 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.205954 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/registration_service/
--rw-rw-r--   0 root         (0)     1003      789 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/registration_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    97874 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/registration_service/async_client.py
--rw-rw-r--   0 root         (0)     1003   111297 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/registration_service/client.py
--rw-rw-r--   0 root         (0)     1003    16348 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/registration_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.205954 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/
--rw-rw-r--   0 root         (0)     1003     1478 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    14274 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    32502 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    33230 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   109730 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.205954 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/types/
--rw-rw-r--   0 root         (0)     1003     1911 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     4827 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/types/endpoint.py
--rw-rw-r--   0 root         (0)     1003     4396 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/types/lookup_service.py
--rw-rw-r--   0 root         (0)     1003     2425 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/types/namespace.py
--rw-rw-r--   0 root         (0)     1003    22661 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/types/registration_service.py
--rw-rw-r--   0 root         (0)     1003     4552 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/types/service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.209954 google-cloud-service-directory-1.8.2/google_cloud_service_directory.egg-info/
--rw-r--r--   0 root         (0)     1003     4636 2023-07-05 15:55:45.000000 google-cloud-service-directory-1.8.2/google_cloud_service_directory.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     4919 2023-07-05 15:55:45.000000 google-cloud-service-directory-1.8.2/google_cloud_service_directory.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:55:45.000000 google-cloud-service-directory-1.8.2/google_cloud_service_directory.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:55:45.000000 google-cloud-service-directory-1.8.2/google_cloud_service_directory.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:55:45.000000 google-cloud-service-directory-1.8.2/google_cloud_service_directory.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-07-05 15:55:45.000000 google-cloud-service-directory-1.8.2/google_cloud_service_directory.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:55:45.000000 google-cloud-service-directory-1.8.2/google_cloud_service_directory.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:55:45.209954 google-cloud-service-directory-1.8.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3008 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.209954 google-cloud-service-directory-1.8.2/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.209954 google-cloud-service-directory-1.8.2/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.209954 google-cloud-service-directory-1.8.2/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.209954 google-cloud-service-directory-1.8.2/tests/unit/gapic/servicedirectory_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/tests/unit/gapic/servicedirectory_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    67100 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/tests/unit/gapic/servicedirectory_v1/test_lookup_service.py
--rw-rw-r--   0 root         (0)     1003   409087 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/tests/unit/gapic/servicedirectory_v1/test_registration_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.209954 google-cloud-service-directory-1.8.2/tests/unit/gapic/servicedirectory_v1beta1/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/tests/unit/gapic/servicedirectory_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003    67752 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/tests/unit/gapic/servicedirectory_v1beta1/test_lookup_service.py
--rw-rw-r--   0 root         (0)     1003   412321 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/tests/unit/gapic/servicedirectory_v1beta1/test_registration_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.606364 google-cloud-service-directory-1.9.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4636 2023-07-24 20:57:12.606364 google-cloud-service-directory-1.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3695 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.582365 google-cloud-service-directory-1.9.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.582365 google-cloud-service-directory-1.9.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.586365 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory/
+-rw-rw-r--   0 root         (0)     1003     2830 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       91 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.586365 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/
+-rw-rw-r--   0 root         (0)     1003     2391 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8096 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       91 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.586365 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.586365 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/lookup_service/
+-rw-rw-r--   0 root         (0)     1003      765 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/lookup_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17303 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/lookup_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    27720 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/lookup_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.586365 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/lookup_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1386 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/lookup_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6688 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/lookup_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13705 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/lookup_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13918 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/lookup_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    19691 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/lookup_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.590365 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/registration_service/
+-rw-rw-r--   0 root         (0)     1003      789 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/registration_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003   101350 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/registration_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003   114733 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/registration_service/client.py
+-rw-rw-r--   0 root         (0)     1003    16223 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/registration_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.590365 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/registration_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1478 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/registration_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14825 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/registration_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    34111 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/registration_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    34839 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/registration_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   116492 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/registration_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.590365 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1911 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4109 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/types/endpoint.py
+-rw-rw-r--   0 root         (0)     1003     4601 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/types/lookup_service.py
+-rw-rw-r--   0 root         (0)     1003     1971 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/types/namespace.py
+-rw-rw-r--   0 root         (0)     1003    22554 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/types/registration_service.py
+-rw-rw-r--   0 root         (0)     1003     3634 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/types/service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.594365 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/
+-rw-rw-r--   0 root         (0)     1003     2396 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8106 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       91 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.594365 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.594365 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/lookup_service/
+-rw-rw-r--   0 root         (0)     1003      765 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/lookup_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17361 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/lookup_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    27778 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/lookup_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.594365 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1386 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6698 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13728 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13941 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    19721 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.598364 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/registration_service/
+-rw-rw-r--   0 root         (0)     1003      789 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/registration_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003   101972 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/registration_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003   115355 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/registration_service/client.py
+-rw-rw-r--   0 root         (0)     1003    16348 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/registration_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.598364 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1478 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14865 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    34203 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    34931 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   117459 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.598364 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/types/
+-rw-rw-r--   0 root         (0)     1003     1911 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4728 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/types/endpoint.py
+-rw-rw-r--   0 root         (0)     1003     4608 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/types/lookup_service.py
+-rw-rw-r--   0 root         (0)     1003     2622 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/types/namespace.py
+-rw-rw-r--   0 root         (0)     1003    23224 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/types/registration_service.py
+-rw-rw-r--   0 root         (0)     1003     4453 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/types/service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.602364 google-cloud-service-directory-1.9.0/google_cloud_service_directory.egg-info/
+-rw-r--r--   0 root         (0)     1003     4636 2023-07-24 20:57:12.000000 google-cloud-service-directory-1.9.0/google_cloud_service_directory.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     4919 2023-07-24 20:57:12.000000 google-cloud-service-directory-1.9.0/google_cloud_service_directory.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-24 20:57:12.000000 google-cloud-service-directory-1.9.0/google_cloud_service_directory.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-24 20:57:12.000000 google-cloud-service-directory-1.9.0/google_cloud_service_directory.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-24 20:57:12.000000 google-cloud-service-directory-1.9.0/google_cloud_service_directory.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-07-24 20:57:12.000000 google-cloud-service-directory-1.9.0/google_cloud_service_directory.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-24 20:57:12.000000 google-cloud-service-directory-1.9.0/google_cloud_service_directory.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-24 20:57:12.606364 google-cloud-service-directory-1.9.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3008 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.602364 google-cloud-service-directory-1.9.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.602364 google-cloud-service-directory-1.9.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.602364 google-cloud-service-directory-1.9.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.602364 google-cloud-service-directory-1.9.0/tests/unit/gapic/servicedirectory_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/tests/unit/gapic/servicedirectory_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    82594 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/tests/unit/gapic/servicedirectory_v1/test_lookup_service.py
+-rw-rw-r--   0 root         (0)     1003   428124 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/tests/unit/gapic/servicedirectory_v1/test_registration_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.602364 google-cloud-service-directory-1.9.0/tests/unit/gapic/servicedirectory_v1beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/tests/unit/gapic/servicedirectory_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    82624 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/tests/unit/gapic/servicedirectory_v1beta1/test_lookup_service.py
+-rw-rw-r--   0 root         (0)     1003   429655 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/tests/unit/gapic/servicedirectory_v1beta1/test_registration_service.py
```

### Comparing `google-cloud-service-directory-1.8.2/LICENSE` & `google-cloud-service-directory-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.2/MANIFEST.in` & `google-cloud-service-directory-1.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.2/PKG-INFO` & `google-cloud-service-directory-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-service-directory
-Version: 1.8.2
+Version: 1.9.0
 Summary: Google Cloud Service Directory API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-service-directory-1.8.2/README.rst` & `google-cloud-service-directory-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory/__init__.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory/__init__.py`

 * *Files 4% similar despite different names*

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

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory/gapic_version.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,15 @@
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
-__version__ = "1.8.2"  # {x-release-please-version}
```

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/__init__.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/__init__.py`

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

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/gapic_metadata.json` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/gapic_version.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,15 @@
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
-__version__ = "1.8.2"  # {x-release-please-version}
```

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/__init__.py` & `google-cloud-service-directory-1.9.0/tests/__init__.py`

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

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/lookup_service/__init__.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/lookup_service/__init__.py`

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

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/lookup_service/async_client.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/lookup_service/async_client.py`

 * *Files 26% similar despite different names*

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
@@ -38,14 +38,16 @@
 from google.cloud.servicedirectory_v1 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
+from google.cloud.location import locations_pb2  # type: ignore
+
 from google.cloud.servicedirectory_v1.types import lookup_service, service
 
 from .client import LookupServiceClient
 from .transports.base import DEFAULT_CLIENT_INFO, LookupServiceTransport
 from .transports.grpc_asyncio import LookupServiceGrpcAsyncIOTransport
 
 
@@ -55,14 +57,16 @@
     _client: LookupServiceClient
 
     DEFAULT_ENDPOINT = LookupServiceClient.DEFAULT_ENDPOINT
     DEFAULT_MTLS_ENDPOINT = LookupServiceClient.DEFAULT_MTLS_ENDPOINT
 
     endpoint_path = staticmethod(LookupServiceClient.endpoint_path)
     parse_endpoint_path = staticmethod(LookupServiceClient.parse_endpoint_path)
+    network_path = staticmethod(LookupServiceClient.network_path)
+    parse_network_path = staticmethod(LookupServiceClient.parse_network_path)
     service_path = staticmethod(LookupServiceClient.service_path)
     parse_service_path = staticmethod(LookupServiceClient.parse_service_path)
     common_billing_account_path = staticmethod(
         LookupServiceClient.common_billing_account_path
     )
     parse_common_billing_account_path = staticmethod(
         LookupServiceClient.parse_common_billing_account_path
@@ -281,14 +285,122 @@
             default_timeout=None,
             client_info=DEFAULT_CLIENT_INFO,
         )
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    async def get_location(
+        self,
+        request: Optional[locations_pb2.GetLocationRequest] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> locations_pb2.Location:
+        r"""Gets information about a location.
+
+        Args:
+            request (:class:`~.location_pb2.GetLocationRequest`):
+                The request object. Request message for
+                `GetLocation` method.
+            retry (google.api_core.retry.Retry): Designation of what errors,
+                 if any, should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            ~.location_pb2.Location:
+                Location object.
+        """
+        # Create or coerce a protobuf request object.
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = locations_pb2.GetLocationRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._client._transport.get_location,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    async def list_locations(
+        self,
+        request: Optional[locations_pb2.ListLocationsRequest] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> locations_pb2.ListLocationsResponse:
+        r"""Lists information about the supported locations for this service.
+
+        Args:
+            request (:class:`~.location_pb2.ListLocationsRequest`):
+                The request object. Request message for
+                `ListLocations` method.
+            retry (google.api_core.retry.Retry): Designation of what errors,
+                 if any, should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            ~.location_pb2.ListLocationsResponse:
+                Response message for ``ListLocations`` method.
+        """
+        # Create or coerce a protobuf request object.
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = locations_pb2.ListLocationsRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._client._transport.list_locations,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
         response = await rpc(
             request,
             retry=retry,
```

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/lookup_service/client.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/lookup_service/client.py`

 * *Files 10% similar despite different names*

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
@@ -42,14 +42,16 @@
 from google.cloud.servicedirectory_v1 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
+from google.cloud.location import locations_pb2  # type: ignore
+
 from google.cloud.servicedirectory_v1.types import lookup_service, service
 
 from .transports.base import DEFAULT_CLIENT_INFO, LookupServiceTransport
 from .transports.grpc import LookupServiceGrpcTransport
 from .transports.grpc_asyncio import LookupServiceGrpcAsyncIOTransport
 from .transports.rest import LookupServiceRestTransport
 
@@ -197,14 +199,34 @@
         m = re.match(
             r"^projects/(?P<project>.+?)/locations/(?P<location>.+?)/namespaces/(?P<namespace>.+?)/services/(?P<service>.+?)/endpoints/(?P<endpoint>.+?)$",
             path,
         )
         return m.groupdict() if m else {}
 
     @staticmethod
+    def network_path(
+        project: str,
+        network: str,
+    ) -> str:
+        """Returns a fully-qualified network string."""
+        return "projects/{project}/locations/global/networks/{network}".format(
+            project=project,
+            network=network,
+        )
+
+    @staticmethod
+    def parse_network_path(path: str) -> Dict[str, str]:
+        """Parses a network path into its component segments."""
+        m = re.match(
+            r"^projects/(?P<project>.+?)/locations/global/networks/(?P<network>.+?)$",
+            path,
+        )
+        return m.groupdict() if m else {}
+
+    @staticmethod
     def service_path(
         project: str,
         location: str,
         namespace: str,
         service: str,
     ) -> str:
         """Returns a fully-qualified service string."""
@@ -562,14 +584,122 @@
         .. warning::
             ONLY use as a context manager if the transport is NOT shared
             with other clients! Exiting the with block will CLOSE the transport
             and may cause errors in other clients!
         """
         self.transport.close()
 
+    def get_location(
+        self,
+        request: Optional[locations_pb2.GetLocationRequest] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> locations_pb2.Location:
+        r"""Gets information about a location.
+
+        Args:
+            request (:class:`~.location_pb2.GetLocationRequest`):
+                The request object. Request message for
+                `GetLocation` method.
+            retry (google.api_core.retry.Retry): Designation of what errors,
+                 if any, should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            ~.location_pb2.Location:
+                Location object.
+        """
+        # Create or coerce a protobuf request object.
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = locations_pb2.GetLocationRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._transport.get_location,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    def list_locations(
+        self,
+        request: Optional[locations_pb2.ListLocationsRequest] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> locations_pb2.ListLocationsResponse:
+        r"""Lists information about the supported locations for this service.
+
+        Args:
+            request (:class:`~.location_pb2.ListLocationsRequest`):
+                The request object. Request message for
+                `ListLocations` method.
+            retry (google.api_core.retry.Retry): Designation of what errors,
+                 if any, should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            ~.location_pb2.ListLocationsResponse:
+                Response message for ``ListLocations`` method.
+        """
+        # Create or coerce a protobuf request object.
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = locations_pb2.ListLocationsRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._transport.list_locations,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
     gapic_version=package_version.__version__
 )
 
 
 __all__ = ("LookupServiceClient",)
```

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/lookup_service/transports/__init__.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/lookup_service/transports/__init__.py`

 * *Files 5% similar despite different names*

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

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/lookup_service/transports/base.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/lookup_service/transports/base.py`

 * *Files 6% similar despite different names*

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
@@ -18,14 +18,15 @@
 
 import google.api_core
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
+from google.cloud.location import locations_pb2  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
 from google.cloud.servicedirectory_v1 import gapic_version as package_version
 from google.cloud.servicedirectory_v1.types import lookup_service
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
     gapic_version=package_version.__version__
@@ -147,12 +148,33 @@
             lookup_service.ResolveServiceResponse,
             Awaitable[lookup_service.ResolveServiceResponse],
         ],
     ]:
         raise NotImplementedError()
 
     @property
+    def get_location(
+        self,
+    ) -> Callable[
+        [locations_pb2.GetLocationRequest],
+        Union[locations_pb2.Location, Awaitable[locations_pb2.Location]],
+    ]:
+        raise NotImplementedError()
+
+    @property
+    def list_locations(
+        self,
+    ) -> Callable[
+        [locations_pb2.ListLocationsRequest],
+        Union[
+            locations_pb2.ListLocationsResponse,
+            Awaitable[locations_pb2.ListLocationsResponse],
+        ],
+    ]:
+        raise NotImplementedError()
+
+    @property
     def kind(self) -> str:
         raise NotImplementedError()
 
 
 __all__ = ("LookupServiceTransport",)
```

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/lookup_service/transports/grpc.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/lookup_service/transports/grpc.py`

 * *Files 11% similar despite different names*

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
@@ -16,14 +16,15 @@
 from typing import Callable, Dict, Optional, Sequence, Tuple, Union
 import warnings
 
 from google.api_core import gapic_v1, grpc_helpers
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
+from google.cloud.location import locations_pb2  # type: ignore
 import grpc  # type: ignore
 
 from google.cloud.servicedirectory_v1.types import lookup_service
 
 from .base import DEFAULT_CLIENT_INFO, LookupServiceTransport
 
 
@@ -258,12 +259,48 @@
             )
         return self._stubs["resolve_service"]
 
     def close(self):
         self.grpc_channel.close()
 
     @property
+    def list_locations(
+        self,
+    ) -> Callable[
+        [locations_pb2.ListLocationsRequest], locations_pb2.ListLocationsResponse
+    ]:
+        r"""Return a callable for the list locations method over gRPC."""
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "list_locations" not in self._stubs:
+            self._stubs["list_locations"] = self.grpc_channel.unary_unary(
+                "/google.cloud.location.Locations/ListLocations",
+                request_serializer=locations_pb2.ListLocationsRequest.SerializeToString,
+                response_deserializer=locations_pb2.ListLocationsResponse.FromString,
+            )
+        return self._stubs["list_locations"]
+
+    @property
+    def get_location(
+        self,
+    ) -> Callable[[locations_pb2.GetLocationRequest], locations_pb2.Location]:
+        r"""Return a callable for the list locations method over gRPC."""
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "get_location" not in self._stubs:
+            self._stubs["get_location"] = self.grpc_channel.unary_unary(
+                "/google.cloud.location.Locations/GetLocation",
+                request_serializer=locations_pb2.GetLocationRequest.SerializeToString,
+                response_deserializer=locations_pb2.Location.FromString,
+            )
+        return self._stubs["get_location"]
+
+    @property
     def kind(self) -> str:
         return "grpc"
 
 
 __all__ = ("LookupServiceGrpcTransport",)
```

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/lookup_service/transports/grpc_asyncio.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/grpc.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,104 +1,60 @@
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
-from typing import Awaitable, Callable, Dict, Optional, Sequence, Tuple, Union
+from typing import Callable, Dict, Optional, Sequence, Tuple, Union
 import warnings
 
-from google.api_core import gapic_v1, grpc_helpers_async
+from google.api_core import gapic_v1, grpc_helpers
+import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
+from google.cloud.location import locations_pb2  # type: ignore
 import grpc  # type: ignore
-from grpc.experimental import aio  # type: ignore
 
-from google.cloud.servicedirectory_v1.types import lookup_service
+from google.cloud.servicedirectory_v1beta1.types import lookup_service
 
 from .base import DEFAULT_CLIENT_INFO, LookupServiceTransport
-from .grpc import LookupServiceGrpcTransport
 
 
-class LookupServiceGrpcAsyncIOTransport(LookupServiceTransport):
-    """gRPC AsyncIO backend transport for LookupService.
+class LookupServiceGrpcTransport(LookupServiceTransport):
+    """gRPC backend transport for LookupService.
 
     Service Directory API for looking up service data at runtime.
 
     This class defines the same methods as the primary client, so the
     primary client can load the underlying transport implementation
     and call it.
 
     It sends protocol buffers over the wire using gRPC (which is built on
     top of HTTP/2); the ``grpcio`` package must be installed.
     """
 
-    _grpc_channel: aio.Channel
-    _stubs: Dict[str, Callable] = {}
-
-    @classmethod
-    def create_channel(
-        cls,
-        host: str = "servicedirectory.googleapis.com",
-        credentials: Optional[ga_credentials.Credentials] = None,
-        credentials_file: Optional[str] = None,
-        scopes: Optional[Sequence[str]] = None,
-        quota_project_id: Optional[str] = None,
-        **kwargs,
-    ) -> aio.Channel:
-        """Create and return a gRPC AsyncIO channel object.
-        Args:
-            host (Optional[str]): The host for the channel to use.
-            credentials (Optional[~.Credentials]): The
-                authorization credentials to attach to requests. These
-                credentials identify this application to the service. If
-                none are specified, the client will attempt to ascertain
-                the credentials from the environment.
-            credentials_file (Optional[str]): A file with credentials that can
-                be loaded with :func:`google.auth.load_credentials_from_file`.
-                This argument is ignored if ``channel`` is provided.
-            scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
-                service. These are only used when credentials are not specified and
-                are passed to :func:`google.auth.default`.
-            quota_project_id (Optional[str]): An optional project to use for billing
-                and quota.
-            kwargs (Optional[dict]): Keyword arguments, which are passed to the
-                channel creation.
-        Returns:
-            aio.Channel: A gRPC AsyncIO channel object.
-        """
-
-        return grpc_helpers_async.create_channel(
-            host,
-            credentials=credentials,
-            credentials_file=credentials_file,
-            quota_project_id=quota_project_id,
-            default_scopes=cls.AUTH_SCOPES,
-            scopes=scopes,
-            default_host=cls.DEFAULT_HOST,
-            **kwargs,
-        )
+    _stubs: Dict[str, Callable]
 
     def __init__(
         self,
         *,
         host: str = "servicedirectory.googleapis.com",
         credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
-        channel: Optional[aio.Channel] = None,
+        channel: Optional[grpc.Channel] = None,
         api_mtls_endpoint: Optional[str] = None,
         client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
         client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
@@ -114,18 +70,17 @@
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
                 This argument is ignored if ``channel`` is provided.
             credentials_file (Optional[str]): A file with credentials that can
                 be loaded with :func:`google.auth.load_credentials_from_file`.
                 This argument is ignored if ``channel`` is provided.
-            scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
-                service. These are only used when credentials are not specified and
-                are passed to :func:`google.auth.default`.
-            channel (Optional[aio.Channel]): A ``Channel`` instance through
+            scopes (Optional(Sequence[str])): A list of scopes. This argument is
+                ignored if ``channel`` is provided.
+            channel (Optional[grpc.Channel]): A ``Channel`` instance through
                 which to make calls.
             api_mtls_endpoint (Optional[str]): Deprecated. The mutual TLS endpoint.
                 If provided, it overrides the ``host`` argument and tries to create
                 a mutual TLS channel with client SSL credentials from
                 ``client_cert_source`` or application default SSL credentials.
             client_cert_source (Optional[Callable[[], Tuple[bytes, bytes]]]):
                 Deprecated. A callback to provide client SSL certificate bytes and
@@ -144,15 +99,15 @@
                 API requests. If ``None``, then default info will be used.
                 Generally, you only need to set this if you're developing
                 your own client library.
             always_use_jwt_access (Optional[bool]): Whether self signed JWT should
                 be used for service account credentials.
 
         Raises:
-            google.auth.exceptions.MutualTlsChannelError: If mutual TLS transport
+          google.auth.exceptions.MutualTLSChannelError: If mutual TLS transport
               creation failed for any reason.
           google.api_core.exceptions.DuplicateCredentialArgs: If both ``credentials``
               and ``credentials_file`` are passed.
         """
         self._grpc_channel = None
         self._ssl_channel_credentials = ssl_channel_credentials
         self._stubs: Dict[str, Callable] = {}
@@ -164,14 +119,15 @@
 
         if channel:
             # Ignore credentials if a channel was passed.
             credentials = False
             # If a channel was explicitly provided, set it.
             self._grpc_channel = channel
             self._ssl_channel_credentials = None
+
         else:
             if api_mtls_endpoint:
                 host = api_mtls_endpoint
 
                 # Create SSL credentials with client_cert_source or application
                 # default SSL credentials.
                 if client_cert_source:
@@ -217,53 +173,135 @@
                     ("grpc.max_receive_message_length", -1),
                 ],
             )
 
         # Wrap messages. This must be done after self._grpc_channel exists
         self._prep_wrapped_messages(client_info)
 
-    @property
-    def grpc_channel(self) -> aio.Channel:
-        """Create the channel designed to connect to this service.
+    @classmethod
+    def create_channel(
+        cls,
+        host: str = "servicedirectory.googleapis.com",
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
+        scopes: Optional[Sequence[str]] = None,
+        quota_project_id: Optional[str] = None,
+        **kwargs,
+    ) -> grpc.Channel:
+        """Create and return a gRPC channel object.
+        Args:
+            host (Optional[str]): The host for the channel to use.
+            credentials (Optional[~.Credentials]): The
+                authorization credentials to attach to requests. These
+                credentials identify this application to the service. If
+                none are specified, the client will attempt to ascertain
+                the credentials from the environment.
+            credentials_file (Optional[str]): A file with credentials that can
+                be loaded with :func:`google.auth.load_credentials_from_file`.
+                This argument is mutually exclusive with credentials.
+            scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
+                service. These are only used when credentials are not specified and
+                are passed to :func:`google.auth.default`.
+            quota_project_id (Optional[str]): An optional project to use for billing
+                and quota.
+            kwargs (Optional[dict]): Keyword arguments, which are passed to the
+                channel creation.
+        Returns:
+            grpc.Channel: A gRPC channel object.
 
-        This property caches on the instance; repeated calls return
-        the same channel.
+        Raises:
+            google.api_core.exceptions.DuplicateCredentialArgs: If both ``credentials``
+              and ``credentials_file`` are passed.
         """
-        # Return the channel from cache.
+
+        return grpc_helpers.create_channel(
+            host,
+            credentials=credentials,
+            credentials_file=credentials_file,
+            quota_project_id=quota_project_id,
+            default_scopes=cls.AUTH_SCOPES,
+            scopes=scopes,
+            default_host=cls.DEFAULT_HOST,
+            **kwargs,
+        )
+
+    @property
+    def grpc_channel(self) -> grpc.Channel:
+        """Return the channel designed to connect to this service."""
         return self._grpc_channel
 
     @property
     def resolve_service(
         self,
     ) -> Callable[
-        [lookup_service.ResolveServiceRequest],
-        Awaitable[lookup_service.ResolveServiceResponse],
+        [lookup_service.ResolveServiceRequest], lookup_service.ResolveServiceResponse
     ]:
         r"""Return a callable for the resolve service method over gRPC.
 
-        Returns a [service][google.cloud.servicedirectory.v1.Service]
-        and its associated endpoints. Resolving a service is not
-        considered an active developer method.
+        Returns a
+        [service][google.cloud.servicedirectory.v1beta1.Service] and its
+        associated endpoints. Resolving a service is not considered an
+        active developer method.
 
         Returns:
             Callable[[~.ResolveServiceRequest],
-                    Awaitable[~.ResolveServiceResponse]]:
+                    ~.ResolveServiceResponse]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "resolve_service" not in self._stubs:
             self._stubs["resolve_service"] = self.grpc_channel.unary_unary(
-                "/google.cloud.servicedirectory.v1.LookupService/ResolveService",
+                "/google.cloud.servicedirectory.v1beta1.LookupService/ResolveService",
                 request_serializer=lookup_service.ResolveServiceRequest.serialize,
                 response_deserializer=lookup_service.ResolveServiceResponse.deserialize,
             )
         return self._stubs["resolve_service"]
 
     def close(self):
-        return self.grpc_channel.close()
+        self.grpc_channel.close()
+
+    @property
+    def list_locations(
+        self,
+    ) -> Callable[
+        [locations_pb2.ListLocationsRequest], locations_pb2.ListLocationsResponse
+    ]:
+        r"""Return a callable for the list locations method over gRPC."""
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "list_locations" not in self._stubs:
+            self._stubs["list_locations"] = self.grpc_channel.unary_unary(
+                "/google.cloud.location.Locations/ListLocations",
+                request_serializer=locations_pb2.ListLocationsRequest.SerializeToString,
+                response_deserializer=locations_pb2.ListLocationsResponse.FromString,
+            )
+        return self._stubs["list_locations"]
+
+    @property
+    def get_location(
+        self,
+    ) -> Callable[[locations_pb2.GetLocationRequest], locations_pb2.Location]:
+        r"""Return a callable for the list locations method over gRPC."""
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "get_location" not in self._stubs:
+            self._stubs["get_location"] = self.grpc_channel.unary_unary(
+                "/google.cloud.location.Locations/GetLocation",
+                request_serializer=locations_pb2.GetLocationRequest.SerializeToString,
+                response_deserializer=locations_pb2.Location.FromString,
+            )
+        return self._stubs["get_location"]
+
+    @property
+    def kind(self) -> str:
+        return "grpc"
 
 
-__all__ = ("LookupServiceGrpcAsyncIOTransport",)
+__all__ = ("LookupServiceGrpcTransport",)
```

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/lookup_service/transports/rest.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/lookup_service/transports/rest.py`

 * *Files 22% similar despite different names*

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
@@ -22,14 +22,15 @@
 
 from google.api_core import gapic_v1, path_template, rest_helpers, rest_streaming
 from google.api_core import exceptions as core_exceptions
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.auth.transport.requests import AuthorizedSession  # type: ignore
+from google.cloud.location import locations_pb2  # type: ignore
 from google.protobuf import json_format
 import grpc  # type: ignore
 from requests import __version__ as requests_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
@@ -96,14 +97,60 @@
 
         Override in a subclass to manipulate the response
         after it is returned by the LookupService server but before
         it is returned to user code.
         """
         return response
 
+    def pre_get_location(
+        self,
+        request: locations_pb2.GetLocationRequest,
+        metadata: Sequence[Tuple[str, str]],
+    ) -> Tuple[locations_pb2.GetLocationRequest, Sequence[Tuple[str, str]]]:
+        """Pre-rpc interceptor for get_location
+
+        Override in a subclass to manipulate the request or metadata
+        before they are sent to the LookupService server.
+        """
+        return request, metadata
+
+    def post_get_location(
+        self, response: locations_pb2.Location
+    ) -> locations_pb2.Location:
+        """Post-rpc interceptor for get_location
+
+        Override in a subclass to manipulate the response
+        after it is returned by the LookupService server but before
+        it is returned to user code.
+        """
+        return response
+
+    def pre_list_locations(
+        self,
+        request: locations_pb2.ListLocationsRequest,
+        metadata: Sequence[Tuple[str, str]],
+    ) -> Tuple[locations_pb2.ListLocationsRequest, Sequence[Tuple[str, str]]]:
+        """Pre-rpc interceptor for list_locations
+
+        Override in a subclass to manipulate the request or metadata
+        before they are sent to the LookupService server.
+        """
+        return request, metadata
+
+    def post_list_locations(
+        self, response: locations_pb2.ListLocationsResponse
+    ) -> locations_pb2.ListLocationsResponse:
+        """Post-rpc interceptor for list_locations
+
+        Override in a subclass to manipulate the response
+        after it is returned by the LookupService server but before
+        it is returned to user code.
+        """
+        return response
+
 
 @dataclasses.dataclass
 class LookupServiceRestStub:
     _session: AuthorizedSession
     _host: str
     _interceptor: LookupServiceRestInterceptor
 
@@ -304,14 +351,148 @@
         [lookup_service.ResolveServiceRequest], lookup_service.ResolveServiceResponse
     ]:
         # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
         # In C++ this would require a dynamic_cast
         return self._ResolveService(self._session, self._host, self._interceptor)  # type: ignore
 
     @property
+    def get_location(self):
+        return self._GetLocation(self._session, self._host, self._interceptor)  # type: ignore
+
+    class _GetLocation(LookupServiceRestStub):
+        def __call__(
+            self,
+            request: locations_pb2.GetLocationRequest,
+            *,
+            retry: OptionalRetry = gapic_v1.method.DEFAULT,
+            timeout: Optional[float] = None,
+            metadata: Sequence[Tuple[str, str]] = (),
+        ) -> locations_pb2.Location:
+
+            r"""Call the get location method over HTTP.
+
+            Args:
+                request (locations_pb2.GetLocationRequest):
+                    The request object for GetLocation method.
+                retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                    should be retried.
+                timeout (float): The timeout for this request.
+                metadata (Sequence[Tuple[str, str]]): Strings which should be
+                    sent along with the request as metadata.
+
+            Returns:
+                locations_pb2.Location: Response from GetLocation method.
+            """
+
+            http_options: List[Dict[str, str]] = [
+                {
+                    "method": "get",
+                    "uri": "/v1/{name=projects/*/locations/*}",
+                },
+            ]
+
+            request, metadata = self._interceptor.pre_get_location(request, metadata)
+            request_kwargs = json_format.MessageToDict(request)
+            transcoded_request = path_template.transcode(http_options, **request_kwargs)
+
+            uri = transcoded_request["uri"]
+            method = transcoded_request["method"]
+
+            # Jsonify the query params
+            query_params = json.loads(json.dumps(transcoded_request["query_params"]))
+
+            # Send the request
+            headers = dict(metadata)
+            headers["Content-Type"] = "application/json"
+
+            response = getattr(self._session, method)(
+                "{host}{uri}".format(host=self._host, uri=uri),
+                timeout=timeout,
+                headers=headers,
+                params=rest_helpers.flatten_query_params(query_params),
+            )
+
+            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
+            # subclass.
+            if response.status_code >= 400:
+                raise core_exceptions.from_http_response(response)
+
+            resp = locations_pb2.Location()
+            resp = json_format.Parse(response.content.decode("utf-8"), resp)
+            resp = self._interceptor.post_get_location(resp)
+            return resp
+
+    @property
+    def list_locations(self):
+        return self._ListLocations(self._session, self._host, self._interceptor)  # type: ignore
+
+    class _ListLocations(LookupServiceRestStub):
+        def __call__(
+            self,
+            request: locations_pb2.ListLocationsRequest,
+            *,
+            retry: OptionalRetry = gapic_v1.method.DEFAULT,
+            timeout: Optional[float] = None,
+            metadata: Sequence[Tuple[str, str]] = (),
+        ) -> locations_pb2.ListLocationsResponse:
+
+            r"""Call the list locations method over HTTP.
+
+            Args:
+                request (locations_pb2.ListLocationsRequest):
+                    The request object for ListLocations method.
+                retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                    should be retried.
+                timeout (float): The timeout for this request.
+                metadata (Sequence[Tuple[str, str]]): Strings which should be
+                    sent along with the request as metadata.
+
+            Returns:
+                locations_pb2.ListLocationsResponse: Response from ListLocations method.
+            """
+
+            http_options: List[Dict[str, str]] = [
+                {
+                    "method": "get",
+                    "uri": "/v1/{name=projects/*}/locations",
+                },
+            ]
+
+            request, metadata = self._interceptor.pre_list_locations(request, metadata)
+            request_kwargs = json_format.MessageToDict(request)
+            transcoded_request = path_template.transcode(http_options, **request_kwargs)
+
+            uri = transcoded_request["uri"]
+            method = transcoded_request["method"]
+
+            # Jsonify the query params
+            query_params = json.loads(json.dumps(transcoded_request["query_params"]))
+
+            # Send the request
+            headers = dict(metadata)
+            headers["Content-Type"] = "application/json"
+
+            response = getattr(self._session, method)(
+                "{host}{uri}".format(host=self._host, uri=uri),
+                timeout=timeout,
+                headers=headers,
+                params=rest_helpers.flatten_query_params(query_params),
+            )
+
+            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
+            # subclass.
+            if response.status_code >= 400:
+                raise core_exceptions.from_http_response(response)
+
+            resp = locations_pb2.ListLocationsResponse()
+            resp = json_format.Parse(response.content.decode("utf-8"), resp)
+            resp = self._interceptor.post_list_locations(resp)
+            return resp
+
+    @property
     def kind(self) -> str:
         return "rest"
 
     def close(self):
         self._session.close()
```

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/registration_service/__init__.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/registration_service/__init__.py`

 * *Files 11% similar despite different names*

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

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/registration_service/async_client.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/registration_service/async_client.py`

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
@@ -38,14 +38,15 @@
 from google.cloud.servicedirectory_v1 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
+from google.cloud.location import locations_pb2  # type: ignore
 from google.iam.v1 import iam_policy_pb2  # type: ignore
 from google.iam.v1 import policy_pb2  # type: ignore
 from google.protobuf import field_mask_pb2  # type: ignore
 
 from google.cloud.servicedirectory_v1.services.registration_service import pagers
 from google.cloud.servicedirectory_v1.types import endpoint
 from google.cloud.servicedirectory_v1.types import endpoint as gcs_endpoint
@@ -83,14 +84,16 @@
     DEFAULT_ENDPOINT = RegistrationServiceClient.DEFAULT_ENDPOINT
     DEFAULT_MTLS_ENDPOINT = RegistrationServiceClient.DEFAULT_MTLS_ENDPOINT
 
     endpoint_path = staticmethod(RegistrationServiceClient.endpoint_path)
     parse_endpoint_path = staticmethod(RegistrationServiceClient.parse_endpoint_path)
     namespace_path = staticmethod(RegistrationServiceClient.namespace_path)
     parse_namespace_path = staticmethod(RegistrationServiceClient.parse_namespace_path)
+    network_path = staticmethod(RegistrationServiceClient.network_path)
+    parse_network_path = staticmethod(RegistrationServiceClient.parse_network_path)
     service_path = staticmethod(RegistrationServiceClient.service_path)
     parse_service_path = staticmethod(RegistrationServiceClient.parse_service_path)
     common_billing_account_path = staticmethod(
         RegistrationServiceClient.common_billing_account_path
     )
     parse_common_billing_account_path = staticmethod(
         RegistrationServiceClient.parse_common_billing_account_path
@@ -253,15 +256,15 @@
         parent: Optional[str] = None,
         namespace: Optional[gcs_namespace.Namespace] = None,
         namespace_id: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_namespace.Namespace:
-        r"""Creates a namespace, and returns the new Namespace.
+        r"""Creates a namespace, and returns the new namespace.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -421,15 +424,15 @@
         Args:
             request (Optional[Union[google.cloud.servicedirectory_v1.types.ListNamespacesRequest, dict]]):
                 The request object. The request message for
                 [RegistrationService.ListNamespaces][google.cloud.servicedirectory.v1.RegistrationService.ListNamespaces].
             parent (:class:`str`):
                 Required. The resource name of the
                 project and location whose namespaces
-                we'd like to list.
+                you'd like to list.
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -817,15 +820,15 @@
         parent: Optional[str] = None,
         service: Optional[gcs_service.Service] = None,
         service_id: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_service.Service:
-        r"""Creates a service, and returns the new Service.
+        r"""Creates a service, and returns the new service.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -981,15 +984,15 @@
 
         Args:
             request (Optional[Union[google.cloud.servicedirectory_v1.types.ListServicesRequest, dict]]):
                 The request object. The request message for
                 [RegistrationService.ListServices][google.cloud.servicedirectory.v1.RegistrationService.ListServices].
             parent (:class:`str`):
                 Required. The resource name of the
-                namespace whose services we'd like to
+                namespace whose services you'd like to
                 list.
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
@@ -1095,16 +1098,16 @@
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.servicedirectory_v1.types.GetServiceRequest, dict]]):
                 The request object. The request message for
                 [RegistrationService.GetService][google.cloud.servicedirectory.v1.RegistrationService.GetService].
                 This should not be used for looking up a service.
-                Insead, use the ``resolve`` method as it will contain
-                all endpoints and associated metadata.
+                Instead, use the ``resolve`` method as it contains all
+                endpoints and associated annotations.
             name (:class:`str`):
                 Required. The name of the service to
                 get.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
@@ -1381,15 +1384,15 @@
         parent: Optional[str] = None,
         endpoint: Optional[gcs_endpoint.Endpoint] = None,
         endpoint_id: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_endpoint.Endpoint:
-        r"""Creates a endpoint, and returns the new Endpoint.
+        r"""Creates an endpoint, and returns the new endpoint.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -1546,15 +1549,15 @@
 
         Args:
             request (Optional[Union[google.cloud.servicedirectory_v1.types.ListEndpointsRequest, dict]]):
                 The request object. The request message for
                 [RegistrationService.ListEndpoints][google.cloud.servicedirectory.v1.RegistrationService.ListEndpoints].
             parent (:class:`str`):
                 Required. The resource name of the
-                service whose endpoints we'd like to
+                service whose endpoints you'd like to
                 list.
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
@@ -1627,15 +1630,15 @@
         request: Optional[Union[registration_service.GetEndpointRequest, dict]] = None,
         *,
         name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> endpoint.Endpoint:
-        r"""Gets a endpoint.
+        r"""Gets an endpoint.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -1735,15 +1738,15 @@
         *,
         endpoint: Optional[gcs_endpoint.Endpoint] = None,
         update_mask: Optional[field_mask_pb2.FieldMask] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_endpoint.Endpoint:
-        r"""Updates a endpoint.
+        r"""Updates an endpoint.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -1848,15 +1851,15 @@
         ] = None,
         *,
         name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> None:
-        r"""Deletes a endpoint.
+        r"""Deletes an endpoint.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -2292,14 +2295,122 @@
         )
 
         # Send the request.
         response = await rpc(
             request,
             retry=retry,
             timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    async def get_location(
+        self,
+        request: Optional[locations_pb2.GetLocationRequest] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> locations_pb2.Location:
+        r"""Gets information about a location.
+
+        Args:
+            request (:class:`~.location_pb2.GetLocationRequest`):
+                The request object. Request message for
+                `GetLocation` method.
+            retry (google.api_core.retry.Retry): Designation of what errors,
+                 if any, should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            ~.location_pb2.Location:
+                Location object.
+        """
+        # Create or coerce a protobuf request object.
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = locations_pb2.GetLocationRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._client._transport.get_location,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    async def list_locations(
+        self,
+        request: Optional[locations_pb2.ListLocationsRequest] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> locations_pb2.ListLocationsResponse:
+        r"""Lists information about the supported locations for this service.
+
+        Args:
+            request (:class:`~.location_pb2.ListLocationsRequest`):
+                The request object. Request message for
+                `ListLocations` method.
+            retry (google.api_core.retry.Retry): Designation of what errors,
+                 if any, should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            ~.location_pb2.ListLocationsResponse:
+                Response message for ``ListLocations`` method.
+        """
+        # Create or coerce a protobuf request object.
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = locations_pb2.ListLocationsRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._client._transport.list_locations,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
     async def __aenter__(self) -> "RegistrationServiceAsyncClient":
```

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/registration_service/client.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/registration_service/client.py`

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
@@ -42,14 +42,15 @@
 from google.cloud.servicedirectory_v1 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
+from google.cloud.location import locations_pb2  # type: ignore
 from google.iam.v1 import iam_policy_pb2  # type: ignore
 from google.iam.v1 import policy_pb2  # type: ignore
 from google.protobuf import field_mask_pb2  # type: ignore
 
 from google.cloud.servicedirectory_v1.services.registration_service import pagers
 from google.cloud.servicedirectory_v1.types import endpoint
 from google.cloud.servicedirectory_v1.types import endpoint as gcs_endpoint
@@ -247,14 +248,34 @@
         m = re.match(
             r"^projects/(?P<project>.+?)/locations/(?P<location>.+?)/namespaces/(?P<namespace>.+?)$",
             path,
         )
         return m.groupdict() if m else {}
 
     @staticmethod
+    def network_path(
+        project: str,
+        network: str,
+    ) -> str:
+        """Returns a fully-qualified network string."""
+        return "projects/{project}/locations/global/networks/{network}".format(
+            project=project,
+            network=network,
+        )
+
+    @staticmethod
+    def parse_network_path(path: str) -> Dict[str, str]:
+        """Parses a network path into its component segments."""
+        m = re.match(
+            r"^projects/(?P<project>.+?)/locations/global/networks/(?P<network>.+?)$",
+            path,
+        )
+        return m.groupdict() if m else {}
+
+    @staticmethod
     def service_path(
         project: str,
         location: str,
         namespace: str,
         service: str,
     ) -> str:
         """Returns a fully-qualified service string."""
@@ -527,15 +548,15 @@
         parent: Optional[str] = None,
         namespace: Optional[gcs_namespace.Namespace] = None,
         namespace_id: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_namespace.Namespace:
-        r"""Creates a namespace, and returns the new Namespace.
+        r"""Creates a namespace, and returns the new namespace.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -695,15 +716,15 @@
         Args:
             request (Union[google.cloud.servicedirectory_v1.types.ListNamespacesRequest, dict]):
                 The request object. The request message for
                 [RegistrationService.ListNamespaces][google.cloud.servicedirectory.v1.RegistrationService.ListNamespaces].
             parent (str):
                 Required. The resource name of the
                 project and location whose namespaces
-                we'd like to list.
+                you'd like to list.
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -1091,15 +1112,15 @@
         parent: Optional[str] = None,
         service: Optional[gcs_service.Service] = None,
         service_id: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_service.Service:
-        r"""Creates a service, and returns the new Service.
+        r"""Creates a service, and returns the new service.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -1255,15 +1276,15 @@
 
         Args:
             request (Union[google.cloud.servicedirectory_v1.types.ListServicesRequest, dict]):
                 The request object. The request message for
                 [RegistrationService.ListServices][google.cloud.servicedirectory.v1.RegistrationService.ListServices].
             parent (str):
                 Required. The resource name of the
-                namespace whose services we'd like to
+                namespace whose services you'd like to
                 list.
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
@@ -1369,16 +1390,16 @@
                 print(response)
 
         Args:
             request (Union[google.cloud.servicedirectory_v1.types.GetServiceRequest, dict]):
                 The request object. The request message for
                 [RegistrationService.GetService][google.cloud.servicedirectory.v1.RegistrationService.GetService].
                 This should not be used for looking up a service.
-                Insead, use the ``resolve`` method as it will contain
-                all endpoints and associated metadata.
+                Instead, use the ``resolve`` method as it contains all
+                endpoints and associated annotations.
             name (str):
                 Required. The name of the service to
                 get.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
@@ -1655,15 +1676,15 @@
         parent: Optional[str] = None,
         endpoint: Optional[gcs_endpoint.Endpoint] = None,
         endpoint_id: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_endpoint.Endpoint:
-        r"""Creates a endpoint, and returns the new Endpoint.
+        r"""Creates an endpoint, and returns the new endpoint.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -1820,15 +1841,15 @@
 
         Args:
             request (Union[google.cloud.servicedirectory_v1.types.ListEndpointsRequest, dict]):
                 The request object. The request message for
                 [RegistrationService.ListEndpoints][google.cloud.servicedirectory.v1.RegistrationService.ListEndpoints].
             parent (str):
                 Required. The resource name of the
-                service whose endpoints we'd like to
+                service whose endpoints you'd like to
                 list.
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
@@ -1901,15 +1922,15 @@
         request: Optional[Union[registration_service.GetEndpointRequest, dict]] = None,
         *,
         name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> endpoint.Endpoint:
-        r"""Gets a endpoint.
+        r"""Gets an endpoint.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -2009,15 +2030,15 @@
         *,
         endpoint: Optional[gcs_endpoint.Endpoint] = None,
         update_mask: Optional[field_mask_pb2.FieldMask] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_endpoint.Endpoint:
-        r"""Updates a endpoint.
+        r"""Updates an endpoint.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -2122,15 +2143,15 @@
         ] = None,
         *,
         name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> None:
-        r"""Deletes a endpoint.
+        r"""Deletes an endpoint.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -2582,14 +2603,122 @@
         .. warning::
             ONLY use as a context manager if the transport is NOT shared
             with other clients! Exiting the with block will CLOSE the transport
             and may cause errors in other clients!
         """
         self.transport.close()
 
+    def get_location(
+        self,
+        request: Optional[locations_pb2.GetLocationRequest] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> locations_pb2.Location:
+        r"""Gets information about a location.
+
+        Args:
+            request (:class:`~.location_pb2.GetLocationRequest`):
+                The request object. Request message for
+                `GetLocation` method.
+            retry (google.api_core.retry.Retry): Designation of what errors,
+                 if any, should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            ~.location_pb2.Location:
+                Location object.
+        """
+        # Create or coerce a protobuf request object.
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = locations_pb2.GetLocationRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._transport.get_location,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    def list_locations(
+        self,
+        request: Optional[locations_pb2.ListLocationsRequest] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> locations_pb2.ListLocationsResponse:
+        r"""Lists information about the supported locations for this service.
+
+        Args:
+            request (:class:`~.location_pb2.ListLocationsRequest`):
+                The request object. Request message for
+                `ListLocations` method.
+            retry (google.api_core.retry.Retry): Designation of what errors,
+                 if any, should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            ~.location_pb2.ListLocationsResponse:
+                Response message for ``ListLocations`` method.
+        """
+        # Create or coerce a protobuf request object.
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = locations_pb2.ListLocationsRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._transport.list_locations,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
     gapic_version=package_version.__version__
 )
 
 
 __all__ = ("RegistrationServiceClient",)
```

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/registration_service/pagers.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/registration_service/pagers.py`

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

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/registration_service/transports/__init__.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/registration_service/transports/__init__.py`

 * *Files 4% similar despite different names*

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

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/registration_service/transports/base.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/registration_service/transports/base.py`

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
@@ -18,14 +18,15 @@
 
 import google.api_core
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
+from google.cloud.location import locations_pb2  # type: ignore
 from google.iam.v1 import iam_policy_pb2  # type: ignore
 from google.iam.v1 import policy_pb2  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 from google.protobuf import empty_pb2  # type: ignore
 
 from google.cloud.servicedirectory_v1 import gapic_version as package_version
 from google.cloud.servicedirectory_v1.types import endpoint
@@ -403,12 +404,33 @@
             iam_policy_pb2.TestIamPermissionsResponse,
             Awaitable[iam_policy_pb2.TestIamPermissionsResponse],
         ],
     ]:
         raise NotImplementedError()
 
     @property
+    def get_location(
+        self,
+    ) -> Callable[
+        [locations_pb2.GetLocationRequest],
+        Union[locations_pb2.Location, Awaitable[locations_pb2.Location]],
+    ]:
+        raise NotImplementedError()
+
+    @property
+    def list_locations(
+        self,
+    ) -> Callable[
+        [locations_pb2.ListLocationsRequest],
+        Union[
+            locations_pb2.ListLocationsResponse,
+            Awaitable[locations_pb2.ListLocationsResponse],
+        ],
+    ]:
+        raise NotImplementedError()
+
+    @property
     def kind(self) -> str:
         raise NotImplementedError()
 
 
 __all__ = ("RegistrationServiceTransport",)
```

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/registration_service/transports/grpc.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/registration_service/transports/grpc.py`

 * *Files 12% similar despite different names*

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
@@ -16,14 +16,15 @@
 from typing import Callable, Dict, Optional, Sequence, Tuple, Union
 import warnings
 
 from google.api_core import gapic_v1, grpc_helpers
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
+from google.cloud.location import locations_pb2  # type: ignore
 from google.iam.v1 import iam_policy_pb2  # type: ignore
 from google.iam.v1 import policy_pb2  # type: ignore
 from google.protobuf import empty_pb2  # type: ignore
 import grpc  # type: ignore
 
 from google.cloud.servicedirectory_v1.types import endpoint
 from google.cloud.servicedirectory_v1.types import endpoint as gcs_endpoint
@@ -255,15 +256,15 @@
     def create_namespace(
         self,
     ) -> Callable[
         [registration_service.CreateNamespaceRequest], gcs_namespace.Namespace
     ]:
         r"""Return a callable for the create namespace method over gRPC.
 
-        Creates a namespace, and returns the new Namespace.
+        Creates a namespace, and returns the new namespace.
 
         Returns:
             Callable[[~.CreateNamespaceRequest],
                     ~.Namespace]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
@@ -391,15 +392,15 @@
 
     @property
     def create_service(
         self,
     ) -> Callable[[registration_service.CreateServiceRequest], gcs_service.Service]:
         r"""Return a callable for the create service method over gRPC.
 
-        Creates a service, and returns the new Service.
+        Creates a service, and returns the new service.
 
         Returns:
             Callable[[~.CreateServiceRequest],
                     ~.Service]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
@@ -525,15 +526,15 @@
 
     @property
     def create_endpoint(
         self,
     ) -> Callable[[registration_service.CreateEndpointRequest], gcs_endpoint.Endpoint]:
         r"""Return a callable for the create endpoint method over gRPC.
 
-        Creates a endpoint, and returns the new Endpoint.
+        Creates an endpoint, and returns the new endpoint.
 
         Returns:
             Callable[[~.CreateEndpointRequest],
                     ~.Endpoint]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
@@ -580,15 +581,15 @@
 
     @property
     def get_endpoint(
         self,
     ) -> Callable[[registration_service.GetEndpointRequest], endpoint.Endpoint]:
         r"""Return a callable for the get endpoint method over gRPC.
 
-        Gets a endpoint.
+        Gets an endpoint.
 
         Returns:
             Callable[[~.GetEndpointRequest],
                     ~.Endpoint]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
@@ -606,15 +607,15 @@
 
     @property
     def update_endpoint(
         self,
     ) -> Callable[[registration_service.UpdateEndpointRequest], gcs_endpoint.Endpoint]:
         r"""Return a callable for the update endpoint method over gRPC.
 
-        Updates a endpoint.
+        Updates an endpoint.
 
         Returns:
             Callable[[~.UpdateEndpointRequest],
                     ~.Endpoint]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
@@ -632,15 +633,15 @@
 
     @property
     def delete_endpoint(
         self,
     ) -> Callable[[registration_service.DeleteEndpointRequest], empty_pb2.Empty]:
         r"""Return a callable for the delete endpoint method over gRPC.
 
-        Deletes a endpoint.
+        Deletes an endpoint.
 
         Returns:
             Callable[[~.DeleteEndpointRequest],
                     ~.Empty]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
@@ -740,12 +741,48 @@
             )
         return self._stubs["test_iam_permissions"]
 
     def close(self):
         self.grpc_channel.close()
 
     @property
+    def list_locations(
+        self,
+    ) -> Callable[
+        [locations_pb2.ListLocationsRequest], locations_pb2.ListLocationsResponse
+    ]:
+        r"""Return a callable for the list locations method over gRPC."""
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "list_locations" not in self._stubs:
+            self._stubs["list_locations"] = self.grpc_channel.unary_unary(
+                "/google.cloud.location.Locations/ListLocations",
+                request_serializer=locations_pb2.ListLocationsRequest.SerializeToString,
+                response_deserializer=locations_pb2.ListLocationsResponse.FromString,
+            )
+        return self._stubs["list_locations"]
+
+    @property
+    def get_location(
+        self,
+    ) -> Callable[[locations_pb2.GetLocationRequest], locations_pb2.Location]:
+        r"""Return a callable for the list locations method over gRPC."""
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "get_location" not in self._stubs:
+            self._stubs["get_location"] = self.grpc_channel.unary_unary(
+                "/google.cloud.location.Locations/GetLocation",
+                request_serializer=locations_pb2.GetLocationRequest.SerializeToString,
+                response_deserializer=locations_pb2.Location.FromString,
+            )
+        return self._stubs["get_location"]
+
+    @property
     def kind(self) -> str:
         return "grpc"
 
 
 __all__ = ("RegistrationServiceGrpcTransport",)
```

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/registration_service/transports/grpc_asyncio.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/registration_service/transports/grpc_asyncio.py`

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
@@ -15,14 +15,15 @@
 #
 from typing import Awaitable, Callable, Dict, Optional, Sequence, Tuple, Union
 import warnings
 
 from google.api_core import gapic_v1, grpc_helpers_async
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
+from google.cloud.location import locations_pb2  # type: ignore
 from google.iam.v1 import iam_policy_pb2  # type: ignore
 from google.iam.v1 import policy_pb2  # type: ignore
 from google.protobuf import empty_pb2  # type: ignore
 import grpc  # type: ignore
 from grpc.experimental import aio  # type: ignore
 
 from google.cloud.servicedirectory_v1.types import endpoint
@@ -259,15 +260,15 @@
         self,
     ) -> Callable[
         [registration_service.CreateNamespaceRequest],
         Awaitable[gcs_namespace.Namespace],
     ]:
         r"""Return a callable for the create namespace method over gRPC.
 
-        Creates a namespace, and returns the new Namespace.
+        Creates a namespace, and returns the new namespace.
 
         Returns:
             Callable[[~.CreateNamespaceRequest],
                     Awaitable[~.Namespace]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
@@ -402,15 +403,15 @@
     def create_service(
         self,
     ) -> Callable[
         [registration_service.CreateServiceRequest], Awaitable[gcs_service.Service]
     ]:
         r"""Return a callable for the create service method over gRPC.
 
-        Creates a service, and returns the new Service.
+        Creates a service, and returns the new service.
 
         Returns:
             Callable[[~.CreateServiceRequest],
                     Awaitable[~.Service]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
@@ -542,15 +543,15 @@
     def create_endpoint(
         self,
     ) -> Callable[
         [registration_service.CreateEndpointRequest], Awaitable[gcs_endpoint.Endpoint]
     ]:
         r"""Return a callable for the create endpoint method over gRPC.
 
-        Creates a endpoint, and returns the new Endpoint.
+        Creates an endpoint, and returns the new endpoint.
 
         Returns:
             Callable[[~.CreateEndpointRequest],
                     Awaitable[~.Endpoint]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
@@ -599,15 +600,15 @@
     def get_endpoint(
         self,
     ) -> Callable[
         [registration_service.GetEndpointRequest], Awaitable[endpoint.Endpoint]
     ]:
         r"""Return a callable for the get endpoint method over gRPC.
 
-        Gets a endpoint.
+        Gets an endpoint.
 
         Returns:
             Callable[[~.GetEndpointRequest],
                     Awaitable[~.Endpoint]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
@@ -627,15 +628,15 @@
     def update_endpoint(
         self,
     ) -> Callable[
         [registration_service.UpdateEndpointRequest], Awaitable[gcs_endpoint.Endpoint]
     ]:
         r"""Return a callable for the update endpoint method over gRPC.
 
-        Updates a endpoint.
+        Updates an endpoint.
 
         Returns:
             Callable[[~.UpdateEndpointRequest],
                     Awaitable[~.Endpoint]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
@@ -655,15 +656,15 @@
     def delete_endpoint(
         self,
     ) -> Callable[
         [registration_service.DeleteEndpointRequest], Awaitable[empty_pb2.Empty]
     ]:
         r"""Return a callable for the delete endpoint method over gRPC.
 
-        Deletes a endpoint.
+        Deletes an endpoint.
 
         Returns:
             Callable[[~.DeleteEndpointRequest],
                     Awaitable[~.Empty]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
@@ -762,9 +763,45 @@
                 response_deserializer=iam_policy_pb2.TestIamPermissionsResponse.FromString,
             )
         return self._stubs["test_iam_permissions"]
 
     def close(self):
         return self.grpc_channel.close()
 
+    @property
+    def list_locations(
+        self,
+    ) -> Callable[
+        [locations_pb2.ListLocationsRequest], locations_pb2.ListLocationsResponse
+    ]:
+        r"""Return a callable for the list locations method over gRPC."""
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "list_locations" not in self._stubs:
+            self._stubs["list_locations"] = self.grpc_channel.unary_unary(
+                "/google.cloud.location.Locations/ListLocations",
+                request_serializer=locations_pb2.ListLocationsRequest.SerializeToString,
+                response_deserializer=locations_pb2.ListLocationsResponse.FromString,
+            )
+        return self._stubs["list_locations"]
+
+    @property
+    def get_location(
+        self,
+    ) -> Callable[[locations_pb2.GetLocationRequest], locations_pb2.Location]:
+        r"""Return a callable for the list locations method over gRPC."""
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "get_location" not in self._stubs:
+            self._stubs["get_location"] = self.grpc_channel.unary_unary(
+                "/google.cloud.location.Locations/GetLocation",
+                request_serializer=locations_pb2.GetLocationRequest.SerializeToString,
+                response_deserializer=locations_pb2.Location.FromString,
+            )
+        return self._stubs["get_location"]
+
 
 __all__ = ("RegistrationServiceGrpcAsyncIOTransport",)
```

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/registration_service/transports/rest.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/rest.py`

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
@@ -22,35 +22,36 @@
 
 from google.api_core import gapic_v1, path_template, rest_helpers, rest_streaming
 from google.api_core import exceptions as core_exceptions
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.auth.transport.requests import AuthorizedSession  # type: ignore
+from google.cloud.location import locations_pb2  # type: ignore
 from google.protobuf import json_format
 import grpc  # type: ignore
 from requests import __version__ as requests_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 
 from google.iam.v1 import iam_policy_pb2  # type: ignore
 from google.iam.v1 import policy_pb2  # type: ignore
 from google.protobuf import empty_pb2  # type: ignore
 
-from google.cloud.servicedirectory_v1.types import endpoint
-from google.cloud.servicedirectory_v1.types import endpoint as gcs_endpoint
-from google.cloud.servicedirectory_v1.types import namespace
-from google.cloud.servicedirectory_v1.types import namespace as gcs_namespace
-from google.cloud.servicedirectory_v1.types import registration_service
-from google.cloud.servicedirectory_v1.types import service
-from google.cloud.servicedirectory_v1.types import service as gcs_service
+from google.cloud.servicedirectory_v1beta1.types import endpoint as gcs_endpoint
+from google.cloud.servicedirectory_v1beta1.types import namespace as gcs_namespace
+from google.cloud.servicedirectory_v1beta1.types import endpoint
+from google.cloud.servicedirectory_v1beta1.types import namespace
+from google.cloud.servicedirectory_v1beta1.types import registration_service
+from google.cloud.servicedirectory_v1beta1.types import service
+from google.cloud.servicedirectory_v1beta1.types import service as gcs_service
 
 from .base import DEFAULT_CLIENT_INFO as BASE_DEFAULT_CLIENT_INFO
 from .base import RegistrationServiceTransport
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
     gapic_version=BASE_DEFAULT_CLIENT_INFO.gapic_version,
     grpc_version=None,
@@ -574,14 +575,60 @@
 
         Override in a subclass to manipulate the response
         after it is returned by the RegistrationService server but before
         it is returned to user code.
         """
         return response
 
+    def pre_get_location(
+        self,
+        request: locations_pb2.GetLocationRequest,
+        metadata: Sequence[Tuple[str, str]],
+    ) -> Tuple[locations_pb2.GetLocationRequest, Sequence[Tuple[str, str]]]:
+        """Pre-rpc interceptor for get_location
+
+        Override in a subclass to manipulate the request or metadata
+        before they are sent to the RegistrationService server.
+        """
+        return request, metadata
+
+    def post_get_location(
+        self, response: locations_pb2.Location
+    ) -> locations_pb2.Location:
+        """Post-rpc interceptor for get_location
+
+        Override in a subclass to manipulate the response
+        after it is returned by the RegistrationService server but before
+        it is returned to user code.
+        """
+        return response
+
+    def pre_list_locations(
+        self,
+        request: locations_pb2.ListLocationsRequest,
+        metadata: Sequence[Tuple[str, str]],
+    ) -> Tuple[locations_pb2.ListLocationsRequest, Sequence[Tuple[str, str]]]:
+        """Pre-rpc interceptor for list_locations
+
+        Override in a subclass to manipulate the request or metadata
+        before they are sent to the RegistrationService server.
+        """
+        return request, metadata
+
+    def post_list_locations(
+        self, response: locations_pb2.ListLocationsResponse
+    ) -> locations_pb2.ListLocationsResponse:
+        """Post-rpc interceptor for list_locations
+
+        Override in a subclass to manipulate the response
+        after it is returned by the RegistrationService server but before
+        it is returned to user code.
+        """
+        return response
+
 
 @dataclasses.dataclass
 class RegistrationServiceRestStub:
     _session: AuthorizedSession
     _host: str
     _interceptor: RegistrationServiceRestInterceptor
 
@@ -589,24 +636,25 @@
 class RegistrationServiceRestTransport(RegistrationServiceTransport):
     """REST backend transport for RegistrationService.
 
     Service Directory API for registering services. It defines the
     following resource model:
 
     -  The API has a collection of
-       [Namespace][google.cloud.servicedirectory.v1.Namespace]
+       [Namespace][google.cloud.servicedirectory.v1beta1.Namespace]
        resources, named ``projects/*/locations/*/namespaces/*``.
 
     -  Each Namespace has a collection of
-       [Service][google.cloud.servicedirectory.v1.Service] resources,
-       named ``projects/*/locations/*/namespaces/*/services/*``.
+       [Service][google.cloud.servicedirectory.v1beta1.Service]
+       resources, named
+       ``projects/*/locations/*/namespaces/*/services/*``.
 
     -  Each Service has a collection of
-       [Endpoint][google.cloud.servicedirectory.v1.Endpoint] resources,
-       named
+       [Endpoint][google.cloud.servicedirectory.v1beta1.Endpoint]
+       resources, named
        ``projects/*/locations/*/namespaces/*/services/*/endpoints/*``.
 
     This class defines the same methods as the primary client, so the
     primary client can load the underlying transport implementation
     and call it.
 
     It sends JSON representations of protocol buffers over HTTP/1.1
@@ -714,33 +762,33 @@
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> gcs_endpoint.Endpoint:
             r"""Call the create endpoint method over HTTP.
 
             Args:
                 request (~.registration_service.CreateEndpointRequest):
                     The request object. The request message for
-                [RegistrationService.CreateEndpoint][google.cloud.servicedirectory.v1.RegistrationService.CreateEndpoint].
+                [RegistrationService.CreateEndpoint][google.cloud.servicedirectory.v1beta1.RegistrationService.CreateEndpoint].
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
                 ~.gcs_endpoint.Endpoint:
                     An individual endpoint that provides a
-                [service][google.cloud.servicedirectory.v1.Service]. The
-                service must already exist to create an endpoint.
+                [service][google.cloud.servicedirectory.v1beta1.Service].
+                The service must already exist to create an endpoint.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "post",
-                    "uri": "/v1/{parent=projects/*/locations/*/namespaces/*/services/*}/endpoints",
+                    "uri": "/v1beta1/{parent=projects/*/locations/*/namespaces/*/services/*}/endpoints",
                     "body": "endpoint",
                 },
             ]
             request, metadata = self._interceptor.pre_create_endpoint(request, metadata)
             pb_request = registration_service.CreateEndpointRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
 
@@ -815,35 +863,35 @@
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> gcs_namespace.Namespace:
             r"""Call the create namespace method over HTTP.
 
             Args:
                 request (~.registration_service.CreateNamespaceRequest):
                     The request object. The request message for
-                [RegistrationService.CreateNamespace][google.cloud.servicedirectory.v1.RegistrationService.CreateNamespace].
+                [RegistrationService.CreateNamespace][google.cloud.servicedirectory.v1beta1.RegistrationService.CreateNamespace].
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
                 ~.gcs_namespace.Namespace:
                     A container for
-                [services][google.cloud.servicedirectory.v1.Service].
+                [services][google.cloud.servicedirectory.v1beta1.Service].
                 Namespaces allow administrators to group services
                 together and define permissions for a collection of
                 services.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "post",
-                    "uri": "/v1/{parent=projects/*/locations/*}/namespaces",
+                    "uri": "/v1beta1/{parent=projects/*/locations/*}/namespaces",
                     "body": "namespace",
                 },
             ]
             request, metadata = self._interceptor.pre_create_namespace(
                 request, metadata
             )
             pb_request = registration_service.CreateNamespaceRequest.pb(request)
@@ -920,34 +968,34 @@
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> gcs_service.Service:
             r"""Call the create service method over HTTP.
 
             Args:
                 request (~.registration_service.CreateServiceRequest):
                     The request object. The request message for
-                [RegistrationService.CreateService][google.cloud.servicedirectory.v1.RegistrationService.CreateService].
+                [RegistrationService.CreateService][google.cloud.servicedirectory.v1beta1.RegistrationService.CreateService].
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
                 ~.gcs_service.Service:
                     An individual service. A service contains a name and
                 optional metadata. A service must exist before
-                [endpoints][google.cloud.servicedirectory.v1.Endpoint]
+                [endpoints][google.cloud.servicedirectory.v1beta1.Endpoint]
                 can be added to it.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "post",
-                    "uri": "/v1/{parent=projects/*/locations/*/namespaces/*}/services",
+                    "uri": "/v1beta1/{parent=projects/*/locations/*/namespaces/*}/services",
                     "body": "service",
                 },
             ]
             request, metadata = self._interceptor.pre_create_service(request, metadata)
             pb_request = registration_service.CreateServiceRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
 
@@ -1020,26 +1068,26 @@
             metadata: Sequence[Tuple[str, str]] = (),
         ):
             r"""Call the delete endpoint method over HTTP.
 
             Args:
                 request (~.registration_service.DeleteEndpointRequest):
                     The request object. The request message for
-                [RegistrationService.DeleteEndpoint][google.cloud.servicedirectory.v1.RegistrationService.DeleteEndpoint].
+                [RegistrationService.DeleteEndpoint][google.cloud.servicedirectory.v1beta1.RegistrationService.DeleteEndpoint].
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "delete",
-                    "uri": "/v1/{name=projects/*/locations/*/namespaces/*/services/*/endpoints/*}",
+                    "uri": "/v1beta1/{name=projects/*/locations/*/namespaces/*/services/*/endpoints/*}",
                 },
             ]
             request, metadata = self._interceptor.pre_delete_endpoint(request, metadata)
             pb_request = registration_service.DeleteEndpointRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
 
             uri = transcoded_request["uri"]
@@ -1095,26 +1143,26 @@
             metadata: Sequence[Tuple[str, str]] = (),
         ):
             r"""Call the delete namespace method over HTTP.
 
             Args:
                 request (~.registration_service.DeleteNamespaceRequest):
                     The request object. The request message for
-                [RegistrationService.DeleteNamespace][google.cloud.servicedirectory.v1.RegistrationService.DeleteNamespace].
+                [RegistrationService.DeleteNamespace][google.cloud.servicedirectory.v1beta1.RegistrationService.DeleteNamespace].
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "delete",
-                    "uri": "/v1/{name=projects/*/locations/*/namespaces/*}",
+                    "uri": "/v1beta1/{name=projects/*/locations/*/namespaces/*}",
                 },
             ]
             request, metadata = self._interceptor.pre_delete_namespace(
                 request, metadata
             )
             pb_request = registration_service.DeleteNamespaceRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
@@ -1172,26 +1220,26 @@
             metadata: Sequence[Tuple[str, str]] = (),
         ):
             r"""Call the delete service method over HTTP.
 
             Args:
                 request (~.registration_service.DeleteServiceRequest):
                     The request object. The request message for
-                [RegistrationService.DeleteService][google.cloud.servicedirectory.v1.RegistrationService.DeleteService].
+                [RegistrationService.DeleteService][google.cloud.servicedirectory.v1beta1.RegistrationService.DeleteService].
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "delete",
-                    "uri": "/v1/{name=projects/*/locations/*/namespaces/*/services/*}",
+                    "uri": "/v1beta1/{name=projects/*/locations/*/namespaces/*/services/*}",
                 },
             ]
             request, metadata = self._interceptor.pre_delete_service(request, metadata)
             pb_request = registration_service.DeleteServiceRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
 
             uri = transcoded_request["uri"]
@@ -1247,35 +1295,35 @@
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> endpoint.Endpoint:
             r"""Call the get endpoint method over HTTP.
 
             Args:
                 request (~.registration_service.GetEndpointRequest):
                     The request object. The request message for
-                [RegistrationService.GetEndpoint][google.cloud.servicedirectory.v1.RegistrationService.GetEndpoint].
+                [RegistrationService.GetEndpoint][google.cloud.servicedirectory.v1beta1.RegistrationService.GetEndpoint].
                 This should not be used to lookup endpoints at runtime.
                 Instead, use the ``resolve`` method.
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
                 ~.endpoint.Endpoint:
                     An individual endpoint that provides a
-                [service][google.cloud.servicedirectory.v1.Service]. The
-                service must already exist to create an endpoint.
+                [service][google.cloud.servicedirectory.v1beta1.Service].
+                The service must already exist to create an endpoint.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "get",
-                    "uri": "/v1/{name=projects/*/locations/*/namespaces/*/services/*/endpoints/*}",
+                    "uri": "/v1beta1/{name=projects/*/locations/*/namespaces/*/services/*/endpoints/*}",
                 },
             ]
             request, metadata = self._interceptor.pre_get_endpoint(request, metadata)
             pb_request = registration_service.GetEndpointRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
 
             uri = transcoded_request["uri"]
@@ -1428,20 +1476,25 @@
                 documentation <https://cloud.google.com/iam/docs/>`__.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "post",
-                    "uri": "/v1/{resource=projects/*/locations/*/namespaces/*}:getIamPolicy",
+                    "uri": "/v1beta1/{resource=projects/*/locations/*/namespaces/*}:getIamPolicy",
+                    "body": "*",
+                },
+                {
+                    "method": "post",
+                    "uri": "/v1beta1/{resource=projects/*/locations/*/namespaces/*/services/*}:getIamPolicy",
                     "body": "*",
                 },
                 {
                     "method": "post",
-                    "uri": "/v1/{resource=projects/*/locations/*/namespaces/*/services/*}:getIamPolicy",
+                    "uri": "/v1beta1/{resource=projects/*/locations/*/namespaces/*/workloads/*}:getIamPolicy",
                     "body": "*",
                 },
             ]
             request, metadata = self._interceptor.pre_get_iam_policy(request, metadata)
             pb_request = request
             transcoded_request = path_template.transcode(http_options, pb_request)
 
@@ -1514,35 +1567,35 @@
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> namespace.Namespace:
             r"""Call the get namespace method over HTTP.
 
             Args:
                 request (~.registration_service.GetNamespaceRequest):
                     The request object. The request message for
-                [RegistrationService.GetNamespace][google.cloud.servicedirectory.v1.RegistrationService.GetNamespace].
+                [RegistrationService.GetNamespace][google.cloud.servicedirectory.v1beta1.RegistrationService.GetNamespace].
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
                 ~.namespace.Namespace:
                     A container for
-                [services][google.cloud.servicedirectory.v1.Service].
+                [services][google.cloud.servicedirectory.v1beta1.Service].
                 Namespaces allow administrators to group services
                 together and define permissions for a collection of
                 services.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "get",
-                    "uri": "/v1/{name=projects/*/locations/*/namespaces/*}",
+                    "uri": "/v1beta1/{name=projects/*/locations/*/namespaces/*}",
                 },
             ]
             request, metadata = self._interceptor.pre_get_namespace(request, metadata)
             pb_request = registration_service.GetNamespaceRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
 
             uri = transcoded_request["uri"]
@@ -1606,37 +1659,37 @@
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> service.Service:
             r"""Call the get service method over HTTP.
 
             Args:
                 request (~.registration_service.GetServiceRequest):
                     The request object. The request message for
-                [RegistrationService.GetService][google.cloud.servicedirectory.v1.RegistrationService.GetService].
+                [RegistrationService.GetService][google.cloud.servicedirectory.v1beta1.RegistrationService.GetService].
                 This should not be used for looking up a service.
-                Insead, use the ``resolve`` method as it will contain
-                all endpoints and associated metadata.
+                Instead, use the ``resolve`` method as it contains all
+                endpoints and associated metadata.
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
                 ~.service.Service:
                     An individual service. A service contains a name and
                 optional metadata. A service must exist before
-                [endpoints][google.cloud.servicedirectory.v1.Endpoint]
+                [endpoints][google.cloud.servicedirectory.v1beta1.Endpoint]
                 can be added to it.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "get",
-                    "uri": "/v1/{name=projects/*/locations/*/namespaces/*/services/*}",
+                    "uri": "/v1beta1/{name=projects/*/locations/*/namespaces/*/services/*}",
                 },
             ]
             request, metadata = self._interceptor.pre_get_service(request, metadata)
             pb_request = registration_service.GetServiceRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
 
             uri = transcoded_request["uri"]
@@ -1700,32 +1753,32 @@
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> registration_service.ListEndpointsResponse:
             r"""Call the list endpoints method over HTTP.
 
             Args:
                 request (~.registration_service.ListEndpointsRequest):
                     The request object. The request message for
-                [RegistrationService.ListEndpoints][google.cloud.servicedirectory.v1.RegistrationService.ListEndpoints].
+                [RegistrationService.ListEndpoints][google.cloud.servicedirectory.v1beta1.RegistrationService.ListEndpoints].
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
                 ~.registration_service.ListEndpointsResponse:
                     The response message for
-                [RegistrationService.ListEndpoints][google.cloud.servicedirectory.v1.RegistrationService.ListEndpoints].
+                [RegistrationService.ListEndpoints][google.cloud.servicedirectory.v1beta1.RegistrationService.ListEndpoints].
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "get",
-                    "uri": "/v1/{parent=projects/*/locations/*/namespaces/*/services/*}/endpoints",
+                    "uri": "/v1beta1/{parent=projects/*/locations/*/namespaces/*/services/*}/endpoints",
                 },
             ]
             request, metadata = self._interceptor.pre_list_endpoints(request, metadata)
             pb_request = registration_service.ListEndpointsRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
 
             uri = transcoded_request["uri"]
@@ -1789,32 +1842,32 @@
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> registration_service.ListNamespacesResponse:
             r"""Call the list namespaces method over HTTP.
 
             Args:
                 request (~.registration_service.ListNamespacesRequest):
                     The request object. The request message for
-                [RegistrationService.ListNamespaces][google.cloud.servicedirectory.v1.RegistrationService.ListNamespaces].
+                [RegistrationService.ListNamespaces][google.cloud.servicedirectory.v1beta1.RegistrationService.ListNamespaces].
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
                 ~.registration_service.ListNamespacesResponse:
                     The response message for
-                [RegistrationService.ListNamespaces][google.cloud.servicedirectory.v1.RegistrationService.ListNamespaces].
+                [RegistrationService.ListNamespaces][google.cloud.servicedirectory.v1beta1.RegistrationService.ListNamespaces].
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "get",
-                    "uri": "/v1/{parent=projects/*/locations/*}/namespaces",
+                    "uri": "/v1beta1/{parent=projects/*/locations/*}/namespaces",
                 },
             ]
             request, metadata = self._interceptor.pre_list_namespaces(request, metadata)
             pb_request = registration_service.ListNamespacesRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
 
             uri = transcoded_request["uri"]
@@ -1878,32 +1931,32 @@
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> registration_service.ListServicesResponse:
             r"""Call the list services method over HTTP.
 
             Args:
                 request (~.registration_service.ListServicesRequest):
                     The request object. The request message for
-                [RegistrationService.ListServices][google.cloud.servicedirectory.v1.RegistrationService.ListServices].
+                [RegistrationService.ListServices][google.cloud.servicedirectory.v1beta1.RegistrationService.ListServices].
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
                 ~.registration_service.ListServicesResponse:
                     The response message for
-                [RegistrationService.ListServices][google.cloud.servicedirectory.v1.RegistrationService.ListServices].
+                [RegistrationService.ListServices][google.cloud.servicedirectory.v1beta1.RegistrationService.ListServices].
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "get",
-                    "uri": "/v1/{parent=projects/*/locations/*/namespaces/*}/services",
+                    "uri": "/v1beta1/{parent=projects/*/locations/*/namespaces/*}/services",
                 },
             ]
             request, metadata = self._interceptor.pre_list_services(request, metadata)
             pb_request = registration_service.ListServicesRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
 
             uri = transcoded_request["uri"]
@@ -2056,20 +2109,25 @@
                 documentation <https://cloud.google.com/iam/docs/>`__.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "post",
-                    "uri": "/v1/{resource=projects/*/locations/*/namespaces/*}:setIamPolicy",
+                    "uri": "/v1beta1/{resource=projects/*/locations/*/namespaces/*}:setIamPolicy",
+                    "body": "*",
+                },
+                {
+                    "method": "post",
+                    "uri": "/v1beta1/{resource=projects/*/locations/*/namespaces/*/services/*}:setIamPolicy",
                     "body": "*",
                 },
                 {
                     "method": "post",
-                    "uri": "/v1/{resource=projects/*/locations/*/namespaces/*/services/*}:setIamPolicy",
+                    "uri": "/v1beta1/{resource=projects/*/locations/*/namespaces/*/workloads/*}:setIamPolicy",
                     "body": "*",
                 },
             ]
             request, metadata = self._interceptor.pre_set_iam_policy(request, metadata)
             pb_request = request
             transcoded_request = path_template.transcode(http_options, pb_request)
 
@@ -2156,20 +2214,25 @@
                 ~.iam_policy_pb2.TestIamPermissionsResponse:
                     Response message for ``TestIamPermissions`` method.
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "post",
-                    "uri": "/v1/{resource=projects/*/locations/*/namespaces/*}:testIamPermissions",
+                    "uri": "/v1beta1/{resource=projects/*/locations/*/namespaces/*}:testIamPermissions",
                     "body": "*",
                 },
                 {
                     "method": "post",
-                    "uri": "/v1/{resource=projects/*/locations/*/namespaces/*/services/*}:testIamPermissions",
+                    "uri": "/v1beta1/{resource=projects/*/locations/*/namespaces/*/services/*}:testIamPermissions",
+                    "body": "*",
+                },
+                {
+                    "method": "post",
+                    "uri": "/v1beta1/{resource=projects/*/locations/*/namespaces/*/workloads/*}:testIamPermissions",
                     "body": "*",
                 },
             ]
             request, metadata = self._interceptor.pre_test_iam_permissions(
                 request, metadata
             )
             pb_request = request
@@ -2246,33 +2309,33 @@
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> gcs_endpoint.Endpoint:
             r"""Call the update endpoint method over HTTP.
 
             Args:
                 request (~.registration_service.UpdateEndpointRequest):
                     The request object. The request message for
-                [RegistrationService.UpdateEndpoint][google.cloud.servicedirectory.v1.RegistrationService.UpdateEndpoint].
+                [RegistrationService.UpdateEndpoint][google.cloud.servicedirectory.v1beta1.RegistrationService.UpdateEndpoint].
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
                 ~.gcs_endpoint.Endpoint:
                     An individual endpoint that provides a
-                [service][google.cloud.servicedirectory.v1.Service]. The
-                service must already exist to create an endpoint.
+                [service][google.cloud.servicedirectory.v1beta1.Service].
+                The service must already exist to create an endpoint.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "patch",
-                    "uri": "/v1/{endpoint.name=projects/*/locations/*/namespaces/*/services/*/endpoints/*}",
+                    "uri": "/v1beta1/{endpoint.name=projects/*/locations/*/namespaces/*/services/*/endpoints/*}",
                     "body": "endpoint",
                 },
             ]
             request, metadata = self._interceptor.pre_update_endpoint(request, metadata)
             pb_request = registration_service.UpdateEndpointRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
 
@@ -2347,35 +2410,35 @@
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> gcs_namespace.Namespace:
             r"""Call the update namespace method over HTTP.
 
             Args:
                 request (~.registration_service.UpdateNamespaceRequest):
                     The request object. The request message for
-                [RegistrationService.UpdateNamespace][google.cloud.servicedirectory.v1.RegistrationService.UpdateNamespace].
+                [RegistrationService.UpdateNamespace][google.cloud.servicedirectory.v1beta1.RegistrationService.UpdateNamespace].
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
                 ~.gcs_namespace.Namespace:
                     A container for
-                [services][google.cloud.servicedirectory.v1.Service].
+                [services][google.cloud.servicedirectory.v1beta1.Service].
                 Namespaces allow administrators to group services
                 together and define permissions for a collection of
                 services.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "patch",
-                    "uri": "/v1/{namespace.name=projects/*/locations/*/namespaces/*}",
+                    "uri": "/v1beta1/{namespace.name=projects/*/locations/*/namespaces/*}",
                     "body": "namespace",
                 },
             ]
             request, metadata = self._interceptor.pre_update_namespace(
                 request, metadata
             )
             pb_request = registration_service.UpdateNamespaceRequest.pb(request)
@@ -2452,34 +2515,34 @@
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> gcs_service.Service:
             r"""Call the update service method over HTTP.
 
             Args:
                 request (~.registration_service.UpdateServiceRequest):
                     The request object. The request message for
-                [RegistrationService.UpdateService][google.cloud.servicedirectory.v1.RegistrationService.UpdateService].
+                [RegistrationService.UpdateService][google.cloud.servicedirectory.v1beta1.RegistrationService.UpdateService].
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
                 ~.gcs_service.Service:
                     An individual service. A service contains a name and
                 optional metadata. A service must exist before
-                [endpoints][google.cloud.servicedirectory.v1.Endpoint]
+                [endpoints][google.cloud.servicedirectory.v1beta1.Endpoint]
                 can be added to it.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "patch",
-                    "uri": "/v1/{service.name=projects/*/locations/*/namespaces/*/services/*}",
+                    "uri": "/v1beta1/{service.name=projects/*/locations/*/namespaces/*/services/*}",
                     "body": "service",
                 },
             ]
             request, metadata = self._interceptor.pre_update_service(request, metadata)
             pb_request = registration_service.UpdateServiceRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
 
@@ -2686,14 +2749,148 @@
         self,
     ) -> Callable[[registration_service.UpdateServiceRequest], gcs_service.Service]:
         # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
         # In C++ this would require a dynamic_cast
         return self._UpdateService(self._session, self._host, self._interceptor)  # type: ignore
 
     @property
+    def get_location(self):
+        return self._GetLocation(self._session, self._host, self._interceptor)  # type: ignore
+
+    class _GetLocation(RegistrationServiceRestStub):
+        def __call__(
+            self,
+            request: locations_pb2.GetLocationRequest,
+            *,
+            retry: OptionalRetry = gapic_v1.method.DEFAULT,
+            timeout: Optional[float] = None,
+            metadata: Sequence[Tuple[str, str]] = (),
+        ) -> locations_pb2.Location:
+
+            r"""Call the get location method over HTTP.
+
+            Args:
+                request (locations_pb2.GetLocationRequest):
+                    The request object for GetLocation method.
+                retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                    should be retried.
+                timeout (float): The timeout for this request.
+                metadata (Sequence[Tuple[str, str]]): Strings which should be
+                    sent along with the request as metadata.
+
+            Returns:
+                locations_pb2.Location: Response from GetLocation method.
+            """
+
+            http_options: List[Dict[str, str]] = [
+                {
+                    "method": "get",
+                    "uri": "/v1beta1/{name=projects/*/locations/*}",
+                },
+            ]
+
+            request, metadata = self._interceptor.pre_get_location(request, metadata)
+            request_kwargs = json_format.MessageToDict(request)
+            transcoded_request = path_template.transcode(http_options, **request_kwargs)
+
+            uri = transcoded_request["uri"]
+            method = transcoded_request["method"]
+
+            # Jsonify the query params
+            query_params = json.loads(json.dumps(transcoded_request["query_params"]))
+
+            # Send the request
+            headers = dict(metadata)
+            headers["Content-Type"] = "application/json"
+
+            response = getattr(self._session, method)(
+                "{host}{uri}".format(host=self._host, uri=uri),
+                timeout=timeout,
+                headers=headers,
+                params=rest_helpers.flatten_query_params(query_params),
+            )
+
+            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
+            # subclass.
+            if response.status_code >= 400:
+                raise core_exceptions.from_http_response(response)
+
+            resp = locations_pb2.Location()
+            resp = json_format.Parse(response.content.decode("utf-8"), resp)
+            resp = self._interceptor.post_get_location(resp)
+            return resp
+
+    @property
+    def list_locations(self):
+        return self._ListLocations(self._session, self._host, self._interceptor)  # type: ignore
+
+    class _ListLocations(RegistrationServiceRestStub):
+        def __call__(
+            self,
+            request: locations_pb2.ListLocationsRequest,
+            *,
+            retry: OptionalRetry = gapic_v1.method.DEFAULT,
+            timeout: Optional[float] = None,
+            metadata: Sequence[Tuple[str, str]] = (),
+        ) -> locations_pb2.ListLocationsResponse:
+
+            r"""Call the list locations method over HTTP.
+
+            Args:
+                request (locations_pb2.ListLocationsRequest):
+                    The request object for ListLocations method.
+                retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                    should be retried.
+                timeout (float): The timeout for this request.
+                metadata (Sequence[Tuple[str, str]]): Strings which should be
+                    sent along with the request as metadata.
+
+            Returns:
+                locations_pb2.ListLocationsResponse: Response from ListLocations method.
+            """
+
+            http_options: List[Dict[str, str]] = [
+                {
+                    "method": "get",
+                    "uri": "/v1beta1/{name=projects/*}/locations",
+                },
+            ]
+
+            request, metadata = self._interceptor.pre_list_locations(request, metadata)
+            request_kwargs = json_format.MessageToDict(request)
+            transcoded_request = path_template.transcode(http_options, **request_kwargs)
+
+            uri = transcoded_request["uri"]
+            method = transcoded_request["method"]
+
+            # Jsonify the query params
+            query_params = json.loads(json.dumps(transcoded_request["query_params"]))
+
+            # Send the request
+            headers = dict(metadata)
+            headers["Content-Type"] = "application/json"
+
+            response = getattr(self._session, method)(
+                "{host}{uri}".format(host=self._host, uri=uri),
+                timeout=timeout,
+                headers=headers,
+                params=rest_helpers.flatten_query_params(query_params),
+            )
+
+            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
+            # subclass.
+            if response.status_code >= 400:
+                raise core_exceptions.from_http_response(response)
+
+            resp = locations_pb2.ListLocationsResponse()
+            resp = json_format.Parse(response.content.decode("utf-8"), resp)
+            resp = self._interceptor.post_list_locations(resp)
+            return resp
+
+    @property
     def kind(self) -> str:
         return "rest"
 
     def close(self):
         self._session.close()
```

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/types/__init__.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/types/__init__.py`

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

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/types/endpoint.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/types/service.py`

 * *Files 16% similar despite different names*

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
@@ -15,79 +15,82 @@
 #
 from __future__ import annotations
 
 from typing import MutableMapping, MutableSequence
 
 import proto  # type: ignore
 
+from google.cloud.servicedirectory_v1.types import endpoint
+
 __protobuf__ = proto.module(
     package="google.cloud.servicedirectory.v1",
     manifest={
-        "Endpoint",
+        "Service",
     },
 )
 
 
-class Endpoint(proto.Message):
-    r"""An individual endpoint that provides a
-    [service][google.cloud.servicedirectory.v1.Service]. The service
-    must already exist to create an endpoint.
+class Service(proto.Message):
+    r"""An individual service. A service contains a name and optional
+    metadata. A service must exist before
+    [endpoints][google.cloud.servicedirectory.v1.Endpoint] can be added
+    to it.
 
     Attributes:
         name (str):
-            Immutable. The resource name for the endpoint in the format
-            ``projects/*/locations/*/namespaces/*/services/*/endpoints/*``.
-        address (str):
-            Optional. An IPv4 or IPv6 address. Service Directory will
-            reject bad addresses like: "8.8.8" "8.8.8.8:53"
-            "test:bad:address" "[::1]" "[::1]:8080" Limited to 45
-            characters.
-        port (int):
-            Optional. Service Directory will reject values outside of
-            [0, 65535].
+            Immutable. The resource name for the service in the format
+            ``projects/*/locations/*/namespaces/*/services/*``.
         annotations (MutableMapping[str, str]):
-            Optional. Annotations for the endpoint. This data can be
-            consumed by service clients. Restrictions:
+            Optional. Annotations for the service. This data can be
+            consumed by service clients.
+
+            Restrictions:
 
-            -  The entire annotations dictionary may contain up to 512
+            -  The entire annotations dictionary may contain up to 2000
                characters, spread accoss all key-value pairs.
-               Annotations that goes beyond any these limits will be
-               rejected.
+               Annotations that go beyond this limit are rejected
             -  Valid annotation keys have two segments: an optional
                prefix and name, separated by a slash (/). The name
                segment is required and must be 63 characters or less,
                beginning and ending with an alphanumeric character
                ([a-z0-9A-Z]) with dashes (-), underscores (_), dots (.),
                and alphanumerics between. The prefix is optional. If
                specified, the prefix must be a DNS subdomain: a series
                of DNS labels separated by dots (.), not longer than 253
                characters in total, followed by a slash (/). Annotations
-               that fails to meet these requirements will be rejected.
-            -  The '(*.)google.com/' and '(*.)googleapis.com/' prefixes
-               are reserved for system annotations managed by Service
-               Directory. If the user tries to write to these keyspaces,
-               those entries will be silently ignored by the system.
-               Note: This field is equivalent to the 'metadata' field in
-               the v1beta1 API. They have the same syntax and read/write
-               to the same location in Service Directory.
+               that fails to meet these requirements are rejected
+
+            Note: This field is equivalent to the ``metadata`` field in
+            the v1beta1 API. They have the same syntax and read/write to
+            the same location in Service Directory.
+        endpoints (MutableSequence[google.cloud.servicedirectory_v1.types.Endpoint]):
+            Output only. Endpoints associated with this service.
+            Returned on
+            [LookupService.ResolveService][google.cloud.servicedirectory.v1.LookupService.ResolveService].
+            Control plane clients should use
+            [RegistrationService.ListEndpoints][google.cloud.servicedirectory.v1.RegistrationService.ListEndpoints].
+        uid (str):
+            Output only. The globally unique identifier
+            of the service in the UUID4 format.
     """
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    address: str = proto.Field(
+    annotations: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
-        number=2,
+        proto.STRING,
+        number=4,
     )
-    port: int = proto.Field(
-        proto.INT32,
+    endpoints: MutableSequence[endpoint.Endpoint] = proto.RepeatedField(
+        proto.MESSAGE,
         number=3,
+        message=endpoint.Endpoint,
     )
-    annotations: MutableMapping[str, str] = proto.MapField(
-        proto.STRING,
+    uid: str = proto.Field(
         proto.STRING,
-        number=5,
+        number=7,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/types/lookup_service.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/types/lookup_service.py`

 * *Files 26% similar despite different names*

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
@@ -15,28 +15,28 @@
 #
 from __future__ import annotations
 
 from typing import MutableMapping, MutableSequence
 
 import proto  # type: ignore
 
-from google.cloud.servicedirectory_v1.types import service as gcs_service
+from google.cloud.servicedirectory_v1beta1.types import service as gcs_service
 
 __protobuf__ = proto.module(
-    package="google.cloud.servicedirectory.v1",
+    package="google.cloud.servicedirectory.v1beta1",
     manifest={
         "ResolveServiceRequest",
         "ResolveServiceResponse",
     },
 )
 
 
 class ResolveServiceRequest(proto.Message):
     r"""The request message for
-    [LookupService.ResolveService][google.cloud.servicedirectory.v1.LookupService.ResolveService].
+    [LookupService.ResolveService][google.cloud.servicedirectory.v1beta1.LookupService.ResolveService].
     Looks up a service by its name, returns the service and its
     endpoints.
 
     Attributes:
         name (str):
             Required. The name of the service to resolve.
         max_endpoints (int):
@@ -45,28 +45,56 @@
             value less than one is specified, the Default is
             used. If a value greater than the Maximum is
             specified, the Maximum is used.
         endpoint_filter (str):
             Optional. The filter applied to the endpoints of the
             resolved service.
 
-            General filter string syntax: () can be "name" or
-            "metadata." for map field. can be "<, >, <=, >=, !=, =, :".
-            Of which ":" means HAS and is roughly the same as "=". must
-            be the same data type as the field. can be "AND, OR, NOT".
+            General ``filter`` string syntax:
+            ``<field> <operator> <value> (<logical connector>)``
+
+            -  ``<field>`` can be ``name``, ``address``, ``port``, or
+               ``metadata.<key>`` for map field
+            -  ``<operator>`` can be ``<``, ``>``, ``<=``, ``>=``,
+               ``!=``, ``=``, ``:``. Of which ``:`` means ``HAS``, and
+               is roughly the same as ``=``
+            -  ``<value>`` must be the same data type as field
+            -  ``<logical connector>`` can be ``AND``, ``OR``, ``NOT``
 
             Examples of valid filters:
 
-            -  "metadata.owner" returns Endpoints that have a label with
-               the key "owner", this is the same as "metadata:owner"
-            -  "metadata.protocol=gRPC" returns Endpoints that have
-               key/value "protocol=gRPC"
-            -  "metadata.owner!=sd AND metadata.foo=bar" returns
-               Endpoints that have "owner" field in metadata with a
-               value that is not "sd" AND have the key/value foo=bar.
+            -  ``metadata.owner`` returns endpoints that have a
+               annotation with the key ``owner``, this is the same as
+               ``metadata:owner``
+            -  ``metadata.protocol=gRPC`` returns endpoints that have
+               key/value ``protocol=gRPC``
+            -  ``address=192.108.1.105`` returns endpoints that have
+               this address
+            -  ``port>8080`` returns endpoints that have port number
+               larger than 8080
+            -
+
+            ``name>projects/my-project/locations/us-east1/namespaces/my-namespace/services/my-service/endpoints/endpoint-c``
+            returns endpoints that have name that is alphabetically
+            later than the string, so "endpoint-e" is returned but
+            "endpoint-a" is not \*
+            ``name=projects/my-project/locations/us-central1/namespaces/my-namespace/services/my-service/endpoints/ep-1``
+            returns the endpoint that has an endpoint_id equal to
+            ``ep-1``
+
+            -  ``metadata.owner!=sd AND metadata.foo=bar`` returns
+               endpoints that have ``owner`` in annotation key but value
+               is not ``sd`` AND have key/value ``foo=bar``
+            -  ``doesnotexist.foo=bar`` returns an empty list. Note that
+               endpoint doesn't have a field called "doesnotexist".
+               Since the filter does not match any endpoint, it returns
+               no results
+
+            For more information about filtering, see `API
+            Filtering <https://aip.dev/160>`__.
     """
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
     max_endpoints: int = proto.Field(
@@ -77,18 +105,18 @@
         proto.STRING,
         number=3,
     )
 
 
 class ResolveServiceResponse(proto.Message):
     r"""The response message for
-    [LookupService.ResolveService][google.cloud.servicedirectory.v1.LookupService.ResolveService].
+    [LookupService.ResolveService][google.cloud.servicedirectory.v1beta1.LookupService.ResolveService].
 
     Attributes:
-        service (google.cloud.servicedirectory_v1.types.Service):
+        service (google.cloud.servicedirectory_v1beta1.types.Service):
 
     """
 
     service: gcs_service.Service = proto.Field(
         proto.MESSAGE,
         number=1,
         message=gcs_service.Service,
```

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/types/namespace.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/types/namespace.py`

 * *Files 16% similar despite different names*

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
@@ -35,24 +35,31 @@
 
     Attributes:
         name (str):
             Immutable. The resource name for the namespace in the format
             ``projects/*/locations/*/namespaces/*``.
         labels (MutableMapping[str, str]):
             Optional. Resource labels associated with
-            this Namespace. No more than 64 user labels can
-            be associated with a given resource.  Label keys
+            this namespace. No more than 64 user labels can
+            be associated with a given resource. Label keys
             and values can be no longer than 63 characters.
+        uid (str):
+            Output only. The globally unique identifier
+            of the namespace in the UUID4 format.
     """
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
     labels: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=2,
     )
+    uid: str = proto.Field(
+        proto.STRING,
+        number=5,
+    )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/types/registration_service.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/types/registration_service.py`

 * *Files 12% similar despite different names*

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
@@ -88,54 +88,69 @@
 class ListNamespacesRequest(proto.Message):
     r"""The request message for
     [RegistrationService.ListNamespaces][google.cloud.servicedirectory.v1.RegistrationService.ListNamespaces].
 
     Attributes:
         parent (str):
             Required. The resource name of the project
-            and location whose namespaces we'd like to list.
+            and location whose namespaces you'd like to
+            list.
         page_size (int):
             Optional. The maximum number of items to
             return.
         page_token (str):
             Optional. The next_page_token value returned from a previous
             List request, if any.
         filter (str):
-            Optional. The filter to list result by.
+            Optional. The filter to list results by.
+
+            General ``filter`` string syntax:
+            ``<field> <operator> <value> (<logical connector>)``
 
-            General filter string syntax: () can be "name", or "labels."
-            for map field. can be "<, >, <=, >=, !=, =, :". Of which ":"
-            means HAS, and is roughly the same as "=". must be the same
-            data type as field. can be "AND, OR, NOT".
+            -  ``<field>`` can be ``name`` or ``labels.<key>`` for map
+               field
+            -  ``<operator>`` can be ``<``, ``>``, ``<=``, ``>=``,
+               ``!=``, ``=``, ``:``. Of which ``:`` means ``HAS``, and
+               is roughly the same as ``=``
+            -  ``<value>`` must be the same data type as field
+            -  ``<logical connector>`` can be ``AND``, ``OR``, ``NOT``
 
             Examples of valid filters:
 
-            -  "labels.owner" returns Namespaces that have a label with
-               the key "owner" this is the same as "labels:owner".
-            -  "labels.protocol=gRPC" returns Namespaces that have
-               key/value "protocol=gRPC".
-            -  "name>projects/my-project/locations/us-east/namespaces/namespace-c"
-               returns Namespaces that have name that is alphabetically
-               later than the string, so "namespace-e" will be returned
-               but "namespace-a" will not be.
-            -  "labels.owner!=sd AND labels.foo=bar" returns Namespaces
-               that have "owner" in label key but value is not "sd" AND
-               have key/value foo=bar.
-            -  "doesnotexist.foo=bar" returns an empty list. Note that
-               Namespace doesn't have a field called "doesnotexist".
-               Since the filter does not match any Namespaces, it
-               returns no results.
+            -  ``labels.owner`` returns namespaces that have a label
+               with the key ``owner``, this is the same as
+               ``labels:owner``
+            -  ``labels.owner=sd`` returns namespaces that have
+               key/value ``owner=sd``
+            -  ``name>projects/my-project/locations/us-east1/namespaces/namespace-c``
+               returns namespaces that have name that is alphabetically
+               later than the string, so "namespace-e" is returned but
+               "namespace-a" is not
+            -  ``labels.owner!=sd AND labels.foo=bar`` returns
+               namespaces that have ``owner`` in label key but value is
+               not ``sd`` AND have key/value ``foo=bar``
+            -  ``doesnotexist.foo=bar`` returns an empty list. Note that
+               namespace doesn't have a field called "doesnotexist".
+               Since the filter does not match any namespaces, it
+               returns no results
+
+            For more information about filtering, see `API
+            Filtering <https://aip.dev/160>`__.
         order_by (str):
-            Optional. The order to list result by.
+            Optional. The order to list results by.
+
+            General ``order_by`` string syntax:
+            ``<field> (<asc|desc>) (,)``
 
-            General order by string syntax: (<asc|desc>) (,) allows
-            values {"name"} <asc/desc> ascending or descending order by
-            . If this is left blank, "asc" is used. Note that an empty
-            order_by string result in default order, which is order by
-            name in ascending order.
+            -  ``<field>`` allows value: ``name``
+            -  ``<asc|desc>`` ascending or descending order by
+               ``<field>``. If this is left blank, ``asc`` is used
+
+            Note that an empty ``order_by`` string results in default
+            order, which is order by ``name`` in ascending order.
     """
 
     parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
     page_size: int = proto.Field(
@@ -278,48 +293,71 @@
 class ListServicesRequest(proto.Message):
     r"""The request message for
     [RegistrationService.ListServices][google.cloud.servicedirectory.v1.RegistrationService.ListServices].
 
     Attributes:
         parent (str):
             Required. The resource name of the namespace
-            whose services we'd like to list.
+            whose services you'd like to list.
         page_size (int):
             Optional. The maximum number of items to
             return.
         page_token (str):
             Optional. The next_page_token value returned from a previous
             List request, if any.
         filter (str):
-            Optional. The filter to list result by.
+            Optional. The filter to list results by.
+
+            General ``filter`` string syntax:
+            ``<field> <operator> <value> (<logical connector>)``
 
-            General filter string syntax: () can be "name", or
-            "metadata." for map field. can be "<, >, <=, >=, !=, =, :".
-            Of which ":" means HAS, and is roughly the same as "=". must
-            be the same data type as field. can be "AND, OR, NOT".
+            -  ``<field>`` can be ``name`` or ``annotations.<key>`` for
+               map field
+            -  ``<operator>`` can be ``<``, ``>``, ``<=``, ``>=``,
+               ``!=``, ``=``, ``:``. Of which ``:`` means ``HAS``, and
+               is roughly the same as ``=``
+            -  ``<value>`` must be the same data type as field
+            -  ``<logical connector>`` can be ``AND``, ``OR``, ``NOT``
 
             Examples of valid filters:
 
-            -  "metadata.owner" returns Services that have a label with
-               the key "owner" this is the same as "metadata:owner".
-            -  "metadata.protocol=gRPC" returns Services that have
-               key/value "protocol=gRPC".
-            -  "name>projects/my-project/locations/us-east/namespaces/my-namespace/services/service-c"
-               returns Services that have name that is alphabetically
-               later than the string, so "service-e" will be returned
-               but "service-a" will not be.
-            -  "metadata.owner!=sd AND metadata.foo=bar" returns
-               Services that have "owner" in label key but value is not
-               "sd" AND have key/value foo=bar.
-            -  "doesnotexist.foo=bar" returns an empty list. Note that
-               Service doesn't have a field called "doesnotexist". Since
-               the filter does not match any Services, it returns no
-               results.
+            -  ``annotations.owner`` returns services that have a
+               annotation with the key ``owner``, this is the same as
+               ``annotations:owner``
+            -  ``annotations.protocol=gRPC`` returns services that have
+               key/value ``protocol=gRPC``
+            -
+
+            ``name>projects/my-project/locations/us-east1/namespaces/my-namespace/services/service-c``
+            returns services that have name that is alphabetically later
+            than the string, so "service-e" is returned but "service-a"
+            is not
+
+            -  ``annotations.owner!=sd AND annotations.foo=bar`` returns
+               services that have ``owner`` in annotation key but value
+               is not ``sd`` AND have key/value ``foo=bar``
+            -  ``doesnotexist.foo=bar`` returns an empty list. Note that
+               service doesn't have a field called "doesnotexist". Since
+               the filter does not match any services, it returns no
+               results
+
+            For more information about filtering, see `API
+            Filtering <https://aip.dev/160>`__.
         order_by (str):
-            Optional. The order to list result by.
+            Optional. The order to list results by.
+
+            General ``order_by`` string syntax:
+            ``<field> (<asc|desc>) (,)``
+
+            -  ``<field>`` allows value: ``name``
+            -  ``<asc|desc>`` ascending or descending order by
+               ``<field>``. If this is left blank, ``asc`` is used
+
+            Note that an empty ``order_by`` string results in default
+            order, which is order by ``name`` in ascending order.
     """
 
     parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
     page_size: int = proto.Field(
@@ -367,17 +405,17 @@
         number=2,
     )
 
 
 class GetServiceRequest(proto.Message):
     r"""The request message for
     [RegistrationService.GetService][google.cloud.servicedirectory.v1.RegistrationService.GetService].
-    This should not be used for looking up a service. Insead, use the
-    ``resolve`` method as it will contain all endpoints and associated
-    metadata.
+    This should not be used for looking up a service. Instead, use the
+    ``resolve`` method as it contains all endpoints and associated
+    annotations.
 
     Attributes:
         name (str):
             Required. The name of the service to get.
     """
 
     name: str = proto.Field(
@@ -463,53 +501,76 @@
 class ListEndpointsRequest(proto.Message):
     r"""The request message for
     [RegistrationService.ListEndpoints][google.cloud.servicedirectory.v1.RegistrationService.ListEndpoints].
 
     Attributes:
         parent (str):
             Required. The resource name of the service
-            whose endpoints we'd like to list.
+            whose endpoints you'd like to list.
         page_size (int):
             Optional. The maximum number of items to
             return.
         page_token (str):
             Optional. The next_page_token value returned from a previous
             List request, if any.
         filter (str):
-            Optional. The filter to list result by.
+            Optional. The filter to list results by.
 
-            General filter string syntax: () can be "name", "address",
-            "port" or "metadata." for map field. can be "<, >, <=, >=,
-            !=, =, :". Of which ":" means HAS, and is roughly the same
-            as "=". must be the same data type as field. can be "AND,
-            OR, NOT".
+            General ``filter`` string syntax:
+            ``<field> <operator> <value> (<logical connector>)``
+
+            -  ``<field>`` can be ``name``, ``address``, ``port``, or
+               ``annotations.<key>`` for map field
+            -  ``<operator>`` can be ``<``, ``>``, ``<=``, ``>=``,
+               ``!=``, ``=``, ``:``. Of which ``:`` means ``HAS``, and
+               is roughly the same as ``=``
+            -  ``<value>`` must be the same data type as field
+            -  ``<logical connector>`` can be ``AND``, ``OR``, ``NOT``
 
             Examples of valid filters:
 
-            -  "metadata.owner" returns Endpoints that have a label with
-               the key "owner" this is the same as "metadata:owner".
-            -  "metadata.protocol=gRPC" returns Endpoints that have
-               key/value "protocol=gRPC".
-            -  "address=192.108.1.105" returns Endpoints that have this
-               address.
-            -  "port>8080" returns Endpoints that have port number
-               larger than 8080.
-            -  "name>projects/my-project/locations/us-east/namespaces/my-namespace/services/my-service/endpoints/endpoint-c"
-               returns Endpoints that have name that is alphabetically
-               later than the string, so "endpoint-e" will be returned
-               but "endpoint-a" will not be.
-            -  "metadata.owner!=sd AND metadata.foo=bar" returns
-               Endpoints that have "owner" in label key but value is not
-               "sd" AND have key/value foo=bar.
-            -  "doesnotexist.foo=bar" returns an empty list. Note that
-               Endpoint doesn't have a field called "doesnotexist".
-               Since the filter does not match any Endpoints, it returns
-               no results.
+            -  ``annotations.owner`` returns endpoints that have a
+               annotation with the key ``owner``, this is the same as
+               ``annotations:owner``
+            -  ``annotations.protocol=gRPC`` returns endpoints that have
+               key/value ``protocol=gRPC``
+            -  ``address=192.108.1.105`` returns endpoints that have
+               this address
+            -  ``port>8080`` returns endpoints that have port number
+               larger than 8080
+            -
+
+            ``name>projects/my-project/locations/us-east1/namespaces/my-namespace/services/my-service/endpoints/endpoint-c``
+            returns endpoints that have name that is alphabetically
+            later than the string, so "endpoint-e" is returned but
+            "endpoint-a" is not
+
+            -  ``annotations.owner!=sd AND annotations.foo=bar`` returns
+               endpoints that have ``owner`` in annotation key but value
+               is not ``sd`` AND have key/value ``foo=bar``
+            -  ``doesnotexist.foo=bar`` returns an empty list. Note that
+               endpoint doesn't have a field called "doesnotexist".
+               Since the filter does not match any endpoints, it returns
+               no results
+
+            For more information about filtering, see `API
+            Filtering <https://aip.dev/160>`__.
         order_by (str):
-            Optional. The order to list result by.
+            Optional. The order to list results by.
+
+            General ``order_by`` string syntax:
+            ``<field> (<asc|desc>) (,)``
+
+            -  ``<field>`` allows values: ``name``, ``address``,
+               ``port``
+            -  ``<asc|desc>`` ascending or descending order by
+               ``<field>``. If this is left blank, ``asc`` is used
+
+            Note that an empty ``order_by`` string results in default
+            order, which is order by ``name`` in ascending order.
     """
 
     parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
     page_size: int = proto.Field(
```

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/types/service.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/types/endpoint.py`

 * *Files 22% similar despite different names*

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
@@ -15,76 +15,104 @@
 #
 from __future__ import annotations
 
 from typing import MutableMapping, MutableSequence
 
 import proto  # type: ignore
 
-from google.cloud.servicedirectory_v1.types import endpoint
-
 __protobuf__ = proto.module(
     package="google.cloud.servicedirectory.v1",
     manifest={
-        "Service",
+        "Endpoint",
     },
 )
 
 
-class Service(proto.Message):
-    r"""An individual service. A service contains a name and optional
-    metadata. A service must exist before
-    [endpoints][google.cloud.servicedirectory.v1.Endpoint] can be added
-    to it.
+class Endpoint(proto.Message):
+    r"""An individual endpoint that provides a
+    [service][google.cloud.servicedirectory.v1.Service]. The service
+    must already exist to create an endpoint.
 
     Attributes:
         name (str):
-            Immutable. The resource name for the service in the format
-            ``projects/*/locations/*/namespaces/*/services/*``.
+            Immutable. The resource name for the endpoint in the format
+            ``projects/*/locations/*/namespaces/*/services/*/endpoints/*``.
+        address (str):
+            Optional. An IPv4 or IPv6 address. Service Directory rejects
+            bad addresses like:
+
+            -  ``8.8.8``
+            -  ``8.8.8.8:53``
+            -  ``test:bad:address``
+            -  ``[::1]``
+            -  ``[::1]:8080``
+
+            Limited to 45 characters.
+        port (int):
+            Optional. Service Directory rejects values outside of
+            ``[0, 65535]``.
         annotations (MutableMapping[str, str]):
-            Optional. Annotations for the service. This data can be
-            consumed by service clients. Restrictions:
+            Optional. Annotations for the endpoint. This data can be
+            consumed by service clients.
+
+            Restrictions:
 
-            -  The entire annotations dictionary may contain up to 2000
+            -  The entire annotations dictionary may contain up to 512
                characters, spread accoss all key-value pairs.
-               Annotations that goes beyond any these limits will be
-               rejected.
+               Annotations that go beyond this limit are rejected
             -  Valid annotation keys have two segments: an optional
                prefix and name, separated by a slash (/). The name
                segment is required and must be 63 characters or less,
                beginning and ending with an alphanumeric character
                ([a-z0-9A-Z]) with dashes (-), underscores (_), dots (.),
                and alphanumerics between. The prefix is optional. If
                specified, the prefix must be a DNS subdomain: a series
                of DNS labels separated by dots (.), not longer than 253
-               characters in total, followed by a slash (/). Annotations
-               that fails to meet these requirements will be rejected.
-            -  The '(*.)google.com/' and '(*.)googleapis.com/' prefixes
-               are reserved for system annotations managed by Service
-               Directory. If the user tries to write to these keyspaces,
-               those entries will be silently ignored by the system.
-               Note: This field is equivalent to the 'metadata' field in
-               the v1beta1 API. They have the same syntax and read/write
-               to the same location in Service Directory.
-        endpoints (MutableSequence[google.cloud.servicedirectory_v1.types.Endpoint]):
-            Output only. Endpoints associated with this
-            service. Returned on LookupService.Resolve.
-            Control plane clients should use
-            RegistrationService.ListEndpoints.
+               characters in total, followed by a slash (/) Annotations
+               that fails to meet these requirements are rejected.
+
+            Note: This field is equivalent to the ``metadata`` field in
+            the v1beta1 API. They have the same syntax and read/write to
+            the same location in Service Directory.
+        network (str):
+            Immutable. The Google Compute Engine network (VPC) of the
+            endpoint in the format
+            ``projects/<project number>/locations/global/networks/*``.
+
+            The project must be specified by project number (project id
+            is rejected). Incorrectly formatted networks are rejected,
+            we also check to make sure that you have the
+            servicedirectory.networks.attach permission on the project
+            specified.
+        uid (str):
+            Output only. The globally unique identifier
+            of the endpoint in the UUID4 format.
     """
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
+    address: str = proto.Field(
+        proto.STRING,
+        number=2,
+    )
+    port: int = proto.Field(
+        proto.INT32,
+        number=3,
+    )
     annotations: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
-        number=4,
+        number=5,
     )
-    endpoints: MutableSequence[endpoint.Endpoint] = proto.RepeatedField(
-        proto.MESSAGE,
-        number=3,
-        message=endpoint.Endpoint,
+    network: str = proto.Field(
+        proto.STRING,
+        number=8,
+    )
+    uid: str = proto.Field(
+        proto.STRING,
+        number=9,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/__init__.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/__init__.py`

 * *Files 4% similar despite different names*

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

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/gapic_metadata.json` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/gapic_version.py` & `google-cloud-service-directory-1.9.0/tests/unit/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,15 @@
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
-__version__ = "1.8.2"  # {x-release-please-version}
```

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/__init__.py` & `google-cloud-service-directory-1.9.0/tests/unit/gapic/__init__.py`

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

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/__init__.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/lookup_service/__init__.py`

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

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/async_client.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/lookup_service/async_client.py`

 * *Files 26% similar despite different names*

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
@@ -38,14 +38,16 @@
 from google.cloud.servicedirectory_v1beta1 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
+from google.cloud.location import locations_pb2  # type: ignore
+
 from google.cloud.servicedirectory_v1beta1.types import lookup_service, service
 
 from .client import LookupServiceClient
 from .transports.base import DEFAULT_CLIENT_INFO, LookupServiceTransport
 from .transports.grpc_asyncio import LookupServiceGrpcAsyncIOTransport
 
 
@@ -267,15 +269,15 @@
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.servicedirectory_v1beta1.types.ResolveServiceResponse:
                 The response message for
-                [LookupService.ResolveService][google.cloud.servicedirectory.v1beta1.LookupService.ResolveService].
+                   [LookupService.ResolveService][google.cloud.servicedirectory.v1beta1.LookupService.ResolveService].
 
         """
         # Create or coerce a protobuf request object.
         request = lookup_service.ResolveServiceRequest(request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
@@ -284,14 +286,122 @@
             default_timeout=None,
             client_info=DEFAULT_CLIENT_INFO,
         )
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    async def get_location(
+        self,
+        request: Optional[locations_pb2.GetLocationRequest] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> locations_pb2.Location:
+        r"""Gets information about a location.
+
+        Args:
+            request (:class:`~.location_pb2.GetLocationRequest`):
+                The request object. Request message for
+                `GetLocation` method.
+            retry (google.api_core.retry.Retry): Designation of what errors,
+                 if any, should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            ~.location_pb2.Location:
+                Location object.
+        """
+        # Create or coerce a protobuf request object.
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = locations_pb2.GetLocationRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._client._transport.get_location,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    async def list_locations(
+        self,
+        request: Optional[locations_pb2.ListLocationsRequest] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> locations_pb2.ListLocationsResponse:
+        r"""Lists information about the supported locations for this service.
+
+        Args:
+            request (:class:`~.location_pb2.ListLocationsRequest`):
+                The request object. Request message for
+                `ListLocations` method.
+            retry (google.api_core.retry.Retry): Designation of what errors,
+                 if any, should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            ~.location_pb2.ListLocationsResponse:
+                Response message for ``ListLocations`` method.
+        """
+        # Create or coerce a protobuf request object.
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = locations_pb2.ListLocationsRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._client._transport.list_locations,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
         response = await rpc(
             request,
             retry=retry,
```

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/client.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/lookup_service/client.py`

 * *Files 3% similar despite different names*

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
@@ -42,14 +42,16 @@
 from google.cloud.servicedirectory_v1beta1 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
+from google.cloud.location import locations_pb2  # type: ignore
+
 from google.cloud.servicedirectory_v1beta1.types import lookup_service, service
 
 from .transports.base import DEFAULT_CLIENT_INFO, LookupServiceTransport
 from .transports.grpc import LookupServiceGrpcTransport
 from .transports.grpc_asyncio import LookupServiceGrpcAsyncIOTransport
 from .transports.rest import LookupServiceRestTransport
 
@@ -538,15 +540,15 @@
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.servicedirectory_v1beta1.types.ResolveServiceResponse:
                 The response message for
-                [LookupService.ResolveService][google.cloud.servicedirectory.v1beta1.LookupService.ResolveService].
+                   [LookupService.ResolveService][google.cloud.servicedirectory.v1beta1.LookupService.ResolveService].
 
         """
         # Create or coerce a protobuf request object.
         # Minor optimization to avoid making a copy if the user passes
         # in a lookup_service.ResolveServiceRequest.
         # There's no risk of modifying the input as we've already verified
         # there are no flattened fields.
@@ -583,14 +585,122 @@
         .. warning::
             ONLY use as a context manager if the transport is NOT shared
             with other clients! Exiting the with block will CLOSE the transport
             and may cause errors in other clients!
         """
         self.transport.close()
 
+    def get_location(
+        self,
+        request: Optional[locations_pb2.GetLocationRequest] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> locations_pb2.Location:
+        r"""Gets information about a location.
+
+        Args:
+            request (:class:`~.location_pb2.GetLocationRequest`):
+                The request object. Request message for
+                `GetLocation` method.
+            retry (google.api_core.retry.Retry): Designation of what errors,
+                 if any, should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            ~.location_pb2.Location:
+                Location object.
+        """
+        # Create or coerce a protobuf request object.
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = locations_pb2.GetLocationRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._transport.get_location,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    def list_locations(
+        self,
+        request: Optional[locations_pb2.ListLocationsRequest] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> locations_pb2.ListLocationsResponse:
+        r"""Lists information about the supported locations for this service.
+
+        Args:
+            request (:class:`~.location_pb2.ListLocationsRequest`):
+                The request object. Request message for
+                `ListLocations` method.
+            retry (google.api_core.retry.Retry): Designation of what errors,
+                 if any, should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            ~.location_pb2.ListLocationsResponse:
+                Response message for ``ListLocations`` method.
+        """
+        # Create or coerce a protobuf request object.
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = locations_pb2.ListLocationsRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._transport.list_locations,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
     gapic_version=package_version.__version__
 )
 
 
 __all__ = ("LookupServiceClient",)
```

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/__init__.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/__init__.py`

 * *Files 5% similar despite different names*

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

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/base.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/base.py`

 * *Files 9% similar despite different names*

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
@@ -18,14 +18,15 @@
 
 import google.api_core
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
+from google.cloud.location import locations_pb2  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
 from google.cloud.servicedirectory_v1beta1 import gapic_version as package_version
 from google.cloud.servicedirectory_v1beta1.types import lookup_service
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
     gapic_version=package_version.__version__
@@ -147,12 +148,33 @@
             lookup_service.ResolveServiceResponse,
             Awaitable[lookup_service.ResolveServiceResponse],
         ],
     ]:
         raise NotImplementedError()
 
     @property
+    def get_location(
+        self,
+    ) -> Callable[
+        [locations_pb2.GetLocationRequest],
+        Union[locations_pb2.Location, Awaitable[locations_pb2.Location]],
+    ]:
+        raise NotImplementedError()
+
+    @property
+    def list_locations(
+        self,
+    ) -> Callable[
+        [locations_pb2.ListLocationsRequest],
+        Union[
+            locations_pb2.ListLocationsResponse,
+            Awaitable[locations_pb2.ListLocationsResponse],
+        ],
+    ]:
+        raise NotImplementedError()
+
+    @property
     def kind(self) -> str:
         raise NotImplementedError()
 
 
 __all__ = ("LookupServiceTransport",)
```

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/grpc.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/grpc_asyncio.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,59 +1,105 @@
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
-from typing import Callable, Dict, Optional, Sequence, Tuple, Union
+from typing import Awaitable, Callable, Dict, Optional, Sequence, Tuple, Union
 import warnings
 
-from google.api_core import gapic_v1, grpc_helpers
-import google.auth  # type: ignore
+from google.api_core import gapic_v1, grpc_helpers_async
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
+from google.cloud.location import locations_pb2  # type: ignore
 import grpc  # type: ignore
+from grpc.experimental import aio  # type: ignore
 
 from google.cloud.servicedirectory_v1beta1.types import lookup_service
 
 from .base import DEFAULT_CLIENT_INFO, LookupServiceTransport
+from .grpc import LookupServiceGrpcTransport
 
 
-class LookupServiceGrpcTransport(LookupServiceTransport):
-    """gRPC backend transport for LookupService.
+class LookupServiceGrpcAsyncIOTransport(LookupServiceTransport):
+    """gRPC AsyncIO backend transport for LookupService.
 
     Service Directory API for looking up service data at runtime.
 
     This class defines the same methods as the primary client, so the
     primary client can load the underlying transport implementation
     and call it.
 
     It sends protocol buffers over the wire using gRPC (which is built on
     top of HTTP/2); the ``grpcio`` package must be installed.
     """
 
-    _stubs: Dict[str, Callable]
+    _grpc_channel: aio.Channel
+    _stubs: Dict[str, Callable] = {}
+
+    @classmethod
+    def create_channel(
+        cls,
+        host: str = "servicedirectory.googleapis.com",
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
+        scopes: Optional[Sequence[str]] = None,
+        quota_project_id: Optional[str] = None,
+        **kwargs,
+    ) -> aio.Channel:
+        """Create and return a gRPC AsyncIO channel object.
+        Args:
+            host (Optional[str]): The host for the channel to use.
+            credentials (Optional[~.Credentials]): The
+                authorization credentials to attach to requests. These
+                credentials identify this application to the service. If
+                none are specified, the client will attempt to ascertain
+                the credentials from the environment.
+            credentials_file (Optional[str]): A file with credentials that can
+                be loaded with :func:`google.auth.load_credentials_from_file`.
+                This argument is ignored if ``channel`` is provided.
+            scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
+                service. These are only used when credentials are not specified and
+                are passed to :func:`google.auth.default`.
+            quota_project_id (Optional[str]): An optional project to use for billing
+                and quota.
+            kwargs (Optional[dict]): Keyword arguments, which are passed to the
+                channel creation.
+        Returns:
+            aio.Channel: A gRPC AsyncIO channel object.
+        """
+
+        return grpc_helpers_async.create_channel(
+            host,
+            credentials=credentials,
+            credentials_file=credentials_file,
+            quota_project_id=quota_project_id,
+            default_scopes=cls.AUTH_SCOPES,
+            scopes=scopes,
+            default_host=cls.DEFAULT_HOST,
+            **kwargs,
+        )
 
     def __init__(
         self,
         *,
         host: str = "servicedirectory.googleapis.com",
         credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
-        channel: Optional[grpc.Channel] = None,
+        channel: Optional[aio.Channel] = None,
         api_mtls_endpoint: Optional[str] = None,
         client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
         client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
@@ -69,17 +115,18 @@
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
                 This argument is ignored if ``channel`` is provided.
             credentials_file (Optional[str]): A file with credentials that can
                 be loaded with :func:`google.auth.load_credentials_from_file`.
                 This argument is ignored if ``channel`` is provided.
-            scopes (Optional(Sequence[str])): A list of scopes. This argument is
-                ignored if ``channel`` is provided.
-            channel (Optional[grpc.Channel]): A ``Channel`` instance through
+            scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
+                service. These are only used when credentials are not specified and
+                are passed to :func:`google.auth.default`.
+            channel (Optional[aio.Channel]): A ``Channel`` instance through
                 which to make calls.
             api_mtls_endpoint (Optional[str]): Deprecated. The mutual TLS endpoint.
                 If provided, it overrides the ``host`` argument and tries to create
                 a mutual TLS channel with client SSL credentials from
                 ``client_cert_source`` or application default SSL credentials.
             client_cert_source (Optional[Callable[[], Tuple[bytes, bytes]]]):
                 Deprecated. A callback to provide client SSL certificate bytes and
@@ -98,15 +145,15 @@
                 API requests. If ``None``, then default info will be used.
                 Generally, you only need to set this if you're developing
                 your own client library.
             always_use_jwt_access (Optional[bool]): Whether self signed JWT should
                 be used for service account credentials.
 
         Raises:
-          google.auth.exceptions.MutualTLSChannelError: If mutual TLS transport
+            google.auth.exceptions.MutualTlsChannelError: If mutual TLS transport
               creation failed for any reason.
           google.api_core.exceptions.DuplicateCredentialArgs: If both ``credentials``
               and ``credentials_file`` are passed.
         """
         self._grpc_channel = None
         self._ssl_channel_credentials = ssl_channel_credentials
         self._stubs: Dict[str, Callable] = {}
@@ -118,15 +165,14 @@
 
         if channel:
             # Ignore credentials if a channel was passed.
             credentials = False
             # If a channel was explicitly provided, set it.
             self._grpc_channel = channel
             self._ssl_channel_credentials = None
-
         else:
             if api_mtls_endpoint:
                 host = api_mtls_endpoint
 
                 # Create SSL credentials with client_cert_source or application
                 # default SSL credentials.
                 if client_cert_source:
@@ -172,82 +218,41 @@
                     ("grpc.max_receive_message_length", -1),
                 ],
             )
 
         # Wrap messages. This must be done after self._grpc_channel exists
         self._prep_wrapped_messages(client_info)
 
-    @classmethod
-    def create_channel(
-        cls,
-        host: str = "servicedirectory.googleapis.com",
-        credentials: Optional[ga_credentials.Credentials] = None,
-        credentials_file: Optional[str] = None,
-        scopes: Optional[Sequence[str]] = None,
-        quota_project_id: Optional[str] = None,
-        **kwargs,
-    ) -> grpc.Channel:
-        """Create and return a gRPC channel object.
-        Args:
-            host (Optional[str]): The host for the channel to use.
-            credentials (Optional[~.Credentials]): The
-                authorization credentials to attach to requests. These
-                credentials identify this application to the service. If
-                none are specified, the client will attempt to ascertain
-                the credentials from the environment.
-            credentials_file (Optional[str]): A file with credentials that can
-                be loaded with :func:`google.auth.load_credentials_from_file`.
-                This argument is mutually exclusive with credentials.
-            scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
-                service. These are only used when credentials are not specified and
-                are passed to :func:`google.auth.default`.
-            quota_project_id (Optional[str]): An optional project to use for billing
-                and quota.
-            kwargs (Optional[dict]): Keyword arguments, which are passed to the
-                channel creation.
-        Returns:
-            grpc.Channel: A gRPC channel object.
+    @property
+    def grpc_channel(self) -> aio.Channel:
+        """Create the channel designed to connect to this service.
 
-        Raises:
-            google.api_core.exceptions.DuplicateCredentialArgs: If both ``credentials``
-              and ``credentials_file`` are passed.
+        This property caches on the instance; repeated calls return
+        the same channel.
         """
-
-        return grpc_helpers.create_channel(
-            host,
-            credentials=credentials,
-            credentials_file=credentials_file,
-            quota_project_id=quota_project_id,
-            default_scopes=cls.AUTH_SCOPES,
-            scopes=scopes,
-            default_host=cls.DEFAULT_HOST,
-            **kwargs,
-        )
-
-    @property
-    def grpc_channel(self) -> grpc.Channel:
-        """Return the channel designed to connect to this service."""
+        # Return the channel from cache.
         return self._grpc_channel
 
     @property
     def resolve_service(
         self,
     ) -> Callable[
-        [lookup_service.ResolveServiceRequest], lookup_service.ResolveServiceResponse
+        [lookup_service.ResolveServiceRequest],
+        Awaitable[lookup_service.ResolveServiceResponse],
     ]:
         r"""Return a callable for the resolve service method over gRPC.
 
         Returns a
         [service][google.cloud.servicedirectory.v1beta1.Service] and its
         associated endpoints. Resolving a service is not considered an
         active developer method.
 
         Returns:
             Callable[[~.ResolveServiceRequest],
-                    ~.ResolveServiceResponse]:
+                    Awaitable[~.ResolveServiceResponse]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -256,15 +261,47 @@
                 "/google.cloud.servicedirectory.v1beta1.LookupService/ResolveService",
                 request_serializer=lookup_service.ResolveServiceRequest.serialize,
                 response_deserializer=lookup_service.ResolveServiceResponse.deserialize,
             )
         return self._stubs["resolve_service"]
 
     def close(self):
-        self.grpc_channel.close()
+        return self.grpc_channel.close()
 
     @property
-    def kind(self) -> str:
-        return "grpc"
+    def list_locations(
+        self,
+    ) -> Callable[
+        [locations_pb2.ListLocationsRequest], locations_pb2.ListLocationsResponse
+    ]:
+        r"""Return a callable for the list locations method over gRPC."""
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "list_locations" not in self._stubs:
+            self._stubs["list_locations"] = self.grpc_channel.unary_unary(
+                "/google.cloud.location.Locations/ListLocations",
+                request_serializer=locations_pb2.ListLocationsRequest.SerializeToString,
+                response_deserializer=locations_pb2.ListLocationsResponse.FromString,
+            )
+        return self._stubs["list_locations"]
+
+    @property
+    def get_location(
+        self,
+    ) -> Callable[[locations_pb2.GetLocationRequest], locations_pb2.Location]:
+        r"""Return a callable for the list locations method over gRPC."""
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "get_location" not in self._stubs:
+            self._stubs["get_location"] = self.grpc_channel.unary_unary(
+                "/google.cloud.location.Locations/GetLocation",
+                request_serializer=locations_pb2.GetLocationRequest.SerializeToString,
+                response_deserializer=locations_pb2.Location.FromString,
+            )
+        return self._stubs["get_location"]
 
 
-__all__ = ("LookupServiceGrpcTransport",)
+__all__ = ("LookupServiceGrpcAsyncIOTransport",)
```

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/grpc_asyncio.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/lookup_service/transports/grpc_asyncio.py`

 * *Files 14% similar despite different names*

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
@@ -15,18 +15,19 @@
 #
 from typing import Awaitable, Callable, Dict, Optional, Sequence, Tuple, Union
 import warnings
 
 from google.api_core import gapic_v1, grpc_helpers_async
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
+from google.cloud.location import locations_pb2  # type: ignore
 import grpc  # type: ignore
 from grpc.experimental import aio  # type: ignore
 
-from google.cloud.servicedirectory_v1beta1.types import lookup_service
+from google.cloud.servicedirectory_v1.types import lookup_service
 
 from .base import DEFAULT_CLIENT_INFO, LookupServiceTransport
 from .grpc import LookupServiceGrpcTransport
 
 
 class LookupServiceGrpcAsyncIOTransport(LookupServiceTransport):
     """gRPC AsyncIO backend transport for LookupService.
@@ -236,35 +237,70 @@
         self,
     ) -> Callable[
         [lookup_service.ResolveServiceRequest],
         Awaitable[lookup_service.ResolveServiceResponse],
     ]:
         r"""Return a callable for the resolve service method over gRPC.
 
-        Returns a
-        [service][google.cloud.servicedirectory.v1beta1.Service] and its
-        associated endpoints. Resolving a service is not considered an
-        active developer method.
+        Returns a [service][google.cloud.servicedirectory.v1.Service]
+        and its associated endpoints. Resolving a service is not
+        considered an active developer method.
 
         Returns:
             Callable[[~.ResolveServiceRequest],
                     Awaitable[~.ResolveServiceResponse]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "resolve_service" not in self._stubs:
             self._stubs["resolve_service"] = self.grpc_channel.unary_unary(
-                "/google.cloud.servicedirectory.v1beta1.LookupService/ResolveService",
+                "/google.cloud.servicedirectory.v1.LookupService/ResolveService",
                 request_serializer=lookup_service.ResolveServiceRequest.serialize,
                 response_deserializer=lookup_service.ResolveServiceResponse.deserialize,
             )
         return self._stubs["resolve_service"]
 
     def close(self):
         return self.grpc_channel.close()
 
+    @property
+    def list_locations(
+        self,
+    ) -> Callable[
+        [locations_pb2.ListLocationsRequest], locations_pb2.ListLocationsResponse
+    ]:
+        r"""Return a callable for the list locations method over gRPC."""
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "list_locations" not in self._stubs:
+            self._stubs["list_locations"] = self.grpc_channel.unary_unary(
+                "/google.cloud.location.Locations/ListLocations",
+                request_serializer=locations_pb2.ListLocationsRequest.SerializeToString,
+                response_deserializer=locations_pb2.ListLocationsResponse.FromString,
+            )
+        return self._stubs["list_locations"]
+
+    @property
+    def get_location(
+        self,
+    ) -> Callable[[locations_pb2.GetLocationRequest], locations_pb2.Location]:
+        r"""Return a callable for the list locations method over gRPC."""
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "get_location" not in self._stubs:
+            self._stubs["get_location"] = self.grpc_channel.unary_unary(
+                "/google.cloud.location.Locations/GetLocation",
+                request_serializer=locations_pb2.GetLocationRequest.SerializeToString,
+                response_deserializer=locations_pb2.Location.FromString,
+            )
+        return self._stubs["get_location"]
+
 
 __all__ = ("LookupServiceGrpcAsyncIOTransport",)
```

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/rest.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/rest.py`

 * *Files 24% similar despite different names*

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
@@ -22,14 +22,15 @@
 
 from google.api_core import gapic_v1, path_template, rest_helpers, rest_streaming
 from google.api_core import exceptions as core_exceptions
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.auth.transport.requests import AuthorizedSession  # type: ignore
+from google.cloud.location import locations_pb2  # type: ignore
 from google.protobuf import json_format
 import grpc  # type: ignore
 from requests import __version__ as requests_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
@@ -96,14 +97,60 @@
 
         Override in a subclass to manipulate the response
         after it is returned by the LookupService server but before
         it is returned to user code.
         """
         return response
 
+    def pre_get_location(
+        self,
+        request: locations_pb2.GetLocationRequest,
+        metadata: Sequence[Tuple[str, str]],
+    ) -> Tuple[locations_pb2.GetLocationRequest, Sequence[Tuple[str, str]]]:
+        """Pre-rpc interceptor for get_location
+
+        Override in a subclass to manipulate the request or metadata
+        before they are sent to the LookupService server.
+        """
+        return request, metadata
+
+    def post_get_location(
+        self, response: locations_pb2.Location
+    ) -> locations_pb2.Location:
+        """Post-rpc interceptor for get_location
+
+        Override in a subclass to manipulate the response
+        after it is returned by the LookupService server but before
+        it is returned to user code.
+        """
+        return response
+
+    def pre_list_locations(
+        self,
+        request: locations_pb2.ListLocationsRequest,
+        metadata: Sequence[Tuple[str, str]],
+    ) -> Tuple[locations_pb2.ListLocationsRequest, Sequence[Tuple[str, str]]]:
+        """Pre-rpc interceptor for list_locations
+
+        Override in a subclass to manipulate the request or metadata
+        before they are sent to the LookupService server.
+        """
+        return request, metadata
+
+    def post_list_locations(
+        self, response: locations_pb2.ListLocationsResponse
+    ) -> locations_pb2.ListLocationsResponse:
+        """Post-rpc interceptor for list_locations
+
+        Override in a subclass to manipulate the response
+        after it is returned by the LookupService server but before
+        it is returned to user code.
+        """
+        return response
+
 
 @dataclasses.dataclass
 class LookupServiceRestStub:
     _session: AuthorizedSession
     _host: str
     _interceptor: LookupServiceRestInterceptor
 
@@ -304,14 +351,148 @@
         [lookup_service.ResolveServiceRequest], lookup_service.ResolveServiceResponse
     ]:
         # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
         # In C++ this would require a dynamic_cast
         return self._ResolveService(self._session, self._host, self._interceptor)  # type: ignore
 
     @property
+    def get_location(self):
+        return self._GetLocation(self._session, self._host, self._interceptor)  # type: ignore
+
+    class _GetLocation(LookupServiceRestStub):
+        def __call__(
+            self,
+            request: locations_pb2.GetLocationRequest,
+            *,
+            retry: OptionalRetry = gapic_v1.method.DEFAULT,
+            timeout: Optional[float] = None,
+            metadata: Sequence[Tuple[str, str]] = (),
+        ) -> locations_pb2.Location:
+
+            r"""Call the get location method over HTTP.
+
+            Args:
+                request (locations_pb2.GetLocationRequest):
+                    The request object for GetLocation method.
+                retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                    should be retried.
+                timeout (float): The timeout for this request.
+                metadata (Sequence[Tuple[str, str]]): Strings which should be
+                    sent along with the request as metadata.
+
+            Returns:
+                locations_pb2.Location: Response from GetLocation method.
+            """
+
+            http_options: List[Dict[str, str]] = [
+                {
+                    "method": "get",
+                    "uri": "/v1beta1/{name=projects/*/locations/*}",
+                },
+            ]
+
+            request, metadata = self._interceptor.pre_get_location(request, metadata)
+            request_kwargs = json_format.MessageToDict(request)
+            transcoded_request = path_template.transcode(http_options, **request_kwargs)
+
+            uri = transcoded_request["uri"]
+            method = transcoded_request["method"]
+
+            # Jsonify the query params
+            query_params = json.loads(json.dumps(transcoded_request["query_params"]))
+
+            # Send the request
+            headers = dict(metadata)
+            headers["Content-Type"] = "application/json"
+
+            response = getattr(self._session, method)(
+                "{host}{uri}".format(host=self._host, uri=uri),
+                timeout=timeout,
+                headers=headers,
+                params=rest_helpers.flatten_query_params(query_params),
+            )
+
+            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
+            # subclass.
+            if response.status_code >= 400:
+                raise core_exceptions.from_http_response(response)
+
+            resp = locations_pb2.Location()
+            resp = json_format.Parse(response.content.decode("utf-8"), resp)
+            resp = self._interceptor.post_get_location(resp)
+            return resp
+
+    @property
+    def list_locations(self):
+        return self._ListLocations(self._session, self._host, self._interceptor)  # type: ignore
+
+    class _ListLocations(LookupServiceRestStub):
+        def __call__(
+            self,
+            request: locations_pb2.ListLocationsRequest,
+            *,
+            retry: OptionalRetry = gapic_v1.method.DEFAULT,
+            timeout: Optional[float] = None,
+            metadata: Sequence[Tuple[str, str]] = (),
+        ) -> locations_pb2.ListLocationsResponse:
+
+            r"""Call the list locations method over HTTP.
+
+            Args:
+                request (locations_pb2.ListLocationsRequest):
+                    The request object for ListLocations method.
+                retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                    should be retried.
+                timeout (float): The timeout for this request.
+                metadata (Sequence[Tuple[str, str]]): Strings which should be
+                    sent along with the request as metadata.
+
+            Returns:
+                locations_pb2.ListLocationsResponse: Response from ListLocations method.
+            """
+
+            http_options: List[Dict[str, str]] = [
+                {
+                    "method": "get",
+                    "uri": "/v1beta1/{name=projects/*}/locations",
+                },
+            ]
+
+            request, metadata = self._interceptor.pre_list_locations(request, metadata)
+            request_kwargs = json_format.MessageToDict(request)
+            transcoded_request = path_template.transcode(http_options, **request_kwargs)
+
+            uri = transcoded_request["uri"]
+            method = transcoded_request["method"]
+
+            # Jsonify the query params
+            query_params = json.loads(json.dumps(transcoded_request["query_params"]))
+
+            # Send the request
+            headers = dict(metadata)
+            headers["Content-Type"] = "application/json"
+
+            response = getattr(self._session, method)(
+                "{host}{uri}".format(host=self._host, uri=uri),
+                timeout=timeout,
+                headers=headers,
+                params=rest_helpers.flatten_query_params(query_params),
+            )
+
+            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
+            # subclass.
+            if response.status_code >= 400:
+                raise core_exceptions.from_http_response(response)
+
+            resp = locations_pb2.ListLocationsResponse()
+            resp = json_format.Parse(response.content.decode("utf-8"), resp)
+            resp = self._interceptor.post_list_locations(resp)
+            return resp
+
+    @property
     def kind(self) -> str:
         return "rest"
 
     def close(self):
         self._session.close()
```

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/registration_service/__init__.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/registration_service/__init__.py`

 * *Files 11% similar despite different names*

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

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/registration_service/async_client.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/registration_service/async_client.py`

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
@@ -38,14 +38,15 @@
 from google.cloud.servicedirectory_v1beta1 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
+from google.cloud.location import locations_pb2  # type: ignore
 from google.iam.v1 import iam_policy_pb2  # type: ignore
 from google.iam.v1 import policy_pb2  # type: ignore
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 
 from google.cloud.servicedirectory_v1beta1.services.registration_service import pagers
 from google.cloud.servicedirectory_v1beta1.types import endpoint as gcs_endpoint
@@ -439,15 +440,15 @@
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.servicedirectory_v1beta1.services.registration_service.pagers.ListNamespacesAsyncPager:
                 The response message for
-                [RegistrationService.ListNamespaces][google.cloud.servicedirectory.v1beta1.RegistrationService.ListNamespaces].
+                   [RegistrationService.ListNamespaces][google.cloud.servicedirectory.v1beta1.RegistrationService.ListNamespaces].
 
                 Iterating over this object will yield results and
                 resolve additional pages automatically.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
@@ -1000,15 +1001,15 @@
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.servicedirectory_v1beta1.services.registration_service.pagers.ListServicesAsyncPager:
                 The response message for
-                [RegistrationService.ListServices][google.cloud.servicedirectory.v1beta1.RegistrationService.ListServices].
+                   [RegistrationService.ListServices][google.cloud.servicedirectory.v1beta1.RegistrationService.ListServices].
 
                 Iterating over this object will yield results and
                 resolve additional pages automatically.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
@@ -1099,15 +1100,15 @@
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.servicedirectory_v1beta1.types.GetServiceRequest, dict]]):
                 The request object. The request message for
                 [RegistrationService.GetService][google.cloud.servicedirectory.v1beta1.RegistrationService.GetService].
                 This should not be used for looking up a service.
-                Insead, use the ``resolve`` method as it contains all
+                Instead, use the ``resolve`` method as it contains all
                 endpoints and associated metadata.
             name (:class:`str`):
                 Required. The name of the service to
                 get.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
@@ -1565,15 +1566,15 @@
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.servicedirectory_v1beta1.services.registration_service.pagers.ListEndpointsAsyncPager:
                 The response message for
-                [RegistrationService.ListEndpoints][google.cloud.servicedirectory.v1beta1.RegistrationService.ListEndpoints].
+                   [RegistrationService.ListEndpoints][google.cloud.servicedirectory.v1beta1.RegistrationService.ListEndpoints].
 
                 Iterating over this object will yield results and
                 resolve additional pages automatically.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
@@ -1941,16 +1942,15 @@
         self,
         request: Optional[Union[iam_policy_pb2.GetIamPolicyRequest, dict]] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> policy_pb2.Policy:
-        r"""Gets the IAM Policy for a resource (namespace or
-        service only).
+        r"""Gets the IAM Policy for a resource
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -2084,16 +2084,15 @@
         self,
         request: Optional[Union[iam_policy_pb2.SetIamPolicyRequest, dict]] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> policy_pb2.Policy:
-        r"""Sets the IAM Policy for a resource (namespace or
-        service only).
+        r"""Sets the IAM Policy for a resource
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -2227,16 +2226,16 @@
         self,
         request: Optional[Union[iam_policy_pb2.TestIamPermissionsRequest, dict]] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> iam_policy_pb2.TestIamPermissionsResponse:
-        r"""Tests IAM permissions for a resource (namespace or
-        service only).
+        r"""Tests IAM permissions for a resource (namespace,
+        service  or service workload only).
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -2296,14 +2295,122 @@
         )
 
         # Send the request.
         response = await rpc(
             request,
             retry=retry,
             timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    async def get_location(
+        self,
+        request: Optional[locations_pb2.GetLocationRequest] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> locations_pb2.Location:
+        r"""Gets information about a location.
+
+        Args:
+            request (:class:`~.location_pb2.GetLocationRequest`):
+                The request object. Request message for
+                `GetLocation` method.
+            retry (google.api_core.retry.Retry): Designation of what errors,
+                 if any, should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            ~.location_pb2.Location:
+                Location object.
+        """
+        # Create or coerce a protobuf request object.
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = locations_pb2.GetLocationRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._client._transport.get_location,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    async def list_locations(
+        self,
+        request: Optional[locations_pb2.ListLocationsRequest] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> locations_pb2.ListLocationsResponse:
+        r"""Lists information about the supported locations for this service.
+
+        Args:
+            request (:class:`~.location_pb2.ListLocationsRequest`):
+                The request object. Request message for
+                `ListLocations` method.
+            retry (google.api_core.retry.Retry): Designation of what errors,
+                 if any, should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            ~.location_pb2.ListLocationsResponse:
+                Response message for ``ListLocations`` method.
+        """
+        # Create or coerce a protobuf request object.
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = locations_pb2.ListLocationsRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._client._transport.list_locations,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
     async def __aenter__(self) -> "RegistrationServiceAsyncClient":
```

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/registration_service/client.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/registration_service/client.py`

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
@@ -42,14 +42,15 @@
 from google.cloud.servicedirectory_v1beta1 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
+from google.cloud.location import locations_pb2  # type: ignore
 from google.iam.v1 import iam_policy_pb2  # type: ignore
 from google.iam.v1 import policy_pb2  # type: ignore
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 
 from google.cloud.servicedirectory_v1beta1.services.registration_service import pagers
 from google.cloud.servicedirectory_v1beta1.types import endpoint as gcs_endpoint
@@ -731,15 +732,15 @@
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.servicedirectory_v1beta1.services.registration_service.pagers.ListNamespacesPager:
                 The response message for
-                [RegistrationService.ListNamespaces][google.cloud.servicedirectory.v1beta1.RegistrationService.ListNamespaces].
+                   [RegistrationService.ListNamespaces][google.cloud.servicedirectory.v1beta1.RegistrationService.ListNamespaces].
 
                 Iterating over this object will yield results and
                 resolve additional pages automatically.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
@@ -1292,15 +1293,15 @@
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.servicedirectory_v1beta1.services.registration_service.pagers.ListServicesPager:
                 The response message for
-                [RegistrationService.ListServices][google.cloud.servicedirectory.v1beta1.RegistrationService.ListServices].
+                   [RegistrationService.ListServices][google.cloud.servicedirectory.v1beta1.RegistrationService.ListServices].
 
                 Iterating over this object will yield results and
                 resolve additional pages automatically.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
@@ -1391,15 +1392,15 @@
                 print(response)
 
         Args:
             request (Union[google.cloud.servicedirectory_v1beta1.types.GetServiceRequest, dict]):
                 The request object. The request message for
                 [RegistrationService.GetService][google.cloud.servicedirectory.v1beta1.RegistrationService.GetService].
                 This should not be used for looking up a service.
-                Insead, use the ``resolve`` method as it contains all
+                Instead, use the ``resolve`` method as it contains all
                 endpoints and associated metadata.
             name (str):
                 Required. The name of the service to
                 get.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
@@ -1857,15 +1858,15 @@
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.servicedirectory_v1beta1.services.registration_service.pagers.ListEndpointsPager:
                 The response message for
-                [RegistrationService.ListEndpoints][google.cloud.servicedirectory.v1beta1.RegistrationService.ListEndpoints].
+                   [RegistrationService.ListEndpoints][google.cloud.servicedirectory.v1beta1.RegistrationService.ListEndpoints].
 
                 Iterating over this object will yield results and
                 resolve additional pages automatically.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
@@ -2233,16 +2234,15 @@
         self,
         request: Optional[Union[iam_policy_pb2.GetIamPolicyRequest, dict]] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> policy_pb2.Policy:
-        r"""Gets the IAM Policy for a resource (namespace or
-        service only).
+        r"""Gets the IAM Policy for a resource
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -2375,16 +2375,15 @@
         self,
         request: Optional[Union[iam_policy_pb2.SetIamPolicyRequest, dict]] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> policy_pb2.Policy:
-        r"""Sets the IAM Policy for a resource (namespace or
-        service only).
+        r"""Sets the IAM Policy for a resource
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -2517,16 +2516,16 @@
         self,
         request: Optional[Union[iam_policy_pb2.TestIamPermissionsRequest, dict]] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> iam_policy_pb2.TestIamPermissionsResponse:
-        r"""Tests IAM permissions for a resource (namespace or
-        service only).
+        r"""Tests IAM permissions for a resource (namespace,
+        service  or service workload only).
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -2604,14 +2603,122 @@
         .. warning::
             ONLY use as a context manager if the transport is NOT shared
             with other clients! Exiting the with block will CLOSE the transport
             and may cause errors in other clients!
         """
         self.transport.close()
 
+    def get_location(
+        self,
+        request: Optional[locations_pb2.GetLocationRequest] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> locations_pb2.Location:
+        r"""Gets information about a location.
+
+        Args:
+            request (:class:`~.location_pb2.GetLocationRequest`):
+                The request object. Request message for
+                `GetLocation` method.
+            retry (google.api_core.retry.Retry): Designation of what errors,
+                 if any, should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            ~.location_pb2.Location:
+                Location object.
+        """
+        # Create or coerce a protobuf request object.
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = locations_pb2.GetLocationRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._transport.get_location,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    def list_locations(
+        self,
+        request: Optional[locations_pb2.ListLocationsRequest] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> locations_pb2.ListLocationsResponse:
+        r"""Lists information about the supported locations for this service.
+
+        Args:
+            request (:class:`~.location_pb2.ListLocationsRequest`):
+                The request object. Request message for
+                `ListLocations` method.
+            retry (google.api_core.retry.Retry): Designation of what errors,
+                 if any, should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            ~.location_pb2.ListLocationsResponse:
+                Response message for ``ListLocations`` method.
+        """
+        # Create or coerce a protobuf request object.
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = locations_pb2.ListLocationsRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._transport.list_locations,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
     gapic_version=package_version.__version__
 )
 
 
 __all__ = ("RegistrationServiceClient",)
```

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/registration_service/pagers.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/registration_service/pagers.py`

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

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/__init__.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/__init__.py`

 * *Files 4% similar despite different names*

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

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/base.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/base.py`

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
@@ -18,14 +18,15 @@
 
 import google.api_core
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
+from google.cloud.location import locations_pb2  # type: ignore
 from google.iam.v1 import iam_policy_pb2  # type: ignore
 from google.iam.v1 import policy_pb2  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 from google.protobuf import empty_pb2  # type: ignore
 
 from google.cloud.servicedirectory_v1beta1 import gapic_version as package_version
 from google.cloud.servicedirectory_v1beta1.types import endpoint as gcs_endpoint
@@ -403,12 +404,33 @@
             iam_policy_pb2.TestIamPermissionsResponse,
             Awaitable[iam_policy_pb2.TestIamPermissionsResponse],
         ],
     ]:
         raise NotImplementedError()
 
     @property
+    def get_location(
+        self,
+    ) -> Callable[
+        [locations_pb2.GetLocationRequest],
+        Union[locations_pb2.Location, Awaitable[locations_pb2.Location]],
+    ]:
+        raise NotImplementedError()
+
+    @property
+    def list_locations(
+        self,
+    ) -> Callable[
+        [locations_pb2.ListLocationsRequest],
+        Union[
+            locations_pb2.ListLocationsResponse,
+            Awaitable[locations_pb2.ListLocationsResponse],
+        ],
+    ]:
+        raise NotImplementedError()
+
+    @property
     def kind(self) -> str:
         raise NotImplementedError()
 
 
 __all__ = ("RegistrationServiceTransport",)
```

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/grpc.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/grpc.py`

 * *Files 8% similar despite different names*

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
@@ -16,14 +16,15 @@
 from typing import Callable, Dict, Optional, Sequence, Tuple, Union
 import warnings
 
 from google.api_core import gapic_v1, grpc_helpers
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
+from google.cloud.location import locations_pb2  # type: ignore
 from google.iam.v1 import iam_policy_pb2  # type: ignore
 from google.iam.v1 import policy_pb2  # type: ignore
 from google.protobuf import empty_pb2  # type: ignore
 import grpc  # type: ignore
 
 from google.cloud.servicedirectory_v1beta1.types import endpoint as gcs_endpoint
 from google.cloud.servicedirectory_v1beta1.types import namespace as gcs_namespace
@@ -659,16 +660,15 @@
 
     @property
     def get_iam_policy(
         self,
     ) -> Callable[[iam_policy_pb2.GetIamPolicyRequest], policy_pb2.Policy]:
         r"""Return a callable for the get iam policy method over gRPC.
 
-        Gets the IAM Policy for a resource (namespace or
-        service only).
+        Gets the IAM Policy for a resource
 
         Returns:
             Callable[[~.GetIamPolicyRequest],
                     ~.Policy]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
@@ -686,16 +686,15 @@
 
     @property
     def set_iam_policy(
         self,
     ) -> Callable[[iam_policy_pb2.SetIamPolicyRequest], policy_pb2.Policy]:
         r"""Return a callable for the set iam policy method over gRPC.
 
-        Sets the IAM Policy for a resource (namespace or
-        service only).
+        Sets the IAM Policy for a resource
 
         Returns:
             Callable[[~.SetIamPolicyRequest],
                     ~.Policy]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
@@ -716,16 +715,16 @@
         self,
     ) -> Callable[
         [iam_policy_pb2.TestIamPermissionsRequest],
         iam_policy_pb2.TestIamPermissionsResponse,
     ]:
         r"""Return a callable for the test iam permissions method over gRPC.
 
-        Tests IAM permissions for a resource (namespace or
-        service only).
+        Tests IAM permissions for a resource (namespace,
+        service  or service workload only).
 
         Returns:
             Callable[[~.TestIamPermissionsRequest],
                     ~.TestIamPermissionsResponse]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
@@ -741,12 +740,48 @@
             )
         return self._stubs["test_iam_permissions"]
 
     def close(self):
         self.grpc_channel.close()
 
     @property
+    def list_locations(
+        self,
+    ) -> Callable[
+        [locations_pb2.ListLocationsRequest], locations_pb2.ListLocationsResponse
+    ]:
+        r"""Return a callable for the list locations method over gRPC."""
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "list_locations" not in self._stubs:
+            self._stubs["list_locations"] = self.grpc_channel.unary_unary(
+                "/google.cloud.location.Locations/ListLocations",
+                request_serializer=locations_pb2.ListLocationsRequest.SerializeToString,
+                response_deserializer=locations_pb2.ListLocationsResponse.FromString,
+            )
+        return self._stubs["list_locations"]
+
+    @property
+    def get_location(
+        self,
+    ) -> Callable[[locations_pb2.GetLocationRequest], locations_pb2.Location]:
+        r"""Return a callable for the list locations method over gRPC."""
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "get_location" not in self._stubs:
+            self._stubs["get_location"] = self.grpc_channel.unary_unary(
+                "/google.cloud.location.Locations/GetLocation",
+                request_serializer=locations_pb2.GetLocationRequest.SerializeToString,
+                response_deserializer=locations_pb2.Location.FromString,
+            )
+        return self._stubs["get_location"]
+
+    @property
     def kind(self) -> str:
         return "grpc"
 
 
 __all__ = ("RegistrationServiceGrpcTransport",)
```

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/grpc_asyncio.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/grpc_asyncio.py`

 * *Files 8% similar despite different names*

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
@@ -15,14 +15,15 @@
 #
 from typing import Awaitable, Callable, Dict, Optional, Sequence, Tuple, Union
 import warnings
 
 from google.api_core import gapic_v1, grpc_helpers_async
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
+from google.cloud.location import locations_pb2  # type: ignore
 from google.iam.v1 import iam_policy_pb2  # type: ignore
 from google.iam.v1 import policy_pb2  # type: ignore
 from google.protobuf import empty_pb2  # type: ignore
 import grpc  # type: ignore
 from grpc.experimental import aio  # type: ignore
 
 from google.cloud.servicedirectory_v1beta1.types import endpoint as gcs_endpoint
@@ -682,16 +683,15 @@
 
     @property
     def get_iam_policy(
         self,
     ) -> Callable[[iam_policy_pb2.GetIamPolicyRequest], Awaitable[policy_pb2.Policy]]:
         r"""Return a callable for the get iam policy method over gRPC.
 
-        Gets the IAM Policy for a resource (namespace or
-        service only).
+        Gets the IAM Policy for a resource
 
         Returns:
             Callable[[~.GetIamPolicyRequest],
                     Awaitable[~.Policy]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
@@ -709,16 +709,15 @@
 
     @property
     def set_iam_policy(
         self,
     ) -> Callable[[iam_policy_pb2.SetIamPolicyRequest], Awaitable[policy_pb2.Policy]]:
         r"""Return a callable for the set iam policy method over gRPC.
 
-        Sets the IAM Policy for a resource (namespace or
-        service only).
+        Sets the IAM Policy for a resource
 
         Returns:
             Callable[[~.SetIamPolicyRequest],
                     Awaitable[~.Policy]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
@@ -739,16 +738,16 @@
         self,
     ) -> Callable[
         [iam_policy_pb2.TestIamPermissionsRequest],
         Awaitable[iam_policy_pb2.TestIamPermissionsResponse],
     ]:
         r"""Return a callable for the test iam permissions method over gRPC.
 
-        Tests IAM permissions for a resource (namespace or
-        service only).
+        Tests IAM permissions for a resource (namespace,
+        service  or service workload only).
 
         Returns:
             Callable[[~.TestIamPermissionsRequest],
                     Awaitable[~.TestIamPermissionsResponse]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
@@ -763,9 +762,45 @@
                 response_deserializer=iam_policy_pb2.TestIamPermissionsResponse.FromString,
             )
         return self._stubs["test_iam_permissions"]
 
     def close(self):
         return self.grpc_channel.close()
 
+    @property
+    def list_locations(
+        self,
+    ) -> Callable[
+        [locations_pb2.ListLocationsRequest], locations_pb2.ListLocationsResponse
+    ]:
+        r"""Return a callable for the list locations method over gRPC."""
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "list_locations" not in self._stubs:
+            self._stubs["list_locations"] = self.grpc_channel.unary_unary(
+                "/google.cloud.location.Locations/ListLocations",
+                request_serializer=locations_pb2.ListLocationsRequest.SerializeToString,
+                response_deserializer=locations_pb2.ListLocationsResponse.FromString,
+            )
+        return self._stubs["list_locations"]
+
+    @property
+    def get_location(
+        self,
+    ) -> Callable[[locations_pb2.GetLocationRequest], locations_pb2.Location]:
+        r"""Return a callable for the list locations method over gRPC."""
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "get_location" not in self._stubs:
+            self._stubs["get_location"] = self.grpc_channel.unary_unary(
+                "/google.cloud.location.Locations/GetLocation",
+                request_serializer=locations_pb2.GetLocationRequest.SerializeToString,
+                response_deserializer=locations_pb2.Location.FromString,
+            )
+        return self._stubs["get_location"]
+
 
 __all__ = ("RegistrationServiceGrpcAsyncIOTransport",)
```

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/rest.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/registration_service/transports/rest.py`

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
@@ -22,35 +22,36 @@
 
 from google.api_core import gapic_v1, path_template, rest_helpers, rest_streaming
 from google.api_core import exceptions as core_exceptions
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.auth.transport.requests import AuthorizedSession  # type: ignore
+from google.cloud.location import locations_pb2  # type: ignore
 from google.protobuf import json_format
 import grpc  # type: ignore
 from requests import __version__ as requests_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 
 from google.iam.v1 import iam_policy_pb2  # type: ignore
 from google.iam.v1 import policy_pb2  # type: ignore
 from google.protobuf import empty_pb2  # type: ignore
 
-from google.cloud.servicedirectory_v1beta1.types import endpoint as gcs_endpoint
-from google.cloud.servicedirectory_v1beta1.types import namespace as gcs_namespace
-from google.cloud.servicedirectory_v1beta1.types import endpoint
-from google.cloud.servicedirectory_v1beta1.types import namespace
-from google.cloud.servicedirectory_v1beta1.types import registration_service
-from google.cloud.servicedirectory_v1beta1.types import service
-from google.cloud.servicedirectory_v1beta1.types import service as gcs_service
+from google.cloud.servicedirectory_v1.types import endpoint
+from google.cloud.servicedirectory_v1.types import endpoint as gcs_endpoint
+from google.cloud.servicedirectory_v1.types import namespace
+from google.cloud.servicedirectory_v1.types import namespace as gcs_namespace
+from google.cloud.servicedirectory_v1.types import registration_service
+from google.cloud.servicedirectory_v1.types import service
+from google.cloud.servicedirectory_v1.types import service as gcs_service
 
 from .base import DEFAULT_CLIENT_INFO as BASE_DEFAULT_CLIENT_INFO
 from .base import RegistrationServiceTransport
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
     gapic_version=BASE_DEFAULT_CLIENT_INFO.gapic_version,
     grpc_version=None,
@@ -574,14 +575,60 @@
 
         Override in a subclass to manipulate the response
         after it is returned by the RegistrationService server but before
         it is returned to user code.
         """
         return response
 
+    def pre_get_location(
+        self,
+        request: locations_pb2.GetLocationRequest,
+        metadata: Sequence[Tuple[str, str]],
+    ) -> Tuple[locations_pb2.GetLocationRequest, Sequence[Tuple[str, str]]]:
+        """Pre-rpc interceptor for get_location
+
+        Override in a subclass to manipulate the request or metadata
+        before they are sent to the RegistrationService server.
+        """
+        return request, metadata
+
+    def post_get_location(
+        self, response: locations_pb2.Location
+    ) -> locations_pb2.Location:
+        """Post-rpc interceptor for get_location
+
+        Override in a subclass to manipulate the response
+        after it is returned by the RegistrationService server but before
+        it is returned to user code.
+        """
+        return response
+
+    def pre_list_locations(
+        self,
+        request: locations_pb2.ListLocationsRequest,
+        metadata: Sequence[Tuple[str, str]],
+    ) -> Tuple[locations_pb2.ListLocationsRequest, Sequence[Tuple[str, str]]]:
+        """Pre-rpc interceptor for list_locations
+
+        Override in a subclass to manipulate the request or metadata
+        before they are sent to the RegistrationService server.
+        """
+        return request, metadata
+
+    def post_list_locations(
+        self, response: locations_pb2.ListLocationsResponse
+    ) -> locations_pb2.ListLocationsResponse:
+        """Post-rpc interceptor for list_locations
+
+        Override in a subclass to manipulate the response
+        after it is returned by the RegistrationService server but before
+        it is returned to user code.
+        """
+        return response
+
 
 @dataclasses.dataclass
 class RegistrationServiceRestStub:
     _session: AuthorizedSession
     _host: str
     _interceptor: RegistrationServiceRestInterceptor
 
@@ -589,25 +636,24 @@
 class RegistrationServiceRestTransport(RegistrationServiceTransport):
     """REST backend transport for RegistrationService.
 
     Service Directory API for registering services. It defines the
     following resource model:
 
     -  The API has a collection of
-       [Namespace][google.cloud.servicedirectory.v1beta1.Namespace]
+       [Namespace][google.cloud.servicedirectory.v1.Namespace]
        resources, named ``projects/*/locations/*/namespaces/*``.
 
     -  Each Namespace has a collection of
-       [Service][google.cloud.servicedirectory.v1beta1.Service]
-       resources, named
-       ``projects/*/locations/*/namespaces/*/services/*``.
+       [Service][google.cloud.servicedirectory.v1.Service] resources,
+       named ``projects/*/locations/*/namespaces/*/services/*``.
 
     -  Each Service has a collection of
-       [Endpoint][google.cloud.servicedirectory.v1beta1.Endpoint]
-       resources, named
+       [Endpoint][google.cloud.servicedirectory.v1.Endpoint] resources,
+       named
        ``projects/*/locations/*/namespaces/*/services/*/endpoints/*``.
 
     This class defines the same methods as the primary client, so the
     primary client can load the underlying transport implementation
     and call it.
 
     It sends JSON representations of protocol buffers over HTTP/1.1
@@ -715,33 +761,33 @@
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> gcs_endpoint.Endpoint:
             r"""Call the create endpoint method over HTTP.
 
             Args:
                 request (~.registration_service.CreateEndpointRequest):
                     The request object. The request message for
-                [RegistrationService.CreateEndpoint][google.cloud.servicedirectory.v1beta1.RegistrationService.CreateEndpoint].
+                [RegistrationService.CreateEndpoint][google.cloud.servicedirectory.v1.RegistrationService.CreateEndpoint].
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
                 ~.gcs_endpoint.Endpoint:
                     An individual endpoint that provides a
-                [service][google.cloud.servicedirectory.v1beta1.Service].
-                The service must already exist to create an endpoint.
+                [service][google.cloud.servicedirectory.v1.Service]. The
+                service must already exist to create an endpoint.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "post",
-                    "uri": "/v1beta1/{parent=projects/*/locations/*/namespaces/*/services/*}/endpoints",
+                    "uri": "/v1/{parent=projects/*/locations/*/namespaces/*/services/*}/endpoints",
                     "body": "endpoint",
                 },
             ]
             request, metadata = self._interceptor.pre_create_endpoint(request, metadata)
             pb_request = registration_service.CreateEndpointRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
 
@@ -816,35 +862,35 @@
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> gcs_namespace.Namespace:
             r"""Call the create namespace method over HTTP.
 
             Args:
                 request (~.registration_service.CreateNamespaceRequest):
                     The request object. The request message for
-                [RegistrationService.CreateNamespace][google.cloud.servicedirectory.v1beta1.RegistrationService.CreateNamespace].
+                [RegistrationService.CreateNamespace][google.cloud.servicedirectory.v1.RegistrationService.CreateNamespace].
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
                 ~.gcs_namespace.Namespace:
                     A container for
-                [services][google.cloud.servicedirectory.v1beta1.Service].
+                [services][google.cloud.servicedirectory.v1.Service].
                 Namespaces allow administrators to group services
                 together and define permissions for a collection of
                 services.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "post",
-                    "uri": "/v1beta1/{parent=projects/*/locations/*}/namespaces",
+                    "uri": "/v1/{parent=projects/*/locations/*}/namespaces",
                     "body": "namespace",
                 },
             ]
             request, metadata = self._interceptor.pre_create_namespace(
                 request, metadata
             )
             pb_request = registration_service.CreateNamespaceRequest.pb(request)
@@ -921,34 +967,34 @@
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> gcs_service.Service:
             r"""Call the create service method over HTTP.
 
             Args:
                 request (~.registration_service.CreateServiceRequest):
                     The request object. The request message for
-                [RegistrationService.CreateService][google.cloud.servicedirectory.v1beta1.RegistrationService.CreateService].
+                [RegistrationService.CreateService][google.cloud.servicedirectory.v1.RegistrationService.CreateService].
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
                 ~.gcs_service.Service:
                     An individual service. A service contains a name and
                 optional metadata. A service must exist before
-                [endpoints][google.cloud.servicedirectory.v1beta1.Endpoint]
+                [endpoints][google.cloud.servicedirectory.v1.Endpoint]
                 can be added to it.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "post",
-                    "uri": "/v1beta1/{parent=projects/*/locations/*/namespaces/*}/services",
+                    "uri": "/v1/{parent=projects/*/locations/*/namespaces/*}/services",
                     "body": "service",
                 },
             ]
             request, metadata = self._interceptor.pre_create_service(request, metadata)
             pb_request = registration_service.CreateServiceRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
 
@@ -1021,26 +1067,26 @@
             metadata: Sequence[Tuple[str, str]] = (),
         ):
             r"""Call the delete endpoint method over HTTP.
 
             Args:
                 request (~.registration_service.DeleteEndpointRequest):
                     The request object. The request message for
-                [RegistrationService.DeleteEndpoint][google.cloud.servicedirectory.v1beta1.RegistrationService.DeleteEndpoint].
+                [RegistrationService.DeleteEndpoint][google.cloud.servicedirectory.v1.RegistrationService.DeleteEndpoint].
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "delete",
-                    "uri": "/v1beta1/{name=projects/*/locations/*/namespaces/*/services/*/endpoints/*}",
+                    "uri": "/v1/{name=projects/*/locations/*/namespaces/*/services/*/endpoints/*}",
                 },
             ]
             request, metadata = self._interceptor.pre_delete_endpoint(request, metadata)
             pb_request = registration_service.DeleteEndpointRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
 
             uri = transcoded_request["uri"]
@@ -1096,26 +1142,26 @@
             metadata: Sequence[Tuple[str, str]] = (),
         ):
             r"""Call the delete namespace method over HTTP.
 
             Args:
                 request (~.registration_service.DeleteNamespaceRequest):
                     The request object. The request message for
-                [RegistrationService.DeleteNamespace][google.cloud.servicedirectory.v1beta1.RegistrationService.DeleteNamespace].
+                [RegistrationService.DeleteNamespace][google.cloud.servicedirectory.v1.RegistrationService.DeleteNamespace].
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "delete",
-                    "uri": "/v1beta1/{name=projects/*/locations/*/namespaces/*}",
+                    "uri": "/v1/{name=projects/*/locations/*/namespaces/*}",
                 },
             ]
             request, metadata = self._interceptor.pre_delete_namespace(
                 request, metadata
             )
             pb_request = registration_service.DeleteNamespaceRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
@@ -1173,26 +1219,26 @@
             metadata: Sequence[Tuple[str, str]] = (),
         ):
             r"""Call the delete service method over HTTP.
 
             Args:
                 request (~.registration_service.DeleteServiceRequest):
                     The request object. The request message for
-                [RegistrationService.DeleteService][google.cloud.servicedirectory.v1beta1.RegistrationService.DeleteService].
+                [RegistrationService.DeleteService][google.cloud.servicedirectory.v1.RegistrationService.DeleteService].
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "delete",
-                    "uri": "/v1beta1/{name=projects/*/locations/*/namespaces/*/services/*}",
+                    "uri": "/v1/{name=projects/*/locations/*/namespaces/*/services/*}",
                 },
             ]
             request, metadata = self._interceptor.pre_delete_service(request, metadata)
             pb_request = registration_service.DeleteServiceRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
 
             uri = transcoded_request["uri"]
@@ -1248,35 +1294,35 @@
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> endpoint.Endpoint:
             r"""Call the get endpoint method over HTTP.
 
             Args:
                 request (~.registration_service.GetEndpointRequest):
                     The request object. The request message for
-                [RegistrationService.GetEndpoint][google.cloud.servicedirectory.v1beta1.RegistrationService.GetEndpoint].
+                [RegistrationService.GetEndpoint][google.cloud.servicedirectory.v1.RegistrationService.GetEndpoint].
                 This should not be used to lookup endpoints at runtime.
                 Instead, use the ``resolve`` method.
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
                 ~.endpoint.Endpoint:
                     An individual endpoint that provides a
-                [service][google.cloud.servicedirectory.v1beta1.Service].
-                The service must already exist to create an endpoint.
+                [service][google.cloud.servicedirectory.v1.Service]. The
+                service must already exist to create an endpoint.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "get",
-                    "uri": "/v1beta1/{name=projects/*/locations/*/namespaces/*/services/*/endpoints/*}",
+                    "uri": "/v1/{name=projects/*/locations/*/namespaces/*/services/*/endpoints/*}",
                 },
             ]
             request, metadata = self._interceptor.pre_get_endpoint(request, metadata)
             pb_request = registration_service.GetEndpointRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
 
             uri = transcoded_request["uri"]
@@ -1429,20 +1475,20 @@
                 documentation <https://cloud.google.com/iam/docs/>`__.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "post",
-                    "uri": "/v1beta1/{resource=projects/*/locations/*/namespaces/*}:getIamPolicy",
+                    "uri": "/v1/{resource=projects/*/locations/*/namespaces/*}:getIamPolicy",
                     "body": "*",
                 },
                 {
                     "method": "post",
-                    "uri": "/v1beta1/{resource=projects/*/locations/*/namespaces/*/services/*}:getIamPolicy",
+                    "uri": "/v1/{resource=projects/*/locations/*/namespaces/*/services/*}:getIamPolicy",
                     "body": "*",
                 },
             ]
             request, metadata = self._interceptor.pre_get_iam_policy(request, metadata)
             pb_request = request
             transcoded_request = path_template.transcode(http_options, pb_request)
 
@@ -1515,35 +1561,35 @@
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> namespace.Namespace:
             r"""Call the get namespace method over HTTP.
 
             Args:
                 request (~.registration_service.GetNamespaceRequest):
                     The request object. The request message for
-                [RegistrationService.GetNamespace][google.cloud.servicedirectory.v1beta1.RegistrationService.GetNamespace].
+                [RegistrationService.GetNamespace][google.cloud.servicedirectory.v1.RegistrationService.GetNamespace].
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
                 ~.namespace.Namespace:
                     A container for
-                [services][google.cloud.servicedirectory.v1beta1.Service].
+                [services][google.cloud.servicedirectory.v1.Service].
                 Namespaces allow administrators to group services
                 together and define permissions for a collection of
                 services.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "get",
-                    "uri": "/v1beta1/{name=projects/*/locations/*/namespaces/*}",
+                    "uri": "/v1/{name=projects/*/locations/*/namespaces/*}",
                 },
             ]
             request, metadata = self._interceptor.pre_get_namespace(request, metadata)
             pb_request = registration_service.GetNamespaceRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
 
             uri = transcoded_request["uri"]
@@ -1607,37 +1653,37 @@
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> service.Service:
             r"""Call the get service method over HTTP.
 
             Args:
                 request (~.registration_service.GetServiceRequest):
                     The request object. The request message for
-                [RegistrationService.GetService][google.cloud.servicedirectory.v1beta1.RegistrationService.GetService].
+                [RegistrationService.GetService][google.cloud.servicedirectory.v1.RegistrationService.GetService].
                 This should not be used for looking up a service.
-                Insead, use the ``resolve`` method as it contains all
-                endpoints and associated metadata.
+                Instead, use the ``resolve`` method as it contains all
+                endpoints and associated annotations.
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
                 ~.service.Service:
                     An individual service. A service contains a name and
                 optional metadata. A service must exist before
-                [endpoints][google.cloud.servicedirectory.v1beta1.Endpoint]
+                [endpoints][google.cloud.servicedirectory.v1.Endpoint]
                 can be added to it.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "get",
-                    "uri": "/v1beta1/{name=projects/*/locations/*/namespaces/*/services/*}",
+                    "uri": "/v1/{name=projects/*/locations/*/namespaces/*/services/*}",
                 },
             ]
             request, metadata = self._interceptor.pre_get_service(request, metadata)
             pb_request = registration_service.GetServiceRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
 
             uri = transcoded_request["uri"]
@@ -1701,32 +1747,32 @@
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> registration_service.ListEndpointsResponse:
             r"""Call the list endpoints method over HTTP.
 
             Args:
                 request (~.registration_service.ListEndpointsRequest):
                     The request object. The request message for
-                [RegistrationService.ListEndpoints][google.cloud.servicedirectory.v1beta1.RegistrationService.ListEndpoints].
+                [RegistrationService.ListEndpoints][google.cloud.servicedirectory.v1.RegistrationService.ListEndpoints].
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
                 ~.registration_service.ListEndpointsResponse:
                     The response message for
-                [RegistrationService.ListEndpoints][google.cloud.servicedirectory.v1beta1.RegistrationService.ListEndpoints].
+                [RegistrationService.ListEndpoints][google.cloud.servicedirectory.v1.RegistrationService.ListEndpoints].
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "get",
-                    "uri": "/v1beta1/{parent=projects/*/locations/*/namespaces/*/services/*}/endpoints",
+                    "uri": "/v1/{parent=projects/*/locations/*/namespaces/*/services/*}/endpoints",
                 },
             ]
             request, metadata = self._interceptor.pre_list_endpoints(request, metadata)
             pb_request = registration_service.ListEndpointsRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
 
             uri = transcoded_request["uri"]
@@ -1790,32 +1836,32 @@
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> registration_service.ListNamespacesResponse:
             r"""Call the list namespaces method over HTTP.
 
             Args:
                 request (~.registration_service.ListNamespacesRequest):
                     The request object. The request message for
-                [RegistrationService.ListNamespaces][google.cloud.servicedirectory.v1beta1.RegistrationService.ListNamespaces].
+                [RegistrationService.ListNamespaces][google.cloud.servicedirectory.v1.RegistrationService.ListNamespaces].
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
                 ~.registration_service.ListNamespacesResponse:
                     The response message for
-                [RegistrationService.ListNamespaces][google.cloud.servicedirectory.v1beta1.RegistrationService.ListNamespaces].
+                [RegistrationService.ListNamespaces][google.cloud.servicedirectory.v1.RegistrationService.ListNamespaces].
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "get",
-                    "uri": "/v1beta1/{parent=projects/*/locations/*}/namespaces",
+                    "uri": "/v1/{parent=projects/*/locations/*}/namespaces",
                 },
             ]
             request, metadata = self._interceptor.pre_list_namespaces(request, metadata)
             pb_request = registration_service.ListNamespacesRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
 
             uri = transcoded_request["uri"]
@@ -1879,32 +1925,32 @@
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> registration_service.ListServicesResponse:
             r"""Call the list services method over HTTP.
 
             Args:
                 request (~.registration_service.ListServicesRequest):
                     The request object. The request message for
-                [RegistrationService.ListServices][google.cloud.servicedirectory.v1beta1.RegistrationService.ListServices].
+                [RegistrationService.ListServices][google.cloud.servicedirectory.v1.RegistrationService.ListServices].
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
                 ~.registration_service.ListServicesResponse:
                     The response message for
-                [RegistrationService.ListServices][google.cloud.servicedirectory.v1beta1.RegistrationService.ListServices].
+                [RegistrationService.ListServices][google.cloud.servicedirectory.v1.RegistrationService.ListServices].
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "get",
-                    "uri": "/v1beta1/{parent=projects/*/locations/*/namespaces/*}/services",
+                    "uri": "/v1/{parent=projects/*/locations/*/namespaces/*}/services",
                 },
             ]
             request, metadata = self._interceptor.pre_list_services(request, metadata)
             pb_request = registration_service.ListServicesRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
 
             uri = transcoded_request["uri"]
@@ -2057,20 +2103,20 @@
                 documentation <https://cloud.google.com/iam/docs/>`__.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "post",
-                    "uri": "/v1beta1/{resource=projects/*/locations/*/namespaces/*}:setIamPolicy",
+                    "uri": "/v1/{resource=projects/*/locations/*/namespaces/*}:setIamPolicy",
                     "body": "*",
                 },
                 {
                     "method": "post",
-                    "uri": "/v1beta1/{resource=projects/*/locations/*/namespaces/*/services/*}:setIamPolicy",
+                    "uri": "/v1/{resource=projects/*/locations/*/namespaces/*/services/*}:setIamPolicy",
                     "body": "*",
                 },
             ]
             request, metadata = self._interceptor.pre_set_iam_policy(request, metadata)
             pb_request = request
             transcoded_request = path_template.transcode(http_options, pb_request)
 
@@ -2157,20 +2203,20 @@
                 ~.iam_policy_pb2.TestIamPermissionsResponse:
                     Response message for ``TestIamPermissions`` method.
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "post",
-                    "uri": "/v1beta1/{resource=projects/*/locations/*/namespaces/*}:testIamPermissions",
+                    "uri": "/v1/{resource=projects/*/locations/*/namespaces/*}:testIamPermissions",
                     "body": "*",
                 },
                 {
                     "method": "post",
-                    "uri": "/v1beta1/{resource=projects/*/locations/*/namespaces/*/services/*}:testIamPermissions",
+                    "uri": "/v1/{resource=projects/*/locations/*/namespaces/*/services/*}:testIamPermissions",
                     "body": "*",
                 },
             ]
             request, metadata = self._interceptor.pre_test_iam_permissions(
                 request, metadata
             )
             pb_request = request
@@ -2247,33 +2293,33 @@
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> gcs_endpoint.Endpoint:
             r"""Call the update endpoint method over HTTP.
 
             Args:
                 request (~.registration_service.UpdateEndpointRequest):
                     The request object. The request message for
-                [RegistrationService.UpdateEndpoint][google.cloud.servicedirectory.v1beta1.RegistrationService.UpdateEndpoint].
+                [RegistrationService.UpdateEndpoint][google.cloud.servicedirectory.v1.RegistrationService.UpdateEndpoint].
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
                 ~.gcs_endpoint.Endpoint:
                     An individual endpoint that provides a
-                [service][google.cloud.servicedirectory.v1beta1.Service].
-                The service must already exist to create an endpoint.
+                [service][google.cloud.servicedirectory.v1.Service]. The
+                service must already exist to create an endpoint.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "patch",
-                    "uri": "/v1beta1/{endpoint.name=projects/*/locations/*/namespaces/*/services/*/endpoints/*}",
+                    "uri": "/v1/{endpoint.name=projects/*/locations/*/namespaces/*/services/*/endpoints/*}",
                     "body": "endpoint",
                 },
             ]
             request, metadata = self._interceptor.pre_update_endpoint(request, metadata)
             pb_request = registration_service.UpdateEndpointRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
 
@@ -2348,35 +2394,35 @@
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> gcs_namespace.Namespace:
             r"""Call the update namespace method over HTTP.
 
             Args:
                 request (~.registration_service.UpdateNamespaceRequest):
                     The request object. The request message for
-                [RegistrationService.UpdateNamespace][google.cloud.servicedirectory.v1beta1.RegistrationService.UpdateNamespace].
+                [RegistrationService.UpdateNamespace][google.cloud.servicedirectory.v1.RegistrationService.UpdateNamespace].
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
                 ~.gcs_namespace.Namespace:
                     A container for
-                [services][google.cloud.servicedirectory.v1beta1.Service].
+                [services][google.cloud.servicedirectory.v1.Service].
                 Namespaces allow administrators to group services
                 together and define permissions for a collection of
                 services.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "patch",
-                    "uri": "/v1beta1/{namespace.name=projects/*/locations/*/namespaces/*}",
+                    "uri": "/v1/{namespace.name=projects/*/locations/*/namespaces/*}",
                     "body": "namespace",
                 },
             ]
             request, metadata = self._interceptor.pre_update_namespace(
                 request, metadata
             )
             pb_request = registration_service.UpdateNamespaceRequest.pb(request)
@@ -2453,34 +2499,34 @@
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> gcs_service.Service:
             r"""Call the update service method over HTTP.
 
             Args:
                 request (~.registration_service.UpdateServiceRequest):
                     The request object. The request message for
-                [RegistrationService.UpdateService][google.cloud.servicedirectory.v1beta1.RegistrationService.UpdateService].
+                [RegistrationService.UpdateService][google.cloud.servicedirectory.v1.RegistrationService.UpdateService].
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
                 ~.gcs_service.Service:
                     An individual service. A service contains a name and
                 optional metadata. A service must exist before
-                [endpoints][google.cloud.servicedirectory.v1beta1.Endpoint]
+                [endpoints][google.cloud.servicedirectory.v1.Endpoint]
                 can be added to it.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "patch",
-                    "uri": "/v1beta1/{service.name=projects/*/locations/*/namespaces/*/services/*}",
+                    "uri": "/v1/{service.name=projects/*/locations/*/namespaces/*/services/*}",
                     "body": "service",
                 },
             ]
             request, metadata = self._interceptor.pre_update_service(request, metadata)
             pb_request = registration_service.UpdateServiceRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
 
@@ -2687,14 +2733,148 @@
         self,
     ) -> Callable[[registration_service.UpdateServiceRequest], gcs_service.Service]:
         # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
         # In C++ this would require a dynamic_cast
         return self._UpdateService(self._session, self._host, self._interceptor)  # type: ignore
 
     @property
+    def get_location(self):
+        return self._GetLocation(self._session, self._host, self._interceptor)  # type: ignore
+
+    class _GetLocation(RegistrationServiceRestStub):
+        def __call__(
+            self,
+            request: locations_pb2.GetLocationRequest,
+            *,
+            retry: OptionalRetry = gapic_v1.method.DEFAULT,
+            timeout: Optional[float] = None,
+            metadata: Sequence[Tuple[str, str]] = (),
+        ) -> locations_pb2.Location:
+
+            r"""Call the get location method over HTTP.
+
+            Args:
+                request (locations_pb2.GetLocationRequest):
+                    The request object for GetLocation method.
+                retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                    should be retried.
+                timeout (float): The timeout for this request.
+                metadata (Sequence[Tuple[str, str]]): Strings which should be
+                    sent along with the request as metadata.
+
+            Returns:
+                locations_pb2.Location: Response from GetLocation method.
+            """
+
+            http_options: List[Dict[str, str]] = [
+                {
+                    "method": "get",
+                    "uri": "/v1/{name=projects/*/locations/*}",
+                },
+            ]
+
+            request, metadata = self._interceptor.pre_get_location(request, metadata)
+            request_kwargs = json_format.MessageToDict(request)
+            transcoded_request = path_template.transcode(http_options, **request_kwargs)
+
+            uri = transcoded_request["uri"]
+            method = transcoded_request["method"]
+
+            # Jsonify the query params
+            query_params = json.loads(json.dumps(transcoded_request["query_params"]))
+
+            # Send the request
+            headers = dict(metadata)
+            headers["Content-Type"] = "application/json"
+
+            response = getattr(self._session, method)(
+                "{host}{uri}".format(host=self._host, uri=uri),
+                timeout=timeout,
+                headers=headers,
+                params=rest_helpers.flatten_query_params(query_params),
+            )
+
+            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
+            # subclass.
+            if response.status_code >= 400:
+                raise core_exceptions.from_http_response(response)
+
+            resp = locations_pb2.Location()
+            resp = json_format.Parse(response.content.decode("utf-8"), resp)
+            resp = self._interceptor.post_get_location(resp)
+            return resp
+
+    @property
+    def list_locations(self):
+        return self._ListLocations(self._session, self._host, self._interceptor)  # type: ignore
+
+    class _ListLocations(RegistrationServiceRestStub):
+        def __call__(
+            self,
+            request: locations_pb2.ListLocationsRequest,
+            *,
+            retry: OptionalRetry = gapic_v1.method.DEFAULT,
+            timeout: Optional[float] = None,
+            metadata: Sequence[Tuple[str, str]] = (),
+        ) -> locations_pb2.ListLocationsResponse:
+
+            r"""Call the list locations method over HTTP.
+
+            Args:
+                request (locations_pb2.ListLocationsRequest):
+                    The request object for ListLocations method.
+                retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                    should be retried.
+                timeout (float): The timeout for this request.
+                metadata (Sequence[Tuple[str, str]]): Strings which should be
+                    sent along with the request as metadata.
+
+            Returns:
+                locations_pb2.ListLocationsResponse: Response from ListLocations method.
+            """
+
+            http_options: List[Dict[str, str]] = [
+                {
+                    "method": "get",
+                    "uri": "/v1/{name=projects/*}/locations",
+                },
+            ]
+
+            request, metadata = self._interceptor.pre_list_locations(request, metadata)
+            request_kwargs = json_format.MessageToDict(request)
+            transcoded_request = path_template.transcode(http_options, **request_kwargs)
+
+            uri = transcoded_request["uri"]
+            method = transcoded_request["method"]
+
+            # Jsonify the query params
+            query_params = json.loads(json.dumps(transcoded_request["query_params"]))
+
+            # Send the request
+            headers = dict(metadata)
+            headers["Content-Type"] = "application/json"
+
+            response = getattr(self._session, method)(
+                "{host}{uri}".format(host=self._host, uri=uri),
+                timeout=timeout,
+                headers=headers,
+                params=rest_helpers.flatten_query_params(query_params),
+            )
+
+            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
+            # subclass.
+            if response.status_code >= 400:
+                raise core_exceptions.from_http_response(response)
+
+            resp = locations_pb2.ListLocationsResponse()
+            resp = json_format.Parse(response.content.decode("utf-8"), resp)
+            resp = self._interceptor.post_list_locations(resp)
+            return resp
+
+    @property
     def kind(self) -> str:
         return "rest"
 
     def close(self):
         self._session.close()
```

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/types/__init__.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/types/__init__.py`

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

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/types/endpoint.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/types/endpoint.py`

 * *Files 5% similar despite different names*

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
@@ -66,19 +66,14 @@
                ending with an alphanumeric character ([a-z0-9A-Z]) with
                dashes (-), underscores (_), dots (.), and alphanumerics
                between. The prefix is optional. If specified, the prefix
                must be a DNS subdomain: a series of DNS labels separated
                by dots (.), not longer than 253 characters in total,
                followed by a slash (/). Metadata that fails to meet
                these requirements are rejected
-            -  The ``(*.)google.com/`` and ``(*.)googleapis.com/``
-               prefixes are reserved for system metadata managed by
-               Service Directory. If the user tries to write to these
-               keyspaces, those entries are silently ignored by the
-               system
 
             Note: This field is equivalent to the ``annotations`` field
             in the v1 API. They have the same syntax and read/write to
             the same location in Service Directory.
         network (str):
             Immutable. The Google Compute Engine network (VPC) of the
             endpoint in the format
@@ -90,14 +85,17 @@
             network or project existence, reachability, or permissions).
         create_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The timestamp when the endpoint
             was created.
         update_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The timestamp when the endpoint
             was last updated.
+        uid (str):
+            Output only. A globally unique identifier (in
+            UUID4 format) for this endpoint.
     """
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
     address: str = proto.Field(
@@ -123,10 +121,14 @@
         message=timestamp_pb2.Timestamp,
     )
     update_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=7,
         message=timestamp_pb2.Timestamp,
     )
+    uid: str = proto.Field(
+        proto.STRING,
+        number=8,
+    )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/types/lookup_service.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/types/lookup_service.py`

 * *Files 9% similar despite different names*

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
@@ -15,28 +15,28 @@
 #
 from __future__ import annotations
 
 from typing import MutableMapping, MutableSequence
 
 import proto  # type: ignore
 
-from google.cloud.servicedirectory_v1beta1.types import service as gcs_service
+from google.cloud.servicedirectory_v1.types import service as gcs_service
 
 __protobuf__ = proto.module(
-    package="google.cloud.servicedirectory.v1beta1",
+    package="google.cloud.servicedirectory.v1",
     manifest={
         "ResolveServiceRequest",
         "ResolveServiceResponse",
     },
 )
 
 
 class ResolveServiceRequest(proto.Message):
     r"""The request message for
-    [LookupService.ResolveService][google.cloud.servicedirectory.v1beta1.LookupService.ResolveService].
+    [LookupService.ResolveService][google.cloud.servicedirectory.v1.LookupService.ResolveService].
     Looks up a service by its name, returns the service and its
     endpoints.
 
     Attributes:
         name (str):
             Required. The name of the service to resolve.
         max_endpoints (int):
@@ -49,40 +49,43 @@
             Optional. The filter applied to the endpoints of the
             resolved service.
 
             General ``filter`` string syntax:
             ``<field> <operator> <value> (<logical connector>)``
 
             -  ``<field>`` can be ``name``, ``address``, ``port``, or
-               ``metadata.<key>`` for map field
+               ``annotations.<key>`` for map field
             -  ``<operator>`` can be ``<``, ``>``, ``<=``, ``>=``,
                ``!=``, ``=``, ``:``. Of which ``:`` means ``HAS``, and
                is roughly the same as ``=``
             -  ``<value>`` must be the same data type as field
             -  ``<logical connector>`` can be ``AND``, ``OR``, ``NOT``
 
             Examples of valid filters:
 
-            -  ``metadata.owner`` returns endpoints that have a
+            -  ``annotations.owner`` returns endpoints that have a
                annotation with the key ``owner``, this is the same as
-               ``metadata:owner``
-            -  ``metadata.protocol=gRPC`` returns endpoints that have
+               ``annotations:owner``
+            -  ``annotations.protocol=gRPC`` returns endpoints that have
                key/value ``protocol=gRPC``
             -  ``address=192.108.1.105`` returns endpoints that have
                this address
             -  ``port>8080`` returns endpoints that have port number
                larger than 8080
             -
 
             ``name>projects/my-project/locations/us-east1/namespaces/my-namespace/services/my-service/endpoints/endpoint-c``
             returns endpoints that have name that is alphabetically
             later than the string, so "endpoint-e" is returned but
-            "endpoint-a" is not
+            "endpoint-a" is not \*
+            ``name=projects/my-project/locations/us-central1/namespaces/my-namespace/services/my-service/endpoints/ep-1``
+            returns the endpoint that has an endpoint_id equal to
+            ``ep-1``
 
-            -  ``metadata.owner!=sd AND metadata.foo=bar`` returns
+            -  ``annotations.owner!=sd AND annotations.foo=bar`` returns
                endpoints that have ``owner`` in annotation key but value
                is not ``sd`` AND have key/value ``foo=bar``
             -  ``doesnotexist.foo=bar`` returns an empty list. Note that
                endpoint doesn't have a field called "doesnotexist".
                Since the filter does not match any endpoint, it returns
                no results
 
@@ -102,18 +105,18 @@
         proto.STRING,
         number=3,
     )
 
 
 class ResolveServiceResponse(proto.Message):
     r"""The response message for
-    [LookupService.ResolveService][google.cloud.servicedirectory.v1beta1.LookupService.ResolveService].
+    [LookupService.ResolveService][google.cloud.servicedirectory.v1.LookupService.ResolveService].
 
     Attributes:
-        service (google.cloud.servicedirectory_v1beta1.types.Service):
+        service (google.cloud.servicedirectory_v1.types.Service):
 
     """
 
     service: gcs_service.Service = proto.Field(
         proto.MESSAGE,
         number=1,
         message=gcs_service.Service,
```

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/types/namespace.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/types/namespace.py`

 * *Files 10% similar despite different names*

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
@@ -45,14 +45,17 @@
             and values can be no longer than 63 characters.
         create_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The timestamp when the namespace
             was created.
         update_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The timestamp when the namespace
             was last updated.
+        uid (str):
+            Output only. A globally unique identifier (in
+            UUID4 format) for this namespace.
     """
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
     labels: MutableMapping[str, str] = proto.MapField(
@@ -66,10 +69,14 @@
         message=timestamp_pb2.Timestamp,
     )
     update_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=5,
         message=timestamp_pb2.Timestamp,
     )
+    uid: str = proto.Field(
+        proto.STRING,
+        number=6,
+    )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/types/registration_service.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/types/registration_service.py`

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
@@ -102,16 +102,16 @@
             List request, if any.
         filter (str):
             Optional. The filter to list results by.
 
             General ``filter`` string syntax:
             ``<field> <operator> <value> (<logical connector>)``
 
-            -  ``<field>`` can be ``name`` or ``labels.<key>`` for map
-               field
+            -  ``<field>`` can be ``name``, ``labels.<key>`` for map
+               field, or ``attributes.<field>`` for attributes field
             -  ``<operator>`` can be ``<``, ``>``, ``<=``, ``>=``,
                ``!=``, ``=``, ``:``. Of which ``:`` means ``HAS``, and
                is roughly the same as ``=``
             -  ``<value>`` must be the same data type as field
             -  ``<logical connector>`` can be ``AND``, ``OR``, ``NOT``
 
             Examples of valid filters:
@@ -128,14 +128,16 @@
             -  ``labels.owner!=sd AND labels.foo=bar`` returns
                namespaces that have ``owner`` in label key but value is
                not ``sd`` AND have key/value ``foo=bar``
             -  ``doesnotexist.foo=bar`` returns an empty list. Note that
                namespace doesn't have a field called "doesnotexist".
                Since the filter does not match any namespaces, it
                returns no results
+            -  ``attributes.managed_registration=true`` returns
+               namespaces that are managed by a GCP product or service
 
             For more information about filtering, see `API
             Filtering <https://aip.dev/160>`__.
         order_by (str):
             Optional. The order to list results by.
 
             General ``order_by`` string syntax:
@@ -335,14 +337,16 @@
             -  ``metadata.owner!=sd AND metadata.foo=bar`` returns
                services that have ``owner`` in metadata key but value is
                not ``sd`` AND have key/value ``foo=bar``
             -  ``doesnotexist.foo=bar`` returns an empty list. Note that
                service doesn't have a field called "doesnotexist". Since
                the filter does not match any services, it returns no
                results
+            -  ``attributes.managed_registration=true`` returns services
+               that are managed by a GCP product or service
 
             For more information about filtering, see `API
             Filtering <https://aip.dev/160>`__.
         order_by (str):
             Optional. The order to list results by.
 
             General ``order_by`` string syntax:
@@ -405,15 +409,15 @@
         number=2,
     )
 
 
 class GetServiceRequest(proto.Message):
     r"""The request message for
     [RegistrationService.GetService][google.cloud.servicedirectory.v1beta1.RegistrationService.GetService].
-    This should not be used for looking up a service. Insead, use the
+    This should not be used for looking up a service. Instead, use the
     ``resolve`` method as it contains all endpoints and associated
     metadata.
 
     Attributes:
         name (str):
             Required. The name of the service to get.
     """
@@ -514,16 +518,17 @@
             List request, if any.
         filter (str):
             Optional. The filter to list results by.
 
             General ``filter`` string syntax:
             ``<field> <operator> <value> (<logical connector>)``
 
-            -  ``<field>`` can be ``name``, ``address``, ``port``, or
-               ``metadata.<key>`` for map field
+            -  ``<field>`` can be ``name``, ``address``, ``port``,
+               ``metadata.<key>`` for map field, or
+               ``attributes.<field>`` for attributes field
             -  ``<operator>`` can be ``<``, ``>``, ``<=``, ``>=``,
                ``!=``, ``=``, ``:``. Of which ``:`` means ``HAS``, and
                is roughly the same as ``=``
             -  ``<value>`` must be the same data type as field
             -  ``<logical connector>`` can be ``AND``, ``OR``, ``NOT``
 
             Examples of valid filters:
@@ -547,14 +552,17 @@
             -  ``metadata.owner!=sd AND metadata.foo=bar`` returns
                endpoints that have ``owner`` in metadata key but value
                is not ``sd`` AND have key/value ``foo=bar``
             -  ``doesnotexist.foo=bar`` returns an empty list. Note that
                endpoint doesn't have a field called "doesnotexist".
                Since the filter does not match any endpoints, it returns
                no results
+            -  ``attributes.kubernetes_resource_type=KUBERNETES_RESOURCE_TYPE_CLUSTER_ IP``
+               returns endpoints with the corresponding
+               kubernetes_resource_type
 
             For more information about filtering, see `API
             Filtering <https://aip.dev/160>`__.
         order_by (str):
             Optional. The order to list results by.
 
             General ``order_by`` string syntax:
```

### Comparing `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/types/service.py` & `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/types/service.py`

 * *Files 7% similar despite different names*

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
@@ -55,19 +55,14 @@
                ending with an alphanumeric character ([a-z0-9A-Z]) with
                dashes (-), underscores (_), dots (.), and alphanumerics
                between. The prefix is optional. If specified, the prefix
                must be a DNS subdomain: a series of DNS labels separated
                by dots (.), not longer than 253 characters in total,
                followed by a slash (/). Metadata that fails to meet
                these requirements are rejected
-            -  The ``(*.)google.com/`` and ``(*.)googleapis.com/``
-               prefixes are reserved for system metadata managed by
-               Service Directory. If the user tries to write to these
-               keyspaces, those entries are silently ignored by the
-               system
 
             Note: This field is equivalent to the ``annotations`` field
             in the v1 API. They have the same syntax and read/write to
             the same location in Service Directory.
         endpoints (MutableSequence[google.cloud.servicedirectory_v1beta1.types.Endpoint]):
             Output only. Endpoints associated with this service.
             Returned on
@@ -75,18 +70,22 @@
             Control plane clients should use
             [RegistrationService.ListEndpoints][google.cloud.servicedirectory.v1beta1.RegistrationService.ListEndpoints].
         create_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The timestamp when the service
             was created.
         update_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The timestamp when the service
-            was last updated. Note: endpoints being
-            created/deleted/updated within the service are
-            not considered service updates for the purpose
-            of this timestamp.
+            was last updated. Note:
+
+            endpoints being created/deleted/updated within
+            the service are not considered service updates
+            for the purpose of this timestamp.
+        uid (str):
+            Output only. A globally unique identifier (in
+            UUID4 format) for this service.
     """
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
     metadata: MutableMapping[str, str] = proto.MapField(
@@ -105,10 +104,14 @@
         message=timestamp_pb2.Timestamp,
     )
     update_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=7,
         message=timestamp_pb2.Timestamp,
     )
+    uid: str = proto.Field(
+        proto.STRING,
+        number=8,
+    )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-service-directory-1.8.2/google_cloud_service_directory.egg-info/PKG-INFO` & `google-cloud-service-directory-1.9.0/google_cloud_service_directory.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-service-directory
-Version: 1.8.2
+Version: 1.9.0
 Summary: Google Cloud Service Directory API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-service-directory-1.8.2/google_cloud_service_directory.egg-info/SOURCES.txt` & `google-cloud-service-directory-1.9.0/google_cloud_service_directory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.2/setup.py` & `google-cloud-service-directory-1.9.0/setup.py`

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

### Comparing `google-cloud-service-directory-1.8.2/tests/__init__.py` & `google-cloud-service-directory-1.9.0/tests/unit/gapic/servicedirectory_v1/__init__.py`

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

### Comparing `google-cloud-service-directory-1.8.2/tests/unit/__init__.py` & `google-cloud-service-directory-1.9.0/tests/unit/gapic/servicedirectory_v1beta1/__init__.py`

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

### Comparing `google-cloud-service-directory-1.8.2/tests/unit/gapic/servicedirectory_v1/test_lookup_service.py` & `google-cloud-service-directory-1.9.0/tests/unit/gapic/servicedirectory_v1/test_lookup_service.py`

 * *Files 21% similar despite different names*

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
@@ -28,14 +28,15 @@
 
 from google.api_core import gapic_v1, grpc_helpers, grpc_helpers_async, path_template
 from google.api_core import client_options
 from google.api_core import exceptions as core_exceptions
 import google.auth
 from google.auth import credentials as ga_credentials
 from google.auth.exceptions import MutualTLSChannelError
+from google.cloud.location import locations_pb2
 from google.oauth2 import service_account
 from google.protobuf import json_format
 import grpc
 from grpc.experimental import aio
 from proto.marshal.rules import wrappers
 from proto.marshal.rules.dates import DurationRule, TimestampRule
 import pytest
@@ -1193,15 +1194,19 @@
         Transport.return_value = None
         transport = transports.LookupServiceTransport(
             credentials=ga_credentials.AnonymousCredentials(),
         )
 
     # Every method on the transport should just blindly
     # raise NotImplementedError.
-    methods = ("resolve_service",)
+    methods = (
+        "resolve_service",
+        "get_location",
+        "list_locations",
+    )
     for method in methods:
         with pytest.raises(NotImplementedError):
             getattr(transport, method)(request=object())
 
     with pytest.raises(NotImplementedError):
         transport.close()
 
@@ -1614,138 +1619,161 @@
     path = LookupServiceClient.endpoint_path(**expected)
 
     # Check that the path construction is reversible.
     actual = LookupServiceClient.parse_endpoint_path(path)
     assert expected == actual
 
 
-def test_service_path():
+def test_network_path():
     project = "scallop"
-    location = "abalone"
-    namespace = "squid"
-    service = "clam"
+    network = "abalone"
+    expected = "projects/{project}/locations/global/networks/{network}".format(
+        project=project,
+        network=network,
+    )
+    actual = LookupServiceClient.network_path(project, network)
+    assert expected == actual
+
+
+def test_parse_network_path():
+    expected = {
+        "project": "squid",
+        "network": "clam",
+    }
+    path = LookupServiceClient.network_path(**expected)
+
+    # Check that the path construction is reversible.
+    actual = LookupServiceClient.parse_network_path(path)
+    assert expected == actual
+
+
+def test_service_path():
+    project = "whelk"
+    location = "octopus"
+    namespace = "oyster"
+    service = "nudibranch"
     expected = "projects/{project}/locations/{location}/namespaces/{namespace}/services/{service}".format(
         project=project,
         location=location,
         namespace=namespace,
         service=service,
     )
     actual = LookupServiceClient.service_path(project, location, namespace, service)
     assert expected == actual
 
 
 def test_parse_service_path():
     expected = {
-        "project": "whelk",
-        "location": "octopus",
-        "namespace": "oyster",
-        "service": "nudibranch",
+        "project": "cuttlefish",
+        "location": "mussel",
+        "namespace": "winkle",
+        "service": "nautilus",
     }
     path = LookupServiceClient.service_path(**expected)
 
     # Check that the path construction is reversible.
     actual = LookupServiceClient.parse_service_path(path)
     assert expected == actual
 
 
 def test_common_billing_account_path():
-    billing_account = "cuttlefish"
+    billing_account = "scallop"
     expected = "billingAccounts/{billing_account}".format(
         billing_account=billing_account,
     )
     actual = LookupServiceClient.common_billing_account_path(billing_account)
     assert expected == actual
 
 
 def test_parse_common_billing_account_path():
     expected = {
-        "billing_account": "mussel",
+        "billing_account": "abalone",
     }
     path = LookupServiceClient.common_billing_account_path(**expected)
 
     # Check that the path construction is reversible.
     actual = LookupServiceClient.parse_common_billing_account_path(path)
     assert expected == actual
 
 
 def test_common_folder_path():
-    folder = "winkle"
+    folder = "squid"
     expected = "folders/{folder}".format(
         folder=folder,
     )
     actual = LookupServiceClient.common_folder_path(folder)
     assert expected == actual
 
 
 def test_parse_common_folder_path():
     expected = {
-        "folder": "nautilus",
+        "folder": "clam",
     }
     path = LookupServiceClient.common_folder_path(**expected)
 
     # Check that the path construction is reversible.
     actual = LookupServiceClient.parse_common_folder_path(path)
     assert expected == actual
 
 
 def test_common_organization_path():
-    organization = "scallop"
+    organization = "whelk"
     expected = "organizations/{organization}".format(
         organization=organization,
     )
     actual = LookupServiceClient.common_organization_path(organization)
     assert expected == actual
 
 
 def test_parse_common_organization_path():
     expected = {
-        "organization": "abalone",
+        "organization": "octopus",
     }
     path = LookupServiceClient.common_organization_path(**expected)
 
     # Check that the path construction is reversible.
     actual = LookupServiceClient.parse_common_organization_path(path)
     assert expected == actual
 
 
 def test_common_project_path():
-    project = "squid"
+    project = "oyster"
     expected = "projects/{project}".format(
         project=project,
     )
     actual = LookupServiceClient.common_project_path(project)
     assert expected == actual
 
 
 def test_parse_common_project_path():
     expected = {
-        "project": "clam",
+        "project": "nudibranch",
     }
     path = LookupServiceClient.common_project_path(**expected)
 
     # Check that the path construction is reversible.
     actual = LookupServiceClient.parse_common_project_path(path)
     assert expected == actual
 
 
 def test_common_location_path():
-    project = "whelk"
-    location = "octopus"
+    project = "cuttlefish"
+    location = "mussel"
     expected = "projects/{project}/locations/{location}".format(
         project=project,
         location=location,
     )
     actual = LookupServiceClient.common_location_path(project, location)
     assert expected == actual
 
 
 def test_parse_common_location_path():
     expected = {
-        "project": "oyster",
-        "location": "nudibranch",
+        "project": "winkle",
+        "location": "nautilus",
     }
     path = LookupServiceClient.common_location_path(**expected)
 
     # Check that the path construction is reversible.
     actual = LookupServiceClient.parse_common_location_path(path)
     assert expected == actual
 
@@ -1783,14 +1811,414 @@
         type(getattr(client.transport, "grpc_channel")), "close"
     ) as close:
         async with client:
             close.assert_not_called()
         close.assert_called_once()
 
 
+def test_get_location_rest_bad_request(
+    transport: str = "rest", request_type=locations_pb2.GetLocationRequest
+):
+    client = LookupServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    request = request_type()
+    request = json_format.ParseDict(
+        {"name": "projects/sample1/locations/sample2"}, request
+    )
+
+    # Mock the http request call within the method and fake a BadRequest error.
+    with mock.patch.object(Session, "request") as req, pytest.raises(
+        core_exceptions.BadRequest
+    ):
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 400
+        response_value.request = Request()
+        req.return_value = response_value
+        client.get_location(request)
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        locations_pb2.GetLocationRequest,
+        dict,
+    ],
+)
+def test_get_location_rest(request_type):
+    client = LookupServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+    request_init = {"name": "projects/sample1/locations/sample2"}
+    request = request_type(**request_init)
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = locations_pb2.Location()
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        json_return_value = json_format.MessageToJson(return_value)
+
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+
+        response = client.get_location(request)
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, locations_pb2.Location)
+
+
+def test_list_locations_rest_bad_request(
+    transport: str = "rest", request_type=locations_pb2.ListLocationsRequest
+):
+    client = LookupServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    request = request_type()
+    request = json_format.ParseDict({"name": "projects/sample1"}, request)
+
+    # Mock the http request call within the method and fake a BadRequest error.
+    with mock.patch.object(Session, "request") as req, pytest.raises(
+        core_exceptions.BadRequest
+    ):
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 400
+        response_value.request = Request()
+        req.return_value = response_value
+        client.list_locations(request)
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        locations_pb2.ListLocationsRequest,
+        dict,
+    ],
+)
+def test_list_locations_rest(request_type):
+    client = LookupServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+    request_init = {"name": "projects/sample1"}
+    request = request_type(**request_init)
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = locations_pb2.ListLocationsResponse()
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        json_return_value = json_format.MessageToJson(return_value)
+
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+
+        response = client.list_locations(request)
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, locations_pb2.ListLocationsResponse)
+
+
+def test_list_locations(transport: str = "grpc"):
+    client = LookupServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = locations_pb2.ListLocationsRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = locations_pb2.ListLocationsResponse()
+        response = client.list_locations(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, locations_pb2.ListLocationsResponse)
+
+
+@pytest.mark.asyncio
+async def test_list_locations_async(transport: str = "grpc"):
+    client = LookupServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = locations_pb2.ListLocationsRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            locations_pb2.ListLocationsResponse()
+        )
+        response = await client.list_locations(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, locations_pb2.ListLocationsResponse)
+
+
+def test_list_locations_field_headers():
+    client = LookupServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = locations_pb2.ListLocationsRequest()
+    request.name = "locations"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        call.return_value = locations_pb2.ListLocationsResponse()
+
+        client.list_locations(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=locations",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_list_locations_field_headers_async():
+    client = LookupServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = locations_pb2.ListLocationsRequest()
+    request.name = "locations"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            locations_pb2.ListLocationsResponse()
+        )
+        await client.list_locations(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=locations",
+    ) in kw["metadata"]
+
+
+def test_list_locations_from_dict():
+    client = LookupServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = locations_pb2.ListLocationsResponse()
+
+        response = client.list_locations(
+            request={
+                "name": "locations",
+            }
+        )
+        call.assert_called()
+
+
+@pytest.mark.asyncio
+async def test_list_locations_from_dict_async():
+    client = LookupServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            locations_pb2.ListLocationsResponse()
+        )
+        response = await client.list_locations(
+            request={
+                "name": "locations",
+            }
+        )
+        call.assert_called()
+
+
+def test_get_location(transport: str = "grpc"):
+    client = LookupServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = locations_pb2.GetLocationRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_location), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = locations_pb2.Location()
+        response = client.get_location(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, locations_pb2.Location)
+
+
+@pytest.mark.asyncio
+async def test_get_location_async(transport: str = "grpc_asyncio"):
+    client = LookupServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = locations_pb2.GetLocationRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_location), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            locations_pb2.Location()
+        )
+        response = await client.get_location(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, locations_pb2.Location)
+
+
+def test_get_location_field_headers():
+    client = LookupServiceClient(credentials=ga_credentials.AnonymousCredentials())
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = locations_pb2.GetLocationRequest()
+    request.name = "locations/abc"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_location), "__call__") as call:
+        call.return_value = locations_pb2.Location()
+
+        client.get_location(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=locations/abc",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_get_location_field_headers_async():
+    client = LookupServiceAsyncClient(credentials=ga_credentials.AnonymousCredentials())
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = locations_pb2.GetLocationRequest()
+    request.name = "locations/abc"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_location), "__call__") as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            locations_pb2.Location()
+        )
+        await client.get_location(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=locations/abc",
+    ) in kw["metadata"]
+
+
+def test_get_location_from_dict():
+    client = LookupServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = locations_pb2.Location()
+
+        response = client.get_location(
+            request={
+                "name": "locations/abc",
+            }
+        )
+        call.assert_called()
+
+
+@pytest.mark.asyncio
+async def test_get_location_from_dict_async():
+    client = LookupServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            locations_pb2.Location()
+        )
+        response = await client.get_location(
+            request={
+                "name": "locations",
+            }
+        )
+        call.assert_called()
+
+
 def test_transport_close():
     transports = {
         "rest": "_session",
         "grpc": "_grpc_channel",
     }
 
     for transport, close_name in transports.items():
```

### Comparing `google-cloud-service-directory-1.8.2/tests/unit/gapic/servicedirectory_v1/test_registration_service.py` & `google-cloud-service-directory-1.9.0/tests/unit/gapic/servicedirectory_v1/test_registration_service.py`

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
@@ -28,14 +28,15 @@
 
 from google.api_core import gapic_v1, grpc_helpers, grpc_helpers_async, path_template
 from google.api_core import client_options
 from google.api_core import exceptions as core_exceptions
 import google.auth
 from google.auth import credentials as ga_credentials
 from google.auth.exceptions import MutualTLSChannelError
+from google.cloud.location import locations_pb2
 from google.iam.v1 import iam_policy_pb2  # type: ignore
 from google.iam.v1 import options_pb2  # type: ignore
 from google.iam.v1 import policy_pb2  # type: ignore
 from google.oauth2 import service_account
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import json_format
 from google.type import expr_pb2  # type: ignore
@@ -777,25 +778,27 @@
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.create_namespace), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = gcs_namespace.Namespace(
             name="name_value",
+            uid="uid_value",
         )
         response = client.create_namespace(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == registration_service.CreateNamespaceRequest()
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, gcs_namespace.Namespace)
     assert response.name == "name_value"
+    assert response.uid == "uid_value"
 
 
 def test_create_namespace_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = RegistrationServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -826,26 +829,28 @@
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.create_namespace), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             gcs_namespace.Namespace(
                 name="name_value",
+                uid="uid_value",
             )
         )
         response = await client.create_namespace(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == registration_service.CreateNamespaceRequest()
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, gcs_namespace.Namespace)
     assert response.name == "name_value"
+    assert response.uid == "uid_value"
 
 
 @pytest.mark.asyncio
 async def test_create_namespace_async_from_dict():
     await test_create_namespace_async(request_type=dict)
 
 
@@ -1453,25 +1458,27 @@
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_namespace), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = namespace.Namespace(
             name="name_value",
+            uid="uid_value",
         )
         response = client.get_namespace(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == registration_service.GetNamespaceRequest()
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, namespace.Namespace)
     assert response.name == "name_value"
+    assert response.uid == "uid_value"
 
 
 def test_get_namespace_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = RegistrationServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -1502,26 +1509,28 @@
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_namespace), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             namespace.Namespace(
                 name="name_value",
+                uid="uid_value",
             )
         )
         response = await client.get_namespace(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == registration_service.GetNamespaceRequest()
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, namespace.Namespace)
     assert response.name == "name_value"
+    assert response.uid == "uid_value"
 
 
 @pytest.mark.asyncio
 async def test_get_namespace_async_from_dict():
     await test_get_namespace_async(request_type=dict)
 
 
@@ -1682,25 +1691,27 @@
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.update_namespace), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = gcs_namespace.Namespace(
             name="name_value",
+            uid="uid_value",
         )
         response = client.update_namespace(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == registration_service.UpdateNamespaceRequest()
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, gcs_namespace.Namespace)
     assert response.name == "name_value"
+    assert response.uid == "uid_value"
 
 
 def test_update_namespace_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = RegistrationServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -1731,26 +1742,28 @@
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.update_namespace), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             gcs_namespace.Namespace(
                 name="name_value",
+                uid="uid_value",
             )
         )
         response = await client.update_namespace(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == registration_service.UpdateNamespaceRequest()
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, gcs_namespace.Namespace)
     assert response.name == "name_value"
+    assert response.uid == "uid_value"
 
 
 @pytest.mark.asyncio
 async def test_update_namespace_async_from_dict():
     await test_update_namespace_async(request_type=dict)
 
 
@@ -2146,25 +2159,27 @@
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.create_service), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = gcs_service.Service(
             name="name_value",
+            uid="uid_value",
         )
         response = client.create_service(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == registration_service.CreateServiceRequest()
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, gcs_service.Service)
     assert response.name == "name_value"
+    assert response.uid == "uid_value"
 
 
 def test_create_service_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = RegistrationServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -2195,26 +2210,28 @@
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.create_service), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             gcs_service.Service(
                 name="name_value",
+                uid="uid_value",
             )
         )
         response = await client.create_service(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == registration_service.CreateServiceRequest()
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, gcs_service.Service)
     assert response.name == "name_value"
+    assert response.uid == "uid_value"
 
 
 @pytest.mark.asyncio
 async def test_create_service_async_from_dict():
     await test_create_service_async(request_type=dict)
 
 
@@ -2818,25 +2835,27 @@
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_service), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = service.Service(
             name="name_value",
+            uid="uid_value",
         )
         response = client.get_service(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == registration_service.GetServiceRequest()
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, service.Service)
     assert response.name == "name_value"
+    assert response.uid == "uid_value"
 
 
 def test_get_service_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = RegistrationServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -2866,26 +2885,28 @@
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_service), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             service.Service(
                 name="name_value",
+                uid="uid_value",
             )
         )
         response = await client.get_service(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == registration_service.GetServiceRequest()
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, service.Service)
     assert response.name == "name_value"
+    assert response.uid == "uid_value"
 
 
 @pytest.mark.asyncio
 async def test_get_service_async_from_dict():
     await test_get_service_async(request_type=dict)
 
 
@@ -3046,25 +3067,27 @@
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.update_service), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = gcs_service.Service(
             name="name_value",
+            uid="uid_value",
         )
         response = client.update_service(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == registration_service.UpdateServiceRequest()
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, gcs_service.Service)
     assert response.name == "name_value"
+    assert response.uid == "uid_value"
 
 
 def test_update_service_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = RegistrationServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -3095,26 +3118,28 @@
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.update_service), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             gcs_service.Service(
                 name="name_value",
+                uid="uid_value",
             )
         )
         response = await client.update_service(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == registration_service.UpdateServiceRequest()
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, gcs_service.Service)
     assert response.name == "name_value"
+    assert response.uid == "uid_value"
 
 
 @pytest.mark.asyncio
 async def test_update_service_async_from_dict():
     await test_update_service_async(request_type=dict)
 
 
@@ -3508,27 +3533,31 @@
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.create_endpoint), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = gcs_endpoint.Endpoint(
             name="name_value",
             address="address_value",
             port=453,
+            network="network_value",
+            uid="uid_value",
         )
         response = client.create_endpoint(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == registration_service.CreateEndpointRequest()
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, gcs_endpoint.Endpoint)
     assert response.name == "name_value"
     assert response.address == "address_value"
     assert response.port == 453
+    assert response.network == "network_value"
+    assert response.uid == "uid_value"
 
 
 def test_create_endpoint_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = RegistrationServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -3561,28 +3590,32 @@
     with mock.patch.object(type(client.transport.create_endpoint), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             gcs_endpoint.Endpoint(
                 name="name_value",
                 address="address_value",
                 port=453,
+                network="network_value",
+                uid="uid_value",
             )
         )
         response = await client.create_endpoint(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == registration_service.CreateEndpointRequest()
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, gcs_endpoint.Endpoint)
     assert response.name == "name_value"
     assert response.address == "address_value"
     assert response.port == 453
+    assert response.network == "network_value"
+    assert response.uid == "uid_value"
 
 
 @pytest.mark.asyncio
 async def test_create_endpoint_async_from_dict():
     await test_create_endpoint_async(request_type=dict)
 
 
@@ -4192,27 +4225,31 @@
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_endpoint), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = endpoint.Endpoint(
             name="name_value",
             address="address_value",
             port=453,
+            network="network_value",
+            uid="uid_value",
         )
         response = client.get_endpoint(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == registration_service.GetEndpointRequest()
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, endpoint.Endpoint)
     assert response.name == "name_value"
     assert response.address == "address_value"
     assert response.port == 453
+    assert response.network == "network_value"
+    assert response.uid == "uid_value"
 
 
 def test_get_endpoint_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = RegistrationServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -4245,28 +4282,32 @@
     with mock.patch.object(type(client.transport.get_endpoint), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             endpoint.Endpoint(
                 name="name_value",
                 address="address_value",
                 port=453,
+                network="network_value",
+                uid="uid_value",
             )
         )
         response = await client.get_endpoint(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == registration_service.GetEndpointRequest()
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, endpoint.Endpoint)
     assert response.name == "name_value"
     assert response.address == "address_value"
     assert response.port == 453
+    assert response.network == "network_value"
+    assert response.uid == "uid_value"
 
 
 @pytest.mark.asyncio
 async def test_get_endpoint_async_from_dict():
     await test_get_endpoint_async(request_type=dict)
 
 
@@ -4429,27 +4470,31 @@
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.update_endpoint), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = gcs_endpoint.Endpoint(
             name="name_value",
             address="address_value",
             port=453,
+            network="network_value",
+            uid="uid_value",
         )
         response = client.update_endpoint(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == registration_service.UpdateEndpointRequest()
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, gcs_endpoint.Endpoint)
     assert response.name == "name_value"
     assert response.address == "address_value"
     assert response.port == 453
+    assert response.network == "network_value"
+    assert response.uid == "uid_value"
 
 
 def test_update_endpoint_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = RegistrationServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -4482,28 +4527,32 @@
     with mock.patch.object(type(client.transport.update_endpoint), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             gcs_endpoint.Endpoint(
                 name="name_value",
                 address="address_value",
                 port=453,
+                network="network_value",
+                uid="uid_value",
             )
         )
         response = await client.update_endpoint(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == registration_service.UpdateEndpointRequest()
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, gcs_endpoint.Endpoint)
     assert response.name == "name_value"
     assert response.address == "address_value"
     assert response.port == 453
+    assert response.network == "network_value"
+    assert response.uid == "uid_value"
 
 
 @pytest.mark.asyncio
 async def test_update_endpoint_async_from_dict():
     await test_update_endpoint_async(request_type=dict)
 
 
@@ -5411,22 +5460,23 @@
     client = RegistrationServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="rest",
     )
 
     # send a request that will satisfy transcoding
     request_init = {"parent": "projects/sample1/locations/sample2"}
-    request_init["namespace"] = {"name": "name_value", "labels": {}}
+    request_init["namespace"] = {"name": "name_value", "labels": {}, "uid": "uid_value"}
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = gcs_namespace.Namespace(
             name="name_value",
+            uid="uid_value",
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = gcs_namespace.Namespace.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -5434,14 +5484,15 @@
         response_value._content = json_return_value.encode("UTF-8")
         req.return_value = response_value
         response = client.create_namespace(request)
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, gcs_namespace.Namespace)
     assert response.name == "name_value"
+    assert response.uid == "uid_value"
 
 
 def test_create_namespace_rest_required_fields(
     request_type=registration_service.CreateNamespaceRequest,
 ):
     transport_class = transports.RegistrationServiceRestTransport
 
@@ -5614,15 +5665,15 @@
     client = RegistrationServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
 
     # send a request that will satisfy transcoding
     request_init = {"parent": "projects/sample1/locations/sample2"}
-    request_init["namespace"] = {"name": "name_value", "labels": {}}
+    request_init["namespace"] = {"name": "name_value", "labels": {}, "uid": "uid_value"}
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a BadRequest error.
     with mock.patch.object(Session, "request") as req, pytest.raises(
         core_exceptions.BadRequest
     ):
         # Wrap the value into a proper Response obj
@@ -6061,14 +6112,15 @@
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = namespace.Namespace(
             name="name_value",
+            uid="uid_value",
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = namespace.Namespace.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -6076,14 +6128,15 @@
         response_value._content = json_return_value.encode("UTF-8")
         req.return_value = response_value
         response = client.get_namespace(request)
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, namespace.Namespace)
     assert response.name == "name_value"
+    assert response.uid == "uid_value"
 
 
 def test_get_namespace_rest_required_fields(
     request_type=registration_service.GetNamespaceRequest,
 ):
     transport_class = transports.RegistrationServiceRestTransport
 
@@ -6326,22 +6379,24 @@
     # send a request that will satisfy transcoding
     request_init = {
         "namespace": {"name": "projects/sample1/locations/sample2/namespaces/sample3"}
     }
     request_init["namespace"] = {
         "name": "projects/sample1/locations/sample2/namespaces/sample3",
         "labels": {},
+        "uid": "uid_value",
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = gcs_namespace.Namespace(
             name="name_value",
+            uid="uid_value",
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = gcs_namespace.Namespace.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -6349,14 +6404,15 @@
         response_value._content = json_return_value.encode("UTF-8")
         req.return_value = response_value
         response = client.update_namespace(request)
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, gcs_namespace.Namespace)
     assert response.name == "name_value"
+    assert response.uid == "uid_value"
 
 
 def test_update_namespace_rest_required_fields(
     request_type=registration_service.UpdateNamespaceRequest,
 ):
     transport_class = transports.RegistrationServiceRestTransport
 
@@ -6515,14 +6571,15 @@
     # send a request that will satisfy transcoding
     request_init = {
         "namespace": {"name": "projects/sample1/locations/sample2/namespaces/sample3"}
     }
     request_init["namespace"] = {
         "name": "projects/sample1/locations/sample2/namespaces/sample3",
         "labels": {},
+        "uid": "uid_value",
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a BadRequest error.
     with mock.patch.object(Session, "request") as req, pytest.raises(
         core_exceptions.BadRequest
     ):
@@ -6876,24 +6933,28 @@
         "annotations": {},
         "endpoints": [
             {
                 "name": "name_value",
                 "address": "address_value",
                 "port": 453,
                 "annotations": {},
+                "network": "network_value",
+                "uid": "uid_value",
             }
         ],
+        "uid": "uid_value",
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = gcs_service.Service(
             name="name_value",
+            uid="uid_value",
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = gcs_service.Service.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -6901,14 +6962,15 @@
         response_value._content = json_return_value.encode("UTF-8")
         req.return_value = response_value
         response = client.create_service(request)
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, gcs_service.Service)
     assert response.name == "name_value"
+    assert response.uid == "uid_value"
 
 
 def test_create_service_rest_required_fields(
     request_type=registration_service.CreateServiceRequest,
 ):
     transport_class = transports.RegistrationServiceRestTransport
 
@@ -7088,16 +7150,19 @@
         "annotations": {},
         "endpoints": [
             {
                 "name": "name_value",
                 "address": "address_value",
                 "port": 453,
                 "annotations": {},
+                "network": "network_value",
+                "uid": "uid_value",
             }
         ],
+        "uid": "uid_value",
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a BadRequest error.
     with mock.patch.object(Session, "request") as req, pytest.raises(
         core_exceptions.BadRequest
     ):
@@ -7545,14 +7610,15 @@
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = service.Service(
             name="name_value",
+            uid="uid_value",
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = service.Service.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -7560,14 +7626,15 @@
         response_value._content = json_return_value.encode("UTF-8")
         req.return_value = response_value
         response = client.get_service(request)
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, service.Service)
     assert response.name == "name_value"
+    assert response.uid == "uid_value"
 
 
 def test_get_service_rest_required_fields(
     request_type=registration_service.GetServiceRequest,
 ):
     transport_class = transports.RegistrationServiceRestTransport
 
@@ -7821,24 +7888,28 @@
         "annotations": {},
         "endpoints": [
             {
                 "name": "name_value",
                 "address": "address_value",
                 "port": 453,
                 "annotations": {},
+                "network": "network_value",
+                "uid": "uid_value",
             }
         ],
+        "uid": "uid_value",
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = gcs_service.Service(
             name="name_value",
+            uid="uid_value",
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = gcs_service.Service.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -7846,14 +7917,15 @@
         response_value._content = json_return_value.encode("UTF-8")
         req.return_value = response_value
         response = client.update_service(request)
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, gcs_service.Service)
     assert response.name == "name_value"
+    assert response.uid == "uid_value"
 
 
 def test_update_service_rest_required_fields(
     request_type=registration_service.UpdateServiceRequest,
 ):
     transport_class = transports.RegistrationServiceRestTransport
 
@@ -8018,16 +8090,19 @@
         "annotations": {},
         "endpoints": [
             {
                 "name": "name_value",
                 "address": "address_value",
                 "port": 453,
                 "annotations": {},
+                "network": "network_value",
+                "uid": "uid_value",
             }
         ],
+        "uid": "uid_value",
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a BadRequest error.
     with mock.patch.object(Session, "request") as req, pytest.raises(
         core_exceptions.BadRequest
     ):
@@ -8384,24 +8459,28 @@
         "parent": "projects/sample1/locations/sample2/namespaces/sample3/services/sample4"
     }
     request_init["endpoint"] = {
         "name": "name_value",
         "address": "address_value",
         "port": 453,
         "annotations": {},
+        "network": "network_value",
+        "uid": "uid_value",
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = gcs_endpoint.Endpoint(
             name="name_value",
             address="address_value",
             port=453,
+            network="network_value",
+            uid="uid_value",
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = gcs_endpoint.Endpoint.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -8411,14 +8490,16 @@
         response = client.create_endpoint(request)
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, gcs_endpoint.Endpoint)
     assert response.name == "name_value"
     assert response.address == "address_value"
     assert response.port == 453
+    assert response.network == "network_value"
+    assert response.uid == "uid_value"
 
 
 def test_create_endpoint_rest_required_fields(
     request_type=registration_service.CreateEndpointRequest,
 ):
     transport_class = transports.RegistrationServiceRestTransport
 
@@ -8598,14 +8679,16 @@
         "parent": "projects/sample1/locations/sample2/namespaces/sample3/services/sample4"
     }
     request_init["endpoint"] = {
         "name": "name_value",
         "address": "address_value",
         "port": 453,
         "annotations": {},
+        "network": "network_value",
+        "uid": "uid_value",
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a BadRequest error.
     with mock.patch.object(Session, "request") as req, pytest.raises(
         core_exceptions.BadRequest
     ):
@@ -9061,14 +9144,16 @@
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = endpoint.Endpoint(
             name="name_value",
             address="address_value",
             port=453,
+            network="network_value",
+            uid="uid_value",
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = endpoint.Endpoint.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -9078,14 +9163,16 @@
         response = client.get_endpoint(request)
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, endpoint.Endpoint)
     assert response.name == "name_value"
     assert response.address == "address_value"
     assert response.port == 453
+    assert response.network == "network_value"
+    assert response.uid == "uid_value"
 
 
 def test_get_endpoint_rest_required_fields(
     request_type=registration_service.GetEndpointRequest,
 ):
     transport_class = transports.RegistrationServiceRestTransport
 
@@ -9335,24 +9422,28 @@
         }
     }
     request_init["endpoint"] = {
         "name": "projects/sample1/locations/sample2/namespaces/sample3/services/sample4/endpoints/sample5",
         "address": "address_value",
         "port": 453,
         "annotations": {},
+        "network": "network_value",
+        "uid": "uid_value",
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = gcs_endpoint.Endpoint(
             name="name_value",
             address="address_value",
             port=453,
+            network="network_value",
+            uid="uid_value",
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = gcs_endpoint.Endpoint.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -9362,14 +9453,16 @@
         response = client.update_endpoint(request)
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, gcs_endpoint.Endpoint)
     assert response.name == "name_value"
     assert response.address == "address_value"
     assert response.port == 453
+    assert response.network == "network_value"
+    assert response.uid == "uid_value"
 
 
 def test_update_endpoint_rest_required_fields(
     request_type=registration_service.UpdateEndpointRequest,
 ):
     transport_class = transports.RegistrationServiceRestTransport
 
@@ -9532,14 +9625,16 @@
         }
     }
     request_init["endpoint"] = {
         "name": "projects/sample1/locations/sample2/namespaces/sample3/services/sample4/endpoints/sample5",
         "address": "address_value",
         "port": 453,
         "annotations": {},
+        "network": "network_value",
+        "uid": "uid_value",
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a BadRequest error.
     with mock.patch.object(Session, "request") as req, pytest.raises(
         core_exceptions.BadRequest
     ):
@@ -10684,14 +10779,16 @@
         "list_endpoints",
         "get_endpoint",
         "update_endpoint",
         "delete_endpoint",
         "get_iam_policy",
         "set_iam_policy",
         "test_iam_permissions",
+        "get_location",
+        "list_locations",
     )
     for method in methods:
         with pytest.raises(NotImplementedError):
             getattr(transport, method)(request=object())
 
     with pytest.raises(NotImplementedError):
         transport.close()
@@ -11186,140 +11283,163 @@
     path = RegistrationServiceClient.namespace_path(**expected)
 
     # Check that the path construction is reversible.
     actual = RegistrationServiceClient.parse_namespace_path(path)
     assert expected == actual
 
 
-def test_service_path():
+def test_network_path():
     project = "oyster"
-    location = "nudibranch"
-    namespace = "cuttlefish"
-    service = "mussel"
+    network = "nudibranch"
+    expected = "projects/{project}/locations/global/networks/{network}".format(
+        project=project,
+        network=network,
+    )
+    actual = RegistrationServiceClient.network_path(project, network)
+    assert expected == actual
+
+
+def test_parse_network_path():
+    expected = {
+        "project": "cuttlefish",
+        "network": "mussel",
+    }
+    path = RegistrationServiceClient.network_path(**expected)
+
+    # Check that the path construction is reversible.
+    actual = RegistrationServiceClient.parse_network_path(path)
+    assert expected == actual
+
+
+def test_service_path():
+    project = "winkle"
+    location = "nautilus"
+    namespace = "scallop"
+    service = "abalone"
     expected = "projects/{project}/locations/{location}/namespaces/{namespace}/services/{service}".format(
         project=project,
         location=location,
         namespace=namespace,
         service=service,
     )
     actual = RegistrationServiceClient.service_path(
         project, location, namespace, service
     )
     assert expected == actual
 
 
 def test_parse_service_path():
     expected = {
-        "project": "winkle",
-        "location": "nautilus",
-        "namespace": "scallop",
-        "service": "abalone",
+        "project": "squid",
+        "location": "clam",
+        "namespace": "whelk",
+        "service": "octopus",
     }
     path = RegistrationServiceClient.service_path(**expected)
 
     # Check that the path construction is reversible.
     actual = RegistrationServiceClient.parse_service_path(path)
     assert expected == actual
 
 
 def test_common_billing_account_path():
-    billing_account = "squid"
+    billing_account = "oyster"
     expected = "billingAccounts/{billing_account}".format(
         billing_account=billing_account,
     )
     actual = RegistrationServiceClient.common_billing_account_path(billing_account)
     assert expected == actual
 
 
 def test_parse_common_billing_account_path():
     expected = {
-        "billing_account": "clam",
+        "billing_account": "nudibranch",
     }
     path = RegistrationServiceClient.common_billing_account_path(**expected)
 
     # Check that the path construction is reversible.
     actual = RegistrationServiceClient.parse_common_billing_account_path(path)
     assert expected == actual
 
 
 def test_common_folder_path():
-    folder = "whelk"
+    folder = "cuttlefish"
     expected = "folders/{folder}".format(
         folder=folder,
     )
     actual = RegistrationServiceClient.common_folder_path(folder)
     assert expected == actual
 
 
 def test_parse_common_folder_path():
     expected = {
-        "folder": "octopus",
+        "folder": "mussel",
     }
     path = RegistrationServiceClient.common_folder_path(**expected)
 
     # Check that the path construction is reversible.
     actual = RegistrationServiceClient.parse_common_folder_path(path)
     assert expected == actual
 
 
 def test_common_organization_path():
-    organization = "oyster"
+    organization = "winkle"
     expected = "organizations/{organization}".format(
         organization=organization,
     )
     actual = RegistrationServiceClient.common_organization_path(organization)
     assert expected == actual
 
 
 def test_parse_common_organization_path():
     expected = {
-        "organization": "nudibranch",
+        "organization": "nautilus",
     }
     path = RegistrationServiceClient.common_organization_path(**expected)
 
     # Check that the path construction is reversible.
     actual = RegistrationServiceClient.parse_common_organization_path(path)
     assert expected == actual
 
 
 def test_common_project_path():
-    project = "cuttlefish"
+    project = "scallop"
     expected = "projects/{project}".format(
         project=project,
     )
     actual = RegistrationServiceClient.common_project_path(project)
     assert expected == actual
 
 
 def test_parse_common_project_path():
     expected = {
-        "project": "mussel",
+        "project": "abalone",
     }
     path = RegistrationServiceClient.common_project_path(**expected)
 
     # Check that the path construction is reversible.
     actual = RegistrationServiceClient.parse_common_project_path(path)
     assert expected == actual
 
 
 def test_common_location_path():
-    project = "winkle"
-    location = "nautilus"
+    project = "squid"
+    location = "clam"
     expected = "projects/{project}/locations/{location}".format(
         project=project,
         location=location,
     )
     actual = RegistrationServiceClient.common_location_path(project, location)
     assert expected == actual
 
 
 def test_parse_common_location_path():
     expected = {
-        "project": "scallop",
-        "location": "abalone",
+        "project": "whelk",
+        "location": "octopus",
     }
     path = RegistrationServiceClient.common_location_path(**expected)
 
     # Check that the path construction is reversible.
     actual = RegistrationServiceClient.parse_common_location_path(path)
     assert expected == actual
 
@@ -11357,14 +11477,418 @@
         type(getattr(client.transport, "grpc_channel")), "close"
     ) as close:
         async with client:
             close.assert_not_called()
         close.assert_called_once()
 
 
+def test_get_location_rest_bad_request(
+    transport: str = "rest", request_type=locations_pb2.GetLocationRequest
+):
+    client = RegistrationServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    request = request_type()
+    request = json_format.ParseDict(
+        {"name": "projects/sample1/locations/sample2"}, request
+    )
+
+    # Mock the http request call within the method and fake a BadRequest error.
+    with mock.patch.object(Session, "request") as req, pytest.raises(
+        core_exceptions.BadRequest
+    ):
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 400
+        response_value.request = Request()
+        req.return_value = response_value
+        client.get_location(request)
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        locations_pb2.GetLocationRequest,
+        dict,
+    ],
+)
+def test_get_location_rest(request_type):
+    client = RegistrationServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+    request_init = {"name": "projects/sample1/locations/sample2"}
+    request = request_type(**request_init)
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = locations_pb2.Location()
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        json_return_value = json_format.MessageToJson(return_value)
+
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+
+        response = client.get_location(request)
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, locations_pb2.Location)
+
+
+def test_list_locations_rest_bad_request(
+    transport: str = "rest", request_type=locations_pb2.ListLocationsRequest
+):
+    client = RegistrationServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    request = request_type()
+    request = json_format.ParseDict({"name": "projects/sample1"}, request)
+
+    # Mock the http request call within the method and fake a BadRequest error.
+    with mock.patch.object(Session, "request") as req, pytest.raises(
+        core_exceptions.BadRequest
+    ):
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 400
+        response_value.request = Request()
+        req.return_value = response_value
+        client.list_locations(request)
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        locations_pb2.ListLocationsRequest,
+        dict,
+    ],
+)
+def test_list_locations_rest(request_type):
+    client = RegistrationServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+    request_init = {"name": "projects/sample1"}
+    request = request_type(**request_init)
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = locations_pb2.ListLocationsResponse()
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        json_return_value = json_format.MessageToJson(return_value)
+
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+
+        response = client.list_locations(request)
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, locations_pb2.ListLocationsResponse)
+
+
+def test_list_locations(transport: str = "grpc"):
+    client = RegistrationServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = locations_pb2.ListLocationsRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = locations_pb2.ListLocationsResponse()
+        response = client.list_locations(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, locations_pb2.ListLocationsResponse)
+
+
+@pytest.mark.asyncio
+async def test_list_locations_async(transport: str = "grpc"):
+    client = RegistrationServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = locations_pb2.ListLocationsRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            locations_pb2.ListLocationsResponse()
+        )
+        response = await client.list_locations(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, locations_pb2.ListLocationsResponse)
+
+
+def test_list_locations_field_headers():
+    client = RegistrationServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = locations_pb2.ListLocationsRequest()
+    request.name = "locations"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        call.return_value = locations_pb2.ListLocationsResponse()
+
+        client.list_locations(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=locations",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_list_locations_field_headers_async():
+    client = RegistrationServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = locations_pb2.ListLocationsRequest()
+    request.name = "locations"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            locations_pb2.ListLocationsResponse()
+        )
+        await client.list_locations(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=locations",
+    ) in kw["metadata"]
+
+
+def test_list_locations_from_dict():
+    client = RegistrationServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = locations_pb2.ListLocationsResponse()
+
+        response = client.list_locations(
+            request={
+                "name": "locations",
+            }
+        )
+        call.assert_called()
+
+
+@pytest.mark.asyncio
+async def test_list_locations_from_dict_async():
+    client = RegistrationServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            locations_pb2.ListLocationsResponse()
+        )
+        response = await client.list_locations(
+            request={
+                "name": "locations",
+            }
+        )
+        call.assert_called()
+
+
+def test_get_location(transport: str = "grpc"):
+    client = RegistrationServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = locations_pb2.GetLocationRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_location), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = locations_pb2.Location()
+        response = client.get_location(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, locations_pb2.Location)
+
+
+@pytest.mark.asyncio
+async def test_get_location_async(transport: str = "grpc_asyncio"):
+    client = RegistrationServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = locations_pb2.GetLocationRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_location), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            locations_pb2.Location()
+        )
+        response = await client.get_location(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, locations_pb2.Location)
+
+
+def test_get_location_field_headers():
+    client = RegistrationServiceClient(
+        credentials=ga_credentials.AnonymousCredentials()
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = locations_pb2.GetLocationRequest()
+    request.name = "locations/abc"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_location), "__call__") as call:
+        call.return_value = locations_pb2.Location()
+
+        client.get_location(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=locations/abc",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_get_location_field_headers_async():
+    client = RegistrationServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials()
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = locations_pb2.GetLocationRequest()
+    request.name = "locations/abc"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_location), "__call__") as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            locations_pb2.Location()
+        )
+        await client.get_location(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=locations/abc",
+    ) in kw["metadata"]
+
+
+def test_get_location_from_dict():
+    client = RegistrationServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = locations_pb2.Location()
+
+        response = client.get_location(
+            request={
+                "name": "locations/abc",
+            }
+        )
+        call.assert_called()
+
+
+@pytest.mark.asyncio
+async def test_get_location_from_dict_async():
+    client = RegistrationServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            locations_pb2.Location()
+        )
+        response = await client.get_location(
+            request={
+                "name": "locations",
+            }
+        )
+        call.assert_called()
+
+
 def test_transport_close():
     transports = {
         "rest": "_session",
         "grpc": "_grpc_channel",
     }
 
     for transport, close_name in transports.items():
```

### Comparing `google-cloud-service-directory-1.8.2/tests/unit/gapic/servicedirectory_v1beta1/test_lookup_service.py` & `google-cloud-service-directory-1.9.0/tests/unit/gapic/servicedirectory_v1beta1/test_lookup_service.py`

 * *Files 18% similar despite different names*

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
@@ -28,14 +28,15 @@
 
 from google.api_core import gapic_v1, grpc_helpers, grpc_helpers_async, path_template
 from google.api_core import client_options
 from google.api_core import exceptions as core_exceptions
 import google.auth
 from google.auth import credentials as ga_credentials
 from google.auth.exceptions import MutualTLSChannelError
+from google.cloud.location import locations_pb2
 from google.oauth2 import service_account
 from google.protobuf import json_format
 import grpc
 from grpc.experimental import aio
 from proto.marshal.rules import wrappers
 from proto.marshal.rules.dates import DurationRule, TimestampRule
 import pytest
@@ -1193,15 +1194,19 @@
         Transport.return_value = None
         transport = transports.LookupServiceTransport(
             credentials=ga_credentials.AnonymousCredentials(),
         )
 
     # Every method on the transport should just blindly
     # raise NotImplementedError.
-    methods = ("resolve_service",)
+    methods = (
+        "resolve_service",
+        "get_location",
+        "list_locations",
+    )
     for method in methods:
         with pytest.raises(NotImplementedError):
             getattr(transport, method)(request=object())
 
     with pytest.raises(NotImplementedError):
         transport.close()
 
@@ -1806,14 +1811,414 @@
         type(getattr(client.transport, "grpc_channel")), "close"
     ) as close:
         async with client:
             close.assert_not_called()
         close.assert_called_once()
 
 
+def test_get_location_rest_bad_request(
+    transport: str = "rest", request_type=locations_pb2.GetLocationRequest
+):
+    client = LookupServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    request = request_type()
+    request = json_format.ParseDict(
+        {"name": "projects/sample1/locations/sample2"}, request
+    )
+
+    # Mock the http request call within the method and fake a BadRequest error.
+    with mock.patch.object(Session, "request") as req, pytest.raises(
+        core_exceptions.BadRequest
+    ):
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 400
+        response_value.request = Request()
+        req.return_value = response_value
+        client.get_location(request)
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        locations_pb2.GetLocationRequest,
+        dict,
+    ],
+)
+def test_get_location_rest(request_type):
+    client = LookupServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+    request_init = {"name": "projects/sample1/locations/sample2"}
+    request = request_type(**request_init)
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = locations_pb2.Location()
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        json_return_value = json_format.MessageToJson(return_value)
+
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+
+        response = client.get_location(request)
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, locations_pb2.Location)
+
+
+def test_list_locations_rest_bad_request(
+    transport: str = "rest", request_type=locations_pb2.ListLocationsRequest
+):
+    client = LookupServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    request = request_type()
+    request = json_format.ParseDict({"name": "projects/sample1"}, request)
+
+    # Mock the http request call within the method and fake a BadRequest error.
+    with mock.patch.object(Session, "request") as req, pytest.raises(
+        core_exceptions.BadRequest
+    ):
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 400
+        response_value.request = Request()
+        req.return_value = response_value
+        client.list_locations(request)
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        locations_pb2.ListLocationsRequest,
+        dict,
+    ],
+)
+def test_list_locations_rest(request_type):
+    client = LookupServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+    request_init = {"name": "projects/sample1"}
+    request = request_type(**request_init)
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = locations_pb2.ListLocationsResponse()
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        json_return_value = json_format.MessageToJson(return_value)
+
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+
+        response = client.list_locations(request)
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, locations_pb2.ListLocationsResponse)
+
+
+def test_list_locations(transport: str = "grpc"):
+    client = LookupServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = locations_pb2.ListLocationsRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = locations_pb2.ListLocationsResponse()
+        response = client.list_locations(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, locations_pb2.ListLocationsResponse)
+
+
+@pytest.mark.asyncio
+async def test_list_locations_async(transport: str = "grpc"):
+    client = LookupServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = locations_pb2.ListLocationsRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            locations_pb2.ListLocationsResponse()
+        )
+        response = await client.list_locations(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, locations_pb2.ListLocationsResponse)
+
+
+def test_list_locations_field_headers():
+    client = LookupServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = locations_pb2.ListLocationsRequest()
+    request.name = "locations"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        call.return_value = locations_pb2.ListLocationsResponse()
+
+        client.list_locations(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=locations",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_list_locations_field_headers_async():
+    client = LookupServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = locations_pb2.ListLocationsRequest()
+    request.name = "locations"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            locations_pb2.ListLocationsResponse()
+        )
+        await client.list_locations(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=locations",
+    ) in kw["metadata"]
+
+
+def test_list_locations_from_dict():
+    client = LookupServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = locations_pb2.ListLocationsResponse()
+
+        response = client.list_locations(
+            request={
+                "name": "locations",
+            }
+        )
+        call.assert_called()
+
+
+@pytest.mark.asyncio
+async def test_list_locations_from_dict_async():
+    client = LookupServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            locations_pb2.ListLocationsResponse()
+        )
+        response = await client.list_locations(
+            request={
+                "name": "locations",
+            }
+        )
+        call.assert_called()
+
+
+def test_get_location(transport: str = "grpc"):
+    client = LookupServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = locations_pb2.GetLocationRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_location), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = locations_pb2.Location()
+        response = client.get_location(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, locations_pb2.Location)
+
+
+@pytest.mark.asyncio
+async def test_get_location_async(transport: str = "grpc_asyncio"):
+    client = LookupServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = locations_pb2.GetLocationRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_location), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            locations_pb2.Location()
+        )
+        response = await client.get_location(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, locations_pb2.Location)
+
+
+def test_get_location_field_headers():
+    client = LookupServiceClient(credentials=ga_credentials.AnonymousCredentials())
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = locations_pb2.GetLocationRequest()
+    request.name = "locations/abc"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_location), "__call__") as call:
+        call.return_value = locations_pb2.Location()
+
+        client.get_location(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=locations/abc",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_get_location_field_headers_async():
+    client = LookupServiceAsyncClient(credentials=ga_credentials.AnonymousCredentials())
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = locations_pb2.GetLocationRequest()
+    request.name = "locations/abc"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_location), "__call__") as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            locations_pb2.Location()
+        )
+        await client.get_location(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=locations/abc",
+    ) in kw["metadata"]
+
+
+def test_get_location_from_dict():
+    client = LookupServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = locations_pb2.Location()
+
+        response = client.get_location(
+            request={
+                "name": "locations/abc",
+            }
+        )
+        call.assert_called()
+
+
+@pytest.mark.asyncio
+async def test_get_location_from_dict_async():
+    client = LookupServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            locations_pb2.Location()
+        )
+        response = await client.get_location(
+            request={
+                "name": "locations",
+            }
+        )
+        call.assert_called()
+
+
 def test_transport_close():
     transports = {
         "rest": "_session",
         "grpc": "_grpc_channel",
     }
 
     for transport, close_name in transports.items():
```

### Comparing `google-cloud-service-directory-1.8.2/tests/unit/gapic/servicedirectory_v1beta1/test_registration_service.py` & `google-cloud-service-directory-1.9.0/tests/unit/gapic/servicedirectory_v1beta1/test_registration_service.py`

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
@@ -28,14 +28,15 @@
 
 from google.api_core import gapic_v1, grpc_helpers, grpc_helpers_async, path_template
 from google.api_core import client_options
 from google.api_core import exceptions as core_exceptions
 import google.auth
 from google.auth import credentials as ga_credentials
 from google.auth.exceptions import MutualTLSChannelError
+from google.cloud.location import locations_pb2
 from google.iam.v1 import iam_policy_pb2  # type: ignore
 from google.iam.v1 import options_pb2  # type: ignore
 from google.iam.v1 import policy_pb2  # type: ignore
 from google.oauth2 import service_account
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import json_format
 from google.protobuf import timestamp_pb2  # type: ignore
@@ -778,25 +779,27 @@
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.create_namespace), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = gcs_namespace.Namespace(
             name="name_value",
+            uid="uid_value",
         )
         response = client.create_namespace(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == registration_service.CreateNamespaceRequest()
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, gcs_namespace.Namespace)
     assert response.name == "name_value"
+    assert response.uid == "uid_value"
 
 
 def test_create_namespace_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = RegistrationServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -827,26 +830,28 @@
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.create_namespace), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             gcs_namespace.Namespace(
                 name="name_value",
+                uid="uid_value",
             )
         )
         response = await client.create_namespace(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == registration_service.CreateNamespaceRequest()
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, gcs_namespace.Namespace)
     assert response.name == "name_value"
+    assert response.uid == "uid_value"
 
 
 @pytest.mark.asyncio
 async def test_create_namespace_async_from_dict():
     await test_create_namespace_async(request_type=dict)
 
 
@@ -1454,25 +1459,27 @@
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_namespace), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = namespace.Namespace(
             name="name_value",
+            uid="uid_value",
         )
         response = client.get_namespace(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == registration_service.GetNamespaceRequest()
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, namespace.Namespace)
     assert response.name == "name_value"
+    assert response.uid == "uid_value"
 
 
 def test_get_namespace_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = RegistrationServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -1503,26 +1510,28 @@
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_namespace), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             namespace.Namespace(
                 name="name_value",
+                uid="uid_value",
             )
         )
         response = await client.get_namespace(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == registration_service.GetNamespaceRequest()
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, namespace.Namespace)
     assert response.name == "name_value"
+    assert response.uid == "uid_value"
 
 
 @pytest.mark.asyncio
 async def test_get_namespace_async_from_dict():
     await test_get_namespace_async(request_type=dict)
 
 
@@ -1683,25 +1692,27 @@
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.update_namespace), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = gcs_namespace.Namespace(
             name="name_value",
+            uid="uid_value",
         )
         response = client.update_namespace(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == registration_service.UpdateNamespaceRequest()
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, gcs_namespace.Namespace)
     assert response.name == "name_value"
+    assert response.uid == "uid_value"
 
 
 def test_update_namespace_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = RegistrationServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -1732,26 +1743,28 @@
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.update_namespace), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             gcs_namespace.Namespace(
                 name="name_value",
+                uid="uid_value",
             )
         )
         response = await client.update_namespace(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == registration_service.UpdateNamespaceRequest()
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, gcs_namespace.Namespace)
     assert response.name == "name_value"
+    assert response.uid == "uid_value"
 
 
 @pytest.mark.asyncio
 async def test_update_namespace_async_from_dict():
     await test_update_namespace_async(request_type=dict)
 
 
@@ -2147,25 +2160,27 @@
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.create_service), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = gcs_service.Service(
             name="name_value",
+            uid="uid_value",
         )
         response = client.create_service(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == registration_service.CreateServiceRequest()
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, gcs_service.Service)
     assert response.name == "name_value"
+    assert response.uid == "uid_value"
 
 
 def test_create_service_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = RegistrationServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -2196,26 +2211,28 @@
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.create_service), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             gcs_service.Service(
                 name="name_value",
+                uid="uid_value",
             )
         )
         response = await client.create_service(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == registration_service.CreateServiceRequest()
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, gcs_service.Service)
     assert response.name == "name_value"
+    assert response.uid == "uid_value"
 
 
 @pytest.mark.asyncio
 async def test_create_service_async_from_dict():
     await test_create_service_async(request_type=dict)
 
 
@@ -2819,25 +2836,27 @@
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_service), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = service.Service(
             name="name_value",
+            uid="uid_value",
         )
         response = client.get_service(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == registration_service.GetServiceRequest()
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, service.Service)
     assert response.name == "name_value"
+    assert response.uid == "uid_value"
 
 
 def test_get_service_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = RegistrationServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -2867,26 +2886,28 @@
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_service), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             service.Service(
                 name="name_value",
+                uid="uid_value",
             )
         )
         response = await client.get_service(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == registration_service.GetServiceRequest()
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, service.Service)
     assert response.name == "name_value"
+    assert response.uid == "uid_value"
 
 
 @pytest.mark.asyncio
 async def test_get_service_async_from_dict():
     await test_get_service_async(request_type=dict)
 
 
@@ -3047,25 +3068,27 @@
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.update_service), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = gcs_service.Service(
             name="name_value",
+            uid="uid_value",
         )
         response = client.update_service(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == registration_service.UpdateServiceRequest()
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, gcs_service.Service)
     assert response.name == "name_value"
+    assert response.uid == "uid_value"
 
 
 def test_update_service_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = RegistrationServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -3096,26 +3119,28 @@
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.update_service), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             gcs_service.Service(
                 name="name_value",
+                uid="uid_value",
             )
         )
         response = await client.update_service(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == registration_service.UpdateServiceRequest()
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, gcs_service.Service)
     assert response.name == "name_value"
+    assert response.uid == "uid_value"
 
 
 @pytest.mark.asyncio
 async def test_update_service_async_from_dict():
     await test_update_service_async(request_type=dict)
 
 
@@ -3510,28 +3535,30 @@
     with mock.patch.object(type(client.transport.create_endpoint), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = gcs_endpoint.Endpoint(
             name="name_value",
             address="address_value",
             port=453,
             network="network_value",
+            uid="uid_value",
         )
         response = client.create_endpoint(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == registration_service.CreateEndpointRequest()
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, gcs_endpoint.Endpoint)
     assert response.name == "name_value"
     assert response.address == "address_value"
     assert response.port == 453
     assert response.network == "network_value"
+    assert response.uid == "uid_value"
 
 
 def test_create_endpoint_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = RegistrationServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -3565,14 +3592,15 @@
         # Designate an appropriate return value for the call.
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             gcs_endpoint.Endpoint(
                 name="name_value",
                 address="address_value",
                 port=453,
                 network="network_value",
+                uid="uid_value",
             )
         )
         response = await client.create_endpoint(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
@@ -3580,14 +3608,15 @@
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, gcs_endpoint.Endpoint)
     assert response.name == "name_value"
     assert response.address == "address_value"
     assert response.port == 453
     assert response.network == "network_value"
+    assert response.uid == "uid_value"
 
 
 @pytest.mark.asyncio
 async def test_create_endpoint_async_from_dict():
     await test_create_endpoint_async(request_type=dict)
 
 
@@ -4198,28 +4227,30 @@
     with mock.patch.object(type(client.transport.get_endpoint), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = endpoint.Endpoint(
             name="name_value",
             address="address_value",
             port=453,
             network="network_value",
+            uid="uid_value",
         )
         response = client.get_endpoint(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == registration_service.GetEndpointRequest()
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, endpoint.Endpoint)
     assert response.name == "name_value"
     assert response.address == "address_value"
     assert response.port == 453
     assert response.network == "network_value"
+    assert response.uid == "uid_value"
 
 
 def test_get_endpoint_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = RegistrationServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -4253,14 +4284,15 @@
         # Designate an appropriate return value for the call.
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             endpoint.Endpoint(
                 name="name_value",
                 address="address_value",
                 port=453,
                 network="network_value",
+                uid="uid_value",
             )
         )
         response = await client.get_endpoint(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
@@ -4268,14 +4300,15 @@
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, endpoint.Endpoint)
     assert response.name == "name_value"
     assert response.address == "address_value"
     assert response.port == 453
     assert response.network == "network_value"
+    assert response.uid == "uid_value"
 
 
 @pytest.mark.asyncio
 async def test_get_endpoint_async_from_dict():
     await test_get_endpoint_async(request_type=dict)
 
 
@@ -4439,28 +4472,30 @@
     with mock.patch.object(type(client.transport.update_endpoint), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = gcs_endpoint.Endpoint(
             name="name_value",
             address="address_value",
             port=453,
             network="network_value",
+            uid="uid_value",
         )
         response = client.update_endpoint(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == registration_service.UpdateEndpointRequest()
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, gcs_endpoint.Endpoint)
     assert response.name == "name_value"
     assert response.address == "address_value"
     assert response.port == 453
     assert response.network == "network_value"
+    assert response.uid == "uid_value"
 
 
 def test_update_endpoint_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = RegistrationServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -4494,14 +4529,15 @@
         # Designate an appropriate return value for the call.
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             gcs_endpoint.Endpoint(
                 name="name_value",
                 address="address_value",
                 port=453,
                 network="network_value",
+                uid="uid_value",
             )
         )
         response = await client.update_endpoint(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
@@ -4509,14 +4545,15 @@
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, gcs_endpoint.Endpoint)
     assert response.name == "name_value"
     assert response.address == "address_value"
     assert response.port == 453
     assert response.network == "network_value"
+    assert response.uid == "uid_value"
 
 
 @pytest.mark.asyncio
 async def test_update_endpoint_async_from_dict():
     await test_update_endpoint_async(request_type=dict)
 
 
@@ -5429,22 +5466,24 @@
     # send a request that will satisfy transcoding
     request_init = {"parent": "projects/sample1/locations/sample2"}
     request_init["namespace"] = {
         "name": "name_value",
         "labels": {},
         "create_time": {"seconds": 751, "nanos": 543},
         "update_time": {},
+        "uid": "uid_value",
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = gcs_namespace.Namespace(
             name="name_value",
+            uid="uid_value",
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = gcs_namespace.Namespace.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -5452,14 +5491,15 @@
         response_value._content = json_return_value.encode("UTF-8")
         req.return_value = response_value
         response = client.create_namespace(request)
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, gcs_namespace.Namespace)
     assert response.name == "name_value"
+    assert response.uid == "uid_value"
 
 
 def test_create_namespace_rest_required_fields(
     request_type=registration_service.CreateNamespaceRequest,
 ):
     transport_class = transports.RegistrationServiceRestTransport
 
@@ -5637,14 +5677,15 @@
     # send a request that will satisfy transcoding
     request_init = {"parent": "projects/sample1/locations/sample2"}
     request_init["namespace"] = {
         "name": "name_value",
         "labels": {},
         "create_time": {"seconds": 751, "nanos": 543},
         "update_time": {},
+        "uid": "uid_value",
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a BadRequest error.
     with mock.patch.object(Session, "request") as req, pytest.raises(
         core_exceptions.BadRequest
     ):
@@ -6086,14 +6127,15 @@
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = namespace.Namespace(
             name="name_value",
+            uid="uid_value",
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = namespace.Namespace.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -6101,14 +6143,15 @@
         response_value._content = json_return_value.encode("UTF-8")
         req.return_value = response_value
         response = client.get_namespace(request)
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, namespace.Namespace)
     assert response.name == "name_value"
+    assert response.uid == "uid_value"
 
 
 def test_get_namespace_rest_required_fields(
     request_type=registration_service.GetNamespaceRequest,
 ):
     transport_class = transports.RegistrationServiceRestTransport
 
@@ -6354,22 +6397,24 @@
         "namespace": {"name": "projects/sample1/locations/sample2/namespaces/sample3"}
     }
     request_init["namespace"] = {
         "name": "projects/sample1/locations/sample2/namespaces/sample3",
         "labels": {},
         "create_time": {"seconds": 751, "nanos": 543},
         "update_time": {},
+        "uid": "uid_value",
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = gcs_namespace.Namespace(
             name="name_value",
+            uid="uid_value",
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = gcs_namespace.Namespace.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -6377,14 +6422,15 @@
         response_value._content = json_return_value.encode("UTF-8")
         req.return_value = response_value
         response = client.update_namespace(request)
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, gcs_namespace.Namespace)
     assert response.name == "name_value"
+    assert response.uid == "uid_value"
 
 
 def test_update_namespace_rest_required_fields(
     request_type=registration_service.UpdateNamespaceRequest,
 ):
     transport_class = transports.RegistrationServiceRestTransport
 
@@ -6545,14 +6591,15 @@
         "namespace": {"name": "projects/sample1/locations/sample2/namespaces/sample3"}
     }
     request_init["namespace"] = {
         "name": "projects/sample1/locations/sample2/namespaces/sample3",
         "labels": {},
         "create_time": {"seconds": 751, "nanos": 543},
         "update_time": {},
+        "uid": "uid_value",
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a BadRequest error.
     with mock.patch.object(Session, "request") as req, pytest.raises(
         core_exceptions.BadRequest
     ):
@@ -6910,26 +6957,29 @@
                 "name": "name_value",
                 "address": "address_value",
                 "port": 453,
                 "metadata": {},
                 "network": "network_value",
                 "create_time": {"seconds": 751, "nanos": 543},
                 "update_time": {},
+                "uid": "uid_value",
             }
         ],
         "create_time": {},
         "update_time": {},
+        "uid": "uid_value",
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = gcs_service.Service(
             name="name_value",
+            uid="uid_value",
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = gcs_service.Service.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -6937,14 +6987,15 @@
         response_value._content = json_return_value.encode("UTF-8")
         req.return_value = response_value
         response = client.create_service(request)
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, gcs_service.Service)
     assert response.name == "name_value"
+    assert response.uid == "uid_value"
 
 
 def test_create_service_rest_required_fields(
     request_type=registration_service.CreateServiceRequest,
 ):
     transport_class = transports.RegistrationServiceRestTransport
 
@@ -7127,18 +7178,20 @@
                 "name": "name_value",
                 "address": "address_value",
                 "port": 453,
                 "metadata": {},
                 "network": "network_value",
                 "create_time": {"seconds": 751, "nanos": 543},
                 "update_time": {},
+                "uid": "uid_value",
             }
         ],
         "create_time": {},
         "update_time": {},
+        "uid": "uid_value",
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a BadRequest error.
     with mock.patch.object(Session, "request") as req, pytest.raises(
         core_exceptions.BadRequest
     ):
@@ -7586,14 +7639,15 @@
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = service.Service(
             name="name_value",
+            uid="uid_value",
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = service.Service.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -7601,14 +7655,15 @@
         response_value._content = json_return_value.encode("UTF-8")
         req.return_value = response_value
         response = client.get_service(request)
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, service.Service)
     assert response.name == "name_value"
+    assert response.uid == "uid_value"
 
 
 def test_get_service_rest_required_fields(
     request_type=registration_service.GetServiceRequest,
 ):
     transport_class = transports.RegistrationServiceRestTransport
 
@@ -7865,26 +7920,29 @@
                 "name": "name_value",
                 "address": "address_value",
                 "port": 453,
                 "metadata": {},
                 "network": "network_value",
                 "create_time": {"seconds": 751, "nanos": 543},
                 "update_time": {},
+                "uid": "uid_value",
             }
         ],
         "create_time": {},
         "update_time": {},
+        "uid": "uid_value",
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = gcs_service.Service(
             name="name_value",
+            uid="uid_value",
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = gcs_service.Service.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -7892,14 +7950,15 @@
         response_value._content = json_return_value.encode("UTF-8")
         req.return_value = response_value
         response = client.update_service(request)
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, gcs_service.Service)
     assert response.name == "name_value"
+    assert response.uid == "uid_value"
 
 
 def test_update_service_rest_required_fields(
     request_type=registration_service.UpdateServiceRequest,
 ):
     transport_class = transports.RegistrationServiceRestTransport
 
@@ -8067,18 +8126,20 @@
                 "name": "name_value",
                 "address": "address_value",
                 "port": 453,
                 "metadata": {},
                 "network": "network_value",
                 "create_time": {"seconds": 751, "nanos": 543},
                 "update_time": {},
+                "uid": "uid_value",
             }
         ],
         "create_time": {},
         "update_time": {},
+        "uid": "uid_value",
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a BadRequest error.
     with mock.patch.object(Session, "request") as req, pytest.raises(
         core_exceptions.BadRequest
     ):
@@ -8438,25 +8499,27 @@
         "name": "name_value",
         "address": "address_value",
         "port": 453,
         "metadata": {},
         "network": "network_value",
         "create_time": {"seconds": 751, "nanos": 543},
         "update_time": {},
+        "uid": "uid_value",
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = gcs_endpoint.Endpoint(
             name="name_value",
             address="address_value",
             port=453,
             network="network_value",
+            uid="uid_value",
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = gcs_endpoint.Endpoint.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -8467,14 +8530,15 @@
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, gcs_endpoint.Endpoint)
     assert response.name == "name_value"
     assert response.address == "address_value"
     assert response.port == 453
     assert response.network == "network_value"
+    assert response.uid == "uid_value"
 
 
 def test_create_endpoint_rest_required_fields(
     request_type=registration_service.CreateEndpointRequest,
 ):
     transport_class = transports.RegistrationServiceRestTransport
 
@@ -8657,14 +8721,15 @@
         "name": "name_value",
         "address": "address_value",
         "port": 453,
         "metadata": {},
         "network": "network_value",
         "create_time": {"seconds": 751, "nanos": 543},
         "update_time": {},
+        "uid": "uid_value",
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a BadRequest error.
     with mock.patch.object(Session, "request") as req, pytest.raises(
         core_exceptions.BadRequest
     ):
@@ -9121,14 +9186,15 @@
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = endpoint.Endpoint(
             name="name_value",
             address="address_value",
             port=453,
             network="network_value",
+            uid="uid_value",
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = endpoint.Endpoint.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -9139,14 +9205,15 @@
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, endpoint.Endpoint)
     assert response.name == "name_value"
     assert response.address == "address_value"
     assert response.port == 453
     assert response.network == "network_value"
+    assert response.uid == "uid_value"
 
 
 def test_get_endpoint_rest_required_fields(
     request_type=registration_service.GetEndpointRequest,
 ):
     transport_class = transports.RegistrationServiceRestTransport
 
@@ -9399,25 +9466,27 @@
         "name": "projects/sample1/locations/sample2/namespaces/sample3/services/sample4/endpoints/sample5",
         "address": "address_value",
         "port": 453,
         "metadata": {},
         "network": "network_value",
         "create_time": {"seconds": 751, "nanos": 543},
         "update_time": {},
+        "uid": "uid_value",
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = gcs_endpoint.Endpoint(
             name="name_value",
             address="address_value",
             port=453,
             network="network_value",
+            uid="uid_value",
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = gcs_endpoint.Endpoint.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -9428,14 +9497,15 @@
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, gcs_endpoint.Endpoint)
     assert response.name == "name_value"
     assert response.address == "address_value"
     assert response.port == 453
     assert response.network == "network_value"
+    assert response.uid == "uid_value"
 
 
 def test_update_endpoint_rest_required_fields(
     request_type=registration_service.UpdateEndpointRequest,
 ):
     transport_class = transports.RegistrationServiceRestTransport
 
@@ -9601,14 +9671,15 @@
         "name": "projects/sample1/locations/sample2/namespaces/sample3/services/sample4/endpoints/sample5",
         "address": "address_value",
         "port": 453,
         "metadata": {},
         "network": "network_value",
         "create_time": {"seconds": 751, "nanos": 543},
         "update_time": {},
+        "uid": "uid_value",
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a BadRequest error.
     with mock.patch.object(Session, "request") as req, pytest.raises(
         core_exceptions.BadRequest
     ):
@@ -10753,14 +10824,16 @@
         "list_endpoints",
         "get_endpoint",
         "update_endpoint",
         "delete_endpoint",
         "get_iam_policy",
         "set_iam_policy",
         "test_iam_permissions",
+        "get_location",
+        "list_locations",
     )
     for method in methods:
         with pytest.raises(NotImplementedError):
             getattr(transport, method)(request=object())
 
     with pytest.raises(NotImplementedError):
         transport.close()
@@ -11449,14 +11522,418 @@
         type(getattr(client.transport, "grpc_channel")), "close"
     ) as close:
         async with client:
             close.assert_not_called()
         close.assert_called_once()
 
 
+def test_get_location_rest_bad_request(
+    transport: str = "rest", request_type=locations_pb2.GetLocationRequest
+):
+    client = RegistrationServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    request = request_type()
+    request = json_format.ParseDict(
+        {"name": "projects/sample1/locations/sample2"}, request
+    )
+
+    # Mock the http request call within the method and fake a BadRequest error.
+    with mock.patch.object(Session, "request") as req, pytest.raises(
+        core_exceptions.BadRequest
+    ):
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 400
+        response_value.request = Request()
+        req.return_value = response_value
+        client.get_location(request)
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        locations_pb2.GetLocationRequest,
+        dict,
+    ],
+)
+def test_get_location_rest(request_type):
+    client = RegistrationServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+    request_init = {"name": "projects/sample1/locations/sample2"}
+    request = request_type(**request_init)
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = locations_pb2.Location()
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        json_return_value = json_format.MessageToJson(return_value)
+
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+
+        response = client.get_location(request)
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, locations_pb2.Location)
+
+
+def test_list_locations_rest_bad_request(
+    transport: str = "rest", request_type=locations_pb2.ListLocationsRequest
+):
+    client = RegistrationServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    request = request_type()
+    request = json_format.ParseDict({"name": "projects/sample1"}, request)
+
+    # Mock the http request call within the method and fake a BadRequest error.
+    with mock.patch.object(Session, "request") as req, pytest.raises(
+        core_exceptions.BadRequest
+    ):
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 400
+        response_value.request = Request()
+        req.return_value = response_value
+        client.list_locations(request)
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        locations_pb2.ListLocationsRequest,
+        dict,
+    ],
+)
+def test_list_locations_rest(request_type):
+    client = RegistrationServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+    request_init = {"name": "projects/sample1"}
+    request = request_type(**request_init)
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = locations_pb2.ListLocationsResponse()
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        json_return_value = json_format.MessageToJson(return_value)
+
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+
+        response = client.list_locations(request)
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, locations_pb2.ListLocationsResponse)
+
+
+def test_list_locations(transport: str = "grpc"):
+    client = RegistrationServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = locations_pb2.ListLocationsRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = locations_pb2.ListLocationsResponse()
+        response = client.list_locations(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, locations_pb2.ListLocationsResponse)
+
+
+@pytest.mark.asyncio
+async def test_list_locations_async(transport: str = "grpc"):
+    client = RegistrationServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = locations_pb2.ListLocationsRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            locations_pb2.ListLocationsResponse()
+        )
+        response = await client.list_locations(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, locations_pb2.ListLocationsResponse)
+
+
+def test_list_locations_field_headers():
+    client = RegistrationServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = locations_pb2.ListLocationsRequest()
+    request.name = "locations"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        call.return_value = locations_pb2.ListLocationsResponse()
+
+        client.list_locations(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=locations",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_list_locations_field_headers_async():
+    client = RegistrationServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = locations_pb2.ListLocationsRequest()
+    request.name = "locations"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            locations_pb2.ListLocationsResponse()
+        )
+        await client.list_locations(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=locations",
+    ) in kw["metadata"]
+
+
+def test_list_locations_from_dict():
+    client = RegistrationServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = locations_pb2.ListLocationsResponse()
+
+        response = client.list_locations(
+            request={
+                "name": "locations",
+            }
+        )
+        call.assert_called()
+
+
+@pytest.mark.asyncio
+async def test_list_locations_from_dict_async():
+    client = RegistrationServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            locations_pb2.ListLocationsResponse()
+        )
+        response = await client.list_locations(
+            request={
+                "name": "locations",
+            }
+        )
+        call.assert_called()
+
+
+def test_get_location(transport: str = "grpc"):
+    client = RegistrationServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = locations_pb2.GetLocationRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_location), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = locations_pb2.Location()
+        response = client.get_location(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, locations_pb2.Location)
+
+
+@pytest.mark.asyncio
+async def test_get_location_async(transport: str = "grpc_asyncio"):
+    client = RegistrationServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = locations_pb2.GetLocationRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_location), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            locations_pb2.Location()
+        )
+        response = await client.get_location(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, locations_pb2.Location)
+
+
+def test_get_location_field_headers():
+    client = RegistrationServiceClient(
+        credentials=ga_credentials.AnonymousCredentials()
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = locations_pb2.GetLocationRequest()
+    request.name = "locations/abc"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_location), "__call__") as call:
+        call.return_value = locations_pb2.Location()
+
+        client.get_location(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=locations/abc",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_get_location_field_headers_async():
+    client = RegistrationServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials()
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = locations_pb2.GetLocationRequest()
+    request.name = "locations/abc"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_location), "__call__") as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            locations_pb2.Location()
+        )
+        await client.get_location(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=locations/abc",
+    ) in kw["metadata"]
+
+
+def test_get_location_from_dict():
+    client = RegistrationServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = locations_pb2.Location()
+
+        response = client.get_location(
+            request={
+                "name": "locations/abc",
+            }
+        )
+        call.assert_called()
+
+
+@pytest.mark.asyncio
+async def test_get_location_from_dict_async():
+    client = RegistrationServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            locations_pb2.Location()
+        )
+        response = await client.get_location(
+            request={
+                "name": "locations",
+            }
+        )
+        call.assert_called()
+
+
 def test_transport_close():
     transports = {
         "rest": "_session",
         "grpc": "_grpc_channel",
     }
 
     for transport, close_name in transports.items():
```

