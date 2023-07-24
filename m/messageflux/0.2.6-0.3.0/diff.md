# Comparing `tmp/messageflux-0.2.6.tar.gz` & `tmp/messageflux-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "messageflux-0.2.6.tar", last modified: Fri Jul 21 12:02:36 2023, max compression
+gzip compressed data, was "messageflux-0.3.0.tar", last modified: Mon Jul 24 14:58:35 2023, max compression
```

## Comparing `messageflux-0.2.6.tar` & `messageflux-0.3.0.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:02:36.229842 messageflux-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-21 12:02:23.000000 messageflux-0.2.6/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-21 12:02:23.000000 messageflux-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-21 12:02:23.000000 messageflux-0.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-07-21 12:02:36.229842 messageflux-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-07-21 12:02:23.000000 messageflux-0.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-21 12:02:24.000000 messageflux-0.2.6/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:02:36.213842 messageflux-0.2.6/_custom_build/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 12:02:23.000000 messageflux-0.2.6/_custom_build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-21 12:02:23.000000 messageflux-0.2.6/_custom_build/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-21 12:02:23.000000 messageflux-0.2.6/_custom_build/make_all_extra_requirements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:02:36.217841 messageflux-0.2.6/messageflux/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/base_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/fastmessage_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:02:36.217841 messageflux-0.2.6/messageflux/iodevices/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:02:36.217841 messageflux-0.2.6/messageflux/iodevices/base/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/base/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     9978 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/base/input_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/base/input_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/base/output_devices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:02:36.221841 messageflux-0.2.6/messageflux/iodevices/collection_device_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/collection_device_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/collection_device_wrapper/collection_input_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/collection_device_wrapper/collection_output_device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:02:36.221841 messageflux-0.2.6/messageflux/iodevices/failover_output_device_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/failover_output_device_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/failover_output_device_wrapper/failover_output_device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:02:36.221841 messageflux-0.2.6/messageflux/iodevices/file_system/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/file_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/file_system/file_system_device_manager_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    24466 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/file_system/file_system_input_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/file_system/file_system_output_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/file_system/file_system_serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:02:36.221841 messageflux-0.2.6/messageflux/iodevices/in_memory_device/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/in_memory_device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/in_memory_device/in_memory_device_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:02:36.221841 messageflux-0.2.6/messageflux/iodevices/message_store_device_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/message_store_device_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/message_store_device_wrapper/file_system_message_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/message_store_device_wrapper/message_store_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/message_store_device_wrapper/message_store_input_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/message_store_device_wrapper/message_store_output_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/message_store_device_wrapper/message_store_transformer_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:02:36.225842 messageflux-0.2.6/messageflux/iodevices/objectstorage/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/objectstorage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/objectstorage/s3_message_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:02:36.225842 messageflux-0.2.6/messageflux/iodevices/objectstorage/s3api/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/objectstorage/s3api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/objectstorage/s3api/s3bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/objectstorage/s3api/s3client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:02:36.225842 messageflux-0.2.6/messageflux/iodevices/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/rabbitmq/fs_poison_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)    14045 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/rabbitmq/rabbitmq_device_manager_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16736 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/rabbitmq/rabbitmq_input_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    15636 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/rabbitmq/rabbitmq_output_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    12168 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/rabbitmq/rabbitmq_poison_counting_input_device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:02:36.225842 messageflux-0.2.6/messageflux/iodevices/round_robin_device_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/round_robin_device_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/round_robin_device_wrapper/roundrobin_io_device_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:02:36.225842 messageflux-0.2.6/messageflux/iodevices/short_circuit_device_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/short_circuit_device_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/short_circuit_device_wrapper/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_input_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_output_device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:02:36.229842 messageflux-0.2.6/messageflux/iodevices/transformer_device_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/transformer_device_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/transformer_device_wrapper/transformer_input_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/transformer_device_wrapper/transformer_output_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/iodevices/transformer_device_wrapper/zlib_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:02:36.229842 messageflux-0.2.6/messageflux/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/logging/LogType.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/logging/bulk_rotating_device_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/logging/bulk_rotating_file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/logging/bulk_rotating_handler_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/logging/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/message_handling_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/metadata_headers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:02:36.229842 messageflux-0.2.6/messageflux/multiprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/multiprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/multiprocessing/multiprocessrunner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6360 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/multiprocessing/singleprocesshandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/pipeline_service.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/server_loop_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:02:36.229842 messageflux-0.2.6/messageflux/service_addons/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/service_addons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/service_addons/loop_health_addon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:02:36.229842 messageflux-0.2.6/messageflux/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-21 12:02:23.000000 messageflux-0.2.6/messageflux/utils/filesystem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:02:36.217841 messageflux-0.2.6/messageflux.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-07-21 12:02:36.000000 messageflux-0.2.6/messageflux.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-07-21 12:02:36.000000 messageflux-0.2.6/messageflux.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 12:02:36.000000 messageflux-0.2.6/messageflux.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-21 12:02:36.000000 messageflux-0.2.6/messageflux.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-21 12:02:36.000000 messageflux-0.2.6/messageflux.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-21 12:02:23.000000 messageflux-0.2.6/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-21 12:02:23.000000 messageflux-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-21 12:02:23.000000 messageflux-0.2.6/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-21 12:02:36.000000 messageflux-0.2.6/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-21 12:02:23.000000 messageflux-0.2.6/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-21 12:02:23.000000 messageflux-0.2.6/requirements-fastmessage.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-21 12:02:23.000000 messageflux-0.2.6/requirements-objectstorage.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-21 12:02:23.000000 messageflux-0.2.6/requirements-rabbitmq.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 12:02:23.000000 messageflux-0.2.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 12:02:36.229842 messageflux-0.2.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:58:35.285151 messageflux-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-24 14:58:21.000000 messageflux-0.3.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-24 14:58:21.000000 messageflux-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-24 14:58:21.000000 messageflux-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-07-24 14:58:35.285151 messageflux-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-07-24 14:58:21.000000 messageflux-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-24 14:58:22.000000 messageflux-0.3.0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:58:35.273151 messageflux-0.3.0/_custom_build/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 14:58:21.000000 messageflux-0.3.0/_custom_build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-24 14:58:21.000000 messageflux-0.3.0/_custom_build/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-24 14:58:21.000000 messageflux-0.3.0/_custom_build/make_all_extra_requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:58:35.277151 messageflux-0.3.0/messageflux/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/base_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/fastmessage_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:58:35.277151 messageflux-0.3.0/messageflux/iodevices/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:58:35.277151 messageflux-0.3.0/messageflux/iodevices/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/base/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10977 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/base/input_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/base/input_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/base/output_devices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:58:35.277151 messageflux-0.3.0/messageflux/iodevices/collection_device_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/collection_device_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/collection_device_wrapper/collection_input_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/collection_device_wrapper/collection_output_device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:58:35.277151 messageflux-0.3.0/messageflux/iodevices/failover_output_device_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/failover_output_device_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/failover_output_device_wrapper/failover_output_device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:58:35.277151 messageflux-0.3.0/messageflux/iodevices/file_system/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/file_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/file_system/file_system_device_manager_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24734 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/file_system/file_system_input_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/file_system/file_system_output_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/file_system/file_system_serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:58:35.277151 messageflux-0.3.0/messageflux/iodevices/in_memory_device/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/in_memory_device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/in_memory_device/in_memory_device_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:58:35.281151 messageflux-0.3.0/messageflux/iodevices/message_store_device_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/message_store_device_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/message_store_device_wrapper/file_system_message_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/message_store_device_wrapper/message_store_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/message_store_device_wrapper/message_store_input_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/message_store_device_wrapper/message_store_output_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/message_store_device_wrapper/message_store_transformer_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:58:35.281151 messageflux-0.3.0/messageflux/iodevices/objectstorage/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/objectstorage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/objectstorage/s3_message_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:58:35.281151 messageflux-0.3.0/messageflux/iodevices/objectstorage/s3api/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/objectstorage/s3api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/objectstorage/s3api/s3bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/objectstorage/s3api/s3client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:58:35.281151 messageflux-0.3.0/messageflux/iodevices/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/rabbitmq/fs_poison_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14045 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/rabbitmq/rabbitmq_device_manager_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18501 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/rabbitmq/rabbitmq_input_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15636 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/rabbitmq/rabbitmq_output_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/rabbitmq/rabbitmq_poison_counting_input_device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:58:35.281151 messageflux-0.3.0/messageflux/iodevices/round_robin_device_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/round_robin_device_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/round_robin_device_wrapper/roundrobin_io_device_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:58:35.281151 messageflux-0.3.0/messageflux/iodevices/short_circuit_device_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/short_circuit_device_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/short_circuit_device_wrapper/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_input_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_output_device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:58:35.281151 messageflux-0.3.0/messageflux/iodevices/transformer_device_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/transformer_device_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/transformer_device_wrapper/transformer_input_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/transformer_device_wrapper/transformer_output_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/transformer_device_wrapper/zlib_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:58:35.281151 messageflux-0.3.0/messageflux/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/logging/LogType.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/logging/bulk_rotating_device_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/logging/bulk_rotating_file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/logging/bulk_rotating_handler_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/logging/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/message_handling_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/metadata_headers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:58:35.281151 messageflux-0.3.0/messageflux/multiprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/multiprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/multiprocessing/multiprocessrunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6360 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/multiprocessing/singleprocesshandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/pipeline_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/server_loop_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:58:35.281151 messageflux-0.3.0/messageflux/service_addons/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/service_addons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/service_addons/loop_health_addon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:58:35.285151 messageflux-0.3.0/messageflux/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/utils/filesystem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:58:35.277151 messageflux-0.3.0/messageflux.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-07-24 14:58:35.000000 messageflux-0.3.0/messageflux.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-07-24 14:58:35.000000 messageflux-0.3.0/messageflux.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 14:58:35.000000 messageflux-0.3.0/messageflux.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-24 14:58:35.000000 messageflux-0.3.0/messageflux.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-24 14:58:35.000000 messageflux-0.3.0/messageflux.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-24 14:58:21.000000 messageflux-0.3.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-24 14:58:21.000000 messageflux-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-24 14:58:21.000000 messageflux-0.3.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-24 14:58:35.000000 messageflux-0.3.0/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-24 14:58:21.000000 messageflux-0.3.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-24 14:58:21.000000 messageflux-0.3.0/requirements-fastmessage.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-24 14:58:21.000000 messageflux-0.3.0/requirements-objectstorage.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-24 14:58:21.000000 messageflux-0.3.0/requirements-rabbitmq.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 14:58:21.000000 messageflux-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 14:58:35.285151 messageflux-0.3.0/setup.cfg
```

### Comparing `messageflux-0.2.6/LICENSE` & `messageflux-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.6/PKG-INFO` & `messageflux-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: messageflux
-Version: 0.2.6
+Version: 0.3.0
 Author-email: Aviv Salem <avivsalem@gmail.com>
 Maintainer-email: Aviv Salem <avivsalem@gmail.com>, Nir Schulman <narsssx@gmail.com>, Rafael Zilberman <Zilberman.rafi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Avivsalem/MessageFlux/
 Project-URL: Documentation, https://messageflux.readthedocs.io/
 Platform: win32
 Platform: linux
