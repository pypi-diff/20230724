# Comparing `tmp/awsso-0.3.8.tar.gz` & `tmp/awsso-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awsso-0.3.8.tar", last modified: Thu Jul 13 06:20:04 2023, max compression
+gzip compressed data, was "awsso-0.3.9.tar", last modified: Thu Jul 13 06:41:01 2023, max compression
```

## Comparing `awsso-0.3.8.tar` & `awsso-0.3.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 hanpenny   (501) staff       (20)        0 2023-07-13 06:20:04.842235 awsso-0.3.8/
--rw-r--r--   0 hanpenny   (501) staff       (20)     1028 2023-07-13 06:20:04.841743 awsso-0.3.8/PKG-INFO
--rw-r--r--   0 hanpenny   (501) staff       (20)      611 2023-02-06 15:29:04.000000 awsso-0.3.8/README.md
-drwxr-xr-x   0 hanpenny   (501) staff       (20)        0 2023-07-13 06:20:04.837230 awsso-0.3.8/awsso/
--rw-r--r--   0 hanpenny   (501) staff       (20)        0 2023-02-06 14:12:11.000000 awsso-0.3.8/awsso/__init__.py
--rwxr-xr-x   0 hanpenny   (501) staff       (20)    32318 2023-07-13 06:19:31.000000 awsso-0.3.8/awsso/awsso.py
-drwxr-xr-x   0 hanpenny   (501) staff       (20)        0 2023-07-13 06:20:04.841126 awsso-0.3.8/awsso.egg-info/
--rw-r--r--   0 hanpenny   (501) staff       (20)     1028 2023-07-13 06:20:04.000000 awsso-0.3.8/awsso.egg-info/PKG-INFO
--rw-r--r--   0 hanpenny   (501) staff       (20)      227 2023-07-13 06:20:04.000000 awsso-0.3.8/awsso.egg-info/SOURCES.txt
--rw-r--r--   0 hanpenny   (501) staff       (20)        1 2023-07-13 06:20:04.000000 awsso-0.3.8/awsso.egg-info/dependency_links.txt
--rw-r--r--   0 hanpenny   (501) staff       (20)       43 2023-07-13 06:20:04.000000 awsso-0.3.8/awsso.egg-info/entry_points.txt
--rw-r--r--   0 hanpenny   (501) staff       (20)       60 2023-07-13 06:20:04.000000 awsso-0.3.8/awsso.egg-info/requires.txt
--rw-r--r--   0 hanpenny   (501) staff       (20)        6 2023-07-13 06:20:04.000000 awsso-0.3.8/awsso.egg-info/top_level.txt
--rw-r--r--   0 hanpenny   (501) staff       (20)       38 2023-07-13 06:20:04.842391 awsso-0.3.8/setup.cfg
--rw-r--r--   0 hanpenny   (501) staff       (20)      986 2023-07-13 06:04:51.000000 awsso-0.3.8/setup.py
+drwxr-xr-x   0 hanpenny   (501) staff       (20)        0 2023-07-13 06:41:01.193244 awsso-0.3.9/
+-rw-r--r--   0 hanpenny   (501) staff       (20)     1028 2023-07-13 06:41:01.193031 awsso-0.3.9/PKG-INFO
+-rw-r--r--   0 hanpenny   (501) staff       (20)      611 2023-02-06 15:29:04.000000 awsso-0.3.9/README.md
+drwxr-xr-x   0 hanpenny   (501) staff       (20)        0 2023-07-13 06:41:01.190718 awsso-0.3.9/awsso/
+-rw-r--r--   0 hanpenny   (501) staff       (20)        0 2023-02-06 14:12:11.000000 awsso-0.3.9/awsso/__init__.py
+-rwxr-xr-x   0 hanpenny   (501) staff       (20)    32947 2023-07-13 06:39:44.000000 awsso-0.3.9/awsso/awsso.py
+drwxr-xr-x   0 hanpenny   (501) staff       (20)        0 2023-07-13 06:41:01.192746 awsso-0.3.9/awsso.egg-info/
+-rw-r--r--   0 hanpenny   (501) staff       (20)     1028 2023-07-13 06:41:01.000000 awsso-0.3.9/awsso.egg-info/PKG-INFO
+-rw-r--r--   0 hanpenny   (501) staff       (20)      227 2023-07-13 06:41:01.000000 awsso-0.3.9/awsso.egg-info/SOURCES.txt
+-rw-r--r--   0 hanpenny   (501) staff       (20)        1 2023-07-13 06:41:01.000000 awsso-0.3.9/awsso.egg-info/dependency_links.txt
+-rw-r--r--   0 hanpenny   (501) staff       (20)       43 2023-07-13 06:41:01.000000 awsso-0.3.9/awsso.egg-info/entry_points.txt
+-rw-r--r--   0 hanpenny   (501) staff       (20)       60 2023-07-13 06:41:01.000000 awsso-0.3.9/awsso.egg-info/requires.txt
+-rw-r--r--   0 hanpenny   (501) staff       (20)        6 2023-07-13 06:41:01.000000 awsso-0.3.9/awsso.egg-info/top_level.txt
+-rw-r--r--   0 hanpenny   (501) staff       (20)       38 2023-07-13 06:41:01.193307 awsso-0.3.9/setup.cfg
+-rw-r--r--   0 hanpenny   (501) staff       (20)      986 2023-07-13 06:40:58.000000 awsso-0.3.9/setup.py
```

### Comparing `awsso-0.3.8/PKG-INFO` & `awsso-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsso
-Version: 0.3.8
+Version: 0.3.9
 Summary: aws command line tool
 Home-page: https://github.com/Hireteammate/tools.git
 Author: linhan
 Author-email: lynnpen@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `awsso-0.3.8/README.md` & `awsso-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `awsso-0.3.8/awsso/awsso.py` & `awsso-0.3.9/awsso/awsso.py`

 * *Files 1% similar despite different names*

```diff
@@ -708,44 +708,48 @@
             ForceDeleteWithoutRecovery=True
         )
         print(ret)
     else:
         print('The sm: {} will not be deleted'.format(keyword))
         sys.exit()
 
