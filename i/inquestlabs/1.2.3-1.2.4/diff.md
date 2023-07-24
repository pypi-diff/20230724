# Comparing `tmp/inquestlabs-1.2.3.tar.gz` & `tmp/inquestlabs-1.2.4.tar.gz`

## Comparing `inquestlabs-1.2.3.tar` & `inquestlabs-1.2.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/.coveragerc
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/CONTRIBUTING.md
--rwxr-xr-x   0        0        0    58471 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/inquestlabs.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/requirements-testing.txt
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/requirements.txt
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/.github/workflows/workflow.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/tests/__init__.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/tests/conftest.py
--rw-r--r--   0        0        0     5064 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/tests/test_api.py
--rw-r--r--   0        0        0     8016 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/tests/test_dfi_attributes.py
--rw-r--r--   0        0        0    23800 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/tests/test_dfi_details.py
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/tests/test_dfi_download.py
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/tests/test_dfi_list.py
--rw-r--r--   0        0        0     4652 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/tests/test_dfi_search.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/tests/test_dfi_sources.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/tests/test_dfi_upload.py
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/tests/test_iocdb_list.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/tests/test_iocdb_search.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/tests/test_iocdb_sources.py
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/tests/test_repdb_list.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/tests/test_repdb_search.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/tests/test_repdb_sources.py
--rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/tests/test_stats.py
--rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/tests/test_yara_b64re.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/tests/test_yara_hexcase.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/tests/test_yara_uint.py
--rw-r--r--   0        0        0     4598 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/tests/test_yara_widere.py
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/.gitignore
--rw-r--r--   0        0        0    18092 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/LICENSE
--rw-r--r--   0        0        0    16551 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/README.md
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/pyproject.toml
--rw-r--r--   0        0        0    38299 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 inquestlabs-1.2.4/.coveragerc
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 inquestlabs-1.2.4/CONTRIBUTING.md
+-rwxr-xr-x   0        0        0    59360 2020-02-02 00:00:00.000000 inquestlabs-1.2.4/inquestlabs.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 inquestlabs-1.2.4/requirements-testing.txt
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 inquestlabs-1.2.4/requirements.txt
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 inquestlabs-1.2.4/.github/workflows/workflow.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 inquestlabs-1.2.4/tests/__init__.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 inquestlabs-1.2.4/tests/conftest.py
+-rw-r--r--   0        0        0     5064 2020-02-02 00:00:00.000000 inquestlabs-1.2.4/tests/test_api.py
+-rw-r--r--   0        0        0     8016 2020-02-02 00:00:00.000000 inquestlabs-1.2.4/tests/test_dfi_attributes.py
+-rw-r--r--   0        0        0    23800 2020-02-02 00:00:00.000000 inquestlabs-1.2.4/tests/test_dfi_details.py
+-rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 inquestlabs-1.2.4/tests/test_dfi_download.py
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 inquestlabs-1.2.4/tests/test_dfi_list.py
+-rw-r--r--   0        0        0     4652 2020-02-02 00:00:00.000000 inquestlabs-1.2.4/tests/test_dfi_search.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 inquestlabs-1.2.4/tests/test_dfi_sources.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 inquestlabs-1.2.4/tests/test_dfi_upload.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 inquestlabs-1.2.4/tests/test_iocdb_list.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 inquestlabs-1.2.4/tests/test_iocdb_search.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 inquestlabs-1.2.4/tests/test_iocdb_sources.py
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 inquestlabs-1.2.4/tests/test_repdb_list.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 inquestlabs-1.2.4/tests/test_repdb_search.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 inquestlabs-1.2.4/tests/test_repdb_sources.py
+-rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 inquestlabs-1.2.4/tests/test_stats.py
+-rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 inquestlabs-1.2.4/tests/test_yara_b64re.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 inquestlabs-1.2.4/tests/test_yara_hexcase.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 inquestlabs-1.2.4/tests/test_yara_uint.py
+-rw-r--r--   0        0        0     4598 2020-02-02 00:00:00.000000 inquestlabs-1.2.4/tests/test_yara_widere.py
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 inquestlabs-1.2.4/.gitignore
+-rw-r--r--   0        0        0    18092 2020-02-02 00:00:00.000000 inquestlabs-1.2.4/LICENSE
+-rw-r--r--   0        0        0    16594 2020-02-02 00:00:00.000000 inquestlabs-1.2.4/README.md
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 inquestlabs-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0    38342 2020-02-02 00:00:00.000000 inquestlabs-1.2.4/PKG-INFO
```

### Comparing `inquestlabs-1.2.3/inquestlabs.py` & `inquestlabs-1.2.4/inquestlabs.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     inquestlabs [options] repdb list
     inquestlabs [options] repdb search <keyword>
     inquestlabs [options] repdb sources
     inquestlabs [options] yara (b64re|base64re) <regex> [(--big-endian|--little-endian)]
     inquestlabs [options] yara hexcase <instring>
     inquestlabs [options] yara uint <instring> [--offset=<offset>] [--hex]
     inquestlabs [options] yara widere <regex> [(--big-endian|--little-endian)]