```

### Comparing `messageflux-0.2.6/README.md` & `messageflux-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.6/_custom_build/make_all_extra_requirements.py` & `messageflux-0.3.0/_custom_build/make_all_extra_requirements.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.6/messageflux/base_service.py` & `messageflux-0.3.0/messageflux/base_service.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.6/messageflux/fastmessage_handler.py` & `messageflux-0.3.0/messageflux/fastmessage_handler.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.6/messageflux/iodevices/base/__init__.py` & `messageflux-0.3.0/messageflux/iodevices/base/__init__.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.6/messageflux/iodevices/base/common.py` & `messageflux-0.3.0/messageflux/iodevices/base/common.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.6/messageflux/iodevices/base/input_devices.py` & `messageflux-0.3.0/messageflux/iodevices/base/input_devices.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
+import threading
 from abc import ABCMeta, abstractmethod
+from time import perf_counter
 from typing import Optional, List, TypeVar, Generic
 
-from time import sleep, perf_counter
-
 from messageflux.iodevices.base.common import MessageBundle, Message, DeviceHeaders
 from messageflux.iodevices.base.input_transaction import InputTransaction, NULLTransaction
 from messageflux.utils import StatefulListIterator, AggregatedException
 
 TManagerType = TypeVar('TManagerType', bound='InputDeviceManager')
 TInputDeviceType = TypeVar('TInputDeviceType', bound='InputDevice')
 