-def _ssm_search(keyword):
+def ssm_search(keyword, option='Contains'):
     client = boto3.client('ssm', region_name=CURRENT_REGION)
     _filter = [
         {
             'Key': 'Name',
-            'Option': 'Contains',
+            'Option': option,
             'Values': [ keyword ]
         }
     ]
     ret = client.describe_parameters(ParameterFilters=_filter, MaxResults=50)
     _ret_list = ret['Parameters']
     _next = ret.get('NextToken')
     while _next:
         ret_tmp = client.describe_parameters(ParameterFilters=_filter, MaxResults=50, NextToken=_next)
         _ret_list.extend(ret_tmp['Parameters'])
         _next = ret_tmp.get('NextToken')
 
     ret_list = [ i['Name'] for i in _ret_list ]
+    return ret_list
 
+def _ssm_search(keyword):
+    ret_list = ssm_search(keyword)
     if len(ret_list) == 0:
         print('Did not find any parameters.')
         sys.exit()
     questions = [
         inquirer.List(
             'name',
             message='Please select parameter',
             choices=ret_list
         ),
     ]
     answer = inquirer.prompt(questions)
+    client = boto3.client('ssm', region_name=CURRENT_REGION)
     ret = client.get_parameter(Name=answer['name'], WithDecryption=True)
     print(ret['Parameter']['Value'])
 
 def _ssm_get(keyword):
     client = boto3.client('ssm', region_name=CURRENT_REGION)
     try:
         ret = client.get_parameter(Name=keyword, WithDecryption=True)
@@ -754,20 +758,31 @@
         print('Get parameter error.')
         sys.exit(1)
 
 def _ssm_delete(keyword):
     client = boto3.client('ssm', region_name=CURRENT_REGION)
     data = input('Please confirm this deletion[y/n]: ')
     if data.strip().lower() == 'y':
-        print('The ssm: {} will be deleted'.format(keyword))
-        try:
-            ret = client.delete_parameter(Name=keyword)
-            print(ret)
-        except client.exceptions.ParameterNotFound:
-            print('Pamameter not found.')
+        if not keyword.endswith('/'):
+            print('The ssm: {} will be deleted'.format(keyword))
+            try:
+                ret = client.delete_parameter(Name=keyword)
+                print(ret)
+            except client.exceptions.ParameterNotFound:
+                print('Pamameter not found.')
+        else:
+            print('The ssm startswith {} will be deleted'.format(keyword))
+            ret_list = ssm_search(keyword, 'BeginsWith')
+            for r in ret_list:
+                print(r)
+            try:
+                ret = client.delete_parameters(Names=ret_list)
+                print(ret)
+            except client.exceptions.ParameterNotFound:
+                print('Pamameter not found.')
     else:
         print('Cancelled.')
         sys.exit()
 
 
 def _env_get(service):
```

### Comparing `awsso-0.3.8/awsso.egg-info/PKG-INFO` & `awsso-0.3.9/awsso.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsso
-Version: 0.3.8
+Version: 0.3.9
 Summary: aws command line tool
 Home-page: https://github.com/Hireteammate/tools.git
 Author: linhan
 Author-email: lynnpen@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `awsso-0.3.8/setup.py` & `awsso-0.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import awsso
 
 with open("README.md","r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="awsso",
-    version="0.3.8",
+    version="0.3.9",
     author="linhan",
     author_email="lynnpen@gmail.com",  
     description="aws command line tool",
     long_description=long_description, 
     long_description_content_type="text/markdown",
     url="https://github.com/Hireteammate/tools.git",
     packages=setuptools.find_packages(),
```

