# Comparing `tmp/furs_fiscalization-0.8.0.tar.gz` & `tmp/furs_fiscalization-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "furs_fiscalization-0.8.0.tar", last modified: Fri Mar 17 10:59:32 2023, max compression
+gzip compressed data, was "furs_fiscalization-0.8.1.tar", last modified: Mon Jul 24 07:14:40 2023, max compression
```

## Comparing `furs_fiscalization-0.8.0.tar` & `furs_fiscalization-0.8.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-03-17 10:59:32.524042 furs_fiscalization-0.8.0/
--rw-rw-rw-   0        0        0     1103 2021-06-15 10:45:52.000000 furs_fiscalization-0.8.0/LICENSE
--rw-rw-rw-   0        0        0      464 2023-03-17 10:59:32.525040 furs_fiscalization-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     5749 2019-12-23 07:20:40.000000 furs_fiscalization-0.8.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-17 10:59:32.511814 furs_fiscalization-0.8.0/furs_fiscalization/
--rw-rw-rw-   0        0        0        2 2019-09-23 10:00:17.000000 furs_fiscalization-0.8.0/furs_fiscalization/__init__.py
--rw-rw-rw-   0        0        0    30067 2021-06-15 10:45:52.000000 furs_fiscalization-0.8.0/furs_fiscalization/api.py
--rw-rw-rw-   0        0        0     3688 2021-06-15 10:45:52.000000 furs_fiscalization-0.8.0/furs_fiscalization/base_api.py
-drwxrwxrwx   0        0        0        0 2023-03-17 10:59:32.523038 furs_fiscalization-0.8.0/furs_fiscalization/certs/
--rw-rw-rw-   0        0        0     1976 2019-09-23 07:19:33.000000 furs_fiscalization-0.8.0/furs_fiscalization/certs/test_certificate.pem
--rw-rw-rw-   0        0        0     6439 2023-03-17 10:49:09.000000 furs_fiscalization-0.8.0/furs_fiscalization/connector.py
--rw-rw-rw-   0        0        0     1033 2021-06-15 10:45:52.000000 furs_fiscalization-0.8.0/furs_fiscalization/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-03-17 10:59:32.521045 furs_fiscalization-0.8.0/furs_fiscalization.egg-info/
--rw-rw-rw-   0        0        0      464 2023-03-17 10:59:32.000000 furs_fiscalization-0.8.0/furs_fiscalization.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      444 2023-03-17 10:59:32.000000 furs_fiscalization-0.8.0/furs_fiscalization.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-17 10:59:32.000000 furs_fiscalization-0.8.0/furs_fiscalization.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-03-17 10:59:32.000000 furs_fiscalization-0.8.0/furs_fiscalization.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-03-17 10:59:32.000000 furs_fiscalization-0.8.0/furs_fiscalization.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-03-17 10:59:32.526063 furs_fiscalization-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0      788 2023-03-17 10:57:46.000000 furs_fiscalization-0.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 07:14:40.856324 furs_fiscalization-0.8.1/
+-rw-rw-rw-   0        0        0     1103 2021-06-15 10:45:52.000000 furs_fiscalization-0.8.1/LICENSE
+-rw-rw-rw-   0        0        0      464 2023-07-24 07:14:40.856324 furs_fiscalization-0.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5749 2019-12-23 07:20:40.000000 furs_fiscalization-0.8.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 07:14:40.841787 furs_fiscalization-0.8.1/furs_fiscalization/
+-rw-rw-rw-   0        0        0        2 2019-09-23 10:00:17.000000 furs_fiscalization-0.8.1/furs_fiscalization/__init__.py
+-rw-rw-rw-   0        0        0    30067 2021-06-15 10:45:52.000000 furs_fiscalization-0.8.1/furs_fiscalization/api.py
+-rw-rw-rw-   0        0        0     3765 2023-07-24 06:52:39.000000 furs_fiscalization-0.8.1/furs_fiscalization/base_api.py
+drwxrwxrwx   0        0        0        0 2023-07-24 07:14:40.855348 furs_fiscalization-0.8.1/furs_fiscalization/certs/
+-rw-rw-rw-   0        0        0     1976 2019-09-23 07:19:33.000000 furs_fiscalization-0.8.1/furs_fiscalization/certs/test_certificate.pem
+-rw-rw-rw-   0        0        0     6676 2023-07-24 07:05:38.000000 furs_fiscalization-0.8.1/furs_fiscalization/connector.py
+-rw-rw-rw-   0        0        0     1033 2021-06-15 10:45:52.000000 furs_fiscalization-0.8.1/furs_fiscalization/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-24 07:14:40.854323 furs_fiscalization-0.8.1/furs_fiscalization.egg-info/
+-rw-rw-rw-   0        0        0      464 2023-07-24 07:14:40.000000 furs_fiscalization-0.8.1/furs_fiscalization.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      444 2023-07-24 07:14:40.000000 furs_fiscalization-0.8.1/furs_fiscalization.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 07:14:40.000000 furs_fiscalization-0.8.1/furs_fiscalization.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-07-24 07:14:40.000000 furs_fiscalization-0.8.1/furs_fiscalization.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-24 07:14:40.000000 furs_fiscalization-0.8.1/furs_fiscalization.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-24 07:14:40.857324 furs_fiscalization-0.8.1/setup.cfg
+-rw-rw-rw-   0        0        0      788 2023-07-24 07:14:06.000000 furs_fiscalization-0.8.1/setup.py
```

### Comparing `furs_fiscalization-0.8.0/LICENSE` & `furs_fiscalization-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `furs_fiscalization-0.8.0/README.md` & `furs_fiscalization-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `furs_fiscalization-0.8.0/furs_fiscalization/api.py` & `furs_fiscalization-0.8.1/furs_fiscalization/api.py`

 * *Files identical despite different names*

### Comparing `furs_fiscalization-0.8.0/furs_fiscalization/base_api.py` & `furs_fiscalization-0.8.1/furs_fiscalization/base_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 from OpenSSL import crypto
+from cryptography.hazmat.primitives.serialization import pkcs12
 from jose import jws
 from requests import codes
 from requests.exceptions import Timeout
 from furs_fiscalization.connector import Connector
 from furs_fiscalization.exceptions import ConnectionException, ConnectionTimedOutException, FURSException
 
 
