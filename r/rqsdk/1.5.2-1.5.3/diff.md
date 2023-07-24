# Comparing `tmp/rqsdk-1.5.2.tar.gz` & `tmp/rqsdk-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rqsdk-1.5.2.tar", last modified: Fri Jul  7 09:38:54 2023, max compression
+gzip compressed data, was "dist/rqsdk-1.5.3.tar", last modified: Mon Jul 24 07:23:59 2023, max compression
```

## Comparing `rqsdk-1.5.2.tar` & `rqsdk-1.5.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-07-07 09:38:54.989753 rqsdk-1.5.2/
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      256 2023-07-07 09:38:52.000000 rqsdk-1.5.2/HISTORY.md
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      173 2023-07-07 09:38:52.000000 rqsdk-1.5.2/MANIFEST.in
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      760 2023-07-07 09:38:54.989753 rqsdk-1.5.2/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)     1111 2023-07-07 09:38:52.000000 rqsdk-1.5.2/README.md
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-07-07 09:38:54.990753 rqsdk-1.5.2/rqsdk/
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      752 2023-07-07 09:38:52.000000 rqsdk-1.5.2/rqsdk/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      680 2023-07-07 09:38:52.000000 rqsdk-1.5.2/rqsdk/__main__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      497 2023-07-07 09:38:54.990753 rqsdk-1.5.2/rqsdk/_version.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)    13017 2023-07-07 09:38:52.000000 rqsdk-1.5.2/rqsdk/cmds.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)     1738 2023-07-07 09:38:52.000000 rqsdk-1.5.2/rqsdk/const.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)     6715 2023-07-07 09:38:52.000000 rqsdk-1.5.2/rqsdk/license_helper.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      319 2023-07-07 09:38:52.000000 rqsdk-1.5.2/rqsdk/proxy_helper.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)     2453 2023-07-07 09:38:52.000000 rqsdk-1.5.2/rqsdk/script_update.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      741 2023-07-07 09:38:52.000000 rqsdk-1.5.2/rqsdk/testing.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-07-07 09:38:54.987753 rqsdk-1.5.2/rqsdk.egg-info/
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      760 2023-07-07 09:38:54.000000 rqsdk-1.5.2/rqsdk.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      438 2023-07-07 09:38:54.000000 rqsdk-1.5.2/rqsdk.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)        1 2023-07-07 09:38:54.000000 rqsdk-1.5.2/rqsdk.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)       44 2023-07-07 09:38:54.000000 rqsdk-1.5.2/rqsdk.egg-info/entry_points.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)        1 2023-07-07 09:38:54.000000 rqsdk-1.5.2/rqsdk.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)     3417 2023-07-07 09:38:54.000000 rqsdk-1.5.2/rqsdk.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)        6 2023-07-07 09:38:54.000000 rqsdk-1.5.2/rqsdk.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      244 2023-07-07 09:38:54.990753 rqsdk-1.5.2/setup.cfg
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)     3140 2023-07-07 09:38:52.000000 rqsdk-1.5.2/setup.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)    79860 2023-07-07 09:38:52.000000 rqsdk-1.5.2/versioneer.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-07-24 07:23:59.187561 rqsdk-1.5.3/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      256 2023-07-24 07:23:53.000000 rqsdk-1.5.3/HISTORY.md
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      173 2023-07-24 07:23:53.000000 rqsdk-1.5.3/MANIFEST.in
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      760 2023-07-24 07:23:59.188561 rqsdk-1.5.3/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)     1111 2023-07-24 07:23:53.000000 rqsdk-1.5.3/README.md
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-07-24 07:23:59.192561 rqsdk-1.5.3/rqsdk/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      752 2023-07-24 07:23:53.000000 rqsdk-1.5.3/rqsdk/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      680 2023-07-24 07:23:53.000000 rqsdk-1.5.3/rqsdk/__main__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      497 2023-07-24 07:23:59.192561 rqsdk-1.5.3/rqsdk/_version.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)    13017 2023-07-24 07:23:53.000000 rqsdk-1.5.3/rqsdk/cmds.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)     1738 2023-07-24 07:23:53.000000 rqsdk-1.5.3/rqsdk/const.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)     6715 2023-07-24 07:23:53.000000 rqsdk-1.5.3/rqsdk/license_helper.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      319 2023-07-24 07:23:53.000000 rqsdk-1.5.3/rqsdk/proxy_helper.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)     2453 2023-07-24 07:23:53.000000 rqsdk-1.5.3/rqsdk/script_update.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      741 2023-07-24 07:23:53.000000 rqsdk-1.5.3/rqsdk/testing.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-07-24 07:23:59.187561 rqsdk-1.5.3/rqsdk.egg-info/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      760 2023-07-24 07:23:58.000000 rqsdk-1.5.3/rqsdk.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      438 2023-07-24 07:23:59.000000 rqsdk-1.5.3/rqsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)        1 2023-07-24 07:23:58.000000 rqsdk-1.5.3/rqsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)       44 2023-07-24 07:23:58.000000 rqsdk-1.5.3/rqsdk.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)        1 2023-07-24 07:23:58.000000 rqsdk-1.5.3/rqsdk.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)     3417 2023-07-24 07:23:59.000000 rqsdk-1.5.3/rqsdk.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)        6 2023-07-24 07:23:59.000000 rqsdk-1.5.3/rqsdk.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      244 2023-07-24 07:23:59.188561 rqsdk-1.5.3/setup.cfg
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)     3140 2023-07-24 07:23:53.000000 rqsdk-1.5.3/setup.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)    79860 2023-07-24 07:23:53.000000 rqsdk-1.5.3/versioneer.py
```

### Comparing `rqsdk-1.5.2/PKG-INFO` & `rqsdk-1.5.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rqsdk
-Version: 1.5.2
+Version: 1.5.3
 Summary: Ricequant Native SDK
 Home-page: https://www.ricequant.com/
 Author: Ricequant
 Author-email: public@ricequant.com
 License: UNKNOWN
 Keywords: rqsdk
 Platform: UNKNOWN
