# Comparing `tmp/apimatic-core-0.2.3.tar.gz` & `tmp/apimatic-core-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apimatic-core-0.2.3.tar", last modified: Thu May 25 12:18:56 2023, max compression
+gzip compressed data, was "apimatic-core-0.2.4.tar", last modified: Mon Jul 24 06:58:09 2023, max compression
```

## Comparing `apimatic-core-0.2.3.tar` & `apimatic-core-0.2.4.tar`

### file list

```diff
@@ -1,129 +1,156 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.107068 apimatic-core-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-05-25 12:18:56.107068 apimatic-core-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9062 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.091068 apimatic-core-0.2.3/apimatic_core/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/api_call.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.091068 apimatic-core-0.2.3/apimatic_core/authentication/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/authentication/header_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.095068 apimatic-core-0.2.3/apimatic_core/authentication/multiple/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/authentication/multiple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/authentication/multiple/and_auth_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/authentication/multiple/auth_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/authentication/multiple/or_auth_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/authentication/multiple/single_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/authentication/query_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.095068 apimatic-core-0.2.3/apimatic_core/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/configurations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/configurations/endpoint_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/configurations/global_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.095068 apimatic-core-0.2.3/apimatic_core/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/decorators/lazy_property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.095068 apimatic-core-0.2.3/apimatic_core/factories/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/factories/http_response_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.095068 apimatic-core-0.2.3/apimatic_core/http/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/http/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.095068 apimatic-core-0.2.3/apimatic_core/http/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/http/configurations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/http/configurations/http_client_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/http/http_callback.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.095068 apimatic-core-0.2.3/apimatic_core/http/request/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/http/request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/http/request/http_request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.095068 apimatic-core-0.2.3/apimatic_core/http/response/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/http/response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/http/response/api_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/http/response/http_response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.095068 apimatic-core-0.2.3/apimatic_core/logger/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/logger/endpoint_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     9845 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/request_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/response_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.099068 apimatic-core-0.2.3/apimatic_core/types/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/types/array_serialization_format.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/types/datetime_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/types/error_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/types/file_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/types/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/types/xml_attributes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.099068 apimatic-core-0.2.3/apimatic_core/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23337 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/utilities/api_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/utilities/auth_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/utilities/comparison_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/utilities/file_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    12961 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/utilities/xml_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.091068 apimatic-core-0.2.3/apimatic_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-05-25 12:18:56.000000 apimatic-core-0.2.3/apimatic_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-05-25 12:18:56.000000 apimatic-core-0.2.3/apimatic_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 12:18:56.000000 apimatic-core-0.2.3/apimatic_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-25 12:18:56.000000 apimatic-core-0.2.3/apimatic_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-25 12:18:56.000000 apimatic-core-0.2.3/apimatic_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 12:18:56.107068 apimatic-core-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.099068 apimatic-core-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.099068 apimatic-core-0.2.3/tests/apimatic_core/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.099068 apimatic-core-0.2.3/tests/apimatic_core/api_call_tests/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/api_call_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/api_call_tests/test_api_call.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.099068 apimatic-core-0.2.3/tests/apimatic_core/api_logger_tests/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/api_logger_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/api_logger_tests/test_api_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    12190 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.099068 apimatic-core-0.2.3/tests/apimatic_core/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.103068 apimatic-core-0.2.3/tests/apimatic_core/mocks/authentications/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/authentications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/authentications/basic_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/authentications/bearer_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/authentications/custom_header_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/authentications/custom_query_authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.103068 apimatic-core-0.2.3/tests/apimatic_core/mocks/callables/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/callables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/callables/base_uri_callable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.103068 apimatic-core-0.2.3/tests/apimatic_core/mocks/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/exceptions/api_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/exceptions/global_test_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/exceptions/local_test_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/exceptions/nested_model_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.103068 apimatic-core-0.2.3/tests/apimatic_core/mocks/http/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/http/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/http/http_response_catcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.103068 apimatic-core-0.2.3/tests/apimatic_core/mocks/logger/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/logger/api_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.107068 apimatic-core-0.2.3/tests/apimatic_core/mocks/models/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/models/api_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/models/cat_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/models/days.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/models/dog_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    15735 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/models/grand_parent_class_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/models/one_of_xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/models/person.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/models/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/models/wolf_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/models/xml_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.107068 apimatic-core-0.2.3/tests/apimatic_core/request_builder_tests/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/request_builder_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45307 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/request_builder_tests/test_request_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.107068 apimatic-core-0.2.3/tests/apimatic_core/response_handler_tests/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/response_handler_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19428 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/response_handler_tests/test_response_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.107068 apimatic-core-0.2.3/tests/apimatic_core/utility_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/utility_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45483 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/utility_tests/test_api_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/utility_tests/test_auth_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)   126287 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/utility_tests/test_comparison_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/utility_tests/test_file_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    34274 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/utility_tests/test_xml_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:58:09.104071 apimatic-core-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10411 2023-07-24 06:58:09.104071 apimatic-core-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10049 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:58:09.088070 apimatic-core-0.2.4/apimatic_core/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/api_call.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:58:09.088070 apimatic-core-0.2.4/apimatic_core/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/authentication/header_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:58:09.088070 apimatic-core-0.2.4/apimatic_core/authentication/multiple/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/authentication/multiple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/authentication/multiple/and_auth_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/authentication/multiple/auth_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/authentication/multiple/or_auth_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/authentication/multiple/single_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/authentication/query_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:58:09.092071 apimatic-core-0.2.4/apimatic_core/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/configurations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/configurations/endpoint_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/configurations/global_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:58:09.092071 apimatic-core-0.2.4/apimatic_core/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/decorators/lazy_property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:58:09.092071 apimatic-core-0.2.4/apimatic_core/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/exceptions/anyof_validation_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/exceptions/oneof_validation_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:58:09.092071 apimatic-core-0.2.4/apimatic_core/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/factories/http_response_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:58:09.092071 apimatic-core-0.2.4/apimatic_core/http/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/http/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:58:09.092071 apimatic-core-0.2.4/apimatic_core/http/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/http/configurations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/http/configurations/http_client_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/http/http_callback.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:58:09.092071 apimatic-core-0.2.4/apimatic_core/http/request/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/http/request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/http/request/http_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:58:09.092071 apimatic-core-0.2.4/apimatic_core/http/response/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/http/response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/http/response/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/http/response/http_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:58:09.092071 apimatic-core-0.2.4/apimatic_core/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/logger/endpoint_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9509 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/request_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/response_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:58:09.092071 apimatic-core-0.2.4/apimatic_core/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/types/array_serialization_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/types/datetime_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/types/error_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/types/file_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/types/parameter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:58:09.092071 apimatic-core-0.2.4/apimatic_core/types/union_types/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/types/union_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/types/union_types/any_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/types/union_types/leaf_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/types/union_types/one_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/types/union_types/union_type_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/types/xml_attributes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:58:09.096071 apimatic-core-0.2.4/apimatic_core/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25683 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/utilities/api_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/utilities/auth_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/utilities/comparison_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/utilities/datetime_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/utilities/file_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/utilities/union_type_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12961 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/apimatic_core/utilities/xml_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:58:09.088070 apimatic-core-0.2.4/apimatic_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10411 2023-07-24 06:58:09.000000 apimatic-core-0.2.4/apimatic_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-07-24 06:58:09.000000 apimatic-core-0.2.4/apimatic_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 06:58:09.000000 apimatic-core-0.2.4/apimatic_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-24 06:58:09.000000 apimatic-core-0.2.4/apimatic_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-24 06:58:09.000000 apimatic-core-0.2.4/apimatic_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 06:58:09.104071 apimatic-core-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:58:09.096071 apimatic-core-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:58:09.096071 apimatic-core-0.2.4/tests/apimatic_core/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:58:09.096071 apimatic-core-0.2.4/tests/apimatic_core/api_call_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/api_call_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/api_call_tests/test_api_call.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:58:09.096071 apimatic-core-0.2.4/tests/apimatic_core/api_logger_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/api_logger_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/api_logger_tests/test_api_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13935 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:58:09.096071 apimatic-core-0.2.4/tests/apimatic_core/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/mocks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:58:09.096071 apimatic-core-0.2.4/tests/apimatic_core/mocks/authentications/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/mocks/authentications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/mocks/authentications/basic_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/mocks/authentications/bearer_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/mocks/authentications/custom_header_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/mocks/authentications/custom_query_authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:58:09.096071 apimatic-core-0.2.4/tests/apimatic_core/mocks/callables/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/mocks/callables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/mocks/callables/base_uri_callable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:58:09.096071 apimatic-core-0.2.4/tests/apimatic_core/mocks/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/mocks/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/mocks/exceptions/api_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/mocks/exceptions/global_test_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/mocks/exceptions/local_test_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/mocks/exceptions/nested_model_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:58:09.096071 apimatic-core-0.2.4/tests/apimatic_core/mocks/http/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/mocks/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/mocks/http/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/mocks/http/http_response_catcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:58:09.100071 apimatic-core-0.2.4/tests/apimatic_core/mocks/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/mocks/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/mocks/logger/api_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:58:09.100071 apimatic-core-0.2.4/tests/apimatic_core/mocks/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/mocks/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/mocks/models/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/mocks/models/atom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/mocks/models/cat_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/mocks/models/complex_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/mocks/models/days.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/mocks/models/deer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/mocks/models/dog_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15735 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/mocks/models/grand_parent_class_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/mocks/models/inner_complex_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/mocks/models/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/mocks/models/months.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/mocks/models/one_of_xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/mocks/models/orbit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/mocks/models/person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/mocks/models/rabbit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/mocks/models/union_type_scalar_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/mocks/models/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/mocks/models/wolf_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/mocks/models/xml_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/mocks/union_type_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:58:09.100071 apimatic-core-0.2.4/tests/apimatic_core/request_builder_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/request_builder_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44470 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/request_builder_tests/test_request_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:58:09.100071 apimatic-core-0.2.4/tests/apimatic_core/response_handler_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/response_handler_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19428 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/response_handler_tests/test_response_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:58:09.100071 apimatic-core-0.2.4/tests/apimatic_core/union_type_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/union_type_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59508 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/union_type_tests/test_any_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59974 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/union_type_tests/test_one_of.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:58:09.104071 apimatic-core-0.2.4/tests/apimatic_core/utility_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/utility_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61724 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/utility_tests/test_api_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/utility_tests/test_auth_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)   126287 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/utility_tests/test_comparison_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/utility_tests/test_datetime_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/utility_tests/test_file_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34274 2023-07-24 06:57:54.000000 apimatic-core-0.2.4/tests/apimatic_core/utility_tests/test_xml_helper.py
```

### Comparing `apimatic-core-0.2.3/LICENSE` & `apimatic-core-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.3/PKG-INFO` & `apimatic-core-0.2.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: apimatic-core
-Version: 0.2.3
-Summary: A library that contains core logic and utilities for consuming REST APIs using Python SDKs generated by APIMatic.
-Home-page: https://github.com/apimatic/core-lib-python
-Author: APIMatic
-Author-email: support@apimatic.io
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # apimatic-core
 [![PyPI][pypi-version]][apimatic-core-pypi-url]
 [![Tests][test-badge]][test-url]
 [![Test Coverage][test-coverage-url]][code-climate-url]
 [![Licence][license-badge]][license-url]
 
 ## Introduction
@@ -73,31 +62,36 @@
 
 ## Logger
 | Name                                                             | Description                                         |
 |------------------------------------------------------------------|-----------------------------------------------------|
 | [`EndpointLogger`](apimatic_core/logger/endpoint_logger.py)      | A class to provide logging for an HTTP request      |
 
 ## Types
