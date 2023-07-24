# Comparing `tmp/zeroconf-0.71.3.tar.gz` & `tmp/zeroconf-0.71.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeroconf-0.71.3.tar", max compression
+gzip compressed data, was "zeroconf-0.71.4.tar", max compression
```

## Comparing `zeroconf-0.71.3.tar` & `zeroconf-0.71.4.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0    55836 2023-07-23 23:24:05.566950 zeroconf-0.71.3/CHANGELOG.md
--rw-r--r--   0        0        0    24380 2023-07-23 23:24:04.762946 zeroconf-0.71.3/COPYING
--rw-r--r--   0        0        0     4407 2023-07-23 23:24:04.762946 zeroconf-0.71.3/README.rst
--rw-r--r--   0        0        0     1060 2023-07-23 23:24:04.762946 zeroconf-0.71.3/build_ext.py
--rw-r--r--   0        0        0     6770 2023-07-23 23:24:04.762946 zeroconf-0.71.3/docs/Makefile
--rw-r--r--   0        0        0      234 2023-07-23 23:24:04.762946 zeroconf-0.71.3/docs/api.rst
--rw-r--r--   0        0        0     8145 2023-07-23 23:24:04.762946 zeroconf-0.71.3/docs/conf.py
--rw-r--r--   0        0        0      991 2023-07-23 23:24:04.762946 zeroconf-0.71.3/docs/index.rst
--rw-r--r--   0        0        0     3995 2023-07-23 23:24:05.642951 zeroconf-0.71.3/pyproject.toml
--rw-r--r--   0        0        0     3868 2023-07-23 23:24:05.574951 zeroconf-0.71.3/src/zeroconf/__init__.py
--rw-r--r--   0        0        0      897 2023-07-23 23:24:04.762946 zeroconf-0.71.3/src/zeroconf/_cache.pxd
--rw-r--r--   0        0        0    10040 2023-07-23 23:24:04.762946 zeroconf-0.71.3/src/zeroconf/_cache.py
--rw-r--r--   0        0        0    39600 2023-07-23 23:24:04.766946 zeroconf-0.71.3/src/zeroconf/_core.py
--rw-r--r--   0        0        0     2119 2023-07-23 23:24:04.766946 zeroconf-0.71.3/src/zeroconf/_dns.pxd
--rw-r--r--   0        0        0    18270 2023-07-23 23:24:04.766946 zeroconf-0.71.3/src/zeroconf/_dns.py
--rw-r--r--   0        0        0     2167 2023-07-23 23:24:04.766946 zeroconf-0.71.3/src/zeroconf/_exceptions.py
--rw-r--r--   0        0        0    24697 2023-07-23 23:24:04.766946 zeroconf-0.71.3/src/zeroconf/_handlers.py
--rw-r--r--   0        0        0     2916 2023-07-23 23:24:04.766946 zeroconf-0.71.3/src/zeroconf/_history.py
--rw-r--r--   0        0        0     2980 2023-07-23 23:24:04.766946 zeroconf-0.71.3/src/zeroconf/_logger.py
--rw-r--r--   0        0        0      971 2023-07-23 23:24:04.766946 zeroconf-0.71.3/src/zeroconf/_protocol/__init__.py
--rw-r--r--   0        0        0     2661 2023-07-23 23:24:04.766946 zeroconf-0.71.3/src/zeroconf/_protocol/incoming.pxd
--rw-r--r--   0        0        0    14353 2023-07-23 23:24:04.766946 zeroconf-0.71.3/src/zeroconf/_protocol/incoming.py
--rw-r--r--   0        0        0     2317 2023-07-23 23:24:04.766946 zeroconf-0.71.3/src/zeroconf/_protocol/outgoing.pxd
--rw-r--r--   0        0        0    17896 2023-07-23 23:24:04.766946 zeroconf-0.71.3/src/zeroconf/_protocol/outgoing.py
--rw-r--r--   0        0        0     2421 2023-07-23 23:24:04.766946 zeroconf-0.71.3/src/zeroconf/_services/__init__.py
--rw-r--r--   0        0        0    23045 2023-07-23 23:24:04.766946 zeroconf-0.71.3/src/zeroconf/_services/browser.py
--rw-r--r--   0        0        0    27815 2023-07-23 23:24:04.766946 zeroconf-0.71.3/src/zeroconf/_services/info.py
--rw-r--r--   0        0        0     3999 2023-07-23 23:24:04.766946 zeroconf-0.71.3/src/zeroconf/_services/registry.py
--rw-r--r--   0        0        0     3003 2023-07-23 23:24:04.766946 zeroconf-0.71.3/src/zeroconf/_services/types.py
--rw-r--r--   0        0        0     2909 2023-07-23 23:24:04.766946 zeroconf-0.71.3/src/zeroconf/_updates.py
--rw-r--r--   0        0        0      971 2023-07-23 23:24:04.766946 zeroconf-0.71.3/src/zeroconf/_utils/__init__.py
--rw-r--r--   0        0        0     4144 2023-07-23 23:24:04.766946 zeroconf-0.71.3/src/zeroconf/_utils/asyncio.py
--rw-r--r--   0        0        0     6904 2023-07-23 23:24:04.766946 zeroconf-0.71.3/src/zeroconf/_utils/name.py
--rw-r--r--   0        0        0    15252 2023-07-23 23:24:04.766946 zeroconf-0.71.3/src/zeroconf/_utils/net.py
--rw-r--r--   0        0        0     1308 2023-07-23 23:24:04.766946 zeroconf-0.71.3/src/zeroconf/_utils/time.py
--rw-r--r--   0        0        0    11084 2023-07-23 23:24:04.766946 zeroconf-0.71.3/src/zeroconf/asyncio.py
--rw-r--r--   0        0        0     4515 2023-07-23 23:24:04.766946 zeroconf-0.71.3/src/zeroconf/const.py
--rw-r--r--   0        0        0        0 2023-07-23 23:24:04.766946 zeroconf-0.71.3/src/zeroconf/py.typed
--rw-r--r--   0        0        0     2416 2023-07-23 23:24:04.766946 zeroconf-0.71.3/tests/__init__.py
--rw-r--r--   0        0        0     1057 2023-07-23 23:24:04.766946 zeroconf-0.71.3/tests/conftest.py
--rw-r--r--   0        0        0      971 2023-07-23 23:24:04.766946 zeroconf-0.71.3/tests/services/__init__.py
--rw-r--r--   0        0        0    42949 2023-07-23 23:24:04.766946 zeroconf-0.71.3/tests/services/test_browser.py
--rw-r--r--   0        0        0    47563 2023-07-23 23:24:04.766946 zeroconf-0.71.3/tests/services/test_info.py
--rw-r--r--   0        0        0     4157 2023-07-23 23:24:04.766946 zeroconf-0.71.3/tests/services/test_registry.py
--rw-r--r--   0        0        0     4681 2023-07-23 23:24:04.766946 zeroconf-0.71.3/tests/services/test_types.py
--rw-r--r--   0        0        0    44525 2023-07-23 23:24:04.766946 zeroconf-0.71.3/tests/test_asyncio.py
--rw-r--r--   0        0        0     8830 2023-07-23 23:24:04.766946 zeroconf-0.71.3/tests/test_cache.py
--rw-r--r--   0        0        0    32599 2023-07-23 23:24:04.766946 zeroconf-0.71.3/tests/test_core.py
--rw-r--r--   0        0        0    14686 2023-07-23 23:24:04.766946 zeroconf-0.71.3/tests/test_dns.py
--rw-r--r--   0        0        0     5021 2023-07-23 23:24:04.766946 zeroconf-0.71.3/tests/test_exceptions.py
--rw-r--r--   0        0        0    67411 2023-07-23 23:24:04.770946 zeroconf-0.71.3/tests/test_handlers.py
--rw-r--r--   0        0        0     2580 2023-07-23 23:24:04.770946 zeroconf-0.71.3/tests/test_history.py
--rw-r--r--   0        0        0     6640 2023-07-23 23:24:04.770946 zeroconf-0.71.3/tests/test_init.py
--rw-r--r--   0        0        0     3396 2023-07-23 23:24:04.770946 zeroconf-0.71.3/tests/test_logger.py
--rw-r--r--   0        0        0    41672 2023-07-23 23:24:04.770946 zeroconf-0.71.3/tests/test_protocol.py
--rw-r--r--   0        0        0     8849 2023-07-23 23:24:04.770946 zeroconf-0.71.3/tests/test_services.py
--rw-r--r--   0        0        0     2240 2023-07-23 23:24:04.770946 zeroconf-0.71.3/tests/test_updates.py
--rw-r--r--   0        0        0      971 2023-07-23 23:24:04.770946 zeroconf-0.71.3/tests/utils/__init__.py
--rw-r--r--   0        0        0     5101 2023-07-23 23:24:04.770946 zeroconf-0.71.3/tests/utils/test_asyncio.py
--rw-r--r--   0        0        0     2045 2023-07-23 23:24:04.770946 zeroconf-0.71.3/tests/utils/test_name.py
--rw-r--r--   0        0        0     9413 2023-07-23 23:24:04.770946 zeroconf-0.71.3/tests/utils/test_net.py
--rw-r--r--   0        0        0     5527 1970-01-01 00:00:00.000000 zeroconf-0.71.3/setup.py
--rw-r--r--   0        0        0     6045 1970-01-01 00:00:00.000000 zeroconf-0.71.3/PKG-INFO
+-rw-r--r--   0        0        0    56117 2023-07-24 16:13:08.265268 zeroconf-0.71.4/CHANGELOG.md
+-rw-r--r--   0        0        0    24380 2023-07-24 16:13:07.129202 zeroconf-0.71.4/COPYING
+-rw-r--r--   0        0        0     4407 2023-07-24 16:13:07.129202 zeroconf-0.71.4/README.rst
+-rw-r--r--   0        0        0     1060 2023-07-24 16:13:07.129202 zeroconf-0.71.4/build_ext.py
+-rw-r--r--   0        0        0     6770 2023-07-24 16:13:07.129202 zeroconf-0.71.4/docs/Makefile
+-rw-r--r--   0        0        0      234 2023-07-24 16:13:07.129202 zeroconf-0.71.4/docs/api.rst
+-rw-r--r--   0        0        0     8145 2023-07-24 16:13:07.129202 zeroconf-0.71.4/docs/conf.py
+-rw-r--r--   0        0        0      991 2023-07-24 16:13:07.129202 zeroconf-0.71.4/docs/index.rst
+-rw-r--r--   0        0        0     3995 2023-07-24 16:13:08.365274 zeroconf-0.71.4/pyproject.toml
+-rw-r--r--   0        0        0     3868 2023-07-24 16:13:08.281269 zeroconf-0.71.4/src/zeroconf/__init__.py
+-rw-r--r--   0        0        0      897 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_cache.pxd
+-rw-r--r--   0        0        0    10040 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_cache.py
+-rw-r--r--   0        0        0    39600 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_core.py
+-rw-r--r--   0        0        0     2119 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_dns.pxd
+-rw-r--r--   0        0        0    18270 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_dns.py
+-rw-r--r--   0        0        0     2167 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_exceptions.py
+-rw-r--r--   0        0        0    24697 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_handlers.py
+-rw-r--r--   0        0        0     2916 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_history.py
+-rw-r--r--   0        0        0     2980 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_logger.py
+-rw-r--r--   0        0        0      971 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_protocol/__init__.py
+-rw-r--r--   0        0        0     2661 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_protocol/incoming.pxd
+-rw-r--r--   0        0        0    14353 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_protocol/incoming.py
+-rw-r--r--   0        0        0     2317 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_protocol/outgoing.pxd
+-rw-r--r--   0        0        0    17896 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_protocol/outgoing.py
+-rw-r--r--   0        0        0     2419 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_services/__init__.py
+-rw-r--r--   0        0        0    23045 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_services/browser.py
+-rw-r--r--   0        0        0    27841 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_services/info.py
+-rw-r--r--   0        0        0     3999 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_services/registry.py
+-rw-r--r--   0        0        0     3003 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_services/types.py
+-rw-r--r--   0        0        0     2909 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_updates.py
+-rw-r--r--   0        0        0      971 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_utils/__init__.py
+-rw-r--r--   0        0        0     4144 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_utils/asyncio.py
+-rw-r--r--   0        0        0     6904 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_utils/name.py
+-rw-r--r--   0        0        0    15252 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_utils/net.py
+-rw-r--r--   0        0        0     1308 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_utils/time.py
+-rw-r--r--   0        0        0    11084 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/asyncio.py
+-rw-r--r--   0        0        0     4515 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/const.py
+-rw-r--r--   0        0        0        0 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/py.typed
+-rw-r--r--   0        0        0     2416 2023-07-24 16:13:07.133203 zeroconf-0.71.4/tests/__init__.py
+-rw-r--r--   0        0        0     1057 2023-07-24 16:13:07.133203 zeroconf-0.71.4/tests/conftest.py
+-rw-r--r--   0        0        0      971 2023-07-24 16:13:07.137203 zeroconf-0.71.4/tests/services/__init__.py
+-rw-r--r--   0        0        0    42949 2023-07-24 16:13:07.137203 zeroconf-0.71.4/tests/services/test_browser.py
+-rw-r--r--   0        0        0    47563 2023-07-24 16:13:07.137203 zeroconf-0.71.4/tests/services/test_info.py
+-rw-r--r--   0        0        0     4157 2023-07-24 16:13:07.137203 zeroconf-0.71.4/tests/services/test_registry.py
+-rw-r--r--   0        0        0     4681 2023-07-24 16:13:07.137203 zeroconf-0.71.4/tests/services/test_types.py
+-rw-r--r--   0        0        0    44525 2023-07-24 16:13:07.137203 zeroconf-0.71.4/tests/test_asyncio.py
+-rw-r--r--   0        0        0     8830 2023-07-24 16:13:07.137203 zeroconf-0.71.4/tests/test_cache.py
+-rw-r--r--   0        0        0    32599 2023-07-24 16:13:07.137203 zeroconf-0.71.4/tests/test_core.py
+-rw-r--r--   0        0        0    14686 2023-07-24 16:13:07.137203 zeroconf-0.71.4/tests/test_dns.py
+-rw-r--r--   0        0        0     5021 2023-07-24 16:13:07.137203 zeroconf-0.71.4/tests/test_exceptions.py
+-rw-r--r--   0        0        0    67411 2023-07-24 16:13:07.137203 zeroconf-0.71.4/tests/test_handlers.py
+-rw-r--r--   0        0        0     2580 2023-07-24 16:13:07.137203 zeroconf-0.71.4/tests/test_history.py
+-rw-r--r--   0        0        0     6640 2023-07-24 16:13:07.137203 zeroconf-0.71.4/tests/test_init.py
+-rw-r--r--   0        0        0     3396 2023-07-24 16:13:07.137203 zeroconf-0.71.4/tests/test_logger.py
+-rw-r--r--   0        0        0    41672 2023-07-24 16:13:07.137203 zeroconf-0.71.4/tests/test_protocol.py
+-rw-r--r--   0        0        0     8849 2023-07-24 16:13:07.137203 zeroconf-0.71.4/tests/test_services.py
+-rw-r--r--   0        0        0     2240 2023-07-24 16:13:07.137203 zeroconf-0.71.4/tests/test_updates.py
+-rw-r--r--   0        0        0      971 2023-07-24 16:13:07.137203 zeroconf-0.71.4/tests/utils/__init__.py
+-rw-r--r--   0        0        0     5101 2023-07-24 16:13:07.137203 zeroconf-0.71.4/tests/utils/test_asyncio.py
+-rw-r--r--   0        0        0     2045 2023-07-24 16:13:07.137203 zeroconf-0.71.4/tests/utils/test_name.py
+-rw-r--r--   0        0        0     9413 2023-07-24 16:13:07.137203 zeroconf-0.71.4/tests/utils/test_net.py
+-rw-r--r--   0        0        0     5527 1970-01-01 00:00:00.000000 zeroconf-0.71.4/setup.py
+-rw-r--r--   0        0        0     6045 1970-01-01 00:00:00.000000 zeroconf-0.71.4/PKG-INFO
```

### Comparing `zeroconf-0.71.3/CHANGELOG.md` & `zeroconf-0.71.4/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.71.4 (2023-07-24)
+
+### Fix
+
+* Cleanup naming from previous refactoring in ServiceInfo ([#1202](https://github.com/python-zeroconf/python-zeroconf/issues/1202)) ([`b272d75`](https://github.com/python-zeroconf/python-zeroconf/commit/b272d75abd982f3be1f4b20f683cac38011cc6f4))
+
 ## v0.71.3 (2023-07-23)
 
 ### Fix
 
 * Pin python-semantic-release to fix release process ([#1200](https://github.com/python-zeroconf/python-zeroconf/issues/1200)) ([`c145a23`](https://github.com/python-zeroconf/python-zeroconf/commit/c145a238d768aa17c3aebe120c20a46bfbec6b99))
 
 ## v0.71.2 (2023-07-23)
```

### Comparing `zeroconf-0.71.3/COPYING` & `zeroconf-0.71.4/COPYING`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/README.rst` & `zeroconf-0.71.4/README.rst`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/build_ext.py` & `zeroconf-0.71.4/build_ext.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/docs/Makefile` & `zeroconf-0.71.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/docs/conf.py` & `zeroconf-0.71.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/docs/index.rst` & `zeroconf-0.71.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/pyproject.toml` & `zeroconf-0.71.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zeroconf"
-version = "0.71.3"
+version = "0.71.4"
 description = "A pure python implementation of multicast DNS service discovery"
 authors = ["Paul Scott-Murphy", "William McBrine", "Jakub Stasiak", "J. Nick Koston"]
 license = "LGPL"
 readme = "README.rst"
 repository = "https://github.com/python-zeroconf/python-zeroconf"
 documentation = "https://python-zeroconf.readthedocs.io"
 classifiers=[
```

### Comparing `zeroconf-0.71.3/src/zeroconf/__init__.py` & `zeroconf-0.71.4/src/zeroconf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 from ._utils.time import (  # noqa # import needed for backwards compat
     current_time_millis,
     millis_to_seconds,
 )
 
 __author__ = 'Paul Scott-Murphy, William McBrine'
 __maintainer__ = 'Jakub Stasiak <jakub@stasiak.at>'
-__version__ = '0.71.3'
+__version__ = '0.71.4'
 __license__ = 'LGPL'
 
 
 __all__ = [
     "__version__",
     "Zeroconf",
     "ServiceInfo",
```

### Comparing `zeroconf-0.71.3/src/zeroconf/_cache.pxd` & `zeroconf-0.71.4/src/zeroconf/_cache.pxd`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/src/zeroconf/_cache.py` & `zeroconf-0.71.4/src/zeroconf/_cache.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/src/zeroconf/_core.py` & `zeroconf-0.71.4/src/zeroconf/_core.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/src/zeroconf/_dns.pxd` & `zeroconf-0.71.4/src/zeroconf/_dns.pxd`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/src/zeroconf/_dns.py` & `zeroconf-0.71.4/src/zeroconf/_dns.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/src/zeroconf/_exceptions.py` & `zeroconf-0.71.4/src/zeroconf/_exceptions.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/src/zeroconf/_handlers.py` & `zeroconf-0.71.4/src/zeroconf/_handlers.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/src/zeroconf/_history.py` & `zeroconf-0.71.4/src/zeroconf/_history.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/src/zeroconf/_logger.py` & `zeroconf-0.71.4/src/zeroconf/_logger.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/src/zeroconf/_protocol/__init__.py` & `zeroconf-0.71.4/src/zeroconf/_protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/src/zeroconf/_protocol/incoming.pxd` & `zeroconf-0.71.4/src/zeroconf/_protocol/incoming.pxd`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/src/zeroconf/_protocol/incoming.py` & `zeroconf-0.71.4/src/zeroconf/_protocol/incoming.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/src/zeroconf/_protocol/outgoing.pxd` & `zeroconf-0.71.4/src/zeroconf/_protocol/outgoing.pxd`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/src/zeroconf/_protocol/outgoing.py` & `zeroconf-0.71.4/src/zeroconf/_protocol/outgoing.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/src/zeroconf/_services/__init__.py` & `zeroconf-0.71.4/src/zeroconf/_services/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,14 @@
         raise NotImplementedError()
 
     def update_service(self, zc: 'Zeroconf', type_: str, name: str) -> None:
         raise NotImplementedError()
 
 
 class Signal:
-
     __slots__ = ('_handlers',)
 
     def __init__(self) -> None:
         self._handlers: List[Callable[..., None]] = []
 
     def fire(self, **kwargs: Any) -> None:
         for h in self._handlers[:]:
@@ -58,15 +57,14 @@
 
     @property
     def registration_interface(self) -> 'SignalRegistrationInterface':
         return SignalRegistrationInterface(self._handlers)
 
 
 class SignalRegistrationInterface:
-
     __slots__ = ('_handlers',)
 
     def __init__(self, handlers: List[Callable[..., None]]) -> None:
         self._handlers = handlers
 
     def register_handler(self, handler: Callable[..., None]) -> 'SignalRegistrationInterface':
         self._handlers.append(handler)
```

### Comparing `zeroconf-0.71.3/src/zeroconf/_services/browser.py` & `zeroconf-0.71.4/src/zeroconf/_services/browser.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/src/zeroconf/_services/info.py` & `zeroconf-0.71.4/src/zeroconf/_services/info.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,17 +17,17 @@
     You should have received a copy of the GNU Lesser General Public
     License along with this library; if not, write to the Free Software
     Foundation, Inc., 51 Franklin St, Fifth Floor, Boston, MA 02110-1301
     USA
 """
 
 import asyncio
-import ipaddress
 import random
 from functools import lru_cache
+from ipaddress import IPv4Address, IPv6Address, _BaseAddress, ip_address
 from typing import TYPE_CHECKING, Dict, List, Optional, Set, Union, cast
 
 from .._dns import (
     DNSAddress,
     DNSNsec,
     DNSPointer,
     DNSQuestionType,
@@ -86,15 +86,15 @@
     # need to make subtypes a first class citizen
     service_name = service_type_name(info.name)
     if not info.type.endswith(service_name):
         raise BadTypeInNameException
     return info.name[: -len(service_name) - 1]
 
 
-_cached_ip_addresses = lru_cache(maxsize=256)(ipaddress.ip_address)
+_cached_ip_addresses = lru_cache(maxsize=256)(ip_address)
 
 
 class ServiceInfo(RecordUpdateListener):
     """Service information.
 
     Constructor parameters are as follows:
 
@@ -154,16 +154,16 @@
             raise TypeError("addresses and parsed_addresses cannot be provided together")
         if not type_.endswith(service_type_name(name, strict=False)):
             raise BadTypeInNameException
         self.text = b''
         self.type = type_
         self._name = name
         self.key = name.lower()
-        self._ipv4_addresses: List[ipaddress.IPv4Address] = []
-        self._ipv6_addresses: List[ipaddress.IPv6Address] = []
+        self._ipv4_addresses: List[IPv4Address] = []
+        self._ipv6_addresses: List[IPv6Address] = []
         if addresses is not None:
             self.addresses = addresses
         elif parsed_addresses is not None:
             self.addresses = [_encode_address(a) for a in parsed_addresses]
         self.port = port
         self.weight = weight
         self.priority = priority
@@ -256,28 +256,28 @@
             ]
         if version_value == _IPVersion_V4Only_value:
             return [addr.packed for addr in self._ipv4_addresses]
         return [addr.packed for addr in self._ipv6_addresses]
 
     def ip_addresses_by_version(
         self, version: IPVersion
-    ) -> Union[List[ipaddress.IPv4Address], List[ipaddress.IPv6Address], List[ipaddress._BaseAddress]]:
+    ) -> Union[List[IPv4Address], List[IPv6Address], List[_BaseAddress]]:
         """List ip_address objects matching IP version.
 
         Addresses are guaranteed to be returned in LIFO (last in, first out)
         order with IPv4 addresses first and IPv6 addresses second.
 
         This means the first address will always be the most recently added
         address of the given IP version.
         """
         return self._ip_addresses_by_version_value(version.value)
 
     def _ip_addresses_by_version_value(
         self, version_value: int
-    ) -> Union[List[ipaddress.IPv4Address], List[ipaddress.IPv6Address], List[ipaddress._BaseAddress]]:
+    ) -> Union[List[IPv4Address], List[IPv6Address], List[_BaseAddress]]:
         """Backend for addresses_by_version that uses the raw value."""
         if version_value == _IPVersion_All_value:
             return [*self._ipv4_addresses, *self._ipv6_addresses]
         if version_value == _IPVersion_V4Only_value:
             return self._ipv4_addresses
         return self._ipv6_addresses
 
@@ -362,39 +362,39 @@
 
     def get_name(self) -> str:
         """Name accessor"""
         return self.name[: len(self.name) - len(self.type) - 1]
 
     def _get_ip_addresses_from_cache_lifo(
         self, zc: 'Zeroconf', now: float, type: int
-    ) -> List[Union[ipaddress.IPv4Address, ipaddress.IPv6Address]]:
+    ) -> List[Union[IPv4Address, IPv6Address]]:
         """Set IPv6 addresses from the cache."""
-        address_list: List[Union[ipaddress.IPv4Address, ipaddress.IPv6Address]] = []
+        address_list: List[Union[IPv4Address, IPv6Address]] = []
         for record in self._get_address_records_from_cache_by_type(zc, type):
             if record.is_expired(now):
                 continue
             try:
-                ip_address = _cached_ip_addresses(record.address)
+                ip_addr = _cached_ip_addresses(record.address)
             except ValueError:
                 continue
             else:
-                address_list.append(ip_address)
+                address_list.append(ip_addr)
         address_list.reverse()  # Reverse to get LIFO order
         return address_list
 
     def _set_ipv6_addresses_from_cache(self, zc: 'Zeroconf', now: float) -> None:
         """Set IPv6 addresses from the cache."""
         self._ipv6_addresses = cast(
-            "List[ipaddress.IPv6Address]", self._get_ip_addresses_from_cache_lifo(zc, now, _TYPE_AAAA)
+            "List[IPv6Address]", self._get_ip_addresses_from_cache_lifo(zc, now, _TYPE_AAAA)
         )
 
     def _set_ipv4_addresses_from_cache(self, zc: 'Zeroconf', now: float) -> None:
         """Set IPv4 addresses from the cache."""
         self._ipv4_addresses = cast(
-            "List[ipaddress.IPv4Address]", self._get_ip_addresses_from_cache_lifo(zc, now, _TYPE_A)
+            "List[IPv4Address]", self._get_ip_addresses_from_cache_lifo(zc, now, _TYPE_A)
         )
 
     def update_record(self, zc: 'Zeroconf', now: float, record: Optional[DNSRecord]) -> None:
         """Updates service information from a DNS record.
 
         This method is deprecated and will be removed in a future version.
         update_records should be implemented instead.
@@ -427,54 +427,57 @@
         """Thread safe record updating.
 
         Returns True if a new record was added.
         """
         if record.is_expired(now):
             return False
 
-        if record.key == self.server_key and isinstance(record, DNSAddress):
+        record_key = record.key
+        if record_key == self.server_key and type(record) is DNSAddress:
             try:
                 ip_addr = _cached_ip_addresses(record.address)
             except ValueError as ex:
                 log.warning("Encountered invalid address while processing %s: %s", record, ex)
                 return False
 
-            if ip_addr.version == 4:
-                if not self._ipv4_addresses:
+            if type(ip_addr) is IPv4Address:
+                if self._ipv4_addresses:
                     self._set_ipv4_addresses_from_cache(zc, now)
 
-                if ip_addr not in self._ipv4_addresses:
-                    self._ipv4_addresses.insert(0, ip_addr)
+                ipv4_addresses = self._ipv4_addresses
+                if ip_addr not in ipv4_addresses:
+                    ipv4_addresses.insert(0, ip_addr)
                     return True
-                elif ip_addr != self._ipv4_addresses[0]:
-                    self._ipv4_addresses.remove(ip_addr)
-                    self._ipv4_addresses.insert(0, ip_addr)
+                elif ip_addr != ipv4_addresses[0]:
+                    ipv4_addresses.remove(ip_addr)
+                    ipv4_addresses.insert(0, ip_addr)
 
                 return False
 
             if not self._ipv6_addresses:
                 self._set_ipv6_addresses_from_cache(zc, now)
 
+            ipv6_addresses = self._ipv6_addresses
             if ip_addr not in self._ipv6_addresses:
-                self._ipv6_addresses.insert(0, ip_addr)
+                ipv6_addresses.insert(0, ip_addr)
                 return True
             elif ip_addr != self._ipv6_addresses[0]:
-                self._ipv6_addresses.remove(ip_addr)
-                self._ipv6_addresses.insert(0, ip_addr)
+                ipv6_addresses.remove(ip_addr)
+                ipv6_addresses.insert(0, ip_addr)
 
             return False
 
-        if record.key != self.key:
+        if record_key != self.key:
             return False
 
-        if record.type == _TYPE_TXT and isinstance(record, DNSText):
+        if record.type == _TYPE_TXT and type(record) is DNSText:
             self._set_text(record.text)
             return True
 
-        if record.type == _TYPE_SRV and isinstance(record, DNSService):
+        if record.type == _TYPE_SRV and type(record) is DNSService:
             old_server_key = self.server_key
             self.name = record.name
             self.server = record.server
             self.server_key = record.server.lower()
             self.port = record.port
             self.weight = record.weight
             self.priority = record.priority
@@ -491,24 +494,25 @@
         version: IPVersion = IPVersion.All,
         created: Optional[float] = None,
     ) -> List[DNSAddress]:
         """Return matching DNSAddress from ServiceInfo."""
         name = self.server or self.name
         ttl = override_ttl if override_ttl is not None else self.host_ttl
         class_ = _CLASS_IN | _CLASS_UNIQUE
+        version_value = version.value
         return [
             DNSAddress(
                 name,
-                _TYPE_AAAA if address.version == 6 else _TYPE_A,
+                _TYPE_AAAA if type(ip_addr) is IPv6Address else _TYPE_A,
                 class_,
                 ttl,
-                address.packed,
+                ip_addr.packed,
                 created=created,
             )
-            for address in self._ip_addresses_by_version_value(version.value)
+            for ip_addr in self._ip_addresses_by_version_value(version_value)
         ]
 
     def dns_pointer(self, override_ttl: Optional[int] = None, created: Optional[float] = None) -> DNSPointer:
         """Return DNSPointer from ServiceInfo."""
         return DNSPointer(
             self.type,
             _TYPE_PTR,
```

### Comparing `zeroconf-0.71.3/src/zeroconf/_services/registry.py` & `zeroconf-0.71.4/src/zeroconf/_services/registry.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/src/zeroconf/_services/types.py` & `zeroconf-0.71.4/src/zeroconf/_services/types.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/src/zeroconf/_updates.py` & `zeroconf-0.71.4/src/zeroconf/_updates.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/src/zeroconf/_utils/__init__.py` & `zeroconf-0.71.4/src/zeroconf/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/src/zeroconf/_utils/asyncio.py` & `zeroconf-0.71.4/src/zeroconf/_utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/src/zeroconf/_utils/name.py` & `zeroconf-0.71.4/src/zeroconf/_utils/name.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/src/zeroconf/_utils/net.py` & `zeroconf-0.71.4/src/zeroconf/_utils/net.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/src/zeroconf/_utils/time.py` & `zeroconf-0.71.4/src/zeroconf/_utils/time.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/src/zeroconf/asyncio.py` & `zeroconf-0.71.4/src/zeroconf/asyncio.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/src/zeroconf/const.py` & `zeroconf-0.71.4/src/zeroconf/const.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/tests/__init__.py` & `zeroconf-0.71.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/tests/conftest.py` & `zeroconf-0.71.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/tests/services/__init__.py` & `zeroconf-0.71.4/tests/services/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/tests/services/test_browser.py` & `zeroconf-0.71.4/tests/services/test_browser.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/tests/services/test_info.py` & `zeroconf-0.71.4/tests/services/test_info.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/tests/services/test_registry.py` & `zeroconf-0.71.4/tests/services/test_registry.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/tests/services/test_types.py` & `zeroconf-0.71.4/tests/services/test_types.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/tests/test_asyncio.py` & `zeroconf-0.71.4/tests/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/tests/test_cache.py` & `zeroconf-0.71.4/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/tests/test_core.py` & `zeroconf-0.71.4/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/tests/test_dns.py` & `zeroconf-0.71.4/tests/test_dns.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/tests/test_exceptions.py` & `zeroconf-0.71.4/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/tests/test_handlers.py` & `zeroconf-0.71.4/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/tests/test_history.py` & `zeroconf-0.71.4/tests/test_history.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/tests/test_init.py` & `zeroconf-0.71.4/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/tests/test_logger.py` & `zeroconf-0.71.4/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/tests/test_protocol.py` & `zeroconf-0.71.4/tests/test_protocol.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/tests/test_services.py` & `zeroconf-0.71.4/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/tests/test_updates.py` & `zeroconf-0.71.4/tests/test_updates.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/tests/utils/__init__.py` & `zeroconf-0.71.4/tests/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/tests/utils/test_asyncio.py` & `zeroconf-0.71.4/tests/utils/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/tests/utils/test_name.py` & `zeroconf-0.71.4/tests/utils/test_name.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/tests/utils/test_net.py` & `zeroconf-0.71.4/tests/utils/test_net.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.3/setup.py` & `zeroconf-0.71.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['ifaddr>=0.1.7']
 
 extras_require = \
 {':python_version < "3.11"': ['async-timeout>=3.0.0']}
 
 setup_kwargs = {
     'name': 'zeroconf',
-    'version': '0.71.3',
+    'version': '0.71.4',
     'description': 'A pure python implementation of multicast DNS service discovery',
     'long_description': 'python-zeroconf\n===============\n\n.. image:: https://github.com/python-zeroconf/python-zeroconf/workflows/CI/badge.svg\n   :target: https://github.com/python-zeroconf/python-zeroconf?query=workflow%3ACI+branch%3Amaster\n\n.. image:: https://img.shields.io/pypi/v/zeroconf.svg\n    :target: https://pypi.python.org/pypi/zeroconf\n\n.. image:: https://codecov.io/gh/python-zeroconf/python-zeroconf/branch/master/graph/badge.svg\n   :target: https://codecov.io/gh/python-zeroconf/python-zeroconf\n\n`Documentation <https://python-zeroconf.readthedocs.io/en/latest/>`_.\n\nThis is fork of pyzeroconf, Multicast DNS Service Discovery for Python,\noriginally by Paul Scott-Murphy (https://github.com/paulsm/pyzeroconf),\nmodified by William McBrine (https://github.com/wmcbrine/pyzeroconf).\n\nThe original William McBrine\'s fork note::\n\n    This fork is used in all of my TiVo-related projects: HME for Python\n    (and therefore HME/VLC), Network Remote, Remote Proxy, and pyTivo.\n    Before this, I was tracking the changes for zeroconf.py in three\n    separate repos. I figured I should have an authoritative source.\n\n    Although I make changes based on my experience with TiVos, I expect that\n    they\'re generally applicable. This version also includes patches found\n    on the now-defunct (?) Launchpad repo of pyzeroconf, and elsewhere\n    around the net -- not always well-documented, sorry.\n\nCompatible with:\n\n* Bonjour\n* Avahi\n\nCompared to some other Zeroconf/Bonjour/Avahi Python packages, python-zeroconf:\n\n* isn\'t tied to Bonjour or Avahi\n* doesn\'t use D-Bus\n* doesn\'t force you to use particular event loop or Twisted (asyncio is used under the hood but not required)\n* is pip-installable\n* has PyPI distribution\n* has an optional cython extension for performance (pure python is supported as well)\n\nPython compatibility\n--------------------\n\n* CPython 3.7+\n* PyPy3.7 7.3+\n\nVersioning\n----------\n\nThis project uses semantic versioning.\n\nStatus\n------\n\nThis project is actively maintained.\n\nTraffic Reduction\n-----------------\n\nBefore version 0.32, most traffic reduction techniques described in https://datatracker.ietf.org/doc/html/rfc6762#section-7\nwhere not implemented which could lead to excessive network traffic.  It is highly recommended that version 0.32 or later\nis used if this is a concern.\n\nIPv6 support\n------------\n\nIPv6 support is relatively new and currently limited, specifically:\n\n* `InterfaceChoice.All` is an alias for `InterfaceChoice.Default` on non-POSIX\n  systems.\n* Dual-stack IPv6 sockets are used, which may not be supported everywhere (some\n  BSD variants do not have them).\n* Listening on localhost (`::1`) does not work. Help with understanding why is\n  appreciated.\n\nHow to get python-zeroconf?\n===========================\n\n* PyPI page https://pypi.org/project/zeroconf/\n* GitHub project https://github.com/python-zeroconf/python-zeroconf\n\nThe easiest way to install python-zeroconf is using pip::\n\n    pip install zeroconf\n\n\n\nHow do I use it?\n================\n\nHere\'s an example of browsing for a service:\n\n.. code-block:: python\n\n    from zeroconf import ServiceBrowser, ServiceListener, Zeroconf\n\n\n    class MyListener(ServiceListener):\n\n        def update_service(self, zc: Zeroconf, type_: str, name: str) -> None:\n            print(f"Service {name} updated")\n\n        def remove_service(self, zc: Zeroconf, type_: str, name: str) -> None:\n            print(f"Service {name} removed")\n\n        def add_service(self, zc: Zeroconf, type_: str, name: str) -> None:\n            info = zc.get_service_info(type_, name)\n            print(f"Service {name} added, service info: {info}")\n\n\n    zeroconf = Zeroconf()\n    listener = MyListener()\n    browser = ServiceBrowser(zeroconf, "_http._tcp.local.", listener)\n    try:\n        input("Press enter to exit...\\n\\n")\n    finally:\n        zeroconf.close()\n\n.. note::\n\n    Discovery and service registration use *all* available network interfaces by default.\n    If you want to customize that you need to specify ``interfaces`` argument when\n    constructing ``Zeroconf`` object (see the code for details).\n\nIf you don\'t know the name of the service you need to browse for, try:\n\n.. code-block:: python\n\n    from zeroconf import ZeroconfServiceTypes\n    print(\'\\n\'.join(ZeroconfServiceTypes.find()))\n\nSee examples directory for more.\n\nChangelog\n=========\n\n`Changelog <CHANGELOG.md>`_\n\nLicense\n=======\n\nLGPL, see COPYING file for details.\n',
     'author': 'Paul Scott-Murphy',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/python-zeroconf/python-zeroconf',
```

### Comparing `zeroconf-0.71.3/PKG-INFO` & `zeroconf-0.71.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeroconf
-Version: 0.71.3
+Version: 0.71.4
 Summary: A pure python implementation of multicast DNS service discovery
 Home-page: https://github.com/python-zeroconf/python-zeroconf
 License: LGPL
 Author: Paul Scott-Murphy
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