+    inquestlabs [options] yara cidr <ipv4>
     inquestlabs [options] lookup ip <ioc>
     inquestlabs [options] lookup domain <ioc>
     inquestlabs [options] report <ioc>
     inquestlabs [options] stats
     inquestlabs [options] setup <apikey>
     inquestlabs [options] trystero list-days
     inquestlabs [options] trystero list-samples <yyyy-mm-dd>
@@ -79,15 +80,15 @@
 import sys
 import os
 import re
 # from importlib.metadata import version
 
 # extract version from installed package metadata
 __application_name__ = "inquestlabs"
-__version__ = "1.2.3"
+__version__ = "1.2.4"
 # __version__ = version(__application_name__)
 __full_version__ = f"{__application_name__} {__version__}"
 
 VALID_CAT    = ["ext", "hash", "ioc"]
 VALID_EXT    = ["code", "context", "metadata", "ocr"]
 VALID_HASH   = ["md5", "sha1", "sha256", "sha512"]
 VALID_IOC    = ["domain", "email", "filename", "filepath", "ip", "registry", "url", "xmpid"]
@@ -140,15 +141,15 @@
         :param verbose:    Values greater than zero provide increased verbosity.
         """
 
         # internalize supplied parameters.
         self.api_key     = api_key
         self.base_url    = base_url
         self.config_file = config
-        self.retries = retries
+        self.retries     = retries
         self.proxies     = proxies
         self.verify_ssl  = verify_ssl
         self.verbosity   = verbose
 
         # internal rate limit tracking.
         self.rlimit_requests_remaining = None   # requests remaining in this rate limit window.
         self.rlimit_reset_epoch_time   = None   # time, in seconds from epoch, that rate limit window resets.
@@ -210,28 +211,30 @@
                     self.api_key_source = "config: %s" % self.config_file
 
             # NOTE: if we still don't have an API key that's fine! InQuest Labs will simply work with some rate limits.
             self.__VERBOSE("api_key=%s" % self.api_key, DEBUG)
             self.__VERBOSE("api_key_source=%s" % self.api_key_source, INFO)
 
     ####################################################################################################################
-    def API (self, api, data=None, path=None, method="GET", raw=False):
+    def API (self, api, data=None, path=None, method="GET", raw=False, params=None):
         """
         Internal API wrapper.
 
         :type  api:    str
         :param api:    API endpoint, appended to base URL.
         :type  data:   dict
         :param data:   Optional data dictionary to pass to endpoint.
         :type  path:   str
         :param path:   Optional path to file to pass to endpoint.
         :type  method: str
         :param method: API method, one of "GET" or "POST".
         :type  raw:    bool
         :param raw:    Default behavior is to expect JSON encoded content, raise this flag to expect raw data.
