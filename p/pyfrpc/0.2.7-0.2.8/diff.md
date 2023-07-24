# Comparing `tmp/pyfrpc-0.2.7.tar.gz` & `tmp/pyfrpc-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfrpc-0.2.7.tar", last modified: Wed Jul 12 14:22:47 2023, max compression
+gzip compressed data, was "pyfrpc-0.2.8.tar", last modified: Mon Jul 24 08:06:59 2023, max compression
```

## Comparing `pyfrpc-0.2.7.tar` & `pyfrpc-0.2.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:22:47.292608 pyfrpc-0.2.7/
--rw-rw-rw-   0 root         (0) root         (0)     1058 2023-07-12 14:22:30.000000 pyfrpc-0.2.7/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-07-12 14:22:30.000000 pyfrpc-0.2.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4423 2023-07-12 14:22:47.292608 pyfrpc-0.2.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3752 2023-07-12 14:22:30.000000 pyfrpc-0.2.7/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 14:22:47.292608 pyfrpc-0.2.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2180 2023-07-12 14:22:30.000000 pyfrpc-0.2.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:22:47.286608 pyfrpc-0.2.7/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:22:47.289608 pyfrpc-0.2.7/src/pyfrpc/
--rw-rw-rw-   0 root         (0) root         (0)      206 2023-07-12 14:22:30.000000 pyfrpc-0.2.7/src/pyfrpc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-07-12 14:22:30.000000 pyfrpc-0.2.7/src/pyfrpc/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)    15603 2023-07-12 14:22:30.000000 pyfrpc-0.2.7/src/pyfrpc/_coding_base_c.pyx
--rw-rw-rw-   0 root         (0) root         (0)    10197 2023-07-12 14:22:30.000000 pyfrpc-0.2.7/src/pyfrpc/_coding_base_py.py
--rw-rw-rw-   0 root         (0) root         (0)     3223 2023-07-12 14:22:30.000000 pyfrpc-0.2.7/src/pyfrpc/asyncclient.py
--rw-rw-rw-   0 root         (0) root         (0)     3939 2023-07-12 14:22:30.000000 pyfrpc-0.2.7/src/pyfrpc/client.py
--rw-rw-rw-   0 root         (0) root         (0)     3278 2023-07-12 14:22:30.000000 pyfrpc-0.2.7/src/pyfrpc/coding.py
--rw-rw-rw-   0 root         (0) root         (0)      718 2023-07-12 14:22:30.000000 pyfrpc-0.2.7/src/pyfrpc/models.py
--rw-rw-rw-   0 root         (0) root         (0)      820 2023-07-12 14:22:30.000000 pyfrpc-0.2.7/src/pyfrpc/netcat.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:22:47.290608 pyfrpc-0.2.7/src/pyfrpc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4423 2023-07-12 14:22:47.000000 pyfrpc-0.2.7/src/pyfrpc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      599 2023-07-12 14:22:47.000000 pyfrpc-0.2.7/src/pyfrpc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 14:22:47.000000 pyfrpc-0.2.7/src/pyfrpc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2023-07-12 14:22:47.000000 pyfrpc-0.2.7/src/pyfrpc.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       40 2023-07-12 14:22:47.000000 pyfrpc-0.2.7/src/pyfrpc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-12 14:22:47.000000 pyfrpc-0.2.7/src/pyfrpc.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:22:47.292608 pyfrpc-0.2.7/test/
--rw-rw-rw-   0 root         (0) root         (0)     2854 2023-07-12 14:22:30.000000 pyfrpc-0.2.7/test/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     2011 2023-07-12 14:22:30.000000 pyfrpc-0.2.7/test/test_fastrpc.py
--rw-rw-rw-   0 root         (0) root         (0)     1596 2023-07-12 14:22:30.000000 pyfrpc-0.2.7/test/test_protocol.py
--rw-rw-rw-   0 root         (0) root         (0)     2401 2023-07-12 14:22:30.000000 pyfrpc-0.2.7/test/test_protocol_v1.py
--rw-rw-rw-   0 root         (0) root         (0)     5658 2023-07-12 14:22:30.000000 pyfrpc-0.2.7/test/test_protocol_v2.py
--rw-rw-rw-   0 root         (0) root         (0)     2672 2023-07-12 14:22:30.000000 pyfrpc-0.2.7/test/test_protocol_v3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 08:06:59.645895 pyfrpc-0.2.8/
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2023-07-24 08:06:43.000000 pyfrpc-0.2.8/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-07-24 08:06:43.000000 pyfrpc-0.2.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4423 2023-07-24 08:06:59.645895 pyfrpc-0.2.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3752 2023-07-24 08:06:43.000000 pyfrpc-0.2.8/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 08:06:59.645895 pyfrpc-0.2.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2180 2023-07-24 08:06:43.000000 pyfrpc-0.2.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 08:06:59.638895 pyfrpc-0.2.8/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 08:06:59.641895 pyfrpc-0.2.8/src/pyfrpc/
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-07-24 08:06:43.000000 pyfrpc-0.2.8/src/pyfrpc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-07-24 08:06:43.000000 pyfrpc-0.2.8/src/pyfrpc/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15603 2023-07-24 08:06:43.000000 pyfrpc-0.2.8/src/pyfrpc/_coding_base_c.pyx
+-rw-rw-rw-   0 root         (0) root         (0)    10197 2023-07-24 08:06:43.000000 pyfrpc-0.2.8/src/pyfrpc/_coding_base_py.py
+-rw-rw-rw-   0 root         (0) root         (0)     3218 2023-07-24 08:06:43.000000 pyfrpc-0.2.8/src/pyfrpc/asyncclient.py
+-rw-rw-rw-   0 root         (0) root         (0)     3939 2023-07-24 08:06:43.000000 pyfrpc-0.2.8/src/pyfrpc/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     3278 2023-07-24 08:06:43.000000 pyfrpc-0.2.8/src/pyfrpc/coding.py
+-rw-rw-rw-   0 root         (0) root         (0)      718 2023-07-24 08:06:43.000000 pyfrpc-0.2.8/src/pyfrpc/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      820 2023-07-24 08:06:43.000000 pyfrpc-0.2.8/src/pyfrpc/netcat.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 08:06:59.643895 pyfrpc-0.2.8/src/pyfrpc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4423 2023-07-24 08:06:59.000000 pyfrpc-0.2.8/src/pyfrpc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      599 2023-07-24 08:06:59.000000 pyfrpc-0.2.8/src/pyfrpc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 08:06:59.000000 pyfrpc-0.2.8/src/pyfrpc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-07-24 08:06:59.000000 pyfrpc-0.2.8/src/pyfrpc.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2023-07-24 08:06:59.000000 pyfrpc-0.2.8/src/pyfrpc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-24 08:06:59.000000 pyfrpc-0.2.8/src/pyfrpc.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 08:06:59.644895 pyfrpc-0.2.8/test/
+-rw-rw-rw-   0 root         (0) root         (0)     2854 2023-07-24 08:06:43.000000 pyfrpc-0.2.8/test/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     2011 2023-07-24 08:06:43.000000 pyfrpc-0.2.8/test/test_fastrpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1596 2023-07-24 08:06:43.000000 pyfrpc-0.2.8/test/test_protocol.py
+-rw-rw-rw-   0 root         (0) root         (0)     2401 2023-07-24 08:06:43.000000 pyfrpc-0.2.8/test/test_protocol_v1.py
+-rw-rw-rw-   0 root         (0) root         (0)     5658 2023-07-24 08:06:43.000000 pyfrpc-0.2.8/test/test_protocol_v2.py
+-rw-rw-rw-   0 root         (0) root         (0)     2672 2023-07-24 08:06:43.000000 pyfrpc-0.2.8/test/test_protocol_v3.py
```

### Comparing `pyfrpc-0.2.7/LICENSE.txt` & `pyfrpc-0.2.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyfrpc-0.2.7/PKG-INFO` & `pyfrpc-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfrpc
-Version: 0.2.7
+Version: 0.2.8
 Summary: Python implementation of fastrpc protocol
 Home-page: https://gitlab.com/vladaburian/pyfrpc
 Author: Vladimir Burian
 License: MIT
 Keywords: frpc fastrpc
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `pyfrpc-0.2.7/README.md` & `pyfrpc-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `pyfrpc-0.2.7/setup.py` & `pyfrpc-0.2.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 PYFRPC_NOEXT = bool(int(os.environ.get('PYFRPC_NOEXT', '0')))
 
 
 setup_args = dict(
     name='pyfrpc',
-    version='0.2.7',
+    version='0.2.8',
     description='Python implementation of fastrpc protocol',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Vladimir Burian',
     license='MIT',
     url='https://gitlab.com/vladaburian/pyfrpc',
     classifiers=[
```

### Comparing `pyfrpc-0.2.7/src/pyfrpc/_coding_base_c.pyx` & `pyfrpc-0.2.8/src/pyfrpc/_coding_base_c.pyx`

 * *Files identical despite different names*

### Comparing `pyfrpc-0.2.7/src/pyfrpc/_coding_base_py.py` & `pyfrpc-0.2.8/src/pyfrpc/_coding_base_py.py`

 * *Files identical despite different names*

### Comparing `pyfrpc-0.2.7/src/pyfrpc/asyncclient.py` & `pyfrpc-0.2.8/src/pyfrpc/asyncclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         })
 
         for k,v in self._opts.items():
             kwargs.setdefault(k, v)
 
         async with self.session.post(url=self._url, data=payload, headers=headers, **kwargs) as res:
             if res.status != 200:
-                raise RuntimeError("bad status code, expected 200, got {:d}".format(res.status_code))
+                raise RuntimeError("bad status code, expected 200, got {:d}".format(res.status))
 
             content = await res.read()
             content_type = res.headers.get("Content-Type", None)
 
         # FRPC decoding
         if content_type == APPLICATION_FRPC:
             payload = decode(content)
```

### Comparing `pyfrpc-0.2.7/src/pyfrpc/client.py` & `pyfrpc-0.2.8/src/pyfrpc/client.py`

 * *Files identical despite different names*

### Comparing `pyfrpc-0.2.7/src/pyfrpc/coding.py` & `pyfrpc-0.2.8/src/pyfrpc/coding.py`

 * *Files identical despite different names*

### Comparing `pyfrpc-0.2.7/src/pyfrpc/models.py` & `pyfrpc-0.2.8/src/pyfrpc/models.py`

 * *Files identical despite different names*

### Comparing `pyfrpc-0.2.7/src/pyfrpc/netcat.py` & `pyfrpc-0.2.8/src/pyfrpc/netcat.py`

 * *Files identical despite different names*

### Comparing `pyfrpc-0.2.7/src/pyfrpc.egg-info/PKG-INFO` & `pyfrpc-0.2.8/src/pyfrpc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfrpc
-Version: 0.2.7
+Version: 0.2.8
 Summary: Python implementation of fastrpc protocol
 Home-page: https://gitlab.com/vladaburian/pyfrpc
 Author: Vladimir Burian
 License: MIT
 Keywords: frpc fastrpc
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `pyfrpc-0.2.7/src/pyfrpc.egg-info/SOURCES.txt` & `pyfrpc-0.2.8/src/pyfrpc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyfrpc-0.2.7/test/conftest.py` & `pyfrpc-0.2.8/test/conftest.py`

 * *Files identical despite different names*

### Comparing `pyfrpc-0.2.7/test/test_fastrpc.py` & `pyfrpc-0.2.8/test/test_fastrpc.py`

 * *Files identical despite different names*

### Comparing `pyfrpc-0.2.7/test/test_protocol.py` & `pyfrpc-0.2.8/test/test_protocol.py`

 * *Files identical despite different names*

### Comparing `pyfrpc-0.2.7/test/test_protocol_v1.py` & `pyfrpc-0.2.8/test/test_protocol_v1.py`

 * *Files identical despite different names*

### Comparing `pyfrpc-0.2.7/test/test_protocol_v2.py` & `pyfrpc-0.2.8/test/test_protocol_v2.py`

 * *Files identical despite different names*

### Comparing `pyfrpc-0.2.7/test/test_protocol_v3.py` & `pyfrpc-0.2.8/test/test_protocol_v3.py`

 * *Files identical despite different names*