```

### Comparing `rqsdk-1.5.2/README.md` & `rqsdk-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `rqsdk-1.5.2/rqsdk/__init__.py` & `rqsdk-1.5.3/rqsdk/__init__.py`

 * *Files identical despite different names*

### Comparing `rqsdk-1.5.2/rqsdk/__main__.py` & `rqsdk-1.5.3/rqsdk/__main__.py`

 * *Files identical despite different names*

### Comparing `rqsdk-1.5.2/rqsdk/cmds.py` & `rqsdk-1.5.3/rqsdk/cmds.py`

 * *Files identical despite different names*

### Comparing `rqsdk-1.5.2/rqsdk/const.py` & `rqsdk-1.5.3/rqsdk/const.py`

 * *Files identical despite different names*

### Comparing `rqsdk-1.5.2/rqsdk/license_helper.py` & `rqsdk-1.5.3/rqsdk/license_helper.py`

 * *Files identical despite different names*

### Comparing `rqsdk-1.5.2/rqsdk/script_update.py` & `rqsdk-1.5.3/rqsdk/script_update.py`

 * *Files identical despite different names*

### Comparing `rqsdk-1.5.2/rqsdk/testing.py` & `rqsdk-1.5.3/rqsdk/testing.py`

 * *Files identical despite different names*

### Comparing `rqsdk-1.5.2/rqsdk.egg-info/PKG-INFO` & `rqsdk-1.5.3/rqsdk.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rqsdk
-Version: 1.5.2
+Version: 1.5.3
 Summary: Ricequant Native SDK
 Home-page: https://www.ricequant.com/
 Author: Ricequant
 Author-email: public@ricequant.com
 License: UNKNOWN
 Keywords: rqsdk
 Platform: UNKNOWN
```

### Comparing `rqsdk-1.5.2/rqsdk.egg-info/requires.txt` & `rqsdk-1.5.3/rqsdk.egg-info/requires.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-requests
 tabulate
-rqdatac>=2.9.44
 wcwidth
-patsy>=0.5.1
-rqdatac_fund==1.0.*,>=1.0.18
-statsmodels>=0.12.1
+requests
 click>=7.0
-pandas>=0.24.2
 pyjwt==1.7.1
+pandas>=0.24.2
+statsmodels>=0.12.1
+rqdatac_fund==1.0.*,>=1.0.18
+patsy>=0.5.1
+rqdatac>=2.9.44
 
 [:python_version <= "3.6"]