+        :type  method: str
+        :param method: Set a parameter for the request.
 
         :rtype:  dict | str
         :return: Response dictionary or string if 'raw' flag is raised.
         """
 
         assert method in ["GET", "POST"]
 
@@ -254,14 +257,15 @@
         kwargs = \
         {
             "data"    : data,
             "files"   : files,
             "headers" : headers,
             "proxies" : self.proxies,
             "verify"  : self.verify_ssl,
+            "params"  : params
         }
 
         # make attempts to dance with the API endpoint, use a jittered exponential back-off delay.
         last_exception = None
         endpoint       = self.base_url + api
         attempt        = 0
 
@@ -1239,14 +1243,31 @@
 
         :rtype:  str
         :return: YARA condition looking for magic at offset via uint() magic.
         """
 
         return self.API("/yara/trigger", dict(trigger=magic, offset=offset, is_hex=is_hex))
 
+    ####################################################################################################################
+    def cidr_to_regex (self, data):
+        """
+        Produce a regular expression from a IPv4 CIDR notation in a form suitable for usage as a YARA string.
+
+        :type  regex:  str
+        :param regex:  Regular expression to convert.
+
+        :rtype:  str
+        :return: Regex string suitable for YARA.
+        """
+
+        # dance with the API and return results.
+        return self.API("/yara/cidr2regex", params={
+            "cidr": data
+        })
+
 ########################################################################################################################
 ########################################################################################################################
 ########################################################################################################################
 
 def main ():
     args = docopt.docopt(__doc__, version=__version__)
 
@@ -1410,14 +1431,18 @@
         elif args['uint']:
             print(labs.yara_uint(args['<instring>'], args['--offset'], args['--hex']))
 
         # inquestlabs [options] yara widere <regex> [(--big-endian|--little-endian)]
         elif args['widere']:
             print(labs.yara_widere(args['<regex>'], endian))
 
+        # inquestlabs [options] yara cidr <ipv4>
+        elif args['cidr']:
+            print(labs.cidr_to_regex(args['<ipv4>']))
+
         # huh?
         else:
             raise inquestlabs_exception("yara argument parsing fail.")
 
     ### IP/DOMAIN LOOKUP ###############################################################################################
     elif args['lookup']:
         if args['ip']:
```

### Comparing `inquestlabs-1.2.3/.github/workflows/workflow.yml` & `inquestlabs-1.2.4/.github/workflows/workflow.yml`

 * *Files identical despite different names*

### Comparing `inquestlabs-1.2.3/tests/test_api.py` & `inquestlabs-1.2.4/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `inquestlabs-1.2.3/tests/test_dfi_attributes.py` & `inquestlabs-1.2.4/tests/test_dfi_attributes.py`

 * *Files identical despite different names*

### Comparing `inquestlabs-1.2.3/tests/test_dfi_details.py` & `inquestlabs-1.2.4/tests/test_dfi_details.py`

 * *Files identical despite different names*

### Comparing `inquestlabs-1.2.3/tests/test_dfi_download.py` & `inquestlabs-1.2.4/tests/test_dfi_download.py`

 * *Files identical despite different names*

### Comparing `inquestlabs-1.2.3/tests/test_dfi_list.py` & `inquestlabs-1.2.4/tests/test_dfi_list.py`

 * *Files identical despite different names*

### Comparing `inquestlabs-1.2.3/tests/test_dfi_search.py` & `inquestlabs-1.2.4/tests/test_dfi_search.py`

 * *Files identical despite different names*

### Comparing `inquestlabs-1.2.3/tests/test_dfi_upload.py` & `inquestlabs-1.2.4/tests/test_dfi_upload.py`

 * *Files identical despite different names*

### Comparing `inquestlabs-1.2.3/tests/test_iocdb_list.py` & `inquestlabs-1.2.4/tests/test_iocdb_list.py`

 * *Files identical despite different names*

### Comparing `inquestlabs-1.2.3/tests/test_iocdb_search.py` & `inquestlabs-1.2.4/tests/test_iocdb_search.py`

 * *Files identical despite different names*

### Comparing `inquestlabs-1.2.3/tests/test_repdb_list.py` & `inquestlabs-1.2.4/tests/test_repdb_list.py`

 * *Files identical despite different names*

