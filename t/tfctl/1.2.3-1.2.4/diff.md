# Comparing `tmp/tfctl-1.2.3.tar.gz` & `tmp/tfctl-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tfctl-1.2.3.tar", last modified: Tue May 17 12:51:20 2022, max compression
+gzip compressed data, was "tfctl-1.2.4.tar", last modified: Mon Jul 24 16:25:18 2023, max compression
```

## Comparing `tfctl-1.2.3.tar` & `tfctl-1.2.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 12:51:20.175848 tfctl-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-05-17 12:51:08.000000 tfctl-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      639 2022-05-17 12:51:20.175848 tfctl-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-05-17 12:51:08.000000 tfctl-1.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-17 12:51:20.175848 tfctl-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1046 2022-05-17 12:51:08.000000 tfctl-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 12:51:20.175848 tfctl-1.2.3/tfctl/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-17 12:51:08.000000 tfctl-1.2.3/tfctl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11002 2022-05-17 12:51:08.000000 tfctl-1.2.3/tfctl/tfctl.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 12:51:20.175848 tfctl-1.2.3/tfctl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      639 2022-05-17 12:51:20.000000 tfctl-1.2.3/tfctl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      235 2022-05-17 12:51:20.000000 tfctl-1.2.3/tfctl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-17 12:51:20.000000 tfctl-1.2.3/tfctl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-05-17 12:51:20.000000 tfctl-1.2.3/tfctl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-05-17 12:51:20.000000 tfctl-1.2.3/tfctl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-05-17 12:51:20.000000 tfctl-1.2.3/tfctl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:25:18.848650 tfctl-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-24 16:25:04.000000 tfctl-1.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-24 16:25:18.848650 tfctl-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-24 16:25:04.000000 tfctl-1.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 16:25:18.848650 tfctl-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-24 16:25:04.000000 tfctl-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:25:18.848650 tfctl-1.2.4/tfctl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:25:04.000000 tfctl-1.2.4/tfctl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11002 2023-07-24 16:25:04.000000 tfctl-1.2.4/tfctl/tfctl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:25:18.848650 tfctl-1.2.4/tfctl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-24 16:25:18.000000 tfctl-1.2.4/tfctl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-24 16:25:18.000000 tfctl-1.2.4/tfctl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 16:25:18.000000 tfctl-1.2.4/tfctl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-24 16:25:18.000000 tfctl-1.2.4/tfctl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-24 16:25:18.000000 tfctl-1.2.4/tfctl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-24 16:25:18.000000 tfctl-1.2.4/tfctl.egg-info/top_level.txt
```

### Comparing `tfctl-1.2.3/LICENSE` & `tfctl-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tfctl-1.2.3/PKG-INFO` & `tfctl-1.2.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 Metadata-Version: 2.1
 Name: tfctl
-Version: 1.2.3
+Version: 1.2.4
 Summary: A control tool for Hashicorp (c) Terraform projects
 Home-page: https://github.com/grauerwf/tfctl
 Author: Grauer W01f
 Author-email: grauerwf@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # tfctl
-
```

### Comparing `tfctl-1.2.3/setup.py` & `tfctl-1.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `tfctl-1.2.3/tfctl/tfctl.py` & `tfctl-1.2.4/tfctl/tfctl.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     COMPREPLY=( $(compgen -W "${env_names}" -- ${cur}) )
 }
 
 complete -F _show_complete tfctl
 '''
 
 user_home = os.path.expanduser('~')
-tf_version = '1.1.9'
+tf_version = '1.5.3'
 tf_arguments = ' '.join(sys.argv[3:])
 tf_base_dir = os.path.join(user_home, '.terraform')
 tf_bin_dir = os.path.join(tf_base_dir, 'bin')
 tf_bin = os.path.join(tf_bin_dir, 'terraform')
 tf_data_dir = os.path.join(tf_base_dir, 'data')
 tf_download_address_tpl = 'https://releases.hashicorp.com/terraform/' \
                           '{0}/terraform_{0}_{1}_{2}.zip'
```

### Comparing `tfctl-1.2.3/tfctl.egg-info/PKG-INFO` & `tfctl-1.2.4/tfctl.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 Metadata-Version: 2.1
 Name: tfctl
-Version: 1.2.3
+Version: 1.2.4
 Summary: A control tool for Hashicorp (c) Terraform projects
 Home-page: https://github.com/grauerwf/tfctl
 Author: Grauer W01f
 Author-email: grauerwf@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # tfctl
-
```