@@ -79,8 +80,8 @@
                                 message=error['ErrorMessage'])
 
         return server_response
 
     def _sign(self, content, digest='SHA256'):
         pkey = self.connector.p12.get_privatekey()
 
-        return crypto.sign(pkey=pkey, data=content, digest=digest)
+        return crypto.sign(pkey=pkey, data=str.encode(content), digest=digest)
```

### Comparing `furs_fiscalization-0.8.0/furs_fiscalization/certs/test_certificate.pem` & `furs_fiscalization-0.8.1/furs_fiscalization/certs/test_certificate.pem`

 * *Files identical despite different names*

### Comparing `furs_fiscalization-0.8.0/furs_fiscalization/connector.py` & `furs_fiscalization-0.8.1/furs_fiscalization/connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import tempfile
 import requests
 from OpenSSL import crypto
+#from cryptography.hazmat.primitives.serialization import pkcs12
 from jose import jws
 
 requests.packages.urllib3.disable_warnings()
 
 FURS_TEST_ENDPOINT = 'https://blagajne-test.fu.gov.si:9002'
 FURS_PRODUCTION_ENDPOINT = 'https://blagajne.fu.gov.si:9003'
 
@@ -54,14 +55,16 @@
 
         :param p12_password: (string) password for the .p12 file
         :return: None
         """
         if self.p12_buffer is None:
             self.p12_buffer = open(self.p12_path, 'rb').read()
         self.p12 = crypto.load_pkcs12(buffer=self.p12_buffer, passphrase=str.encode(p12_password))
+        #private_key, certificate, additional_certificates = pkcs12.load_key_and_certificates(self.p12_buffer, str.encode(p12_password))
+        #self.p12 = certificate
         self._store_temp_files()
 
     def _store_temp_files(self):
         """
         Requests library requires string path to PKey and Cert - therefore we save those into
         temporary files on the file system.
```

### Comparing `furs_fiscalization-0.8.0/furs_fiscalization/exceptions.py` & `furs_fiscalization-0.8.1/furs_fiscalization/exceptions.py`

 * *Files identical despite different names*

### Comparing `furs_fiscalization-0.8.0/setup.py` & `furs_fiscalization-0.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name='furs_fiscalization',
     packages=['furs_fiscalization'],
-    version='0.8.0',
+    version='0.8.1',
     license='MIT',
     description='Python library for simplified communication with FURS (Financna uprava Republike Slovenije).',
     author='Hermes d.o.o.',
     author_email='info@hermes-solutions.si ',
     url='https://github.com/HermesGH/furs-fiscalization',
     download_url='https://github.com/HermesGH/furs-fiscalization/archive/v0.7.0.zip',
     keywords=['FURS', 'fiscal', 'fiscal register', 'davcne blagajne'],
```