@@ -50,39 +50,50 @@
     def manager(self) -> TManagerType:
         """
         :return: the input device manager that created this device
         """
         return self._manager
 
     def read_message(self,
+                     cancellation_token: threading.Event,
                      timeout: Optional[float] = None,
                      with_transaction: bool = True) -> Optional['ReadResult']:
         """
         this method returns a message from the device. and makes sure that the input device name header is present
+
+        :param cancellation_token: the cancellation token for this service. this can be used to know if cancellation
+        was requested
+
         :param timeout: an optional timeout (in seconds) to wait for the device to return a message.
         after 'timeout' seconds, if the device doesn't have a message to return, it will return None
         :param with_transaction: 'True' if the device should read message within transaction,
         or 'False' if the message is automatically committed
 
         :return: a ReadResult object or None if no message was available.
         the device headers can contain extra information about the device that returned the message
         """
-        read_result = self._read_message(timeout=timeout, with_transaction=with_transaction)
+        read_result = self._read_message(cancellation_token=cancellation_token,
+                                         timeout=timeout,
+                                         with_transaction=with_transaction)
         if read_result is not None:
             read_result.device_headers.setdefault(self.INPUT_DEVICE_NAME_HEADER, self.name)
 
         return read_result
 
     @abstractmethod
     def _read_message(self,
+                      cancellation_token: threading.Event,
                       timeout: Optional[float] = None,
                       with_transaction: bool = True) -> Optional['ReadResult']:
         """
         this method returns a message from the device (should be implemented by child classes)
 
+        :param cancellation_token: the cancellation token for this service. this can be used to know if cancellation
+        was requested
+
         :param timeout: an optional timeout (in seconds) to wait for the device to return a message.
         after 'timeout' seconds, if the device doesn't have a message to return, it will return None
 
         :param with_transaction: 'True' if the device should read message within transaction,
         or 'False' if the message is automatically committed
 
         :return: a ReadResult object or None if no message was available.
@@ -118,19 +129,23 @@
     def last_read_device(self) -> Optional[InputDevice]:
         """
         :return: the last device that was read (in case it returned data/raised exception)
         """
         return self._last_read_device
 
     def _read_message(self,
+                      cancellation_token: threading.Event,
                       timeout: Optional[float] = None,
                       with_transaction: bool = True) -> Optional['ReadResult']:
         """
         this method returns a message from the first device available in inner devices
 
+        :param cancellation_token: the cancellation token for this service. this can be used to know if cancellation
+        was requested
+
         :param timeout: an optional timeout (in seconds) to wait for the device to return a message.
         after 'timeout' seconds, if the device doesn't have a message to return, it will return None
 
         :param with_transaction: 'True' if the device should read message within transaction,
         or 'False' if the message is automatically committed
 
         :return: a ReadResult object or None if no message was available.
@@ -140,27 +155,29 @@
         end_time = 0.0
         if timeout is not None:
             end_time = perf_counter() + timeout
 
         while True:
             for inner_device in self._inner_devices_iterator:
                 self._last_read_device = inner_device
-                read_result = inner_device.read_message(timeout=0, with_transaction=with_transaction)
+                read_result = inner_device.read_message(cancellation_token=cancellation_token,
+                                                        timeout=0,
+                                                        with_transaction=with_transaction)
                 if read_result is not None:
                     return read_result
 
                 if timeout is not None and perf_counter() >= end_time:
                     break
 
             if timeout is not None and perf_counter() >= end_time:
                 self._last_read_device = None
                 return None
             else:
                 # if all the devices were empty, wait before performing another iteration.
-                sleep(self._SLEEP_BETWEEN_ITERATIONS)
+                cancellation_token.wait(self._SLEEP_BETWEEN_ITERATIONS)
 
     def close(self):
         """
         tries to close underlying devices
         """
         for inner_device in self._inner_devices_iterator:
             try:
@@ -233,15 +250,18 @@
     """
     this is a stub for creating a null transaction
     """
 
     def __init__(self):
         super(_NullDevice, self).__init__(_NullInputDeviceManager(), '__NULL__')
 
-    def _read_message(self, timeout: Optional[float] = None, with_transaction: bool = True) -> Optional['ReadResult']:
+    def _read_message(self,
+                      cancellation_token: threading.Event,
+                      timeout: Optional[float] = None,
+                      with_transaction: bool = True) -> Optional['ReadResult']:
         """
         always returns None immediately
         """
         return None
 
 
 NULL_TRANSACTION = NULLTransaction(_NullDevice())  # this is a const NullTransaction, for convenience
```

### Comparing `messageflux-0.2.6/messageflux/iodevices/base/input_transaction.py` & `messageflux-0.3.0/messageflux/iodevices/base/input_transaction.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import threading
 from abc import ABCMeta, abstractmethod
 from enum import Enum, unique
 from threading import Event
 from typing import Optional, List, TYPE_CHECKING
 
 from messageflux.utils import KwargsException
 
@@ -144,27 +145,34 @@
         :param device: the input device to read the messages from
         :param with_transaction: 'True' if we should actually use transactions, 'False' otherwise
         """
         super().__init__(device)
         self._with_transaction = with_transaction
         self._transactions: List[InputTransaction] = []
 
-    def read_message(self, timeout: Optional[float] = None) -> Optional['ReadResult']:
+    def read_message(self,
+                     cancellation_token: threading.Event,
+                     timeout: Optional[float] = None) -> Optional['ReadResult']:
         """
         this method returns a message from the device, and adds its transaction to the transaction scope
 
