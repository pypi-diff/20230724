# Comparing `tmp/airflow-provider-sifflet-1.0.2.tar.gz` & `tmp/airflow-provider-sifflet-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow-provider-sifflet-1.0.2.tar", last modified: Fri Jul 21 09:37:08 2023, max compression
+gzip compressed data, was "airflow-provider-sifflet-1.0.3.tar", last modified: Mon Jul 24 16:59:02 2023, max compression
```

## Comparing `airflow-provider-sifflet-1.0.2.tar` & `airflow-provider-sifflet-1.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-21 09:37:08.241206 airflow-provider-sifflet-1.0.2/
--rw-r--r--   0 baptiste   (501) staff       (20)     2672 2023-07-21 09:37:08.241073 airflow-provider-sifflet-1.0.2/PKG-INFO
--rw-r--r--   0 baptiste   (501) staff       (20)     2059 2023-07-10 13:24:52.000000 airflow-provider-sifflet-1.0.2/README.md
-drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-21 09:37:08.239960 airflow-provider-sifflet-1.0.2/airflow_provider_sifflet.egg-info/
--rw-r--r--   0 baptiste   (501) staff       (20)     2672 2023-07-21 09:37:08.000000 airflow-provider-sifflet-1.0.2/airflow_provider_sifflet.egg-info/PKG-INFO
--rw-r--r--   0 baptiste   (501) staff       (20)      572 2023-07-21 09:37:08.000000 airflow-provider-sifflet-1.0.2/airflow_provider_sifflet.egg-info/SOURCES.txt
--rw-r--r--   0 baptiste   (501) staff       (20)        1 2023-07-21 09:37:08.000000 airflow-provider-sifflet-1.0.2/airflow_provider_sifflet.egg-info/dependency_links.txt
--rw-r--r--   0 baptiste   (501) staff       (20)       95 2023-07-21 09:37:08.000000 airflow-provider-sifflet-1.0.2/airflow_provider_sifflet.egg-info/entry_points.txt
--rw-r--r--   0 baptiste   (501) staff       (20)       65 2023-07-21 09:37:08.000000 airflow-provider-sifflet-1.0.2/airflow_provider_sifflet.egg-info/requires.txt
--rw-r--r--   0 baptiste   (501) staff       (20)       17 2023-07-21 09:37:08.000000 airflow-provider-sifflet-1.0.2/airflow_provider_sifflet.egg-info/top_level.txt
--rw-r--r--   0 baptiste   (501) staff       (20)      284 2022-08-11 16:27:52.000000 airflow-provider-sifflet-1.0.2/pyproject.toml
--rw-r--r--   0 baptiste   (501) staff       (20)       38 2023-07-21 09:37:08.241245 airflow-provider-sifflet-1.0.2/setup.cfg
--rw-r--r--   0 baptiste   (501) staff       (20)     1701 2023-07-20 17:15:24.000000 airflow-provider-sifflet-1.0.2/setup.py
-drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-21 09:37:08.240211 airflow-provider-sifflet-1.0.2/sifflet_provider/
--rw-r--r--   0 baptiste   (501) staff       (20)       27 2023-07-20 17:15:19.000000 airflow-provider-sifflet-1.0.2/sifflet_provider/__init__.py
--rw-r--r--   0 baptiste   (501) staff       (20)      904 2023-01-16 14:54:26.000000 airflow-provider-sifflet-1.0.2/sifflet_provider/get_provider_info.py
-drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-21 09:37:08.240471 airflow-provider-sifflet-1.0.2/sifflet_provider/hooks/
--rw-r--r--   0 baptiste   (501) staff       (20)        0 2022-08-11 16:27:52.000000 airflow-provider-sifflet-1.0.2/sifflet_provider/hooks/__init__.py
--rw-r--r--   0 baptiste   (501) staff       (20)     1674 2023-07-20 17:15:19.000000 airflow-provider-sifflet-1.0.2/sifflet_provider/hooks/sifflet_hook.py
-drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-21 09:37:08.240859 airflow-provider-sifflet-1.0.2/sifflet_provider/operators/
--rw-r--r--   0 baptiste   (501) staff       (20)        0 2022-08-11 16:27:52.000000 airflow-provider-sifflet-1.0.2/sifflet_provider/operators/__init__.py
--rw-r--r--   0 baptiste   (501) staff       (20)     1780 2023-07-20 17:15:19.000000 airflow-provider-sifflet-1.0.2/sifflet_provider/operators/dbt.py
--rw-r--r--   0 baptiste   (501) staff       (20)     1331 2023-07-20 17:15:19.000000 airflow-provider-sifflet-1.0.2/sifflet_provider/operators/rule.py
+drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-24 16:59:02.243856 airflow-provider-sifflet-1.0.3/
+-rw-r--r--   0 baptiste   (501) staff       (20)     2672 2023-07-24 16:59:02.243705 airflow-provider-sifflet-1.0.3/PKG-INFO
+-rw-r--r--   0 baptiste   (501) staff       (20)     2059 2023-07-10 13:24:52.000000 airflow-provider-sifflet-1.0.3/README.md
+drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-24 16:59:02.242630 airflow-provider-sifflet-1.0.3/airflow_provider_sifflet.egg-info/
+-rw-r--r--   0 baptiste   (501) staff       (20)     2672 2023-07-24 16:59:02.000000 airflow-provider-sifflet-1.0.3/airflow_provider_sifflet.egg-info/PKG-INFO
+-rw-r--r--   0 baptiste   (501) staff       (20)      572 2023-07-24 16:59:02.000000 airflow-provider-sifflet-1.0.3/airflow_provider_sifflet.egg-info/SOURCES.txt
+-rw-r--r--   0 baptiste   (501) staff       (20)        1 2023-07-24 16:59:02.000000 airflow-provider-sifflet-1.0.3/airflow_provider_sifflet.egg-info/dependency_links.txt
+-rw-r--r--   0 baptiste   (501) staff       (20)       95 2023-07-24 16:59:02.000000 airflow-provider-sifflet-1.0.3/airflow_provider_sifflet.egg-info/entry_points.txt
+-rw-r--r--   0 baptiste   (501) staff       (20)       65 2023-07-24 16:59:02.000000 airflow-provider-sifflet-1.0.3/airflow_provider_sifflet.egg-info/requires.txt
+-rw-r--r--   0 baptiste   (501) staff       (20)       17 2023-07-24 16:59:02.000000 airflow-provider-sifflet-1.0.3/airflow_provider_sifflet.egg-info/top_level.txt
+-rw-r--r--   0 baptiste   (501) staff       (20)      284 2022-08-11 16:27:52.000000 airflow-provider-sifflet-1.0.3/pyproject.toml
+-rw-r--r--   0 baptiste   (501) staff       (20)       38 2023-07-24 16:59:02.243902 airflow-provider-sifflet-1.0.3/setup.cfg
+-rw-r--r--   0 baptiste   (501) staff       (20)     1701 2023-07-24 16:57:17.000000 airflow-provider-sifflet-1.0.3/setup.py
+drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-24 16:59:02.242894 airflow-provider-sifflet-1.0.3/sifflet_provider/
+-rw-r--r--   0 baptiste   (501) staff       (20)       27 2023-07-24 16:57:07.000000 airflow-provider-sifflet-1.0.3/sifflet_provider/__init__.py
+-rw-r--r--   0 baptiste   (501) staff       (20)      904 2023-01-16 14:54:26.000000 airflow-provider-sifflet-1.0.3/sifflet_provider/get_provider_info.py
+drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-24 16:59:02.243131 airflow-provider-sifflet-1.0.3/sifflet_provider/hooks/
+-rw-r--r--   0 baptiste   (501) staff       (20)        0 2022-08-11 16:27:52.000000 airflow-provider-sifflet-1.0.3/sifflet_provider/hooks/__init__.py
+-rw-r--r--   0 baptiste   (501) staff       (20)     1674 2023-07-24 14:37:03.000000 airflow-provider-sifflet-1.0.3/sifflet_provider/hooks/sifflet_hook.py
+drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-24 16:59:02.243506 airflow-provider-sifflet-1.0.3/sifflet_provider/operators/
+-rw-r--r--   0 baptiste   (501) staff       (20)        0 2022-08-11 16:27:52.000000 airflow-provider-sifflet-1.0.3/sifflet_provider/operators/__init__.py
+-rw-r--r--   0 baptiste   (501) staff       (20)     1780 2023-07-24 14:37:03.000000 airflow-provider-sifflet-1.0.3/sifflet_provider/operators/dbt.py
+-rw-r--r--   0 baptiste   (501) staff       (20)     1331 2023-07-24 14:37:03.000000 airflow-provider-sifflet-1.0.3/sifflet_provider/operators/rule.py
```

### Comparing `airflow-provider-sifflet-1.0.2/PKG-INFO` & `airflow-provider-sifflet-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-provider-sifflet
-Version: 1.0.2
+Version: 1.0.3
 Summary: Provider package airflow-provider-sifflet for Apache Airflow
 Home-page: https://www.siffletdata.com/
 Author: Sifflet
 Author-email: support@siffletdata.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `airflow-provider-sifflet-1.0.2/README.md` & `airflow-provider-sifflet-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `airflow-provider-sifflet-1.0.2/airflow_provider_sifflet.egg-info/PKG-INFO` & `airflow-provider-sifflet-1.0.3/airflow_provider_sifflet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-provider-sifflet