-cryptography==2.9.2
 python-rapidjson<=1.5
 numpy>=1.19.5
+cryptography==2.9.2
 
 [:python_version <= "3.7"]
 scipy<=1.7.3
 
 [:python_version == "3.7"]
 numpy>=1.20.0
 
@@ -24,40 +24,40 @@
 pyopenssl>22.0.0
 
 [:python_version >= "3.8"]
 numpy>=1.23.0
 scipy<=1.10.1,>=1.8.0
 
 [rqalpha_plus]
-rqalpha-mod-spot==1.0.9
-rqalpha-plus==4.2.4
+rqalpha-mod-ricequant-data==2.4.0
+h5py>=3.0.0
+rqalpha-mod-rqfactor==1.0.10
 rqalpha-mod-option==1.1.23
 tabulate
-rqalpha-mod-ricequant-data==2.4.0
-rqdatac>=2.9.44
-rqalpha-mod-fund==0.0.12
+requests
+rqalpha-mod-convertible==1.2.15
+ta-lib>=0.4.20
 rqdatac_fund==1.0.*,>=1.0.18
-statsmodels>=0.12.1
-rqalpha-mod-rqfactor==1.0.10
 matplotlib>=3.1.0
+rqrisk==1.0.7
+rqalpha-plus==4.2.4
 rqalpha==5.1.1
-rqalpha-mod-optimizer2==1.0.8
+patsy>=0.5.1
+rqalpha-mod-fund==0.0.13
 rqfactor==1.3.*,>=1.3.1
-requests
-rqalpha-mod-incremental==0.0.8
-rqalpha-mod-convertible==1.2.15
-h5py>=3.0.0
+rqalpha-mod-optimizer2==1.0.8
 hdf5plugin
-rqrisk==1.0.7
-ta-lib>=0.4.20
 wcwidth
-patsy>=0.5.1
-pandas>=0.24.2
 click>=7.0
 pyjwt==1.7.1
+pandas>=0.24.2
+rqalpha-mod-incremental==0.0.8
+rqalpha-mod-spot==1.0.9
+statsmodels>=0.12.1
+rqdatac>=2.9.44
 
 [rqalpha_plus:python_version <= "3.6"]
 python-rapidjson<=1.5
 numpy>=1.19.5
 cryptography==2.9.2
 
 [rqalpha_plus:python_version <= "3.7"]
@@ -66,33 +66,33 @@
 [rqalpha_plus:python_version == "3.7"]
 numpy>=1.20.0
 
 [rqalpha_plus:python_version > "3.7"]
 pyopenssl>22.0.0
 
 [rqalpha_plus:python_version >= "3.8"]
-scipy<=1.10.1,>=1.8.0
 numpy>=1.23.0
+scipy<=1.10.1,>=1.8.0
 
 [rqdatac]
-requests
 tabulate
-rqdatac>=2.9.44
 wcwidth
-patsy>=0.5.1
-rqdatac_fund==1.0.*,>=1.0.18
-statsmodels>=0.12.1
+requests
 click>=7.0
-pandas>=0.24.2
 pyjwt==1.7.1
+pandas>=0.24.2
+statsmodels>=0.12.1
+rqdatac_fund==1.0.*,>=1.0.18
+patsy>=0.5.1
+rqdatac>=2.9.44
 
 [rqdatac:python_version <= "3.6"]
-cryptography==2.9.2
 python-rapidjson<=1.5
 numpy>=1.19.5
+cryptography==2.9.2
 
 [rqdatac:python_version <= "3.7"]
 scipy<=1.7.3
 
 [rqdatac:python_version == "3.7"]
 numpy>=1.20.0
 
@@ -101,25 +101,25 @@
 
 [rqdatac:python_version >= "3.8"]
 numpy>=1.23.0
 scipy<=1.10.1,>=1.8.0
 
 [rqfactor]
 tabulate
-rqdatac>=2.9.44
-rqdatac_fund==1.0.*,>=1.0.18
-statsmodels>=0.12.1
-rqfactor==1.3.*,>=1.3.1
 requests
 ta-lib>=0.4.20
-wcwidth
+rqdatac_fund==1.0.*,>=1.0.18
 patsy>=0.5.1
-pandas>=0.24.2
+rqfactor==1.3.*,>=1.3.1
+wcwidth
 click>=7.0
 pyjwt==1.7.1