+        :param cancellation_token: the cancellation token for this service. this can be used to know if cancellation
+        was requested
+
         :param timeout: an optional timeout (in seconds) to wait for the device to return a message.
         after 'timeout' seconds (None means block until message is available).
          if the device doesn't have a message to return after timeout seconds, it will return None
 
         :return: a ReadResult object or None if no message was available.
         the device headers can contain extra information about the device that returned the message
         """
 
-        read_result = self.device.read_message(timeout=timeout, with_transaction=self._with_transaction)
+        read_result = self.device.read_message(cancellation_token=cancellation_token,
+                                               timeout=timeout,
+                                               with_transaction=self._with_transaction)
 
         if read_result is not None:
             self._transactions.append(read_result.transaction)
 
         return read_result
 
     def _commit(self):
```

### Comparing `messageflux-0.2.6/messageflux/iodevices/base/output_devices.py` & `messageflux-0.3.0/messageflux/iodevices/base/output_devices.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.6/messageflux/iodevices/collection_device_wrapper/collection_input_device.py` & `messageflux-0.3.0/messageflux/iodevices/collection_device_wrapper/collection_input_device.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
+import threading
+from time import perf_counter
 from typing import Optional, Collection, List, Callable
 
-from time import sleep, perf_counter
-
 from messageflux import InputDevice, ReadResult
 from messageflux.iodevices.base import InputDeviceManager, InputDeviceException
 
 
 class CollectionInputDevice(InputDevice['CollectionInputDeviceManager']):
     """
     this class reads from a collection of input devices.
@@ -26,18 +26,24 @@
         :param input_devices: the devices that this aggregate device reads from
 
         """
         super(CollectionInputDevice, self).__init__(device_manager, device_name)
         self._input_devices = input_devices
         self._logger = logging.getLogger(__name__)
 
-    def _read_message(self, timeout: Optional[float] = None, with_transaction: bool = True) -> Optional['ReadResult']:
+    def _read_message(self,
+                      cancellation_token: threading.Event,
+                      timeout: Optional[float] = None,
+                      with_transaction: bool = True) -> Optional['ReadResult']:
         """
         reads a message from device
 
+        :param cancellation_token: the cancellation token for this service. this can be used to know if cancellation
+        was requested
+
         :param timeout: an optional timeout (in seconds) to wait for the device to return a message.
         after 'timeout' seconds, if the device doesn't have a message to return, it will return None
 
         :param with_transaction: 'True' if the device should read message within transaction,
         or 'False' if the message is automatically committed
 
         :return: a ReadResult object or None if no message was available.
@@ -47,15 +53,17 @@
         if timeout is not None:
             end_time = perf_counter() + timeout
 
         while True:
             failures = []
             for curr_device in self._input_devices:
                 try:
-                    read_result = curr_device._read_message(0, with_transaction=with_transaction)
+                    read_result = curr_device._read_message(cancellation_token=cancellation_token,
+                                                            timeout=0,
+                                                            with_transaction=with_transaction)
                     if read_result is not None:
                         return read_result
                     if timeout is not None and perf_counter() >= end_time:
                         break
                 except Exception as ex:
                     failures.append(ex)
                     self._logger.warning(f"Error reading from {curr_device.name} device", exc_info=True)
@@ -66,15 +74,15 @@
                 self._logger.error('Error reading from CollectionInputDevice - all devices failed')
                 raise InputDeviceException('Error reading from CollectionInputDevice - all devices failed',
                                            inner_exceptions=failures)
 
             if timeout is not None and perf_counter() >= end_time:
                 return None
             else:
-                sleep(self._SLEEP_BETWEEN_ITERATIONS)
+                cancellation_token.wait(self._SLEEP_BETWEEN_ITERATIONS)
 
     def close(self):
         """
         closes the connection to device
         """
         for device in self._input_devices:
             try:
```

### Comparing `messageflux-0.2.6/messageflux/iodevices/collection_device_wrapper/collection_output_device.py` & `messageflux-0.3.0/messageflux/iodevices/collection_device_wrapper/collection_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.6/messageflux/iodevices/failover_output_device_wrapper/failover_output_device.py` & `messageflux-0.3.0/messageflux/iodevices/failover_output_device_wrapper/failover_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.6/messageflux/iodevices/file_system/__init__.py` & `messageflux-0.3.0/messageflux/iodevices/file_system/__init__.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.6/messageflux/iodevices/file_system/file_system_device_manager_base.py` & `messageflux-0.3.0/messageflux/iodevices/file_system/file_system_device_manager_base.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.6/messageflux/iodevices/file_system/file_system_input_device.py` & `messageflux-0.3.0/messageflux/iodevices/file_system/file_system_input_device.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import json
 import logging
 import os
 import random
 import threading
+import time
 from collections import defaultdict
 from random import randint
 from typing import Optional, Dict, List, Set, Iterator
 
-import time
-
 from messageflux.iodevices.base import InputTransaction, InputDeviceManager, InputDevice, ReadResult, \
     InputDeviceException
 from messageflux.iodevices.file_system.file_system_device_manager_base import FileSystemDeviceManagerBase
 from messageflux.iodevices.file_system.file_system_serializer import FileSystemSerializerBase, \
     DefaultFileSystemSerializer
 from messageflux.metadata_headers import MetadataHeaders
 from messageflux.utils import get_random_id
@@ -402,18 +401,24 @@
         file_path = direntry.path
         return FileSystemInputTransaction.read_file(self,
                                                     org_path=file_path,
                                                     tmp_folder=self._tmp_folder,
                                                     with_transaction=with_transaction,
                                                     serializer=self._serializer)
 