-Version: 1.0.2
+Version: 1.0.3
 Summary: Provider package airflow-provider-sifflet for Apache Airflow
 Home-page: https://www.siffletdata.com/
 Author: Sifflet
 Author-email: support@siffletdata.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `airflow-provider-sifflet-1.0.2/airflow_provider_sifflet.egg-info/SOURCES.txt` & `airflow-provider-sifflet-1.0.3/airflow_provider_sifflet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `airflow-provider-sifflet-1.0.2/setup.py` & `airflow-provider-sifflet-1.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         name="airflow-provider-sifflet",
         description="Provider package airflow-provider-sifflet for Apache Airflow",
         version=sifflet_provider.__version__,
         long_description=long_description,
         long_description_content_type="text/markdown",
         license="Apache License 2.0",
         packages=find_packages(include=["sifflet_provider", "sifflet_provider.*"]),
-        install_requires=["sifflet-sdk>=0.3.0"],
+        install_requires=["sifflet-sdk>=0.3.1"],
         setup_requires=["setuptools", "wheel"],
         author="Sifflet",
         author_email="support@siffletdata.com",
         url="https://www.siffletdata.com/",
         classifiers=[
             "Development Status :: 4 - Beta",
             "Environment :: Console",
```

### Comparing `airflow-provider-sifflet-1.0.2/sifflet_provider/get_provider_info.py` & `airflow-provider-sifflet-1.0.3/sifflet_provider/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-sifflet-1.0.2/sifflet_provider/hooks/sifflet_hook.py` & `airflow-provider-sifflet-1.0.3/sifflet_provider/hooks/sifflet_hook.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-sifflet-1.0.2/sifflet_provider/operators/dbt.py` & `airflow-provider-sifflet-1.0.3/sifflet_provider/operators/dbt.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-sifflet-1.0.2/sifflet_provider/operators/rule.py` & `airflow-provider-sifflet-1.0.3/sifflet_provider/operators/rule.py`

 * *Files identical despite different names*