### Comparing `inquestlabs-1.2.3/tests/test_repdb_search.py` & `inquestlabs-1.2.4/tests/test_repdb_search.py`

 * *Files identical despite different names*

### Comparing `inquestlabs-1.2.3/tests/test_stats.py` & `inquestlabs-1.2.4/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `inquestlabs-1.2.3/tests/test_yara_b64re.py` & `inquestlabs-1.2.4/tests/test_yara_b64re.py`

 * *Files identical despite different names*

### Comparing `inquestlabs-1.2.3/tests/test_yara_hexcase.py` & `inquestlabs-1.2.4/tests/test_yara_hexcase.py`

 * *Files identical despite different names*

### Comparing `inquestlabs-1.2.3/tests/test_yara_uint.py` & `inquestlabs-1.2.4/tests/test_yara_uint.py`

 * *Files identical despite different names*

### Comparing `inquestlabs-1.2.3/tests/test_yara_widere.py` & `inquestlabs-1.2.4/tests/test_yara_widere.py`

 * *Files identical despite different names*

### Comparing `inquestlabs-1.2.3/.gitignore` & `inquestlabs-1.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `inquestlabs-1.2.3/LICENSE` & `inquestlabs-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `inquestlabs-1.2.3/README.md` & `inquestlabs-1.2.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     inquestlabs [options] repdb list
     inquestlabs [options] repdb search <keyword>
     inquestlabs [options] repdb sources
     inquestlabs [options] yara (b64re|base64re) <regex> [(--big-endian|--little-endian)]
     inquestlabs [options] yara hexcase <instring>
     inquestlabs [options] yara uint <instring> [--offset=<offset>] [--hex]
     inquestlabs [options] yara widere <regex> [(--big-endian|--little-endian)]
+    inquestlabs [options] yara cidr <ipv4>
     inquestlabs [options] lookup ip <ioc>
     inquestlabs [options] lookup domain <ioc>
     inquestlabs [options] report <ioc>
     inquestlabs [options] stats
     inquestlabs [options] setup <apikey>
     inquestlabs [options] trystero list-days
     inquestlabs [options] trystero list-samples <yyyy-mm-dd>
```

### Comparing `inquestlabs-1.2.3/pyproject.toml` & `inquestlabs-1.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "wheel"]
 build-backend = "hatchling.build"
 
 [project]
 name = "inquestlabs"
-version = "1.2.3"
+version = "1.2.4"
 license = {file = "LICENSE"}
 authors = [
 	{ name="InQuest", email="labs@inquest.net" },
 ]
 description = "A Pythonic interface and CLI tool for the InQuest Labs API"
 readme = "README.md"
 requires-python = ">=3.6"
```

### Comparing `inquestlabs-1.2.3/PKG-INFO` & `inquestlabs-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inquestlabs
-Version: 1.2.3
+Version: 1.2.4
 Summary: A Pythonic interface and CLI tool for the InQuest Labs API
 Project-URL: Homepage, https://labs.inquest.net/
 Project-URL: Repository, https://github.com/InQuest/python-inquestlabs
 Project-URL: Bug Tracker, https://github.com/InQuest/python-inquestlabs/issues
 Author-email: InQuest <labs@inquest.net>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
@@ -417,14 +417,15 @@
     inquestlabs [options] repdb list
     inquestlabs [options] repdb search <keyword>
     inquestlabs [options] repdb sources
     inquestlabs [options] yara (b64re|base64re) <regex> [(--big-endian|--little-endian)]
     inquestlabs [options] yara hexcase <instring>
     inquestlabs [options] yara uint <instring> [--offset=<offset>] [--hex]
     inquestlabs [options] yara widere <regex> [(--big-endian|--little-endian)]
+    inquestlabs [options] yara cidr <ipv4>
     inquestlabs [options] lookup ip <ioc>
     inquestlabs [options] lookup domain <ioc>
     inquestlabs [options] report <ioc>
     inquestlabs [options] stats
     inquestlabs [options] setup <apikey>
     inquestlabs [options] trystero list-days
     inquestlabs [options] trystero list-samples <yyyy-mm-dd>
```