-    def _read_message(self, timeout: Optional[float] = None, with_transaction: bool = True) -> Optional[ReadResult]:
+    def _read_message(self,
+                      cancellation_token: threading.Event,
+                      timeout: Optional[float] = None,
+                      with_transaction: bool = True) -> Optional[ReadResult]:
         """
         this method returns a message from the file system
 
+        :param cancellation_token: the cancellation token for this service. this can be used to know if cancellation
+        was requested
+
         :param timeout: an optional timeout (in seconds) to wait for the device to return a message.
         after 'timeout' seconds, if the device doesn't have a message to return, it will return None
 
         :param with_transaction: 'True' if the device should read message within transaction,
         or 'False' if the message is automatically committed
 
         :return: a ReadResult object or None if no message was available.
@@ -437,15 +442,15 @@
                             read_result.device_headers.update(fs_metadata)
                             return read_result
                         if timeout is not None and time.perf_counter() >= deadline:
                             break
 
                     if timeout is not None and time.perf_counter() >= deadline:
                         break
-                    time.sleep(self._SLEEP_BETWEEN_BATCHES)
+                    cancellation_token.wait(self._SLEEP_BETWEEN_BATCHES)
             else:
                 while True:
                     got_file = False
                     for direntry in self._get_unsorted_filenames():
                         got_file = True
                         try:
                             fs_metadata = {self.FILENAME_HEADER_NAME: direntry.name,
@@ -459,15 +464,15 @@
                             return read_result
 
                     # couldn't read any file from batch. try bigger batch next time
                     self._increase_batch_size()
                     if timeout is not None and time.perf_counter() >= deadline:
                         break
                     if not got_file:
-                        time.sleep(self._SLEEP_BETWEEN_BATCHES)
+                        cancellation_token.wait(self._SLEEP_BETWEEN_BATCHES)
 
             return None
 
         except Exception as e:
             raise InputDeviceException('Error reading product from device') from e
```

### Comparing `messageflux-0.2.6/messageflux/iodevices/file_system/file_system_output_device.py` & `messageflux-0.3.0/messageflux/iodevices/file_system/file_system_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.6/messageflux/iodevices/file_system/file_system_serializer.py` & `messageflux-0.3.0/messageflux/iodevices/file_system/file_system_serializer.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.6/messageflux/iodevices/in_memory_device/in_memory_device_manager.py` & `messageflux-0.3.0/messageflux/iodevices/in_memory_device/in_memory_device_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import heapq
+import threading
 import time
 from functools import total_ordering
 from threading import Condition
 from typing import Optional, Dict, List, Tuple
 
 from messageflux.iodevices.base import (Message,
                                         InputDeviceManager,
@@ -66,15 +67,19 @@
                  name: str,
                  queue: List[_QueueMessage],
                  queue_not_empty_condition: Condition):
         super().__init__(manager, name)
         self._queue = queue
         self._queue_not_empty = queue_not_empty_condition
 
-    def _read_message(self, timeout: Optional[float] = None, with_transaction: bool = True) -> Optional[ReadResult]:
+    def _read_message(self,
+                      cancellation_token: threading.Event,
+                      timeout: Optional[float] = None,
+                      with_transaction: bool = True) -> Optional[ReadResult]:
+
         with self._queue_not_empty:
             if self._queue_not_empty.wait_for(lambda: any(self._queue), timeout):
                 queue_message = heapq.heappop(self._queue)
                 transaction: InputTransaction
                 if with_transaction:
                     transaction = self.InMemoryTransaction(self, queue_message)
                 else:
```

### Comparing `messageflux-0.2.6/messageflux/iodevices/message_store_device_wrapper/file_system_message_store.py` & `messageflux-0.3.0/messageflux/iodevices/message_store_device_wrapper/file_system_message_store.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.6/messageflux/iodevices/message_store_device_wrapper/message_store_base.py` & `messageflux-0.3.0/messageflux/iodevices/message_store_device_wrapper/message_store_base.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.6/messageflux/iodevices/message_store_device_wrapper/message_store_input_device.py` & `messageflux-0.3.0/messageflux/iodevices/message_store_device_wrapper/message_store_input_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.6/messageflux/iodevices/message_store_device_wrapper/message_store_output_device.py` & `messageflux-0.3.0/messageflux/iodevices/message_store_device_wrapper/message_store_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.6/messageflux/iodevices/message_store_device_wrapper/message_store_transformer_base.py` & `messageflux-0.3.0/messageflux/iodevices/message_store_device_wrapper/message_store_transformer_base.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.6/messageflux/iodevices/objectstorage/s3_message_store.py` & `messageflux-0.3.0/messageflux/iodevices/objectstorage/s3_message_store.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.6/messageflux/iodevices/objectstorage/s3api/s3bucket.py` & `messageflux-0.3.0/messageflux/iodevices/objectstorage/s3api/s3bucket.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.6/messageflux/iodevices/objectstorage/s3api/s3client.py` & `messageflux-0.3.0/messageflux/iodevices/objectstorage/s3api/s3client.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.6/messageflux/iodevices/rabbitmq/fs_poison_counter.py` & `messageflux-0.3.0/messageflux/iodevices/rabbitmq/fs_poison_counter.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.6/messageflux/iodevices/rabbitmq/rabbitmq_device_manager_base.py` & `messageflux-0.3.0/messageflux/iodevices/rabbitmq/rabbitmq_device_manager_base.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.6/messageflux/iodevices/rabbitmq/rabbitmq_input_device.py` & `messageflux-0.3.0/messageflux/iodevices/rabbitmq/rabbitmq_input_device.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 import os
 import socket
 import ssl
+import threading
 from io import BytesIO
 from typing import TYPE_CHECKING, Dict, Optional, Tuple, Union, List, Any
 
 from messageflux.iodevices.base import InputDevice, InputTransaction, ReadResult, InputDeviceException, Message, \
     InputDeviceManager
 from messageflux.iodevices.base.input_transaction import NULLTransaction
 from messageflux.iodevices.rabbitmq.rabbitmq_device_manager_base import RabbitMQDeviceManagerBase
@@ -22,24 +23,27 @@
 
 class RabbitMQInputTransaction(InputTransaction):
     """
     represents a InputTransaction for RabbitMQ
     """
 
     def __init__(self,
+                 cancellation_token: threading.Event,
                  device: 'RabbitMQInputDevice',
                  channel: 'BlockingChannel',
                  delivery_tag: int):
         """
 
+        :param cancellation_token: the cancellation token, to check before acking
         :param device: the device that returned this transaction
         :param channel: the BlockingChannel that the item was read from
         :param delivery_tag: the delivery tag for this item
         """
         super(RabbitMQInputTransaction, self).__init__(device=device)
+        self._cancellation_token = cancellation_token
         self._channel = channel
         self._delivery_tag = delivery_tag
         self._logger = logging.getLogger(__name__)
 
     @property
     def channel(self) -> 'BlockingChannel':
         """
@@ -52,32 +56,42 @@
         """
         the delivery tag for this item
         """
         return self._delivery_tag
 
     def _commit(self):
         try:
+            if self._cancellation_token.is_set():
+                try:
+                    self._channel.cancel()  # cancel the consumer before acking
+                except Exception:
+                    pass
             self._channel.basic_ack(self._delivery_tag)
         except Exception:
             self._logger.warning('commit failed', exc_info=True)
 
     def _rollback(self):
         try:
+            if self._cancellation_token.is_set():
+                try:
+                    self._channel.cancel()  # cancel the consumer before nacking
+                except Exception:
+                    pass
             self._channel.basic_nack(self._delivery_tag, requeue=True)
         except Exception:
             self._logger.warning('rollback failed', exc_info=True)
 
 
 class RabbitMQInputDevice(InputDevice['RabbitMQInputDeviceManager']):
     """
     represents an RabbitMQ input device
     """
 
-    _channel: Union[ThreadLocalMember[Optional['BlockingChannel']],
-                    Optional['BlockingChannel']] = ThreadLocalMember(init_value=None)
+    _channel: Union[ThreadLocalMember[Optional['BlockingChannel']], Optional['BlockingChannel']] = ThreadLocalMember(
+        init_value=None)
 
     @staticmethod
     def _get_rabbit_headers(method_frame, header_frame):
         return {
             "exchange": method_frame.exchange,
             "routing_key": method_frame.routing_key,
             "content_type": header_frame.content_type,
@@ -126,15 +140,18 @@
         """
         reconnects the RabbitMQ device manager
         """
         try:
             if self._channel is not None and self._channel.is_open:
                 assert self._channel is not None
                 if self._use_consumer:
-                    self._channel.cancel()
+                    try:
+                        self._channel.cancel()
+                    except Exception:
+                        pass
                 self._channel.close()
             self._channel = self._device_manager.connection.channel()
 
             assert self._channel is not None
             self._channel.basic_qos(prefetch_count=self._prefetch_count)
         except Exception as e:
             raise InputDeviceException('Could not connect to rabbitmq.') from e
@@ -145,18 +162,22 @@
         """
         if self._channel is None or not self._channel.is_open:
             self._reconnect_device_manager()
 
         assert self._channel is not None
         return self._channel
 
-    def _get_data_from_queue(self, timeout: Optional[float], with_transaction: bool) -> Optional['ReadResult']:
+    def _get_data_from_queue(self,
+                             cancellation_token: threading.Event,
+                             timeout: Optional[float],
+                             with_transaction: bool) -> Optional['ReadResult']:
         """
         performs a single read from queue
 
+        :param cancellation_token: the cancellation token, to pass to transaction
         :param timeout: the timeout in seconds to block. negative number means no blocking
         :param with_transaction: does this read is to be done with transaction?
         :return: the stream and metadata, or None,None if no message in queue
         """
         channel = self._get_channel()
         get_timeout: Optional[float] = None
         if timeout is not None:
@@ -170,59 +191,68 @@
                                                                        with_transaction=with_transaction)
         if method_frame is None:  # no message in queue
             return None
 
         assert body is not None
         assert header_frame is not None
 
-        return self._create_response_from_frames(body,
-                                                 header_frame,
-                                                 method_frame,
-                                                 channel,
-                                                 with_transaction)
+        return self._create_response_from_frames(cancellation_token=cancellation_token,
+                                                 body=body,
+                                                 header_frame=header_frame,
+                                                 method_frame=method_frame,
+                                                 channel=channel,
+                                                 with_transaction=with_transaction)
 
     def _create_response_from_frames(self,
+                                     cancellation_token: threading.Event,
                                      body: bytes,
                                      header_frame: spec.BasicProperties,
                                      method_frame: Union[spec.Basic.Deliver, spec.Basic.GetOk],
                                      channel: 'BlockingChannel',
                                      with_transaction: bool) -> ReadResult:
         """
         creates the read result from the data returned from rabbitmq
 
+        :param cancellation_token: the cancellation token, to pass to transaction
         :param body: the body of the message
         :param header_frame: the header frame of the message
         :param method_frame: the method frame of the message
         :param channel: the channel we read the message from
         :param with_transaction: should we use a transaction
 
         :return: ReadResult object
         """
 
         delivery_tag = method_frame.delivery_tag
         assert delivery_tag is not None
         if with_transaction:
-            transaction: InputTransaction = RabbitMQInputTransaction(self, channel, delivery_tag)
+            transaction: InputTransaction = RabbitMQInputTransaction(cancellation_token=cancellation_token,
+                                                                     device=self,
+                                                                     channel=channel,
+                                                                     delivery_tag=delivery_tag)
         else:
             transaction = NULLTransaction(self)
         headers: Dict[str, Any] = header_frame.headers or {}  # type: ignore
         # get the rabbitmq headers as for device headers
         rabbit_headers = self._get_rabbit_headers(method_frame, header_frame)
 
         buf = BytesIO(body)
         return ReadResult(message=Message(buf, headers),
                           device_headers=rabbit_headers,
                           transaction=transaction)
 
     def _get_frames_from_queue(self,
                                channel: 'BlockingChannel',
                                timeout: Optional[float],
-                               with_transaction: bool) -> Tuple[Optional[bytes],
-                                                                Optional[spec.BasicProperties],
-                                                                Optional[Union[spec.Basic.Deliver, spec.Basic.GetOk]]]:
+                               with_transaction: bool) -> Tuple[
+        Optional[bytes],
+        Optional[spec.BasicProperties],
+        Optional[Union[spec.Basic.Deliver, spec.Basic.GetOk]]
+    ]:
+
         """
         gets the actual frame from queue. use_consumer effects this method
 
         :param BlockingChannel channel: the channel
         :param float timeout: the timeout
         :param bool with_transaction: do we operate within a transaction scope
         """
@@ -249,32 +279,39 @@
                                                                     arguments=self._consumer_args, auto_ack=auto_ack))
         else:
             method_frame, header_frame, body = channel.basic_get(queue=self._queue_name,  # type: ignore
                                                                  auto_ack=auto_ack)
 
         return body, header_frame, method_frame
 
-    def _read_message(self, timeout: Optional[float] = None, with_transaction: bool = True) -> Optional['ReadResult']:
+    def _read_message(self,
+                      cancellation_token: threading.Event,
+                      timeout: Optional[float] = None,
+                      with_transaction: bool = True) -> Optional['ReadResult']:
         """
         reads a stream from InputDevice (tries getting a message. if it fails, reconnects and tries again once)
 
         :param timeout: the timeout in seconds to block. negative number means no blocking
         :return: a tuple of stream and metadata from InputDevice, or (None, None) if no message is available
         """
         try:
             from pika.exceptions import AMQPConnectionError, AMQPChannelError
         except ImportError as exc:
             raise ImportError('Please Install the required extra: messageflux[rabbitmq]') from exc
 
         try:
-            return self._get_data_from_queue(timeout=timeout, with_transaction=with_transaction)
+            return self._get_data_from_queue(cancellation_token=cancellation_token,
+                                             timeout=timeout,
+                                             with_transaction=with_transaction)
         except (AMQPConnectionError, AMQPChannelError):
             self._reconnect_device_manager()
             try:
-                return self._get_data_from_queue(timeout=timeout, with_transaction=with_transaction)
+                return self._get_data_from_queue(cancellation_token=cancellation_token,
+                                                 timeout=timeout,
+                                                 with_transaction=with_transaction)
             except Exception:
                 self._logger.exception(f"AMQError thrown. failed to get message. device name: {self._queue_name}")
                 raise
         except Exception as e:
             raise InputDeviceException('Error reading from device') from e
 
     def close(self):
```

### Comparing `messageflux-0.2.6/messageflux/iodevices/rabbitmq/rabbitmq_output_device.py` & `messageflux-0.3.0/messageflux/iodevices/rabbitmq/rabbitmq_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.6/messageflux/iodevices/rabbitmq/rabbitmq_poison_counting_input_device.py` & `messageflux-0.3.0/messageflux/iodevices/rabbitmq/rabbitmq_poison_counting_input_device.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import ssl
+import threading
 from abc import ABCMeta, abstractmethod
-from typing import List, Dict, Optional
-
 from time import perf_counter
+from typing import List, Dict, Optional
 
 from messageflux.iodevices.base import InputTransaction, ReadResult
 from messageflux.iodevices.rabbitmq.rabbitmq_input_device import RabbitMQInputDevice, RabbitMQInputDeviceManager
 
 
 class PoisonCounterBase(metaclass=ABCMeta):
     """
@@ -104,18 +104,21 @@
                          consumer_args=consumer_args,
                          prefetch_count=prefetch_count,
                          use_consumer=use_consumer)
         self._max_poison_count = max_poison_count
         self._poison_counter = poison_counter
 
     def _get_data_from_queue(self,
+                             cancellation_token: threading.Event,
                              timeout: Optional[float],
                              with_transaction: bool) -> Optional['ReadResult']:
         """
         performs a single read from queue
+
+        :param cancellation_token: the cancellation token, to pass to transaction
         :param timeout: the timeout in seconds to block. None means no blocking
         :param with_transaction: does this read is to be done with transaction?
         :return: the stream and metadata, or None,None if no message in queue
         """
         start_time = perf_counter()
 
         while True:
@@ -137,17 +140,20 @@
                 break
 
             else:  # this message was redelivered. protect from poison message
                 assert header_frame is not None
                 message_id = f'{self.name}-{header_frame.message_id}-{header_frame.timestamp}'
                 redeliver_count = self._poison_counter.increment_and_return_counter(message_id)
                 if redeliver_count < self._max_poison_count:  # this message is below the max_poison_threshold
-                    read_result = self._create_response_from_frames(body, header_frame, method_frame,
-                                                                    channel,
-                                                                    with_transaction)
+                    read_result = self._create_response_from_frames(cancellation_token=cancellation_token,
+                                                                    body=body,
+                                                                    header_frame=header_frame,
+                                                                    method_frame=method_frame,
+                                                                    channel=channel,
+                                                                    with_transaction=with_transaction)
                     return ReadResult(message=read_result.message,
                                       device_headers=read_result.device_headers,
                                       transaction=RabbitMQNoPoisonInputTransactionWrapper(
                                           inner_transaction=read_result.transaction,
                                           poison_counter=self._poison_counter,
                                           message_id=message_id))
 
@@ -168,15 +174,20 @@
                 # but only if we're not exceeding timeout
                 if timeout is not None:
                     if perf_counter() >= start_time + max(timeout, 1):
                         return None
 
                 continue
 
-        return self._create_response_from_frames(body, header_frame, method_frame, channel, with_transaction)
+        return self._create_response_from_frames(cancellation_token=cancellation_token,
+                                                 body=body,
+                                                 header_frame=header_frame,
+                                                 method_frame=method_frame,
+                                                 channel=channel,
+                                                 with_transaction=with_transaction)
 
 
 class RabbitMQPoisonCountingInputDeviceManager(RabbitMQInputDeviceManager):
     """
     rabbitmq input device manager, that adds handling with poison messages (for classic queues)
     """
```

### Comparing `messageflux-0.2.6/messageflux/iodevices/round_robin_device_wrapper/roundrobin_io_device_manager.py` & `messageflux-0.3.0/messageflux/iodevices/round_robin_device_wrapper/roundrobin_io_device_manager.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.6/messageflux/iodevices/short_circuit_device_wrapper/common.py` & `messageflux-0.3.0/messageflux/iodevices/short_circuit_device_wrapper/common.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.6/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_input_device.py` & `messageflux-0.3.0/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_input_device.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import threading
 from typing import Optional
 
 from messageflux.iodevices.base import InputDevice, ReadResult, InputDeviceManager
 from messageflux.iodevices.short_circuit_device_wrapper.common import ShortCircuitDeviceBase
 
 
 class ShortCircuitInputDevice(ShortCircuitDeviceBase, InputDevice['ShortCircuitInputDeviceManager']):
@@ -15,18 +16,23 @@
                  inner_device: InputDevice,
                  short_circuit_fail_count: int,
                  short_circuit_time: int):
         InputDevice.__init__(self, manager, name)
         ShortCircuitDeviceBase.__init__(self, short_circuit_fail_count, short_circuit_time)
         self._inner_device = inner_device
 
-    def _read_message(self, timeout: Optional[float] = None, with_transaction: bool = True) -> Optional[ReadResult]:
+    def _read_message(self,
+                      cancellation_token: threading.Event,
+                      timeout: Optional[float] = None,
+                      with_transaction: bool = True) -> Optional[ReadResult]:
         self._validate_short_circuit()
         with self._failure_count_context():