-| Name                                                                         | Description                                                                  |
-|------------------------------------------------------------------------------|------------------------------------------------------------------------------|
-| [`SerializationFormats`](apimatic_core/types/array_serialization_format.py)  | An Enumeration of Array serialization formats                                |
-| [`DateTimeFormat`](apimatic_core/types/datetime_format.py )                  | An Enumeration of Date Time formats                                          |
-| [`ErrorCase`](apimatic_core/types/error_case.py )                            | A class to represent Exception types                                         |
-| [`FileWrapper`](apimatic_core/types/file_wrapper.py)                         | A wrapper to allow passing in content type for file uploads                  |
-| [`Parameter`](apimatic_core/types/parameter.py )                             | A class to represent information about a Parameter passed in an endpoint     |
-| [`XmlAttributes`](apimatic_core/types/xml_attributes.py )                    | A class to represent information about a XML Parameter passed in an endpoint |
+| Name                                                                          | Description                                                                  |
+|-------------------------------------------------------------------------------|------------------------------------------------------------------------------|
+| [`SerializationFormats`](apimatic_core/types/array_serialization_format.py)   | An Enumeration of Array serialization formats                                |
+| [`DateTimeFormat`](apimatic_core/types/datetime_format.py )                   | An Enumeration of Date Time formats                                          |
+| [`ErrorCase`](apimatic_core/types/error_case.py )                             | A class to represent Exception types                                         |
+| [`FileWrapper`](apimatic_core/types/file_wrapper.py)                          | A wrapper to allow passing in content type for file uploads                  |
+| [`Parameter`](apimatic_core/types/parameter.py )                              | A class to represent information about a Parameter passed in an endpoint     |
+| [`XmlAttributes`](apimatic_core/types/xml_attributes.py )                     | A class to represent information about a XML Parameter passed in an endpoint |
+| [`OneOf`](apimatic_core/types/union_types/one_of.py )                         | A class to represent information about OneOf union types                     |
+| [`AnyOf`](apimatic_core/types/union_types/any_of.py )                         | A class to represent information about AnyOf union types                     |
+| [`LeafType`](apimatic_core/types/union_types/leaf_type.py )                   | A class to represent the case information in an OneOf or AnyOf union type    |
 
 ## Utilities
