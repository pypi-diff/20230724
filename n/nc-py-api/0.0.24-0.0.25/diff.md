# Comparing `tmp/nc_py_api-0.0.24.tar.gz` & `tmp/nc_py_api-0.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nc_py_api-0.0.24.tar", last modified: Tue Jul 18 20:10:33 2023, max compression
+gzip compressed data, was "nc_py_api-0.0.25.tar", last modified: Mon Jul 24 19:20:45 2023, max compression
```

## Comparing `nc_py_api-0.0.24.tar` & `nc_py_api-0.0.25.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 20:10:33.026886 nc_py_api-0.0.24/
--rw-r--r--   0 runner    (1001) docker     (122)      864 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     1551 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      230 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     4117 2023-07-18 20:10:33.026886 nc_py_api-0.0.24/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2640 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 20:10:33.022885 nc_py_api-0.0.24/nc_py_api/
--rw-r--r--   0 runner    (1001) docker     (122)      457 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/nc_py_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13514 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/nc_py_api/_session.py
--rw-r--r--   0 runner    (1001) docker     (122)       52 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/nc_py_api/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/nc_py_api/appconfig_preferences_ex.py
--rw-r--r--   0 runner    (1001) docker     (122)     2510 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/nc_py_api/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)      534 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/nc_py_api/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     1042 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/nc_py_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    23440 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/nc_py_api/files.py
--rw-r--r--   0 runner    (1001) docker     (122)     1657 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/nc_py_api/integration_fastapi.py
--rw-r--r--   0 runner    (1001) docker     (122)      928 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/nc_py_api/misc.py
--rw-r--r--   0 runner    (1001) docker     (122)     4111 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/nc_py_api/nextcloud.py
--rw-r--r--   0 runner    (1001) docker     (122)      352 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/nc_py_api/options.py
--rw-r--r--   0 runner    (1001) docker     (122)      971 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/nc_py_api/preferences.py
--rw-r--r--   0 runner    (1001) docker     (122)     1464 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/nc_py_api/theming.py
--rw-r--r--   0 runner    (1001) docker     (122)     1592 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/nc_py_api/ui_files_actions_menu.py
--rw-r--r--   0 runner    (1001) docker     (122)     3035 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/nc_py_api/users.py
--rw-r--r--   0 runner    (1001) docker     (122)     2612 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/nc_py_api/users_groups.py
--rw-r--r--   0 runner    (1001) docker     (122)     4232 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/nc_py_api/users_status.py
--rw-r--r--   0 runner    (1001) docker     (122)     3047 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/nc_py_api/weather_status.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 20:10:33.026886 nc_py_api-0.0.24/nc_py_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4117 2023-07-18 20:10:33.000000 nc_py_api-0.0.24/nc_py_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      735 2023-07-18 20:10:33.000000 nc_py_api-0.0.24/nc_py_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-18 20:10:33.000000 nc_py_api-0.0.24/nc_py_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      289 2023-07-18 20:10:33.000000 nc_py_api-0.0.24/nc_py_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-18 20:10:33.000000 nc_py_api-0.0.24/nc_py_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-18 20:10:24.000000 nc_py_api-0.0.24/nc_py_api.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)     1434 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1782 2023-07-18 20:10:33.026886 nc_py_api-0.0.24/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      344 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 19:20:45.594195 nc_py_api-0.0.25/
+-rw-r--r--   0 runner    (1001) docker     (122)      475 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (122)     1050 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1551 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      246 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4095 2023-07-24 19:20:45.594195 nc_py_api-0.0.25/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2596 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 19:20:45.594195 nc_py_api-0.0.25/nc_py_api/
+-rw-r--r--   0 runner    (1001) docker     (122)      560 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/nc_py_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13624 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/nc_py_api/_session.py
+-rw-r--r--   0 runner    (1001) docker     (122)       52 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/nc_py_api/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2501 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/nc_py_api/appconfig_preferences_ex.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/nc_py_api/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2050 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/nc_py_api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1214 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/nc_py_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24442 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/nc_py_api/files.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5026 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/nc_py_api/files_sharing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1657 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/nc_py_api/integration_fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)      917 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/nc_py_api/misc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4243 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/nc_py_api/nextcloud.py
+-rw-r--r--   0 runner    (1001) docker     (122)      352 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/nc_py_api/options.py
+-rw-r--r--   0 runner    (1001) docker     (122)      971 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/nc_py_api/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1452 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/nc_py_api/theming.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1788 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/nc_py_api/ui_files_actions_menu.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3035 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/nc_py_api/users.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2612 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/nc_py_api/users_groups.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4266 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/nc_py_api/users_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3141 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/nc_py_api/weather_status.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 19:20:45.594195 nc_py_api-0.0.25/nc_py_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4095 2023-07-24 19:20:45.000000 nc_py_api-0.0.25/nc_py_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      770 2023-07-24 19:20:45.000000 nc_py_api-0.0.25/nc_py_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-24 19:20:45.000000 nc_py_api-0.0.25/nc_py_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      316 2023-07-24 19:20:45.000000 nc_py_api-0.0.25/nc_py_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-24 19:20:45.000000 nc_py_api-0.0.25/nc_py_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-24 19:20:36.000000 nc_py_api-0.0.25/nc_py_api.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)     1436 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1810 2023-07-24 19:20:45.594195 nc_py_api-0.0.25/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      344 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/setup.py
```

### Comparing `nc_py_api-0.0.24/CHANGELOG.md` & `nc_py_api-0.0.25/CHANGELOG.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,23 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
-## [0.0.24 - 2023-07-xx]
+## [0.0.25 - 2023-07-25]
+
+### Added
+
+- First `Files Sharing` APIs.
+
+### Changed
+
+- Updated documentation, description.
+- Updated `FsNode` class with properties for parsing permissions.
+
+## [0.0.24 - 2023-07-18]
 
 ### Added
 
 - `VERIFY_NC_CERTIFICATE` option.
 - `apps.ex_app_get_list` and `apps.ex_app_get_info` methods.
 - `files.download2stream` and `files.upload_stream` methods.
 - most of `FileAPI` can accept `FsNode` as a path.
