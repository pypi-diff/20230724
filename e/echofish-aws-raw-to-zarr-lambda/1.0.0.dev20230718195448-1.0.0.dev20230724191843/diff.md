# Comparing `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230718195448.tar.gz` & `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724191843.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230718195448.tar", last modified: Tue Jul 18 19:55:52 2023, max compression
+gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724191843.tar", last modified: Mon Jul 24 19:19:47 2023, max compression
```

## Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230718195448.tar` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724191843.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 19:55:52.623814 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230718195448/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-07-18 19:54:43.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230718195448/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-18 19:55:52.623814 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230718195448/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2113 2023-07-18 19:54:43.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230718195448/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 19:55:52.623814 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230718195448/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      709 2023-07-18 19:55:48.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230718195448/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 19:55:52.619814 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230718195448/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 19:55:52.623814 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230718195448/src/echofish_aws_raw_to_zarr_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 19:54:43.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230718195448/src/echofish_aws_raw_to_zarr_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-07-18 19:54:43.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230718195448/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
--rw-r--r--   0 root         (0) root         (0)    15839 2023-07-18 19:54:43.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230718195448/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)     1302 2023-07-18 19:54:43.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230718195448/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
--rw-r--r--   0 root         (0) root         (0)     3398 2023-07-18 19:54:43.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230718195448/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
--rw-r--r--   0 root         (0) root         (0)      297 2023-07-18 19:54:43.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230718195448/src/echofish_aws_raw_to_zarr_lambda/sns_operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 19:55:52.623814 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230718195448/src/echofish_aws_raw_to_zarr_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-18 19:55:52.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230718195448/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      641 2023-07-18 19:55:52.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230718195448/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 19:55:52.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230718195448/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      139 2023-07-18 19:55:52.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230718195448/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-07-18 19:55:52.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230718195448/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:19:47.392298 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724191843/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-07-24 19:18:38.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724191843/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-24 19:19:47.392298 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724191843/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-07-24 19:18:38.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724191843/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 19:19:47.392298 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724191843/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      709 2023-07-24 19:19:42.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724191843/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:19:47.388298 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724191843/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:19:47.388298 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724191843/src/echofish_aws_raw_to_zarr_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 19:18:38.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724191843/src/echofish_aws_raw_to_zarr_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-07-24 19:18:38.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724191843/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
+-rw-r--r--   0 root         (0) root         (0)    15839 2023-07-24 19:18:38.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724191843/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1302 2023-07-24 19:18:38.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724191843/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
+-rw-r--r--   0 root         (0) root         (0)     3494 2023-07-24 19:18:38.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724191843/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
+-rw-r--r--   0 root         (0) root         (0)      297 2023-07-24 19:18:38.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724191843/src/echofish_aws_raw_to_zarr_lambda/sns_operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:19:47.392298 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724191843/src/echofish_aws_raw_to_zarr_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-24 19:19:47.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724191843/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      641 2023-07-24 19:19:47.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724191843/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 19:19:47.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724191843/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      139 2023-07-24 19:19:47.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724191843/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-24 19:19:47.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724191843/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230718195448/LICENSE` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724191843/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230718195448/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724191843/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230718195448
+Version: 1.0.0.dev20230724191843
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230718195448/README.md` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724191843/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230718195448/setup.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724191843/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-raw-to-zarr-lambda",
-  version="1.0.0.dev20230718195448",
+  version="1.0.0.dev20230724191843",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230718195448/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724191843/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230718195448/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724191843/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230718195448/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724191843/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230718195448/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724191843/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,20 +7,22 @@
     def __get_client(
             self,
             access_key_id=None,
             secret_access_key=None
     ):
         session = boto3.Session()
         if access_key_id:
+            print('access_key_id is present')
             s3_client = session.client(
                 service_name='s3',
                 aws_access_key_id=access_key_id,
                 aws_secret_access_key=secret_access_key
             )
         else:
+            print('access_key_id is not present')
             s3_client = session.client(service_name='s3')
         return s3_client
 
     #####################################################################
     def __chunked(
             self,
             ll: list,
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230718195448/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724191843/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230718195448
+Version: 1.0.0.dev20230724191843
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230718195448/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724191843/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