-| Name                                                               | Description                                                                          |
-|--------------------------------------------------------------------|--------------------------------------------------------------------------------------|
-| [`ApiHelper`](apimatic_core/utilities/api_helper.py)               | A Helper Class with various functions associated with making an API Call             |
-| [`AuthHelper`](apimatic_core/utilities/auth_helper.py)             | A Helper Class with various functions associated with authentication in API Calls    |
-| [`ComparisonHelper`](apimatic_core/utilities/comparison_helper.py) | A Helper Class used for the comparison of expected and actual API response           |
-| [` FileHelper`](apimatic_core/utilities/file_helper.py)            | A Helper Class for files                                                             |
-| [`XmlHelper`](apimatic_core/utilities/xml_helper.py )              | A Helper class that holds utility methods for xml serialization and deserialization. |
+| Name                                                               | Description                                                                                              |
+|--------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------|
+| [`ApiHelper`](apimatic_core/utilities/api_helper.py)               | A Helper Class with various functions associated with making an API Call                                 |
+| [`AuthHelper`](apimatic_core/utilities/auth_helper.py)             | A Helper Class with various functions associated with authentication in API Calls                        |
+| [`ComparisonHelper`](apimatic_core/utilities/comparison_helper.py) | A Helper Class used for the comparison of expected and actual API response                               |
+| [`FileHelper`](apimatic_core/utilities/file_helper.py)             | A Helper Class for files                                                                                 |
+| [`XmlHelper`](apimatic_core/utilities/xml_helper.py )              | A Helper class that holds utility methods for xml serialization and deserialization.                     |
+| [`DateTimeHelper`](apimatic_core/utilities/datetime_helper.py )    | A Helper class that holds utility methods for validation of different datetime formats.                  |
+| [`UnionTypeHelper`](apimatic_core/utilities/union_type_helper.py ) | A Helper class that holds utility methods for deserialization and validation of OneOf/AnyOf union types. |
 
 ## Links
 * [apimatic-core-interfaces](https://pypi.org/project/apimatic-core-interfaces/)
 
 
 [pypi-version]: https://img.shields.io/pypi/v/apimatic-core
 [apimatic-core-pypi-url]: https://pypi.org/project/apimatic-core/
```

### Comparing `apimatic-core-0.2.3/README.md` & `apimatic-core-0.2.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: apimatic-core
+Version: 0.2.4
+Summary: A library that contains core logic and utilities for consuming REST APIs using Python SDKs generated by APIMatic.
+Home-page: https://github.com/apimatic/core-lib-python
+Author: APIMatic
+Author-email: support@apimatic.io
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # apimatic-core
 [![PyPI][pypi-version]][apimatic-core-pypi-url]
 [![Tests][test-badge]][test-url]
 [![Test Coverage][test-coverage-url]][code-climate-url]
 [![Licence][license-badge]][license-url]
 
 ## Introduction
@@ -62,31 +73,36 @@
 
 ## Logger
 | Name                                                             | Description                                         |
 |------------------------------------------------------------------|-----------------------------------------------------|
 | [`EndpointLogger`](apimatic_core/logger/endpoint_logger.py)      | A class to provide logging for an HTTP request      |
 
 ## Types
-| Name                                                                         | Description                                                                  |
-|------------------------------------------------------------------------------|------------------------------------------------------------------------------|
-| [`SerializationFormats`](apimatic_core/types/array_serialization_format.py)  | An Enumeration of Array serialization formats                                |
-| [`DateTimeFormat`](apimatic_core/types/datetime_format.py )                  | An Enumeration of Date Time formats                                          |
-| [`ErrorCase`](apimatic_core/types/error_case.py )                            | A class to represent Exception types                                         |
-| [`FileWrapper`](apimatic_core/types/file_wrapper.py)                         | A wrapper to allow passing in content type for file uploads                  |
-| [`Parameter`](apimatic_core/types/parameter.py )                             | A class to represent information about a Parameter passed in an endpoint     |
-| [`XmlAttributes`](apimatic_core/types/xml_attributes.py )                    | A class to represent information about a XML Parameter passed in an endpoint |
+| Name                                                                          | Description                                                                  |
+|-------------------------------------------------------------------------------|------------------------------------------------------------------------------|
+| [`SerializationFormats`](apimatic_core/types/array_serialization_format.py)   | An Enumeration of Array serialization formats                                |
+| [`DateTimeFormat`](apimatic_core/types/datetime_format.py )                   | An Enumeration of Date Time formats                                          |
+| [`ErrorCase`](apimatic_core/types/error_case.py )                             | A class to represent Exception types                                         |
+| [`FileWrapper`](apimatic_core/types/file_wrapper.py)                          | A wrapper to allow passing in content type for file uploads                  |
+| [`Parameter`](apimatic_core/types/parameter.py )                              | A class to represent information about a Parameter passed in an endpoint     |
+| [`XmlAttributes`](apimatic_core/types/xml_attributes.py )                     | A class to represent information about a XML Parameter passed in an endpoint |
+| [`OneOf`](apimatic_core/types/union_types/one_of.py )                         | A class to represent information about OneOf union types                     |
+| [`AnyOf`](apimatic_core/types/union_types/any_of.py )                         | A class to represent information about AnyOf union types                     |
+| [`LeafType`](apimatic_core/types/union_types/leaf_type.py )                   | A class to represent the case information in an OneOf or AnyOf union type    |
 
 ## Utilities
-| Name                                                               | Description                                                                          |
-|--------------------------------------------------------------------|--------------------------------------------------------------------------------------|
-| [`ApiHelper`](apimatic_core/utilities/api_helper.py)               | A Helper Class with various functions associated with making an API Call             |
-| [`AuthHelper`](apimatic_core/utilities/auth_helper.py)             | A Helper Class with various functions associated with authentication in API Calls    |
-| [`ComparisonHelper`](apimatic_core/utilities/comparison_helper.py) | A Helper Class used for the comparison of expected and actual API response           |
-| [` FileHelper`](apimatic_core/utilities/file_helper.py)            | A Helper Class for files                                                             |
-| [`XmlHelper`](apimatic_core/utilities/xml_helper.py )              | A Helper class that holds utility methods for xml serialization and deserialization. |
+| Name                                                               | Description                                                                                              |
+|--------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------|
+| [`ApiHelper`](apimatic_core/utilities/api_helper.py)               | A Helper Class with various functions associated with making an API Call                                 |
+| [`AuthHelper`](apimatic_core/utilities/auth_helper.py)             | A Helper Class with various functions associated with authentication in API Calls                        |
+| [`ComparisonHelper`](apimatic_core/utilities/comparison_helper.py) | A Helper Class used for the comparison of expected and actual API response                               |
+| [`FileHelper`](apimatic_core/utilities/file_helper.py)             | A Helper Class for files                                                                                 |
+| [`XmlHelper`](apimatic_core/utilities/xml_helper.py )              | A Helper class that holds utility methods for xml serialization and deserialization.                     |
+| [`DateTimeHelper`](apimatic_core/utilities/datetime_helper.py )    | A Helper class that holds utility methods for validation of different datetime formats.                  |
+| [`UnionTypeHelper`](apimatic_core/utilities/union_type_helper.py ) | A Helper class that holds utility methods for deserialization and validation of OneOf/AnyOf union types. |
 
 ## Links
 * [apimatic-core-interfaces](https://pypi.org/project/apimatic-core-interfaces/)
 
 
 [pypi-version]: https://img.shields.io/pypi/v/apimatic-core
 [apimatic-core-pypi-url]: https://pypi.org/project/apimatic-core/
```

### Comparing `apimatic-core-0.2.3/apimatic_core/api_call.py` & `apimatic-core-0.2.4/apimatic_core/api_call.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.3/apimatic_core/authentication/multiple/and_auth_group.py` & `apimatic-core-0.2.4/apimatic_core/authentication/multiple/and_auth_group.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.3/apimatic_core/authentication/multiple/auth_group.py` & `apimatic-core-0.2.4/apimatic_core/authentication/multiple/auth_group.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
     def with_auth_managers(self, auth_managers):
         for participant in self.auth_participants:
             self.mapped_group.append(participant.with_auth_managers(auth_managers))
 
         return self
 
-    def is_valid(self):
+    def is_valid(self):  # pragma: no cover
         ...
 
     def apply(self, http_request):
         if not self.is_valid_group:
             return
 
         for participant in self.mapped_group:
```

### Comparing `apimatic-core-0.2.3/apimatic_core/authentication/multiple/or_auth_group.py` & `apimatic-core-0.2.4/apimatic_core/authentication/multiple/or_auth_group.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.3/apimatic_core/authentication/multiple/single_auth.py` & `apimatic-core-0.2.4/apimatic_core/authentication/multiple/single_auth.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.3/apimatic_core/configurations/endpoint_configuration.py` & `apimatic-core-0.2.4/apimatic_core/configurations/endpoint_configuration.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.3/apimatic_core/configurations/global_configuration.py` & `apimatic-core-0.2.4/apimatic_core/configurations/global_configuration.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.3/apimatic_core/http/configurations/http_client_configuration.py` & `apimatic-core-0.2.4/apimatic_core/http/configurations/http_client_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 from apimatic_core.factories.http_response_factory import HttpResponseFactory
 
 
-class HttpClientConfiguration(object):
+class HttpClientConfiguration(object):  # pragma: no cover
     """A class used for configuring the SDK by a user.
     """
 
     @property
     def http_response_factory(self):
         return self._http_response_factory
```

### Comparing `apimatic-core-0.2.3/apimatic_core/http/http_callback.py` & `apimatic-core-0.2.4/apimatic_core/http/http_callback.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,25 +5,23 @@
     HTTP call for an endpoint is made.
 
     This class should not be instantiated but should be used as a base class
     for HttpCallBack classes.
 
     """
 
-    def on_before_request(self,
-                          request):
+    def on_before_request(self, request):  # pragma: no cover
         """The controller will call this method before making the HttpRequest.
 
         Args:
             request (HttpRequest): The request object which will be sent
                 to the HttpClient to be executed.
         """
         raise NotImplementedError("This method has not been implemented.")
 
-    def on_after_response(self,
-                          http_response):
+    def on_after_response(self, http_response):  # pragma: no cover
         """The controller will call this method after making the HttpRequest.
 
         Args:
             http_response (HttpResponse): The HttpResponse of the API call.
         """
         raise NotImplementedError("This method has not been implemented.")
```

### Comparing `apimatic-core-0.2.3/apimatic_core/http/request/http_request.py` & `apimatic-core-0.2.4/apimatic_core/http/request/http_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         Args:
             name (string): The name of the header.
             value (string): The value of the header.
 
         """
         self.headers[name] = value
 
-    def add_parameter(self, name, value):
+    def add_parameter(self, name, value):  # pragma: no cover
         """ Add a parameter to the HttpRequest.
 
         Args:
             name (string): The name of the parameter.
             value (string): The value of the parameter.
 
         """
```

### Comparing `apimatic-core-0.2.3/apimatic_core/http/response/api_response.py` & `apimatic-core-0.2.4/apimatic_core/http/response/api_response.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.3/apimatic_core/http/response/http_response.py` & `apimatic-core-0.2.4/apimatic_core/http/response/http_response.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.3/apimatic_core/request_builder.py` & `apimatic-core-0.2.4/apimatic_core/request_builder.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,14 @@
         self._header_params = {}
         self._query_params = {}
         self._form_params = {}
         self._additional_form_params = {}
         self._additional_query_params = {}
         self._multipart_params = []
         self._body_param = None
-        self._should_wrap_body_param = None
         self._body_serializer = None
         self._auth = None
         self._array_serialization_format = SerializationFormats.INDEXED
         self._xml_attributes = None
         self._endpoint_name_for_logging = None
         self._endpoint_logger = None
 
@@ -86,18 +85,14 @@
             if not self._body_param:
                 self._body_param = dict()
             self._body_param[body_param.get_key()] = body_param.get_value()
         else:
             self._body_param = body_param.get_value()
         return self
 
-    def should_wrap_body_param(self, should_wrap_body_param):
-        self._should_wrap_body_param = should_wrap_body_param
-        return self
-
     def body_serializer(self, body_serializer):
         self._body_serializer = body_serializer
         return self
 
     def auth(self, auth):
         self._auth = auth
         return self
@@ -180,16 +175,14 @@
 
         if self._xml_attributes:
             return self.process_xml_parameters(self._body_serializer)
         elif self._form_params or self._additional_form_params:
             self.add_additional_form_params()
             return ApiHelper.form_encode_parameters(self._form_params, self._array_serialization_format)
         elif self._body_param is not None and self._body_serializer:
-            if self._should_wrap_body_param:
-                return self._body_serializer(self.resolve_body_param(), self._should_wrap_body_param)
             return self._body_serializer(self.resolve_body_param())
         elif self._body_param is not None and not self._body_serializer:
             return self.resolve_body_param()
 
     def process_xml_parameters(self, body_serializer):
         if self._xml_attributes.get_array_item_name():
             return body_serializer(self._xml_attributes.get_value(),
```

### Comparing `apimatic-core-0.2.3/apimatic_core/response_handler.py` & `apimatic-core-0.2.4/apimatic_core/response_handler.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.3/apimatic_core/types/array_serialization_format.py` & `apimatic-core-0.2.4/apimatic_core/types/array_serialization_format.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.3/apimatic_core/types/error_case.py` & `apimatic-core-0.2.4/apimatic_core/types/error_case.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.3/apimatic_core/types/parameter.py` & `apimatic-core-0.2.4/apimatic_core/types/parameter.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,15 @@
             self
     ):
         self._key = None
         self._value = None
         self._is_required = False
         self._should_encode = False
         self._default_content_type = None
+        self._validator = None
 
     def key(self, key):
         self._key = key
         return self
 
     def value(self, value):
         self._value = value
@@ -38,11 +39,18 @@
         self._should_encode = should_encode
         return self
 
     def default_content_type(self, default_content_type):
         self._default_content_type = default_content_type
         return self
 
+    def validator(self, validator):
+        self._validator = validator
+        return self
+
     def validate(self):
         if self._is_required and self._value is None:
             raise ValueError("Required parameter {} cannot be None.".format(self._key))
 
+        if self._validator is not None and self._validator(self._value):
+            return
+
```

### Comparing `apimatic-core-0.2.3/apimatic_core/types/xml_attributes.py` & `apimatic-core-0.2.4/apimatic_core/types/xml_attributes.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.3/apimatic_core/utilities/api_helper.py` & `apimatic-core-0.2.4/apimatic_core/utilities/api_helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 # -*- coding: utf-8 -*-
 from collections import abc
 import re
 import datetime
 import calendar
 import email.utils as eut
 from time import mktime
-
 import jsonpickle
 import dateutil.parser
 from jsonpointer import JsonPointerException, resolve_pointer
-
 from apimatic_core.types.datetime_format import DateTimeFormat
 from apimatic_core.types.file_wrapper import FileWrapper
 from apimatic_core.types.array_serialization_format import SerializationFormats
 from requests.utils import quote
 
 
 class ApiHelper(object):
@@ -25,34 +23,14 @@
     class.
 
     """
 
     SKIP = '#$%^S0K1I2P3))*'
 
     @staticmethod
-    def get_request_parameter(value, is_wrapped=False):
-        """get the correct serialization method for a oneof/anyof parameter type.
-
-        Args:
-            value: the value of the request parameter
-            is_wrapped: whether parameter are wrapped in object or not
-
-        Returns:
-             A correct serialized value which can be used
-             when sending a request.
-
-        """
-
-        if type(value) is str:
-            return value
-        if is_wrapped:
-            return ApiHelper.json_serialize_wrapped_params(value)
-        return ApiHelper.json_serialize(value)
-
-    @staticmethod
     def json_serialize_wrapped_params(obj):
         """JSON Serialization of a given wrapped object.
 
         Args:
             obj (object): The object to serialize.
 
         Returns:
@@ -75,39 +53,57 @@
             obj (object): The object to serialize.
             should_encode: whether to encode at end or not
 
         Returns:
             str: The JSON serialized string of the object.
 
         """
+
         if obj is None:
             return None
 
+        if isinstance(obj, str):
+            return obj
+
         # Resolve any Names if it's one of our objects that needs to have this called on
         if isinstance(obj, list):
             value = list()
             for item in obj:
-                if hasattr(item, "_names"):
+                if isinstance(item, dict) or isinstance(item, list):
+                    value.append(ApiHelper.json_serialize(item, False))
+                elif hasattr(item, "_names"):
                     value.append(ApiHelper.to_dictionary(item))
                 else:
                     value.append(item)
             obj = value
+        elif isinstance(obj, dict):
+            value = dict()
+            for key, item in obj.items():
+                if isinstance(item, list) or isinstance(item, dict):
+                    value[key] = ApiHelper.json_serialize(item, False)
+                elif hasattr(item, "_names"):
+                    value[key] = ApiHelper.to_dictionary(item)
+                else:
+                    value[key] = item
+            obj = value
         else:
             if hasattr(obj, "_names"):
                 obj = ApiHelper.to_dictionary(obj)
         if not should_encode:
             return obj
         return jsonpickle.encode(obj, False)
 
     @staticmethod
     def json_deserialize(json, unboxing_function=None, as_dict=False):
         """JSON Deserialization of a given string.
 
         Args:
             json (str): The JSON serialized string to deserialize.
+            unboxing_function (callable): The deserialization funtion to be used.
+            as_dict (bool): The flag to determine to deserialize json as dictionary type
 
         Returns:
             dict: A dictionary representing the data contained in the
                 JSON serialized string.
 
         """
         if json is None:
@@ -171,14 +167,17 @@
            datetime_format: The date time format to deserialize into
 
         Returns:
             dict: A dictionary representing the data contained in the
                 JSON serialized string.
 
         """
+        if response is None:
+            return None
+
         if isinstance(response, str):
             deserialized_response = ApiHelper.json_deserialize(response)
         else:
             deserialized_response = response
 
         if DateTimeFormat.HTTP_DATE_TIME == datetime_format:
             if isinstance(deserialized_response, list):
@@ -196,14 +195,23 @@
             if isinstance(deserialized_response, list):
                 return [element.datetime for element in
                         ApiHelper.json_deserialize(response, ApiHelper.RFC3339DateTime.from_value)]
             else:
                 return ApiHelper.RFC3339DateTime.from_value(response).datetime
 
     @staticmethod
+    def deserialize_union_type(union_type, response, should_deserialize=True):
+        if should_deserialize:
+            response = ApiHelper.json_deserialize(response, as_dict=True)
+
+        union_type_result = union_type.validate(response)
+
+        return union_type_result.deserialize(response)
+
+    @staticmethod
     def get_content_type(value):
         """Get content type header for oneof.
 
         Args:
             value: The value passed by the user.
 
         Returns:
@@ -310,17 +318,15 @@
                 replace_value = quote(str(value), safe='') if encode else str(value)
 
             url = url.replace('{{{0}}}'.format(key), str(replace_value))
 
         return url
 
     @staticmethod
-    def append_url_with_query_parameters(url,
-                                         parameters,
-                                         array_serialization="indexed"):
+    def append_url_with_query_parameters(url, parameters, array_serialization="indexed"):
         """Adds query parameters to a URL.
 
         Args:
             url (str): The URL string.
             parameters (dict): The query parameters to add to the URL.
             array_serialization (str): The format of array parameter serialization.
 
@@ -373,16 +379,15 @@
         query_url = url[len(protocol): index if index != -1 else None]
         query_url = re.sub("//+", "/", query_url)
         parameters = url[index:] if index != -1 else ""
 
         return protocol + query_url + parameters
 
     @staticmethod
-    def form_encode_parameters(form_parameters,
-                               array_serialization="indexed"):
+    def form_encode_parameters(form_parameters, array_serialization="indexed"):
         """Form encodes a dictionary of form parameters
 
         Args:
             form_parameters (dictionary): The given dictionary which has
             atleast one model to form encode.
             array_serialization (str): The format of array parameter serialization.
 
@@ -449,14 +454,17 @@
 
         """
         dictionary = dict()
 
         optional_fields = obj._optionals if hasattr(obj, "_optionals") else []
         nullable_fields = obj._nullables if hasattr(obj, "_nullables") else []
 
+        if hasattr(obj, 'validate'):
+            obj.validate(obj)
+
         # Loop through all properties in this model
         names = {k: v for k, v in obj.__dict__.items() if v is not None} if should_ignore_null_values else obj._names
         for name in names:
             value = getattr(obj, name, ApiHelper.SKIP)
 
             if value is ApiHelper.SKIP:
                 continue
@@ -466,27 +474,33 @@
                     raise ValueError(f"The value for {name} can not be None for {obj}")
                 else:
                     dictionary[obj._names[name]] = None
             elif isinstance(value, list):
                 # Loop through each item
                 dictionary[obj._names[name]] = list()
                 for item in value:
-                    dictionary[obj._names[name]].append(
-                        ApiHelper.to_dictionary(item, should_ignore_null_values) if hasattr(item, "_names") else item)
+                    if isinstance(item, list) or isinstance(item, dict):
+                        dictionary[obj._names[name]].append(ApiHelper.process_nested_collection(
+                            item, should_ignore_null_values))
+                    else:
+                        dictionary[obj._names[name]].append(ApiHelper.to_dictionary(item, should_ignore_null_values)
+                                                            if hasattr(item, "_names") else item)
             elif isinstance(value, dict):
                 # Loop through each item
                 dictionary[obj._names[name]] = dict()
-                for key in value:
-                    dictionary[obj._names[name]][key] = ApiHelper.to_dictionary(value[key],
-                                                                                should_ignore_null_values) if hasattr(
-                        value[key],
-                        "_names") else \
-                        value[key]
+                for k, v in value.items():
+                    if isinstance(v, list) or isinstance(v, dict):
+                        dictionary[obj._names[name]][k] = ApiHelper.process_nested_collection(
+                            v, should_ignore_null_values)
+                    else:
+                        dictionary[obj._names[name]][k] = ApiHelper.to_dictionary(value[k], should_ignore_null_values) \
+                            if hasattr(value[k], "_names") else value[k]
             else:
-                dictionary[obj._names[name]] = ApiHelper.to_dictionary(value, should_ignore_null_values) if hasattr(value, "_names") else value
+                dictionary[obj._names[name]] = ApiHelper.to_dictionary(value, should_ignore_null_values) if \
+                    hasattr(value, "_names") else value
 
         # Loop through all additional properties in this model
         if hasattr(obj, "additional_properties"):
             for name in obj.additional_properties:
                 value = obj.additional_properties.get(name)
                 if isinstance(value, list):
                     # Loop through each item
@@ -505,22 +519,54 @@
                     dictionary[name] = ApiHelper.to_dictionary(value, should_ignore_null_values) if hasattr(value,
                                                                                  "additional_properties") else value
 
         # Return the result
         return dictionary
 
     @staticmethod
+    def process_nested_collection(value, should_ignore_null_values):
+        if isinstance(value, list):
+            return [ApiHelper.process_nested_collection(item, should_ignore_null_values) for item in value]
+
+        if isinstance(value, dict):
+            return {k: ApiHelper.process_nested_collection(v, should_ignore_null_values) for k, v in value.items()}
+
+        return ApiHelper.to_dictionary(value, should_ignore_null_values) if hasattr(value, "_names") else value
+
+    @staticmethod
+    def apply_datetime_converter(value, datetime_converter_obj):
+        if isinstance(value, list):
+            return [ApiHelper.apply_datetime_converter(item, datetime_converter_obj) for item in value]
+
+        if isinstance(value, dict):
+            return {k: ApiHelper.apply_datetime_converter(v, datetime_converter_obj) for k, v in value.items()}
+
+        if isinstance(value, datetime.datetime):
+            return ApiHelper.when_defined(datetime_converter_obj, value)
+
+        return value
+
+    @staticmethod
     def when_defined(func, value):
         return func(value) if value else None
 
     @staticmethod
     def is_file_wrapper_instance(param):
         return isinstance(param, FileWrapper)
 
     @staticmethod
+    def is_valid_type(value, type_callable):
+        if isinstance(value, list):
+            return all(ApiHelper.is_valid_type(item, type_callable) for item in value)
+        elif isinstance(value, dict):
+            return all(ApiHelper.is_valid_type(item, type_callable) for item in value.values())
+
+        return value is not None and type_callable(value)
+
+    @staticmethod
     def resolve_template_placeholders_using_json_pointer(placeholders, value, template):
         """Updates all placeholders in the given message template with provided value.
 
         Args:
             placeholders: The placeholders that need to be searched and replaced in the given template value.
             value: The dictionary containing the actual values to replace with.
             template: The template string containing placeholders.
@@ -589,25 +635,24 @@
 
         def __repr__(self):
             return str(self.value)
 
         def __getstate__(self):
             return self.value
 
-        def __setstate__(self, state):
+        def __setstate__(self, state):  # pragma: no cover
             pass
 
     class HttpDateTime(CustomDate):
 
         """ A wrapper class for datetime to support HTTP date format."""
 
         @classmethod
         def from_datetime(cls, date_time):
-            return eut.formatdate(timeval=mktime(date_time.timetuple()),
-                                  localtime=False, usegmt=True)
+            return eut.formatdate(timeval=mktime(date_time.timetuple()), localtime=False, usegmt=True)
 
         @classmethod
         def from_value(cls, value):
             dtime = datetime.datetime.fromtimestamp(eut.mktime_tz(eut.parsedate_tz(value)))
             return cls(dtime, value)
 
     class UnixDateTime(CustomDate):
```

### Comparing `apimatic-core-0.2.3/apimatic_core/utilities/auth_helper.py` & `apimatic-core-0.2.4/apimatic_core/utilities/auth_helper.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.3/apimatic_core/utilities/comparison_helper.py` & `apimatic-core-0.2.4/apimatic_core/utilities/comparison_helper.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.3/apimatic_core/utilities/file_helper.py` & `apimatic-core-0.2.4/apimatic_core/utilities/file_helper.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.3/apimatic_core/utilities/xml_helper.py` & `apimatic-core-0.2.4/apimatic_core/utilities/xml_helper.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.3/apimatic_core.egg-info/PKG-INFO` & `apimatic-core-0.2.4/apimatic_core.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apimatic-core
-Version: 0.2.3
+Version: 0.2.4
 Summary: A library that contains core logic and utilities for consuming REST APIs using Python SDKs generated by APIMatic.
 Home-page: https://github.com/apimatic/core-lib-python
 Author: APIMatic
 Author-email: support@apimatic.io
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -73,31 +73,36 @@
 
 ## Logger
 | Name                                                             | Description                                         |
 |------------------------------------------------------------------|-----------------------------------------------------|
 | [`EndpointLogger`](apimatic_core/logger/endpoint_logger.py)      | A class to provide logging for an HTTP request      |
 
 ## Types
-| Name                                                                         | Description                                                                  |
-|------------------------------------------------------------------------------|------------------------------------------------------------------------------|
-| [`SerializationFormats`](apimatic_core/types/array_serialization_format.py)  | An Enumeration of Array serialization formats                                |
-| [`DateTimeFormat`](apimatic_core/types/datetime_format.py )                  | An Enumeration of Date Time formats                                          |
-| [`ErrorCase`](apimatic_core/types/error_case.py )                            | A class to represent Exception types                                         |
-| [`FileWrapper`](apimatic_core/types/file_wrapper.py)                         | A wrapper to allow passing in content type for file uploads                  |
-| [`Parameter`](apimatic_core/types/parameter.py )                             | A class to represent information about a Parameter passed in an endpoint     |
-| [`XmlAttributes`](apimatic_core/types/xml_attributes.py )                    | A class to represent information about a XML Parameter passed in an endpoint |
+| Name                                                                          | Description                                                                  |
+|-------------------------------------------------------------------------------|------------------------------------------------------------------------------|
+| [`SerializationFormats`](apimatic_core/types/array_serialization_format.py)   | An Enumeration of Array serialization formats                                |
+| [`DateTimeFormat`](apimatic_core/types/datetime_format.py )                   | An Enumeration of Date Time formats                                          |
+| [`ErrorCase`](apimatic_core/types/error_case.py )                             | A class to represent Exception types                                         |
+| [`FileWrapper`](apimatic_core/types/file_wrapper.py)                          | A wrapper to allow passing in content type for file uploads                  |
+| [`Parameter`](apimatic_core/types/parameter.py )                              | A class to represent information about a Parameter passed in an endpoint     |
+| [`XmlAttributes`](apimatic_core/types/xml_attributes.py )                     | A class to represent information about a XML Parameter passed in an endpoint |
+| [`OneOf`](apimatic_core/types/union_types/one_of.py )                         | A class to represent information about OneOf union types                     |
+| [`AnyOf`](apimatic_core/types/union_types/any_of.py )                         | A class to represent information about AnyOf union types                     |
+| [`LeafType`](apimatic_core/types/union_types/leaf_type.py )                   | A class to represent the case information in an OneOf or AnyOf union type    |
 
 ## Utilities
-| Name                                                               | Description                                                                          |
-|--------------------------------------------------------------------|--------------------------------------------------------------------------------------|
-| [`ApiHelper`](apimatic_core/utilities/api_helper.py)               | A Helper Class with various functions associated with making an API Call             |
-| [`AuthHelper`](apimatic_core/utilities/auth_helper.py)             | A Helper Class with various functions associated with authentication in API Calls    |
-| [`ComparisonHelper`](apimatic_core/utilities/comparison_helper.py) | A Helper Class used for the comparison of expected and actual API response           |
-| [` FileHelper`](apimatic_core/utilities/file_helper.py)            | A Helper Class for files                                                             |
-| [`XmlHelper`](apimatic_core/utilities/xml_helper.py )              | A Helper class that holds utility methods for xml serialization and deserialization. |
+| Name                                                               | Description                                                                                              |
+|--------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------|
+| [`ApiHelper`](apimatic_core/utilities/api_helper.py)               | A Helper Class with various functions associated with making an API Call                                 |
+| [`AuthHelper`](apimatic_core/utilities/auth_helper.py)             | A Helper Class with various functions associated with authentication in API Calls                        |
+| [`ComparisonHelper`](apimatic_core/utilities/comparison_helper.py) | A Helper Class used for the comparison of expected and actual API response                               |
+| [`FileHelper`](apimatic_core/utilities/file_helper.py)             | A Helper Class for files                                                                                 |
+| [`XmlHelper`](apimatic_core/utilities/xml_helper.py )              | A Helper class that holds utility methods for xml serialization and deserialization.                     |
+| [`DateTimeHelper`](apimatic_core/utilities/datetime_helper.py )    | A Helper class that holds utility methods for validation of different datetime formats.                  |
+| [`UnionTypeHelper`](apimatic_core/utilities/union_type_helper.py ) | A Helper class that holds utility methods for deserialization and validation of OneOf/AnyOf union types. |
 
 ## Links
 * [apimatic-core-interfaces](https://pypi.org/project/apimatic-core-interfaces/)
 
 
 [pypi-version]: https://img.shields.io/pypi/v/apimatic-core
 [apimatic-core-pypi-url]: https://pypi.org/project/apimatic-core/
```

### Comparing `apimatic-core-0.2.3/apimatic_core.egg-info/SOURCES.txt` & `apimatic-core-0.2.4/apimatic_core.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -20,14 +20,17 @@
 apimatic_core/authentication/multiple/or_auth_group.py
 apimatic_core/authentication/multiple/single_auth.py
 apimatic_core/configurations/__init__.py
 apimatic_core/configurations/endpoint_configuration.py
 apimatic_core/configurations/global_configuration.py
 apimatic_core/decorators/__init__.py
 apimatic_core/decorators/lazy_property.py
+apimatic_core/exceptions/__init__.py
+apimatic_core/exceptions/anyof_validation_exception.py
+apimatic_core/exceptions/oneof_validation_exception.py
 apimatic_core/factories/__init__.py
 apimatic_core/factories/http_response_factory.py
 apimatic_core/http/__init__.py
 apimatic_core/http/http_callback.py
 apimatic_core/http/configurations/__init__.py
 apimatic_core/http/configurations/http_client_configuration.py
 apimatic_core/http/request/__init__.py
@@ -40,28 +43,36 @@
 apimatic_core/types/__init__.py
 apimatic_core/types/array_serialization_format.py
 apimatic_core/types/datetime_format.py
 apimatic_core/types/error_case.py
 apimatic_core/types/file_wrapper.py
 apimatic_core/types/parameter.py
 apimatic_core/types/xml_attributes.py
+apimatic_core/types/union_types/__init__.py
+apimatic_core/types/union_types/any_of.py
+apimatic_core/types/union_types/leaf_type.py
+apimatic_core/types/union_types/one_of.py
+apimatic_core/types/union_types/union_type_context.py
 apimatic_core/utilities/__init__.py
 apimatic_core/utilities/api_helper.py
 apimatic_core/utilities/auth_helper.py
 apimatic_core/utilities/comparison_helper.py
+apimatic_core/utilities/datetime_helper.py
 apimatic_core/utilities/file_helper.py
+apimatic_core/utilities/union_type_helper.py
 apimatic_core/utilities/xml_helper.py
 tests/__init__.py
 tests/apimatic_core/__init__.py
 tests/apimatic_core/base.py
 tests/apimatic_core/api_call_tests/__init__.py
 tests/apimatic_core/api_call_tests/test_api_call.py
 tests/apimatic_core/api_logger_tests/__init__.py
 tests/apimatic_core/api_logger_tests/test_api_logger.py
 tests/apimatic_core/mocks/__init__.py
+tests/apimatic_core/mocks/union_type_lookup.py
 tests/apimatic_core/mocks/authentications/__init__.py
 tests/apimatic_core/mocks/authentications/basic_auth.py
 tests/apimatic_core/mocks/authentications/bearer_auth.py
 tests/apimatic_core/mocks/authentications/custom_header_authentication.py
 tests/apimatic_core/mocks/authentications/custom_query_authentication.py
 tests/apimatic_core/mocks/callables/__init__.py
 tests/apimatic_core/mocks/callables/base_uri_callable.py
@@ -73,26 +84,39 @@
 tests/apimatic_core/mocks/http/__init__.py
 tests/apimatic_core/mocks/http/http_client.py
 tests/apimatic_core/mocks/http/http_response_catcher.py
 tests/apimatic_core/mocks/logger/__init__.py
 tests/apimatic_core/mocks/logger/api_logger.py
 tests/apimatic_core/mocks/models/__init__.py
 tests/apimatic_core/mocks/models/api_response.py
+tests/apimatic_core/mocks/models/atom.py
 tests/apimatic_core/mocks/models/cat_model.py
+tests/apimatic_core/mocks/models/complex_type.py
 tests/apimatic_core/mocks/models/days.py
+tests/apimatic_core/mocks/models/deer.py
 tests/apimatic_core/mocks/models/dog_model.py
 tests/apimatic_core/mocks/models/grand_parent_class_model.py
+tests/apimatic_core/mocks/models/inner_complex_type.py
+tests/apimatic_core/mocks/models/lion.py
+tests/apimatic_core/mocks/models/months.py
 tests/apimatic_core/mocks/models/one_of_xml.py
+tests/apimatic_core/mocks/models/orbit.py
 tests/apimatic_core/mocks/models/person.py
+tests/apimatic_core/mocks/models/rabbit.py
+tests/apimatic_core/mocks/models/union_type_scalar_model.py
 tests/apimatic_core/mocks/models/validate.py
 tests/apimatic_core/mocks/models/wolf_model.py
 tests/apimatic_core/mocks/models/xml_model.py
 tests/apimatic_core/request_builder_tests/__init__.py
 tests/apimatic_core/request_builder_tests/test_request_builder.py
 tests/apimatic_core/response_handler_tests/__init__.py
 tests/apimatic_core/response_handler_tests/test_response_handler.py
+tests/apimatic_core/union_type_tests/__init__.py
+tests/apimatic_core/union_type_tests/test_any_of.py
+tests/apimatic_core/union_type_tests/test_one_of.py
 tests/apimatic_core/utility_tests/__init__.py
 tests/apimatic_core/utility_tests/test_api_helper.py
 tests/apimatic_core/utility_tests/test_auth_helper.py
 tests/apimatic_core/utility_tests/test_comparison_helper.py
+tests/apimatic_core/utility_tests/test_datetime_helper.py
 tests/apimatic_core/utility_tests/test_file_helper.py
 tests/apimatic_core/utility_tests/test_xml_helper.py
```

### Comparing `apimatic-core-0.2.3/setup.py` & `apimatic-core-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         long_description = fh.read()
 else:
     with open('README.md', 'r', encoding='utf-8') as fh:
         long_description = fh.read()
 
 setup(
     name='apimatic-core',
-    version='0.2.3',
+    version='0.2.4',
     description='A library that contains core logic and utilities for '
                 'consuming REST APIs using Python SDKs generated by APIMatic.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='APIMatic',
     author_email='support@apimatic.io',
     license='MIT',
```

### Comparing `apimatic-core-0.2.3/tests/apimatic_core/api_call_tests/test_api_call.py` & `apimatic-core-0.2.4/tests/apimatic_core/api_call_tests/test_api_call.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.3/tests/apimatic_core/api_logger_tests/test_api_logger.py` & `apimatic-core-0.2.4/tests/apimatic_core/api_logger_tests/test_api_logger.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.3/tests/apimatic_core/base.py` & `apimatic-core-0.2.4/tests/apimatic_core/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,16 +20,19 @@
 from tests.apimatic_core.mocks.authentications.custom_header_authentication import CustomHeaderAuthentication
 from tests.apimatic_core.mocks.authentications.custom_query_authentication import CustomQueryAuthentication
 from tests.apimatic_core.mocks.exceptions.global_test_exception import GlobalTestException
 from tests.apimatic_core.mocks.exceptions.nested_model_exception import NestedModelException
 from tests.apimatic_core.mocks.http.http_response_catcher import HttpResponseCatcher
 from tests.apimatic_core.mocks.http.http_client import MockHttpClient
 from tests.apimatic_core.mocks.models.cat_model import CatModel
+from tests.apimatic_core.mocks.models.complex_type import ComplexType
 from tests.apimatic_core.mocks.models.dog_model import DogModel
+from tests.apimatic_core.mocks.models.inner_complex_type import InnerComplexType
 from tests.apimatic_core.mocks.models.one_of_xml import OneOfXML
+from tests.apimatic_core.mocks.models.union_type_scalar_model import UnionTypeScalarModel
 from tests.apimatic_core.mocks.models.wolf_model import WolfModel
 from tests.apimatic_core.mocks.models.xml_model import XMLModel
 from tests.apimatic_core.mocks.models.days import Days
 from tests.apimatic_core.mocks.models.person import Employee, Person
 from tests.apimatic_core.mocks.callables.base_uri_callable import Server, BaseUriCallable
 
 
@@ -247,7 +250,31 @@
             {'basic_auth': BasicAuth(None, None), 'bearer_auth': BearerAuth(None),
              'custom_header_auth': CustomHeaderAuthentication(None)})
 
     @property
     def global_configuration_with_partially_initialized_auth_params(self):
         return self.global_configuration.auth_managers(
             {'basic_auth': BasicAuth(None, None), 'custom_header_auth': self.custom_header_auth()})
+
+    @staticmethod
+    def get_complex_type():
+        inner_complex_type = InnerComplexType(boolean_type=True,
+                                              long_type=100003,
+                                              string_type='abc',
+                                              precision_type=55.44,
+                                              string_list_type=['item1', 'item2'],
+                                              additional_properties={'key0': 'abc', 'key1': 400})
+
+        return ComplexType(inner_complex_type=inner_complex_type,
+                           inner_complex_list_type=[inner_complex_type, inner_complex_type],
+                           inner_complex_list_of_map_type=[{'key0': inner_complex_type, 'key1': inner_complex_type}],
+                           inner_complex_map_type={'key0': inner_complex_type, 'key1': inner_complex_type},
+                           inner_complex_map_of_list_type={'key0': [inner_complex_type, inner_complex_type],
+                                                           'key2': [inner_complex_type, inner_complex_type]},
+                           additional_properties={'prop1': [1, 2, 3], 'prop2': {'key0': 'abc', 'key1': 'def'}})
+
+    @staticmethod
+    def get_union_type_scalar_model():
+        return UnionTypeScalarModel(any_of_required=1.5,
+                                    one_of_req_nullable='abc',
+                                    one_of_optional=200,
+                                    any_of_opt_nullable=True)
```

### Comparing `apimatic-core-0.2.3/tests/apimatic_core/mocks/authentications/basic_auth.py` & `apimatic-core-0.2.4/tests/apimatic_core/mocks/authentications/basic_auth.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.3/tests/apimatic_core/mocks/authentications/custom_query_authentication.py` & `apimatic-core-0.2.4/tests/apimatic_core/mocks/authentications/custom_query_authentication.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.3/tests/apimatic_core/mocks/callables/base_uri_callable.py` & `apimatic-core-0.2.4/tests/apimatic_core/mocks/callables/base_uri_callable.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.3/tests/apimatic_core/mocks/exceptions/api_exception.py` & `apimatic-core-0.2.4/tests/apimatic_core/mocks/exceptions/api_exception.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.3/tests/apimatic_core/mocks/exceptions/global_test_exception.py` & `apimatic-core-0.2.4/tests/apimatic_core/mocks/exceptions/global_test_exception.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.3/tests/apimatic_core/mocks/exceptions/local_test_exception.py` & `apimatic-core-0.2.4/tests/apimatic_core/mocks/exceptions/local_test_exception.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.3/tests/apimatic_core/mocks/exceptions/nested_model_exception.py` & `apimatic-core-0.2.4/tests/apimatic_core/mocks/exceptions/nested_model_exception.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.3/tests/apimatic_core/mocks/http/http_client.py` & `apimatic-core-0.2.4/tests/apimatic_core/mocks/http/http_client.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.3/tests/apimatic_core/mocks/models/api_response.py` & `apimatic-core-0.2.4/tests/apimatic_core/mocks/models/api_response.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.3/tests/apimatic_core/mocks/models/cat_model.py` & `apimatic-core-0.2.4/tests/apimatic_core/mocks/models/cat_model.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.3/tests/apimatic_core/mocks/models/dog_model.py` & `apimatic-core-0.2.4/tests/apimatic_core/mocks/models/dog_model.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.3/tests/apimatic_core/mocks/models/grand_parent_class_model.py` & `apimatic-core-0.2.4/tests/apimatic_core/mocks/models/grand_parent_class_model.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.3/tests/apimatic_core/mocks/models/one_of_xml.py` & `apimatic-core-0.2.4/tests/apimatic_core/mocks/models/one_of_xml.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.3/tests/apimatic_core/mocks/models/person.py` & `apimatic-core-0.2.4/tests/apimatic_core/mocks/models/person.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.3/tests/apimatic_core/mocks/models/validate.py` & `apimatic-core-0.2.4/tests/apimatic_core/mocks/models/validate.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.3/tests/apimatic_core/mocks/models/wolf_model.py` & `apimatic-core-0.2.4/tests/apimatic_core/mocks/models/wolf_model.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.3/tests/apimatic_core/mocks/models/xml_model.py` & `apimatic-core-0.2.4/tests/apimatic_core/mocks/models/xml_model.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.3/tests/apimatic_core/request_builder_tests/test_request_builder.py` & `apimatic-core-0.2.4/tests/apimatic_core/request_builder_tests/test_request_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from apimatic_core.types.xml_attributes import XmlAttributes
 from apimatic_core.utilities.api_helper import ApiHelper
 from apimatic_core.utilities.auth_helper import AuthHelper
 from apimatic_core.utilities.xml_helper import XmlHelper
 from tests.apimatic_core.base import Base
 from tests.apimatic_core.mocks.callables.base_uri_callable import Server
 from requests.utils import quote
+from tests.apimatic_core.mocks.union_type_lookup import UnionTypeLookUp
 
 
 class TestRequestBuilder(Base):
 
     @pytest.mark.parametrize('input_server, expected_base_uri', [
         (Server.DEFAULT, 'http://localhost:3000/'),
         (Server.AUTH_SERVER, 'http://authserver:5000/')
@@ -413,35 +414,26 @@
         http_request = self.new_request_builder \
             .body_param(Parameter()
                         .value(input_body_param_value)) \
             .body_serializer(ApiHelper.json_serialize) \
             .build(self.global_configuration)
         assert http_request.parameters == expected_body_param_value
 
-    @pytest.mark.parametrize('input_body_param_value, input_should_wrap_body_param,'
-                             'input_body_key, expected_body_param_value', [
-                                 (100, False, None, '100'),
-                                 (100, True, 'body', '{"body": 100}'),
-                                 ([1, 2, 3, 4], False, None, '[1, 2, 3, 4]'),
-                                 ([1, 2, 3, 4], True, 'body', '{"body": [1, 2, 3, 4]}'),
-                                 ({'key1': 'value1', 'key2': [1, 2, 3, 4]}, False, None,
-                                  '{"key1": "value1", "key2": [1, 2, 3, 4]}'),
-                                 ({'key1': 'value1', 'key2': [1, 2, 3, 4]}, True, 'body',
-                                  '{"body": {"key1": "value1", "key2": [1, 2, 3, 4]}}')
-                             ])
-    def test_type_combinator_body_param_with_serializer(self, input_body_param_value, input_should_wrap_body_param,
-                                                        input_body_key, expected_body_param_value):
+    @pytest.mark.parametrize('input_value, expected_value', [
+        (100, '100'),
+        (True, 'true')
+    ])
+    def test_type_combinator_validation_in_request(self, input_value, expected_value):
         http_request = self.new_request_builder \
             .body_param(Parameter()
-                        .key(input_body_key)
-                        .value(input_body_param_value)) \
-            .body_serializer(ApiHelper.get_request_parameter) \
-            .should_wrap_body_param(input_should_wrap_body_param) \
+                        .validator(lambda value: UnionTypeLookUp.get('ScalarTypes'))
+                        .value(input_value)) \
+            .body_serializer(ApiHelper.json_serialize) \
             .build(self.global_configuration)
-        assert http_request.parameters == expected_body_param_value
+        assert http_request.parameters == expected_value
 
     @pytest.mark.parametrize('input_body_param_value, expected_body_param_value', [
         (Base.xml_model(), '<AttributesAndElements string="String" number="10000" boolean="false">'
                            '<string>Hey! I am being tested.</string>'
                            '<number>5000</number>'
                            '<boolean>false</boolean>'
                            '<elements>'
```

### Comparing `apimatic-core-0.2.3/tests/apimatic_core/response_handler_tests/test_response_handler.py` & `apimatic-core-0.2.4/tests/apimatic_core/response_handler_tests/test_response_handler.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.3/tests/apimatic_core/utility_tests/test_api_helper.py` & `apimatic-core-0.2.4/tests/apimatic_core/utility_tests/test_api_helper.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,29 @@
 from datetime import datetime, date
 import jsonpickle
 import pytest
+from apimatic_core.types.union_types.leaf_type import LeafType
+from apimatic_core.types.union_types.one_of import OneOf
+from apimatic_core.types.union_types.union_type_context import UnionTypeContext
 from dateutil.tz import tzutc
 
 from apimatic_core.types.array_serialization_format import SerializationFormats
 from apimatic_core.types.datetime_format import DateTimeFormat
 from apimatic_core.types.file_wrapper import FileWrapper
 from apimatic_core.utilities.api_helper import ApiHelper
 from tests.apimatic_core.base import Base
+from tests.apimatic_core.mocks.models.days import Days
 
 from tests.apimatic_core.mocks.models.grand_parent_class_model import ChildClassModel
 from tests.apimatic_core.mocks.models.person import Employee
 from requests.utils import quote
 
 
 class TestApiHelper(Base):
 
-    @pytest.mark.parametrize('expected_value, input_value, is_wrapped', [
-        ('value', 'value', False),
-        ('true', True, False),
-        ('{{"bodyScalar": true, "bodyNonScalar": {{"address": "street abc", "age": 27, '
-         '"birthday": "1994-02-13", "birthtime": "{0}", "department": '
-         '"IT", "dependents": [{{"address": "street abc", "age": 12, "birthday": '
-         '"1994-02-13", "birthtime": "{0}", "name": "John", "uid": '
-         '7654321, "personType": "Per", "key1": "value1", "key2": "value2"}}], '
-         '"hiredAt": "{1}", "joiningDay": "Monday", "name": '
-         '"Bob", "salary": 30000, "uid": 1234567, "workingDays": ["Monday", '
-         '"Tuesday"], "personType": "Empl"}}}}'.format(Base.get_rfc3339_datetime(datetime(1994, 2, 13, 5, 30, 15)),
-                                                       Base.get_http_datetime(datetime(1994, 2, 13, 5, 30, 15))),
-         Base.wrapped_parameters(), True),
-    ])
-    def test_get_request_parameter(self, expected_value, input_value, is_wrapped):
-        request_param = ApiHelper.get_request_parameter(input_value, is_wrapped)
-        assert request_param == expected_value
-
     @pytest.mark.parametrize('input_value, expected_value', [
         (None, None),
         (Base.wrapped_parameters(), '{{"bodyScalar": true, "bodyNonScalar": {{"address": "street abc", "age": 27, '
                                     '"birthday": "1994-02-13", "birthtime": "{0}", "department": '
                                     '"IT", "dependents": [{{"address": "street abc", "age": 12, "birthday": '
                                     '"1994-02-13", "birthtime": "{0}", "name": "John", "uid": '
                                     '7654321, "personType": "Per", "key1": "value1", "key2": "value2"}}], '
@@ -67,26 +53,98 @@
          '"IT", "dependents": [{{"address": "street abc", "age": 12, "birthday": '
          '"1994-02-13", "birthtime": "{0}", "name": "John", "uid": '
          '7654321, "personType": "Per", "key1": "value1", "key2": "value2"}}], '
          '"hiredAt": "{1}", "joiningDay": "Monday", "name": '
          '"Bob", "salary": 30000, "uid": 1234567, "workingDays": ["Monday", '
          '"Tuesday"], "personType": "Empl"}}]'.format(Base.get_rfc3339_datetime(datetime(1994, 2, 13, 5, 30, 15)),
                                                       Base.get_http_datetime(datetime(1994, 2, 13, 5, 30, 15)))),
+        ([[Base.employee_model(), Base.employee_model()], [Base.employee_model(), Base.employee_model()]],
+         '[[{{"address": "street abc", "age": 27, '
+         '"birthday": "1994-02-13", "birthtime": "{0}", "department": '
+         '"IT", "dependents": [{{"address": "street abc", "age": 12, "birthday": '
+         '"1994-02-13", "birthtime": "{0}", "name": "John", "uid": '
+         '7654321, "personType": "Per", "key1": "value1", "key2": "value2"}}], '
+         '"hiredAt": "{1}", "joiningDay": "Monday", "name": '
+         '"Bob", "salary": 30000, "uid": 1234567, "workingDays": ["Monday", '
+         '"Tuesday"], "personType": "Empl"}}, '
+         '{{"address": "street abc", "age": 27, '
+         '"birthday": "1994-02-13", "birthtime": "{0}", "department": '
+         '"IT", "dependents": [{{"address": "street abc", "age": 12, "birthday": '
+         '"1994-02-13", "birthtime": "{0}", "name": "John", "uid": '
+         '7654321, "personType": "Per", "key1": "value1", "key2": "value2"}}], '
+         '"hiredAt": "{1}", "joiningDay": "Monday", "name": '
+         '"Bob", "salary": 30000, "uid": 1234567, "workingDays": ["Monday", '
+         '"Tuesday"], "personType": "Empl"}}], [{{"address": "street abc", "age": 27, '
+         '"birthday": "1994-02-13", "birthtime": "{0}", "department": '
+         '"IT", "dependents": [{{"address": "street abc", "age": 12, "birthday": '
+         '"1994-02-13", "birthtime": "{0}", "name": "John", "uid": '
+         '7654321, "personType": "Per", "key1": "value1", "key2": "value2"}}], '
+         '"hiredAt": "{1}", "joiningDay": "Monday", "name": '
+         '"Bob", "salary": 30000, "uid": 1234567, "workingDays": ["Monday", '
+         '"Tuesday"], "personType": "Empl"}}, '
+         '{{"address": "street abc", "age": 27, '
+         '"birthday": "1994-02-13", "birthtime": "{0}", "department": '
+         '"IT", "dependents": [{{"address": "street abc", "age": 12, "birthday": '
+         '"1994-02-13", "birthtime": "{0}", "name": "John", "uid": '
+         '7654321, "personType": "Per", "key1": "value1", "key2": "value2"}}], '
+         '"hiredAt": "{1}", "joiningDay": "Monday", "name": '
+         '"Bob", "salary": 30000, "uid": 1234567, "workingDays": ["Monday", '
+         '"Tuesday"], "personType": "Empl"}}]]'.format(Base.get_rfc3339_datetime(datetime(1994, 2, 13, 5, 30, 15)),
+                                                      Base.get_http_datetime(datetime(1994, 2, 13, 5, 30, 15)))),
+        ({'key0': [Base.employee_model(), Base.employee_model()],
+          'key1': [Base.employee_model(), Base.employee_model()]},
+         '{{"key0": [{{"address": "street abc", "age": 27, '
+         '"birthday": "1994-02-13", "birthtime": "{0}", "department": '
+         '"IT", "dependents": [{{"address": "street abc", "age": 12, "birthday": '
+         '"1994-02-13", "birthtime": "{0}", "name": "John", "uid": '
+         '7654321, "personType": "Per", "key1": "value1", "key2": "value2"}}], '
+         '"hiredAt": "{1}", "joiningDay": "Monday", "name": '
+         '"Bob", "salary": 30000, "uid": 1234567, "workingDays": ["Monday", '
+         '"Tuesday"], "personType": "Empl"}}, '
+         '{{"address": "street abc", "age": 27, '
+         '"birthday": "1994-02-13", "birthtime": "{0}", "department": '
+         '"IT", "dependents": [{{"address": "street abc", "age": 12, "birthday": '
+         '"1994-02-13", "birthtime": "{0}", "name": "John", "uid": '
+         '7654321, "personType": "Per", "key1": "value1", "key2": "value2"}}], '
+         '"hiredAt": "{1}", "joiningDay": "Monday", "name": '
+         '"Bob", "salary": 30000, "uid": 1234567, "workingDays": ["Monday", '
+         '"Tuesday"], "personType": "Empl"}}], "key1": [{{"address": "street abc", "age": 27, '
+         '"birthday": "1994-02-13", "birthtime": "{0}", "department": '
+         '"IT", "dependents": [{{"address": "street abc", "age": 12, "birthday": '
+         '"1994-02-13", "birthtime": "{0}", "name": "John", "uid": '
+         '7654321, "personType": "Per", "key1": "value1", "key2": "value2"}}], '
+         '"hiredAt": "{1}", "joiningDay": "Monday", "name": '
+         '"Bob", "salary": 30000, "uid": 1234567, "workingDays": ["Monday", '
+         '"Tuesday"], "personType": "Empl"}}, '
+         '{{"address": "street abc", "age": 27, '
+         '"birthday": "1994-02-13", "birthtime": "{0}", "department": '
+         '"IT", "dependents": [{{"address": "street abc", "age": 12, "birthday": '
+         '"1994-02-13", "birthtime": "{0}", "name": "John", "uid": '
+         '7654321, "personType": "Per", "key1": "value1", "key2": "value2"}}], '
+         '"hiredAt": "{1}", "joiningDay": "Monday", "name": '
+         '"Bob", "salary": 30000, "uid": 1234567, "workingDays": ["Monday", '
+         '"Tuesday"], "personType": "Empl"}}]}}'.format(Base.get_rfc3339_datetime(datetime(1994, 2, 13, 5, 30, 15)),
+                                                      Base.get_http_datetime(datetime(1994, 2, 13, 5, 30, 15)))),
         ([1, 2, 3], '[1, 2, 3]'),
+        ({'key0': 1, 'key1': 'abc'}, '{"key0": 1, "key1": "abc"}'),
+        ([[1, 2, 3], ['abc', 'def']], '[[1, 2, 3], ["abc", "def"]]'),
+        ([{'key0': [1, 2, 3]}, {'key1': ['abc', 'def']}], '[{"key0": [1, 2, 3]}, {"key1": ["abc", "def"]}]'),
+        ({'key0': [1, 2, 3], 'key1': ['abc', 'def']}, '{"key0": [1, 2, 3], "key1": ["abc", "def"]}'),
         (Base.employee_model(),
          '{{"address": "street abc", "age": 27, '
          '"birthday": "1994-02-13", "birthtime": "{0}", "department": '
          '"IT", "dependents": [{{"address": "street abc", "age": 12, "birthday": '
          '"1994-02-13", "birthtime": "{0}", "name": "John", "uid": '
          '7654321, "personType": "Per", "key1": "value1", "key2": "value2"}}], '
          '"hiredAt": "{1}", "joiningDay": "Monday", "name": '
          '"Bob", "salary": 30000, "uid": 1234567, "workingDays": ["Monday", '
          '"Tuesday"], "personType": "Empl"}}'.format(Base.get_rfc3339_datetime(datetime(1994, 2, 13, 5, 30, 15)),
                                                      Base.get_http_datetime(datetime(1994, 2, 13, 5, 30, 15)))),
-        (1, '1')
+        (1, '1'),
+        ('1', '1')
     ])
     def test_json_serialize(self, input_value, expected_value):
         serialized_value = ApiHelper.json_serialize(input_value)
         assert serialized_value == expected_value
 
     @pytest.mark.parametrize('input_json_value, unboxing_function, as_dict, expected_value', [
         (None, None, False, None),
@@ -94,31 +152,25 @@
         (ApiHelper.json_serialize(Base.employee_model()), Employee.from_dictionary, False,
          ApiHelper.json_serialize(Base.employee_model())),
         (ApiHelper.json_serialize([Base.employee_model(), Base.employee_model()]),
          Employee.from_dictionary, False,
          ApiHelper.json_serialize([Base.employee_model(), Base.employee_model()])),
         (ApiHelper.json_serialize({'key1': Base.employee_model(), 'key2': Base.employee_model()}),
          Employee.from_dictionary, True,
-         '{{"key1": {{"department": "IT", "dependents": [{{"address": "street abc", '
-         '"age": 12, "birthday": "1994-02-13", "birthtime": "{0}", '
-         '"name": "John", "uid": 7654321, "person_type": "Per", '
-         '"additional_properties": {{"person_type": "Per", "additional_properties": '
-         '{{"key1": "value1", "key2": "value2"}}}}}}], "hired_at": null, "joining_day": '
-         '"Monday", "salary": 30000, "working_days": null, "additional_properties": '
-         '{{}}, "address": "street abc", "age": 27, "birthday": "1994-02-13", '
-         '"birthtime": "{0}", "name": "Bob", "uid": 1234567, '
-         '"person_type": "Empl"}}, "key2": {{"department": "IT", "dependents": '
-         '[{{"address": "street abc", "age": 12, "birthday": "1994-02-13", "birthtime": '
-         '"{0}", "name": "John", "uid": 7654321, "person_type": "Per", '
-         '"additional_properties": {{"person_type": "Per", "additional_properties": '
-         '{{"key1": "value1", "key2": "value2"}}}}}}], "hired_at": null, "joining_day": '
-         '"Monday", "salary": 30000, "working_days": null, "additional_properties": '
-         '{{}}, "address": "street abc", "age": 27, "birthday": "1994-02-13", '
-         '"birthtime": "{0}", "name": "Bob", "uid": 1234567, '
-         '"person_type": "Empl"}}}}'.format(Base.get_rfc3339_datetime(datetime(1994, 2, 13, 5, 30, 15)))),
+         '{{"key1": {{"address": "street abc", "age": 27, "birthday": "1994-02-13", "birthtime": "{0}", '
+         '"department": "IT", "dependents": [{{"address": "street abc", "age": 12, "birthday": "1994-02-13", '
+         '"birthtime": "{0}", "name": "John", "uid": 7654321, "personType": "Per", "key1": "value1", '
+         '"key2": "value2"}}], "hiredAt": "{1}", "joiningDay": "Monday", "name": "Bob", "salary": 30000, '
+         '"uid": 1234567, "workingDays": ["Monday", "Tuesday"], "personType": "Empl"}}, "key2": '
+         '{{"address": "street abc", "age": 27, "birthday": "1994-02-13", "birthtime": "{0}", "department": "IT",'
+         ' "dependents": [{{"address": "street abc", "age": 12, "birthday": "1994-02-13", "birthtime": "{0}", '
+         '"name": "John", "uid": 7654321, "personType": "Per", "key1": "value1", "key2": "value2"}}], "hiredAt": "{1}",'
+         ' "joiningDay": "Monday", "name": "Bob", "salary": 30000, "uid": 1234567, "workingDays": ["Monday",'
+         ' "Tuesday"], "personType": "Empl"}}}}'.format(Base.get_rfc3339_datetime(datetime(1994, 2, 13, 5, 30, 15)),
+                                                        Base.get_http_datetime(datetime(1994, 2, 13, 5, 30, 15))))
 
     ])
     def test_json_deserialize(self, input_json_value, unboxing_function, as_dict, expected_value):
         deserialized_value = ApiHelper.json_deserialize(input_json_value, unboxing_function, as_dict)
         assert ApiHelper.json_serialize(deserialized_value) == expected_value
 
     @pytest.mark.parametrize('input_json', [
@@ -299,14 +351,36 @@
          '"IT", "dependents": [{{"address": "street abc", "age": 12, "birthday": '
          '"1994-02-13", "birthtime": "{0}", "name": "John", "uid": '
          '7654321, "personType": "Per", "key1": "value1", "key2": "value2"}}], '
          '"hiredAt": "{1}", "joiningDay": "Monday", "name": '
          '"Bob", "salary": 30000, "uid": 1234567, "workingDays": ["Monday", '
          '"Tuesday"], "personType": "Empl"}}'.format(Base.get_rfc3339_datetime(datetime(1994, 2, 13, 5, 30, 15)),
                                                      Base.get_http_datetime(datetime(1994, 2, 13, 5, 30, 15)))),
+        (Base.get_complex_type(),
+         '{"innerComplexListType": [{"booleanType": true, "longType": 100003, "precisionType": 55.44, '
+         '"stringListType": ["item1", "item2"], "stringType": "abc", "key0": "abc", "key1": 400}, '
+         '{"booleanType": true, "longType": 100003, "precisionType": 55.44, "stringListType": ["item1", "item2"],'
+         ' "stringType": "abc", "key0": "abc", "key1": 400}], "innerComplexType": {"booleanType": true, '
+         '"longType": 100003, "precisionType": 55.44, "stringListType": ["item1", "item2"], "stringType": "abc",'
+         ' "key0": "abc", "key1": 400}, "innerComplexListOfMapType": [{"key0": {"booleanType": true, '
+         '"longType": 100003, "precisionType": 55.44, "stringListType": ["item1", "item2"], '
+         '"stringType": "abc", "key0": "abc", "key1": 400}, "key1": {"booleanType": true, "longType": 100003, '
+         '"precisionType": 55.44, "stringListType": ["item1", "item2"], "stringType": "abc", "key0": "abc", '
+         '"key1": 400}}], "innerComplexMapOfListType": {"key0": [{"booleanType": true, "longType": 100003, '
+         '"precisionType": 55.44, "stringListType": ["item1", "item2"], "stringType": "abc", "key0": "abc", '
+         '"key1": 400}, {"booleanType": true, "longType": 100003, "precisionType": 55.44, "stringListType": '
+         '["item1", "item2"], "stringType": "abc", "key0": "abc", "key1": 400}], "key2": [{"booleanType": true, '
+         '"longType": 100003, "precisionType": 55.44, "stringListType": ["item1", "item2"], "stringType": "abc", '
+         '"key0": "abc", "key1": 400}, {"booleanType": true, "longType": 100003, "precisionType": 55.44, '
+         '"stringListType": ["item1", "item2"], "stringType": "abc", "key0": "abc", "key1": 400}]}, '
+         '"innerComplexMapType": {"key0": {"booleanType": true, "longType": 100003, "precisionType": 55.44, '
+         '"stringListType": ["item1", "item2"], "stringType": "abc", "key0": "abc", "key1": 400}, "key1": '
+         '{"booleanType": true, "longType": 100003, "precisionType": 55.44, "stringListType": ["item1", "item2"], '
+         '"stringType": "abc", "key0": "abc", "key1": 400}}, "prop1": [1, 2, 3], "prop2": {"key0": "abc", '
+         '"key1": "def"}}'),
         (ApiHelper.json_deserialize('{"Grand_Parent_Required_Nullable":{"key1": "value1", "key2": "value2"},'
                                     '"Grand_Parent_Required":"not nullable and required","class":23,'
                                     '"Parent_Optional_Nullable_With '
                                     '_Default_Value":"Has default value","Parent_Required_Nullable":nul'
                                     'l,"Parent_Required":"not nullable and required","Optional_Nullable'
                                     '":"setted optionalNullable","Optional_Nullable_With_Default_Value"'
                                     ':"With default value","Required_Nullable":null,"Required":"not nul'
@@ -328,14 +402,16 @@
          '"{0}", "name": "John", "uid": 7654321, "personType": "Per", '
          '"key1": {{"inner_key1": "inner_val1", "inner_key2": "inner_val2"}}, "key2": '
          '["value2", "value3"]}}], "hiredAt": "{1}", '
          '"joiningDay": "Monday", "name": "Bob", "salary": 30000, "uid": 1234567, '
          '"workingDays": ["Monday", "Tuesday"], "personType": "Empl"}}'.format(
              Base.get_rfc3339_datetime(datetime(1994, 2, 13, 5, 30, 15)),
              Base.get_http_datetime(datetime(1994, 2, 13, 5, 30, 15)))),
+        (Base.get_union_type_scalar_model(),
+         '{"anyOfRequired": 1.5, "oneOfReqNullable": "abc", "oneOfOptional": 200, "anyOfOptNullable": true}'),
 
     ])
     def test_to_dictionary(self, obj, expected_value):
         assert jsonpickle.encode(ApiHelper.to_dictionary(obj), False) == expected_value
 
     @pytest.mark.parametrize('obj, should_ignore_null_values, expected_value', [
         (Base.employee_model_additional_dictionary(), True,
@@ -460,14 +536,113 @@
     ])
     def test_when_defined(self, input_function, input_body, expected_value):
         if input_body is not None:
             assert str(ApiHelper.when_defined(input_function, input_body)) == expected_value
         else:
             assert ApiHelper.when_defined(input_function, input_body) == expected_value
 
+    @pytest.mark.parametrize('input_value, input_converter, expected_obj', [
+        (datetime(1994, 2, 13, 5, 30, 15), ApiHelper.RFC3339DateTime,
+         ApiHelper.RFC3339DateTime),
+        (datetime(1994, 2, 13, 5, 30, 15), ApiHelper.HttpDateTime, ApiHelper.HttpDateTime),
+        (datetime(1994, 2, 13, 5, 30, 15), ApiHelper.UnixDateTime, ApiHelper.UnixDateTime),
+        (500, ApiHelper.UnixDateTime, int),
+        ('500', ApiHelper.UnixDateTime, str),
+        (None, ApiHelper.RFC3339DateTime, None)
+    ])
+    def test_apply_date_time_converter(self, input_value, input_converter, expected_obj):
+        if input_value is None:
+            assert ApiHelper.apply_datetime_converter(input_value, input_converter) == expected_obj
+        else:
+            assert isinstance(ApiHelper.apply_datetime_converter(input_value, input_converter), expected_obj)
+
+    @pytest.mark.parametrize('input_value, input_converter, expected_obj', [
+        ([datetime(1994, 2, 13, 5, 30, 15), datetime(1994, 2, 13, 5, 30, 15)], ApiHelper.RFC3339DateTime,
+         [ApiHelper.RFC3339DateTime, ApiHelper.RFC3339DateTime]),
+        ([datetime(1994, 2, 13, 5, 30, 15), datetime(1994, 2, 13, 5, 30, 15)], ApiHelper.HttpDateTime,
+         [ApiHelper.HttpDateTime, ApiHelper.HttpDateTime]),
+        ([datetime(1994, 2, 13, 5, 30, 15), datetime(1994, 2, 13, 5, 30, 15)], ApiHelper.UnixDateTime,
+         [ApiHelper.UnixDateTime, ApiHelper.UnixDateTime]),
+        ([500, 1000], ApiHelper.UnixDateTime, [int, int]),
+        (['500', '1000'], ApiHelper.UnixDateTime, [str, str]),
+        (['500', datetime(1994, 2, 13, 5, 30, 15)], ApiHelper.UnixDateTime, [str, ApiHelper.UnixDateTime]),
+        (None, ApiHelper.RFC3339DateTime, None)
+    ])
+    def test_apply_date_time_converter_to_list(self, input_value, input_converter, expected_obj):
+        if input_value is None:
+            assert ApiHelper.apply_datetime_converter(input_value, input_converter) == expected_obj
+        else:
+            actual_converted_value = ApiHelper.apply_datetime_converter(input_value, input_converter)
+            for index, actual_value in enumerate(actual_converted_value):
+                assert isinstance(actual_value, expected_obj[index])
+
+    @pytest.mark.parametrize('input_value, input_converter, expected_obj', [
+        ([[datetime(1994, 2, 13, 5, 30, 15), datetime(1994, 2, 13, 5, 30, 15)]], ApiHelper.RFC3339DateTime,
+         [[ApiHelper.RFC3339DateTime, ApiHelper.RFC3339DateTime]]),
+        ([[datetime(1994, 2, 13, 5, 30, 15), datetime(1994, 2, 13, 5, 30, 15)]], ApiHelper.HttpDateTime,
+         [[ApiHelper.HttpDateTime, ApiHelper.HttpDateTime]]),
+        ([[datetime(1994, 2, 13, 5, 30, 15), datetime(1994, 2, 13, 5, 30, 15)]], ApiHelper.UnixDateTime,
+         [[ApiHelper.UnixDateTime, ApiHelper.UnixDateTime]]),
+        ([[500, 1000]], ApiHelper.UnixDateTime, [[int, int]]),
+        ([['500', '1000']], ApiHelper.UnixDateTime, [[str, str]]),
+        ([['500', datetime(1994, 2, 13, 5, 30, 15)]], ApiHelper.UnixDateTime, [[str, ApiHelper.UnixDateTime]]),
+        (None, ApiHelper.RFC3339DateTime, None)
+    ])
+    def test_apply_date_time_converter_to_list_of_list(self, input_value, input_converter, expected_obj):
+        if input_value is None:
+            assert ApiHelper.apply_datetime_converter(input_value, input_converter) == expected_obj
+        else:
+            actual_converted_value = ApiHelper.apply_datetime_converter(input_value, input_converter)
+            for outer_index, actual_outer_value in enumerate(actual_converted_value):
+                for index, actual_value in enumerate(actual_outer_value):
+                    assert isinstance(actual_value, expected_obj[outer_index][index])
+
+    @pytest.mark.parametrize('input_value, input_converter, expected_obj', [
+        ({'key0': datetime(1994, 2, 13, 5, 30, 15), 'key1': datetime(1994, 2, 13, 5, 30, 15)}, ApiHelper.RFC3339DateTime,
+         [ApiHelper.RFC3339DateTime, ApiHelper.RFC3339DateTime]),
+        ({'key0': datetime(1994, 2, 13, 5, 30, 15), 'key1': datetime(1994, 2, 13, 5, 30, 15)}, ApiHelper.HttpDateTime,
+         [ApiHelper.HttpDateTime, ApiHelper.HttpDateTime]),
+        ({'key0': datetime(1994, 2, 13, 5, 30, 15), 'key1': datetime(1994, 2, 13, 5, 30, 15)}, ApiHelper.UnixDateTime,
+         [ApiHelper.UnixDateTime, ApiHelper.UnixDateTime]),
+        ({'key0': '5000', 'key1': datetime(1994, 2, 13, 5, 30, 15)}, ApiHelper.UnixDateTime,
+         [str, ApiHelper.UnixDateTime]),
+        ({'key0': 5000, 'key1': 10000}, ApiHelper.UnixDateTime, [int, int]),
+        ({'key0': '5000', 'key1': '10000'}, ApiHelper.UnixDateTime, [str, str]),
+        (None, ApiHelper.RFC3339DateTime, None)
+    ])
+    def test_apply_date_time_converter_to_dict(self, input_value, input_converter, expected_obj):
+        if input_value is None:
+            assert ApiHelper.apply_datetime_converter(input_value, input_converter) == expected_obj
+        else:
+            actual_converted_value = ApiHelper.apply_datetime_converter(input_value, input_converter)
+            for index, actual_value in enumerate(actual_converted_value.values()):
+                assert isinstance(actual_value, expected_obj[index])
+
+    @pytest.mark.parametrize('input_value, input_converter, expected_obj', [
+        ({'key': {'key0': datetime(1994, 2, 13, 5, 30, 15), 'key1': datetime(1994, 2, 13, 5, 30, 15)}},
+         ApiHelper.RFC3339DateTime, {'key': [ApiHelper.RFC3339DateTime, ApiHelper.RFC3339DateTime]}),
+        ({'key': {'key0': datetime(1994, 2, 13, 5, 30, 15), 'key1': datetime(1994, 2, 13, 5, 30, 15)}}, ApiHelper.HttpDateTime,
+         {'key': [ApiHelper.HttpDateTime, ApiHelper.HttpDateTime]}),
+        ({'key': {'key0': datetime(1994, 2, 13, 5, 30, 15), 'key1': datetime(1994, 2, 13, 5, 30, 15)}}, ApiHelper.UnixDateTime,
+         {'key': [ApiHelper.UnixDateTime, ApiHelper.UnixDateTime]}),
+        ({'key': {'key0': '5000', 'key1': datetime(1994, 2, 13, 5, 30, 15)}}, ApiHelper.UnixDateTime,
+         {'key': [str, ApiHelper.UnixDateTime]}),
+        ({'key': {'key0': 5000, 'key1': 10000}}, ApiHelper.UnixDateTime, {'key': [int, int]}),
+        ({'key': {'key0': '5000', 'key1': '10000'}}, ApiHelper.UnixDateTime, {'key': [str, str]}),
+        (None, ApiHelper.RFC3339DateTime, None)
+    ])
+    def test_apply_date_time_converter_to_dict_of_dict(self, input_value, input_converter, expected_obj):
+        if input_value is None:
+            assert ApiHelper.apply_datetime_converter(input_value, input_converter) == expected_obj
+        else:
+            actual_converted_value = ApiHelper.apply_datetime_converter(input_value, input_converter)
+            for outer_key, actual_outer_value in actual_converted_value.items():
+                for index, actual_value in enumerate(actual_outer_value.values()):
+                    assert isinstance(actual_value, expected_obj[outer_key][index])
+
     @pytest.mark.parametrize('input_array,formatting, is_query, expected_array', [
         ([1, True, 'string', 2.36, Base.get_rfc3339_datetime(datetime(1994, 2, 13, 5, 30, 15)),
           str(date(1994, 2, 13))], SerializationFormats.INDEXED, False, [('test_array[0]', 1),
                                                                          ('test_array[1]', True),
                                                                          ('test_array[2]', 'string'),
                                                                          ('test_array[3]', 2.36),
                                                                          ('test_array[4]', Base.get_rfc3339_datetime(
@@ -669,7 +844,50 @@
          'Test template -- ')
     ])
     def test_resolve_template_placeholders_using_json_pointer(self, input_placeholders, input_value, input_template,
                                                               expected_message):
         actual_message = ApiHelper.resolve_template_placeholders_using_json_pointer(input_placeholders, input_value,
                                                                                     input_template)
         assert actual_message == expected_message
+
+    @pytest.mark.parametrize('input_value, input_callable, expected_value', [
+        (100, lambda value: isinstance(value, int), True),
+        ('100', lambda value: isinstance(value, str), True),
+        ("Sunday", lambda value: Days.validate(value), True),
+        (100.5, lambda value: isinstance(value, str), False),
+        ("Invalid", lambda value: Days.validate(value), False),
+        (None, lambda value: isinstance(value, str), False),
+        (None, None, False),
+
+        ([100, 200], lambda value: isinstance(value, int), True),
+        (['100', '200'], lambda value: isinstance(value, str), True),
+        (["Sunday", "Monday"], lambda value: Days.validate(value), True),
+        ([100.5, 200], lambda value: isinstance(value, str), False),
+        (["Invalid1", "Invalid2"], lambda value: Days.validate(value), False),
+        ([None, None], lambda value: isinstance(value, str), False),
+
+        ([[100, 200], [300, 400]], lambda value: isinstance(value, int), True),
+        ([['100', '200'], ['abc', 'def']], lambda value: isinstance(value, str), True),
+        ([["Sunday", "Monday"], ["Tuesday", "Friday"]], lambda value: Days.validate(value), True),
+        ([[100.5, 200], [400, 500]], lambda value: isinstance(value, str), False),
+        ([["Invalid1", "Invalid2"], ["Sunday", "Invalid4"]], lambda value: Days.validate(value), False),
+        ([[None, None], [None, None]], lambda value: isinstance(value, str), False),
+
+        ({'key0': 100, 'key2': 200}, lambda value: isinstance(value, int), True),
+        ({'key0': 'abc', 'key2': 'def'}, lambda value: isinstance(value, str), True),
+        ({'key0': 'Sunday', 'key2': 'Tuesday'}, lambda value: Days.validate(value), True),
+        ({'key0': 100.5, 'key2': 200}, lambda value: isinstance(value, str), False),
+        ({'key0': "Invalid1", 'key2': "Invalid2"}, lambda value: Days.validate(value), False),
+        ({'key0': None, 'key2': None}, lambda value: isinstance(value, str), False),
+    ])
+    def test_is_valid_type(self, input_value, input_callable, expected_value):
+        actual_value = ApiHelper.is_valid_type(input_value, input_callable)
+        assert actual_value == expected_value
+
+    @pytest.mark.parametrize('input_value, input_union_type, input_should_deserialize, expected_value', [
+        (100, OneOf([LeafType(int), LeafType(str)]), False, 100),
+        ('[100, "200"]', OneOf([LeafType(int), LeafType(str)], UnionTypeContext.create(is_array=True)), True,
+         [100, '200']),
+    ])
+    def test_union_type_deserialize(self, input_value, input_union_type, input_should_deserialize, expected_value):
+        actual_value = ApiHelper.deserialize_union_type(input_union_type, input_value, input_should_deserialize)
+        assert actual_value == expected_value
```

### Comparing `apimatic-core-0.2.3/tests/apimatic_core/utility_tests/test_auth_helper.py` & `apimatic-core-0.2.4/tests/apimatic_core/utility_tests/test_auth_helper.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.3/tests/apimatic_core/utility_tests/test_comparison_helper.py` & `apimatic-core-0.2.4/tests/apimatic_core/utility_tests/test_comparison_helper.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.3/tests/apimatic_core/utility_tests/test_file_helper.py` & `apimatic-core-0.2.4/tests/apimatic_core/utility_tests/test_file_helper.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.3/tests/apimatic_core/utility_tests/test_xml_helper.py` & `apimatic-core-0.2.4/tests/apimatic_core/utility_tests/test_xml_helper.py`

 * *Files identical despite different names*