-            return self._inner_device.read_message(timeout=timeout, with_transaction=with_transaction)
+            return self._inner_device.read_message(cancellation_token=cancellation_token,
+                                                   timeout=timeout,
+                                                   with_transaction=with_transaction)
 
     def close(self):
         """
         closes the inner device
         """
         self._inner_device.close()
```

### Comparing `messageflux-0.2.6/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_output_device.py` & `messageflux-0.3.0/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.6/messageflux/iodevices/transformer_device_wrapper/transformer_input_device.py` & `messageflux-0.3.0/messageflux/iodevices/transformer_device_wrapper/transformer_input_device.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import threading
 from abc import ABCMeta, abstractmethod
 from typing import Optional
 
 from messageflux.iodevices.base import InputDevice, ReadResult, InputDeviceManager
 
 
 class InputTransformerBase(metaclass=ABCMeta):
@@ -52,16 +53,21 @@
         :param inner_device: the inner device that it wraps
         :param transformer: the transformer to use to transform the incoming messages
         """
         super(TransformerInputDevice, self).__init__(manager, name)
         self._transformer = transformer
         self._inner_device = inner_device
 
-    def _read_message(self, timeout: Optional[float] = None, with_transaction: bool = True) -> Optional[ReadResult]:
-        read_result = self._inner_device.read_message(timeout=timeout, with_transaction=with_transaction)
+    def _read_message(self,
+                      cancellation_token: threading.Event,
+                      timeout: Optional[float] = None,
+                      with_transaction: bool = True) -> Optional[ReadResult]:
+        read_result = self._inner_device.read_message(cancellation_token=cancellation_token,
+                                                      timeout=timeout,
+                                                      with_transaction=with_transaction)
         if read_result is not None:
             read_result = self._transformer.transform_incoming_message(self, read_result)
 
         return read_result
 
     def close(self):
         """
```

### Comparing `messageflux-0.2.6/messageflux/iodevices/transformer_device_wrapper/transformer_output_device.py` & `messageflux-0.3.0/messageflux/iodevices/transformer_device_wrapper/transformer_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.6/messageflux/iodevices/transformer_device_wrapper/zlib_transformer.py` & `messageflux-0.3.0/messageflux/iodevices/transformer_device_wrapper/zlib_transformer.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.6/messageflux/logging/bulk_rotating_device_handler.py` & `messageflux-0.3.0/messageflux/logging/bulk_rotating_device_handler.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.6/messageflux/logging/bulk_rotating_file_handler.py` & `messageflux-0.3.0/messageflux/logging/bulk_rotating_file_handler.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.6/messageflux/logging/bulk_rotating_handler_base.py` & `messageflux-0.3.0/messageflux/logging/bulk_rotating_handler_base.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.6/messageflux/message_handling_service.py` & `messageflux-0.3.0/messageflux/message_handling_service.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,15 +53,16 @@
     def _server_loop(self, cancellation_token: threading.Event):
         assert self._aggregate_input_device is not None
         with InputTransactionScope(device=self._aggregate_input_device,
                                    with_transaction=self._use_transactions) as transaction_scope:
             batch: List[Tuple[InputDevice, ReadResult]] = []
 
             # read first message with _read_timeout anyway
-            read_result = transaction_scope.read_message(timeout=self._read_timeout)
+            read_result = transaction_scope.read_message(cancellation_token=cancellation_token,
+                                                         timeout=self._read_timeout)
             if read_result is not None:
                 last_read_device = self._aggregate_input_device.last_read_device
                 assert last_read_device is not None
                 batch.append((last_read_device, read_result))
 
             end_time = time() + self._read_timeout
             for i in range(self._max_batch_read_count - 1):  # try to read the rest of the batch
@@ -71,15 +72,16 @@
                     break
 
                 if self._wait_for_batch_count:
                     timeout = remaining_time  # if wait_for_batch_count, try to read another message with remaining time
                 else:
                     timeout = 0  # if not wait_for_batch, try to read another message without waiting at all
 
-                read_result = transaction_scope.read_message(timeout=timeout)
+                read_result = transaction_scope.read_message(cancellation_token=cancellation_token,
+                                                             timeout=timeout)
                 if read_result is None:
                     break  # no more messages to read
                 last_read_device = self._aggregate_input_device.last_read_device
                 assert last_read_device is not None
                 batch.append((last_read_device, read_result))
 
             if batch:
```

### Comparing `messageflux-0.2.6/messageflux/multiprocessing/multiprocessrunner.py` & `messageflux-0.3.0/messageflux/multiprocessing/multiprocessrunner.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.6/messageflux/multiprocessing/singleprocesshandler.py` & `messageflux-0.3.0/messageflux/multiprocessing/singleprocesshandler.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.6/messageflux/pipeline_service.py` & `messageflux-0.3.0/messageflux/pipeline_service.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.6/messageflux/server_loop_service.py` & `messageflux-0.3.0/messageflux/server_loop_service.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.6/messageflux/service_addons/loop_health_addon.py` & `messageflux-0.3.0/messageflux/service_addons/loop_health_addon.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.6/messageflux/utils/__init__.py` & `messageflux-0.3.0/messageflux/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.6/messageflux/utils/context.py` & `messageflux-0.3.0/messageflux/utils/context.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.6/messageflux/utils/filesystem.py` & `messageflux-0.3.0/messageflux/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.6/messageflux.egg-info/PKG-INFO` & `messageflux-0.3.0/messageflux.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: messageflux
-Version: 0.2.6
+Version: 0.3.0
 Author-email: Aviv Salem <avivsalem@gmail.com>
 Maintainer-email: Aviv Salem <avivsalem@gmail.com>, Nir Schulman <narsssx@gmail.com>, Rafael Zilberman <Zilberman.rafi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Avivsalem/MessageFlux/
 Project-URL: Documentation, https://messageflux.readthedocs.io/
 Platform: win32
 Platform: linux
```

### Comparing `messageflux-0.2.6/messageflux.egg-info/SOURCES.txt` & `messageflux-0.3.0/messageflux.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.6/pyproject.toml` & `messageflux-0.3.0/pyproject.toml`

 * *Files identical despite different names*