+pandas>=0.24.2
+statsmodels>=0.12.1
+rqdatac>=2.9.44
 
 [rqfactor:python_version <= "3.6"]
 python-rapidjson<=1.5
 numpy>=1.19.5
 cryptography==2.9.2
 
 [rqfactor:python_version <= "3.7"]
@@ -128,33 +128,33 @@
 [rqfactor:python_version == "3.7"]
 numpy>=1.20.0
 
 [rqfactor:python_version > "3.7"]
 pyopenssl>22.0.0
 
 [rqfactor:python_version >= "3.8"]
-scipy<=1.10.1,>=1.8.0
 numpy>=1.23.0
+scipy<=1.10.1,>=1.8.0
 
 [rqoptimizer]
-ecos==2.0.10
-rqoptimizer2==1.2.*,>=1.2.17
+scs==2.1.4
 tabulate
-rqdatac>=2.9.44
+ecos==2.0.10
+requests
 rqdatac_fund==1.0.*,>=1.0.18
-statsmodels>=0.12.1
+patsy>=0.5.1
 rqoptimizer==1.2.*,>=1.2.17
-requests
 osqp==0.6.2.post5
-scs==2.1.4
 wcwidth
-patsy>=0.5.1
-pandas>=0.24.2
 click>=7.0
 pyjwt==1.7.1
+pandas>=0.24.2
+rqoptimizer2==1.2.*,>=1.2.17
+statsmodels>=0.12.1
+rqdatac>=2.9.44
 
 [rqoptimizer:python_version <= "3.6"]
 python-rapidjson<=1.5
 numpy>=1.19.5
 cryptography==2.9.2
 
 [rqoptimizer:python_version <= "3.7"]
@@ -169,29 +169,29 @@
 [rqoptimizer:python_version > "3.7"]
 pyopenssl>22.0.0
 
 [rqoptimizer:python_version >= "3.7"]
 cvxpy==1.2.0
 
 [rqoptimizer:python_version >= "3.8"]
-scipy<=1.10.1,>=1.8.0
 numpy>=1.23.0
+scipy<=1.10.1,>=1.8.0
 
 [rqpattr]
 tabulate
-rqdatac>=2.9.44
-rqpattr>=0.0.2
-rqdatac_fund==1.0.*,>=1.0.18
-statsmodels>=0.12.1
 requests
-wcwidth
+rqdatac_fund==1.0.*,>=1.0.18
+rqpattr>=0.0.2
 patsy>=0.5.1
-pandas>=0.24.2
+wcwidth
 click>=7.0
 pyjwt==1.7.1
+pandas>=0.24.2
+statsmodels>=0.12.1
+rqdatac>=2.9.44
 
 [rqpattr:python_version <= "3.6"]
 python-rapidjson<=1.5
 numpy>=1.19.5
 cryptography==2.9.2
 
 [rqpattr:python_version <= "3.7"]
@@ -200,9 +200,9 @@
 [rqpattr:python_version == "3.7"]
 numpy>=1.20.0
 
 [rqpattr:python_version > "3.7"]
 pyopenssl>22.0.0
 
 [rqpattr:python_version >= "3.8"]
-scipy<=1.10.1,>=1.8.0
 numpy>=1.23.0
+scipy<=1.10.1,>=1.8.0
```

### Comparing `rqsdk-1.5.2/setup.py` & `rqsdk-1.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     "rqalpha==5.1.1",
     "rqalpha-mod-option==1.1.23",
     "rqalpha-mod-optimizer2==1.0.8",
     "rqalpha-mod-convertible==1.2.15",
     "rqalpha-mod-ricequant-data==2.4.0",
     "rqalpha-mod-rqfactor==1.0.10",
     "rqalpha-mod-spot==1.0.9",
-    "rqalpha-mod-fund==0.0.12",
+    "rqalpha-mod-fund==0.0.13",
     "rqalpha-mod-incremental==0.0.8",
     "rqalpha-plus==4.2.4",
     "rqrisk==1.0.7",
     "h5py>=3.0.0",
     "hdf5plugin",
     "matplotlib>=3.1.0",
 }
```

### Comparing `rqsdk-1.5.2/versioneer.py` & `rqsdk-1.5.3/versioneer.py`

 * *Files identical despite different names*