```

### Comparing `nc_py_api-0.0.24/LICENSE.txt` & `nc_py_api-0.0.25/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.24/PKG-INFO` & `nc_py_api-0.0.25/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nc_py_api
-Version: 0.0.24
+Version: 0.0.25
 Summary: Nextcloud Python Framework
 Home-page: https://github.com/cloud-py-api/nc_py_api
 Author: Alexander Piskun
 License: BSD-3-Clause
 Project-URL: Source, https://github.com/cloud-py-api/nc_py_api
 Keywords: nextcloud,api,framework
 Classifier: Development Status :: 1 - Planning
@@ -28,61 +28,64 @@
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: bench
 Provides-Extra: dev
 License-File: LICENSE.txt
+License-File: AUTHORS
 
 # Official Nextcloud Python Framework
 
 [![Analysis & Coverage](https://github.com/cloud-py-api/nc_py_api/actions/workflows/analysis-coverage.yml/badge.svg)](https://github.com/cloud-py-api/nc_py_api/actions/workflows/analysis-coverage.yml)
 [![Docs](https://github.com/cloud-py-api/nc_py_api/actions/workflows/docs.yml/badge.svg)](https://cloud-py-api.github.io/nc_py_api/)
 [![codecov](https://codecov.io/github/cloud-py-api/nc_py_api/branch/main/graph/badge.svg?token=C91PL3FYDQ)](https://codecov.io/github/cloud-py-api/nc_py_api)
 
 ![NextcloudVersion](https://img.shields.io/badge/Nextcloud-26%20%7C%2027%20%7C%2028-blue)
 ![PythonVersion](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue)
 ![impl](https://img.shields.io/pypi/implementation/nc_py_api)
 ![pypi](https://img.shields.io/pypi/v/nc_py_api.svg)
 
-### Remark
-
-Project cloud-py-api was **abandoned** and divided into two parts:
- * `nc_py_api` - this repository, which contains Python Framework to work with Nextcloud and `app_ecosystem_v2`
- * `app_ecosystem_v2` - New [Nextcloud Application Ecosystem](https://github.com/cloud-py-api/app_ecosystem_v2) that allows writing applications for Nextcloud in any language
-
-**_Projects stage: under heavy prototyping and developing_**
+Python library that provides a robust and well-documented API that allows developers to interact with and extend Nextcloud's functionality.
 
 ### Basic Features:
- * Listing, enabling and disabling of the applications
  * Operations with Files and Folders
  * ~~Operations with Trash bin and File versions~~
  * Operations with Users and User Groups
- * User status manipulation
+ * User status
  * Weather status
  * ~~Nextcloud notifications support~~
- * ~~Shares operations support~~
+ * Shares support
  * ~~Talk support~~
 
-### Extended Features with installed App_ecosystem_v2:
- * Defining callback routes with FastAPI for Nextcloud
+### Extended Features with AppEcosystemV2:
+ * Defining callback routes with `FastAPI` for Nextcloud
  * Registering UI elements in Nextcloud
  * Storing logs to the `nextcloud.log` file
  * Get/save key-value pairs in AppConfigEx/PreferencesEx tables.
  * **Tons of the cool stuff that is coming soon**
 
+### Support
+
+You can support us in several ways:
+
+- ⭐️ Star our work (it really motivates)
+- ❗️ Create an Issue or feature request (bring to us an excellent idea)
+- 💁 Resolve some Issue or create a Pull Request (contribute to this project)
+- 🙏 Write an example of its use or correct a typo in the documentation.
+
 ### 🚀 How to start
 
-In very close near future we will publish examples
+In a very close near future we will publish examples
 
 ### More Information
 
-- [Documentation](https://nc_py_api.readthedocs.io/)
+- [Documentation](https://cloud-py-api.github.io/nc_py_api/)
   - [Using it as a simple client](to-do)
   - [Writing a simple Nextcloud application](to-do)
-  - [Writing a Nextcloud system application](to-do)
+  - [Writing a Nextcloud System Application](to-do)
 - [Examples](https://github.com/cloud-py-api/nc_py_api/tree/main/examples)
 - [Contribute](https://github.com/cloud-py-api/nc_py_api/blob/main/.github/CONTRIBUTING.md)
   - [Discussions](https://github.com/cloud-py-api/nc_py_api/discussions)
   - [Issues](https://github.com/cloud-py-api/nc_py_api/issues)
   - [Setting up dev environment](to-do)
 - [Changelog](https://github.com/cloud-py-api/nc_py_api/blob/main/CHANGELOG.md)
```

### Comparing `nc_py_api-0.0.24/README.md` & `nc_py_api-0.0.25/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -5,49 +5,51 @@
 [![codecov](https://codecov.io/github/cloud-py-api/nc_py_api/branch/main/graph/badge.svg?token=C91PL3FYDQ)](https://codecov.io/github/cloud-py-api/nc_py_api)
 
 ![NextcloudVersion](https://img.shields.io/badge/Nextcloud-26%20%7C%2027%20%7C%2028-blue)
 ![PythonVersion](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue)
 ![impl](https://img.shields.io/pypi/implementation/nc_py_api)
 ![pypi](https://img.shields.io/pypi/v/nc_py_api.svg)
 
-### Remark
-
-Project cloud-py-api was **abandoned** and divided into two parts:
- * `nc_py_api` - this repository, which contains Python Framework to work with Nextcloud and `app_ecosystem_v2`
- * `app_ecosystem_v2` - New [Nextcloud Application Ecosystem](https://github.com/cloud-py-api/app_ecosystem_v2) that allows writing applications for Nextcloud in any language
-
-**_Projects stage: under heavy prototyping and developing_**
+Python library that provides a robust and well-documented API that allows developers to interact with and extend Nextcloud's functionality.
 
 ### Basic Features:
- * Listing, enabling and disabling of the applications
  * Operations with Files and Folders
  * ~~Operations with Trash bin and File versions~~
  * Operations with Users and User Groups
- * User status manipulation
+ * User status
  * Weather status
  * ~~Nextcloud notifications support~~
- * ~~Shares operations support~~
+ * Shares support
  * ~~Talk support~~
 
-### Extended Features with installed App_ecosystem_v2:
- * Defining callback routes with FastAPI for Nextcloud
+### Extended Features with AppEcosystemV2:
+ * Defining callback routes with `FastAPI` for Nextcloud
  * Registering UI elements in Nextcloud
  * Storing logs to the `nextcloud.log` file
  * Get/save key-value pairs in AppConfigEx/PreferencesEx tables.
  * **Tons of the cool stuff that is coming soon**
 
+### Support
+
+You can support us in several ways:
+
+- ⭐️ Star our work (it really motivates)
+- ❗️ Create an Issue or feature request (bring to us an excellent idea)
+- 💁 Resolve some Issue or create a Pull Request (contribute to this project)
+- 🙏 Write an example of its use or correct a typo in the documentation.
+
 ### 🚀 How to start
 
-In very close near future we will publish examples
+In a very close near future we will publish examples
 
 ### More Information
 
-- [Documentation](https://nc_py_api.readthedocs.io/)
+- [Documentation](https://cloud-py-api.github.io/nc_py_api/)
   - [Using it as a simple client](to-do)
   - [Writing a simple Nextcloud application](to-do)
-  - [Writing a Nextcloud system application](to-do)
+  - [Writing a Nextcloud System Application](to-do)
 - [Examples](https://github.com/cloud-py-api/nc_py_api/tree/main/examples)
 - [Contribute](https://github.com/cloud-py-api/nc_py_api/blob/main/.github/CONTRIBUTING.md)
   - [Discussions](https://github.com/cloud-py-api/nc_py_api/discussions)
   - [Issues](https://github.com/cloud-py-api/nc_py_api/issues)
   - [Setting up dev environment](to-do)
 - [Changelog](https://github.com/cloud-py-api/nc_py_api/blob/main/CHANGELOG.md)
```

### Comparing `nc_py_api-0.0.24/nc_py_api/_session.py` & `nc_py_api-0.0.25/nc_py_api/_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 from urllib.parse import quote, urlencode
 
 from fastapi import Request
 from httpx import Client, Limits, ReadTimeout, Response
 from xxhash import xxh64
 
 from . import options
-from .exceptions import NextcloudException, check_error
+from .constants import OCSRespond
+from .exceptions import NextcloudException, NextcloudExceptionNotFound, check_error
 
 
 class ServerVersion(TypedDict):
     major: int
     minor: int
     micro: int
     string: str
@@ -134,25 +135,25 @@
                 response = self.adapter.request(
                     method, url_params, headers=headers, content=data, timeout=timeout, **kwargs
                 )
         except ReadTimeout:
             raise NextcloudException(408, info=info) from None
 
         check_error(response.status_code, info)
-        if not response.text:
-            raise ValueError(f"Response is empty. Status code: {response.status_code}")
         response_data = loads(response.text)
         ocs_meta = response_data["ocs"]["meta"]
         if ocs_meta["status"] != "ok":
             if not nested_req:
                 if ocs_meta["statuscode"] == 403:
                     if str(ocs_meta["message"]).lower().find("password confirmation is required") != -1:
                         self.adapter.close()
                         self.init_adapter(restart=True)
                         return self._ocs(method, path_params, headers, data, **kwargs, nested_req=True)
+            if ocs_meta["statuscode"] in (404, OCSRespond.RESPOND_NOT_FOUND):
+                raise NextcloudExceptionNotFound(reason=ocs_meta["message"], info=info)
             raise NextcloudException(status_code=ocs_meta["statuscode"], reason=ocs_meta["message"], info=info)
         return response_data["ocs"]["data"]
 
     def dav(self, method: str, path: str, data: Optional[Union[str, bytes]] = None, **kwargs) -> Response:
         headers = kwargs.pop("headers", {})
         data_bytes = None
         if data is not None:
```

### Comparing `nc_py_api-0.0.24/nc_py_api/apps.py` & `nc_py_api-0.0.25/nc_py_api/apps.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 class ExAppInfo(TypedDict):
     id: str
     name: str
     version: str
     enabled: bool
-    last_response_time: int
+    last_check_time: int
     system: bool
 
 
 class AppAPI:
     def __init__(self, session: NcSessionBasic):
         self._session = session
```

### Comparing `nc_py_api-0.0.24/nc_py_api/exceptions.py` & `nc_py_api-0.0.25/nc_py_api/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,19 @@
 
     def __str__(self):
         reason = f" {self.reason}" if self.reason else ""
         info = f" <{self.info}>" if self.info else ""
         return f"[{self.status_code}]{reason}{info}"
 
 
+class NextcloudExceptionNotFound(NextcloudException):
+    def __init__(self, reason="Not found", info: str = ""):
+        super().__init__(404, reason=reason, info=info)
+
+
 def check_error(code: int, info: str = ""):
     if 996 <= code <= 999:
         if code == 996:
             phrase = "Server error"
         elif code == 997:
             phrase = "Unauthorised"
         elif code == 998:
```

### Comparing `nc_py_api-0.0.24/nc_py_api/files.py` & `nc_py_api-0.0.25/nc_py_api/files.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Nextcloud API for working with file system.
+Nextcloud API for working with the file system.
 """
 
 import builtins
 import os
 from dataclasses import dataclass
 from datetime import datetime
 from email.utils import parsedate_to_datetime
@@ -31,14 +31,15 @@
     fileid: int
     """Object file ID."""
     etag: str
     size: int
     content_length: int
     last_modified: datetime
     permissions: str
+    """Permissions for the object."""
     favorite: bool
 
 
 @dataclass
 class FsNode:
     """A class that represents a Nextcloud file object.
 
@@ -95,14 +96,46 @@
 
     def __str__(self):
         return (
             f"{'Dir' if self.is_dir else 'File'}: `{self.name}` with id={self.info['fileid']}"
             f" last modified at {str(self.last_modified)} and {self.info['permissions']} permissions."
         )
 
+    @property
+    def is_shared(self) -> bool:
+        return self.info["permissions"].find("S") != -1
+
+    @property
+    def is_shareable(self) -> bool:
+        return self.info["permissions"].find("R") != -1
+
+    @property
+    def is_mounted(self) -> bool:
+        return self.info["permissions"].find("M") != -1
+
+    @property
+    def is_readable(self) -> bool:
+        return self.info["permissions"].find("G") != -1
+
+    @property
+    def is_deletable(self) -> bool:
+        return self.info["permissions"].find("D") != -1
+
+    @property
+    def is_updatable(self) -> bool:
+        if self.is_dir:
+            return self.info["permissions"].find("NV") != -1
+        return self.info["permissions"].find("W") != -1
+
+    @property
+    def is_creatable(self) -> bool:
+        if not self.is_dir:
+            return False
+        return self.info["permissions"].find("CK") != -1
+
 
 PROPFIND_PROPERTIES = [
     "d:resourcetype",
     "d:getlastmodified",
     "d:getcontentlength",
     "d:getetag",
     "oc:size",
@@ -131,14 +164,16 @@
     "size": "oc:size",  # gt, gte, eq, lt
     "favorite": "oc:favorite",  # eq
     "fileid": "oc:fileid",  # eq
 }
 
 
 class FilesAPI:
+    """This class provides all WebDAV functionality related to the files."""
+
     def __init__(self, session: NcSessionBasic):
         self._session = session
 
     def listdir(self, path: Union[str, FsNode] = "", exclude_self=True) -> list[FsNode]:
         """Returns a list of all entries in the specified directory.
 
         :param path: Path to the directory to get the list.
```

### Comparing `nc_py_api-0.0.24/nc_py_api/integration_fastapi.py` & `nc_py_api-0.0.25/nc_py_api/integration_fastapi.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.24/nc_py_api/misc.py` & `nc_py_api-0.0.25/nc_py_api/misc.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,14 @@
             data[k] = kwargs[k]
     return data
 
 
 def require_capabilities(capabilities: Union[str, list[str]], srv_capabilities: dict) -> None:
     result = check_capabilities(capabilities, srv_capabilities)
     if result:
-        raise NextcloudException(404, f"{result} capability is not available")
+        raise NextcloudException(404, f"{result} is not available")
 
 
 def check_capabilities(capabilities: Union[str, list[str]], srv_capabilities: dict) -> list[str]:
     if isinstance(capabilities, str):
         capabilities = [capabilities]
     return [i for i in capabilities if i not in srv_capabilities]
```

### Comparing `nc_py_api-0.0.24/nc_py_api/nextcloud.py` & `nc_py_api-0.0.25/nc_py_api/nextcloud.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,37 +7,40 @@
 from fastapi import Request
 
 from ._session import AppConfig, NcSession, NcSessionApp, NcSessionBasic, ServerVersion
 from .appconfig_preferences_ex import AppConfigExAPI, PreferencesExAPI
 from .apps import AppAPI
 from .constants import APP_V2_BASIC_URL, ApiScope, LogLvl
 from .files import FilesAPI
+from .files_sharing import FilesSharingAPI
 from .misc import check_capabilities
 from .preferences import PreferencesAPI
 from .theming import ThemingInfo, get_parsed_theme
 from .ui_files_actions_menu import UiFilesActionsAPI
 from .users import UsersAPI
 from .users_groups import UserGroupsAPI
 from .users_status import UserStatusAPI
 from .weather_status import WeatherStatusAPI
 
 
 class NextcloudBasic(ABC):
     apps: AppAPI
     files: FilesAPI
+    files_sharing: FilesSharingAPI
     preferences_api: PreferencesAPI
     users: UsersAPI
     users_groups: UserGroupsAPI
     users_status: UserStatusAPI
     weather_status: WeatherStatusAPI
     _session: NcSessionBasic
 
     def _init_api(self, session: NcSessionBasic):
         self.apps = AppAPI(session)
         self.files = FilesAPI(session)
+        self.files_sharing = FilesSharingAPI(session)
         self.preferences_api = PreferencesAPI(session)
         self.users = UsersAPI(session)
         self.users_groups = UserGroupsAPI(session)
         self.users_status = UserStatusAPI(session)
         self.weather_status = WeatherStatusAPI(session)
 
     @property
```

### Comparing `nc_py_api-0.0.24/nc_py_api/preferences.py` & `nc_py_api-0.0.25/nc_py_api/preferences.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Nextcloud API for working with classics app's storage with user context(table oc_preferences).
 """
 
 from ._session import NcSessionBasic
 from .misc import check_capabilities, require_capabilities
 
-ENDPOINT = "/ocs/v2.php/apps/provisioning_api/api/v1/config/users"
+ENDPOINT = "/ocs/v1.php/apps/provisioning_api/api/v1/config/users"
 
 
 class PreferencesAPI:
     def __init__(self, session: NcSessionBasic):
         self._session = session
 
     @property
```

### Comparing `nc_py_api-0.0.24/nc_py_api/theming.py` & `nc_py_api-0.0.25/nc_py_api/theming.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,32 +16,32 @@
     color_element_dark: tuple[int, int, int]
     logo: str
     background: str
     background_plain: bool
     background_default: bool
 
 
-def __convert_str_color(theming_capability: dict, key: str) -> tuple[int, int, int]:
+def convert_str_color(theming_capability: dict, key: str) -> tuple[int, int, int]:
     if key not in theming_capability:
         return 0, 0, 0
     value = theming_capability[key]
     if not value or value == "#":
         return 0, 0, 0
     return int(value[1:3], 16), int(value[3:5], 16), int(value[5:7], 16)
 
 
 def get_parsed_theme(theming_capability: dict) -> ThemingInfo:
     i = theming_capability
     return ThemingInfo(
         name=i["name"],
         url=i["url"],
         slogan=i["slogan"],
-        color=__convert_str_color(i, "color"),
-        color_text=__convert_str_color(i, "color-text"),
-        color_element=__convert_str_color(i, "color-element"),
-        color_element_bright=__convert_str_color(i, "color-element-bright"),
-        color_element_dark=__convert_str_color(i, "color-element-dark"),
+        color=convert_str_color(i, "color"),
+        color_text=convert_str_color(i, "color-text"),
+        color_element=convert_str_color(i, "color-element"),
+        color_element_bright=convert_str_color(i, "color-element-bright"),
+        color_element_dark=convert_str_color(i, "color-element-dark"),
         logo=i["logo"],
         background=i.get("background", ""),
         background_plain=i.get("background-plain", False),
         background_default=i.get("background-default", False),
     )
```

### Comparing `nc_py_api-0.0.24/nc_py_api/ui_files_actions_menu.py` & `nc_py_api-0.0.25/nc_py_api/ui_files_actions_menu.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Nextcloud API for working with drop down file's menu.
 """
 
 from pydantic import BaseModel
 
 from ._session import NcSessionApp
 from .constants import APP_V2_BASIC_URL
+from .exceptions import NextcloudExceptionNotFound
 from .misc import require_capabilities
 
 
 class UiActionFileInfo(BaseModel):
     fileId: int
     name: str
     dir: str
@@ -24,27 +25,31 @@
 ENDPOINT_SUFFIX = "files/actions/menu"
 
 
 class UiFilesActionsAPI:
     def __init__(self, session: NcSessionApp):
         self._session = session
 
-    def register(self, name: str, display_name: str, callback_url: str, **kwargs):
+    def register(self, name: str, display_name: str, callback_url: str, **kwargs) -> None:
         require_capabilities("app_ecosystem_v2", self._session.capabilities)
         params = {
             "fileActionMenuParams": {
                 "name": name,
                 "display_name": display_name,
                 "mime": kwargs.get("mime", "file"),
                 "permissions": kwargs.get("permissions", 31),
                 "order": kwargs.get("order", 0),
                 "icon": kwargs.get("icon", ""),
                 "icon_class": kwargs.get("icon_class", "icon-app-ecosystem-v2"),
                 "action_handler": callback_url,
             },
         }
-        return self._session.ocs(method="POST", path=f"{APP_V2_BASIC_URL}/{ENDPOINT_SUFFIX}", json=params)
+        self._session.ocs(method="POST", path=f"{APP_V2_BASIC_URL}/{ENDPOINT_SUFFIX}", json=params)
 
-    def unregister(self, name: str):
+    def unregister(self, name: str, not_fail=True) -> None:
         require_capabilities("app_ecosystem_v2", self._session.capabilities)
         params = {"fileActionMenuName": name}
-        return self._session.ocs(method="DELETE", path=f"{APP_V2_BASIC_URL}/{ENDPOINT_SUFFIX}", json=params)
+        try:
+            self._session.ocs(method="DELETE", path=f"{APP_V2_BASIC_URL}/{ENDPOINT_SUFFIX}", json=params)
+        except NextcloudExceptionNotFound as e:
+            if not not_fail:
+                raise e from None
```

### Comparing `nc_py_api-0.0.24/nc_py_api/users.py` & `nc_py_api-0.0.25/nc_py_api/users.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.24/nc_py_api/users_groups.py` & `nc_py_api-0.0.25/nc_py_api/users_groups.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.24/nc_py_api/users_status.py` & `nc_py_api-0.0.25/nc_py_api/users_status.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 Nextcloud API for working with users statuses.
 """
 
 from typing import Literal, Optional, TypedDict, Union
 
 from ._session import NcSessionBasic
-from .exceptions import NextcloudException
+from .exceptions import NextcloudExceptionNotFound
 from .misc import check_capabilities, kwargs_to_dict, require_capabilities
 
-ENDPOINT = "/ocs/v2.php/apps/user_status/api/v1"
+ENDPOINT = "/ocs/v1.php/apps/user_status/api/v1"
 
 
 class PredefinedStatus(TypedDict):
     id: str
     icon: str
     message: str
     clearAt: Optional[dict]
@@ -34,14 +34,16 @@
 
 class UserStatusAPI:
     def __init__(self, session: NcSessionBasic):
         self._session = session
 
     @property
     def available(self) -> bool:
+        """Returns True if the Nextcloud instance supports this feature, False otherwise."""
+
         return not check_capabilities("user_status", self._session.capabilities)
 
     def get_list(self, limit: Optional[int] = None, offset: Optional[int] = None) -> list[UserStatus]:
         require_capabilities("user_status", self._session.capabilities)
         data = kwargs_to_dict(["limit", "offset"], limit=limit, offset=offset)
         return self._session.ocs(method="GET", path=f"{ENDPOINT}/statuses", params=data)
 
@@ -49,18 +51,16 @@
         require_capabilities("user_status", self._session.capabilities)
         return self._session.ocs(method="GET", path=f"{ENDPOINT}/user_status")
 
     def get(self, user_id: str) -> Optional[UserStatus]:
         require_capabilities("user_status", self._session.capabilities)
         try:
             return self._session.ocs(method="GET", path=f"{ENDPOINT}/statuses/{user_id}")
-        except NextcloudException as e:
-            if e.status_code == 404:
-                return None
-            raise e from None
+        except NextcloudExceptionNotFound:
+            return None
 
     def get_predefined(self) -> list[PredefinedStatus]:
         if self._session.nc_version["major"] < 27:
             return []
         require_capabilities("user_status", self._session.capabilities)
         return self._session.ocs(method="GET", path=f"{ENDPOINT}/predefined_statuses")
```

### Comparing `nc_py_api-0.0.24/nc_py_api/weather_status.py` & `nc_py_api-0.0.25/nc_py_api/weather_status.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from enum import IntEnum
 from typing import Optional, TypedDict, Union
 
 from ._session import NcSessionBasic
 from .misc import check_capabilities, require_capabilities
 
-ENDPOINT = "/ocs/v2.php/apps/weather_status/api/v1"
+ENDPOINT = "/ocs/v1.php/apps/weather_status/api/v1"
 
 
 class WeatherLocationMode(IntEnum):
     UNKNOWN = 0
     MODE_BROWSER_LOCATION = 1
     MODE_MANUAL_LOCATION = 2
 
@@ -26,14 +26,16 @@
 
 class WeatherStatusAPI:
     def __init__(self, session: NcSessionBasic):
         self._session = session
 
     @property
     def available(self) -> bool:
+        """Returns True if the Nextcloud instance supports this feature, False otherwise."""
+
         return not check_capabilities("weather_status", self._session.capabilities)
 
     def get_location(self) -> WeatherLocation:
         require_capabilities("weather_status", self._session.capabilities)
         result = self._session.ocs(method="GET", path=f"{ENDPOINT}/location")
         lat = result.get("lat", "")
         lon = result.get("lon", "")
```

### Comparing `nc_py_api-0.0.24/nc_py_api.egg-info/PKG-INFO` & `nc_py_api-0.0.25/nc_py_api.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nc-py-api
-Version: 0.0.24
+Version: 0.0.25
 Summary: Nextcloud Python Framework
 Home-page: https://github.com/cloud-py-api/nc_py_api
 Author: Alexander Piskun
 License: BSD-3-Clause
 Project-URL: Source, https://github.com/cloud-py-api/nc_py_api
 Keywords: nextcloud,api,framework
 Classifier: Development Status :: 1 - Planning
@@ -28,61 +28,64 @@
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: bench
 Provides-Extra: dev
 License-File: LICENSE.txt
+License-File: AUTHORS
 
 # Official Nextcloud Python Framework
 
 [![Analysis & Coverage](https://github.com/cloud-py-api/nc_py_api/actions/workflows/analysis-coverage.yml/badge.svg)](https://github.com/cloud-py-api/nc_py_api/actions/workflows/analysis-coverage.yml)
 [![Docs](https://github.com/cloud-py-api/nc_py_api/actions/workflows/docs.yml/badge.svg)](https://cloud-py-api.github.io/nc_py_api/)
 [![codecov](https://codecov.io/github/cloud-py-api/nc_py_api/branch/main/graph/badge.svg?token=C91PL3FYDQ)](https://codecov.io/github/cloud-py-api/nc_py_api)
 
 ![NextcloudVersion](https://img.shields.io/badge/Nextcloud-26%20%7C%2027%20%7C%2028-blue)
 ![PythonVersion](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue)
 ![impl](https://img.shields.io/pypi/implementation/nc_py_api)
 ![pypi](https://img.shields.io/pypi/v/nc_py_api.svg)
 
-### Remark
-
-Project cloud-py-api was **abandoned** and divided into two parts:
- * `nc_py_api` - this repository, which contains Python Framework to work with Nextcloud and `app_ecosystem_v2`
- * `app_ecosystem_v2` - New [Nextcloud Application Ecosystem](https://github.com/cloud-py-api/app_ecosystem_v2) that allows writing applications for Nextcloud in any language
-
-**_Projects stage: under heavy prototyping and developing_**
+Python library that provides a robust and well-documented API that allows developers to interact with and extend Nextcloud's functionality.
 
 ### Basic Features:
- * Listing, enabling and disabling of the applications
  * Operations with Files and Folders
  * ~~Operations with Trash bin and File versions~~
  * Operations with Users and User Groups
- * User status manipulation
+ * User status
  * Weather status
  * ~~Nextcloud notifications support~~
- * ~~Shares operations support~~
+ * Shares support
  * ~~Talk support~~
 
-### Extended Features with installed App_ecosystem_v2:
- * Defining callback routes with FastAPI for Nextcloud
+### Extended Features with AppEcosystemV2:
+ * Defining callback routes with `FastAPI` for Nextcloud
  * Registering UI elements in Nextcloud
  * Storing logs to the `nextcloud.log` file
  * Get/save key-value pairs in AppConfigEx/PreferencesEx tables.
  * **Tons of the cool stuff that is coming soon**
 
+### Support
+
+You can support us in several ways:
+
+- ⭐️ Star our work (it really motivates)
+- ❗️ Create an Issue or feature request (bring to us an excellent idea)
+- 💁 Resolve some Issue or create a Pull Request (contribute to this project)
+- 🙏 Write an example of its use or correct a typo in the documentation.
+
 ### 🚀 How to start
 
-In very close near future we will publish examples
+In a very close near future we will publish examples
 
 ### More Information
 
-- [Documentation](https://nc_py_api.readthedocs.io/)
+- [Documentation](https://cloud-py-api.github.io/nc_py_api/)
   - [Using it as a simple client](to-do)
   - [Writing a simple Nextcloud application](to-do)
-  - [Writing a Nextcloud system application](to-do)
+  - [Writing a Nextcloud System Application](to-do)
 - [Examples](https://github.com/cloud-py-api/nc_py_api/tree/main/examples)
 - [Contribute](https://github.com/cloud-py-api/nc_py_api/blob/main/.github/CONTRIBUTING.md)
   - [Discussions](https://github.com/cloud-py-api/nc_py_api/discussions)
   - [Issues](https://github.com/cloud-py-api/nc_py_api/issues)
   - [Setting up dev environment](to-do)
 - [Changelog](https://github.com/cloud-py-api/nc_py_api/blob/main/CHANGELOG.md)
```

### Comparing `nc_py_api-0.0.24/nc_py_api.egg-info/SOURCES.txt` & `nc_py_api-0.0.25/nc_py_api.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+AUTHORS
 CHANGELOG.md
 LICENSE.txt
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
@@ -9,14 +10,15 @@
 nc_py_api/_session.py
 nc_py_api/_version.py
 nc_py_api/appconfig_preferences_ex.py
 nc_py_api/apps.py
 nc_py_api/constants.py
 nc_py_api/exceptions.py
 nc_py_api/files.py
+nc_py_api/files_sharing.py
 nc_py_api/integration_fastapi.py
 nc_py_api/misc.py
 nc_py_api/nextcloud.py
 nc_py_api/options.py
 nc_py_api/preferences.py
 nc_py_api/theming.py
 nc_py_api/ui_files_actions_menu.py
```

### Comparing `nc_py_api-0.0.24/pyproject.toml` & `nc_py_api-0.0.25/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [build-system]
 requires = [
-  "setuptools>=60",
+  "setuptools>=67.8",
   "wheel",
 ]
 
 [tool.black]
 line-length = 120
 target-versions = ["py39"]
 preview = true
```

### Comparing `nc_py_api-0.0.24/setup.cfg` & `nc_py_api-0.0.25/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -37,33 +37,34 @@
 install_requires = 
 	requests==2.31.0
 	httpx==0.24.1
 	xmltodict==0.13.0
 	pydantic==2.0.3
 	xxhash==3.2.0
 	fastapi==0.100.0
+	uvicorn[standard]==0.23.1
 
 [options.extras_require]
 docs = 
 	sphinx>=4.4
 	sphinx-issues>=3.0.1
 	sphinx-rtd-theme>=1.0
 	sphinx-copybutton
 	sphinx-inline-tabs
 bench = 
 	matplotlib
 	py-cpuinfo
 	numpy
 dev = 
+	selenium
 	pytest
 	pre-commit
 	pylint
 	coverage
 	pillow
-	uvicorn
 
 [flake8]
 max-line-length = 120
 target-version = ["py39"]
 ignore = 
 	E203,
 	W503,
```

