# Comparing `tmp/smart_app_framework-2.2.0rc7-py3-none-any.whl.zip` & `tmp/smart_app_framework-2.2.0rc8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -325,11 +325,11 @@
 -rw-r--r--  2.0 unx     1325 b- defN 80-Jan-01 00:00 smart_kit/utils/cache.py
 -rw-r--r--  2.0 unx     3946 b- defN 80-Jan-01 00:00 smart_kit/utils/diff.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 smart_kit/utils/logger_writer/__init__.py
 -rw-r--r--  2.0 unx     3322 b- defN 80-Jan-01 00:00 smart_kit/utils/logger_writer/logger_formatter.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 smart_kit/utils/monitoring.py
 -rw-r--r--  2.0 unx      332 b- defN 80-Jan-01 00:00 smart_kit/utils/object_location.py
 -rw-r--r--  2.0 unx      320 b- defN 80-Jan-01 00:00 smart_kit/utils/picklable_mock.py
--rw-r--r--  2.0 unx    10823 b- defN 80-Jan-01 00:00 smart_app_framework-2.2.0rc7.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 smart_app_framework-2.2.0rc7.dist-info/WHEEL
-?rw-r--r--  2.0 unx    32268 b- defN 16-Jan-01 00:00 smart_app_framework-2.2.0rc7.dist-info/RECORD
-333 files, 986511 bytes uncompressed, 253742 bytes compressed:  74.3%
+-rw-r--r--  2.0 unx    10824 b- defN 80-Jan-01 00:00 smart_app_framework-2.2.0rc8.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 smart_app_framework-2.2.0rc8.dist-info/WHEEL
+?rw-r--r--  2.0 unx    32268 b- defN 16-Jan-01 00:00 smart_app_framework-2.2.0rc8.dist-info/RECORD
+333 files, 986512 bytes uncompressed, 253742 bytes compressed:  74.3%
```

## zipnote {}

```diff
@@ -984,17 +984,17 @@
 
 Filename: smart_kit/utils/object_location.py
 Comment: 
 
 Filename: smart_kit/utils/picklable_mock.py
 Comment: 
 
-Filename: smart_app_framework-2.2.0rc7.dist-info/METADATA
+Filename: smart_app_framework-2.2.0rc8.dist-info/METADATA
 Comment: 
 
-Filename: smart_app_framework-2.2.0rc7.dist-info/WHEEL
+Filename: smart_app_framework-2.2.0rc8.dist-info/WHEEL
 Comment: 
 
-Filename: smart_app_framework-2.2.0rc7.dist-info/RECORD
+Filename: smart_app_framework-2.2.0rc8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `smart_app_framework-2.2.0rc7.dist-info/METADATA` & `smart_app_framework-2.2.0rc8.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: smart-app-framework
-Version: 2.2.0rc7
+Version: 2.2.0rc8
 Summary: Python-фреймворк, который позволяет создавать смартапы для виртуальных ассистентов Салют.
 Author: Salute Developers
 Author-email: developer@sberdevices.ru
 Requires-Python: >=3.8.1,<3.12
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: ml
 Requires-Dist: Jinja2 (==3.0.3)
 Requires-Dist: PyYAML (==5.3)
-Requires-Dist: Twisted (==22.8.0)
 Requires-Dist: aiohttp (==3.8.4)
 Requires-Dist: boto (==2.49.0)
 Requires-Dist: cachetools (==5.3.0)
 Requires-Dist: confluent_kafka (==1.9.2) ; python_version < "3.11"
 Requires-Dist: confluent_kafka (==2.0.2) ; python_version >= "3.11.dev0" and python_version < "3.12.dev0"
 Requires-Dist: croniter (==1.3.7)
 Requires-Dist: dill (==0.3.6)
@@ -46,14 +45,15 @@
 Requires-Dist: tabulate (==0.9.0)
 Requires-Dist: tensorflow (==2.12.0) ; (sys_platform == "darwin" and platform_machine == "x86_64") and (extra == "ml")
 Requires-Dist: tensorflow (==2.12.0) ; (sys_platform == "linux" and platform_machine == "x86_64") and (extra == "ml")
 Requires-Dist: tensorflow-aarch64 (==2.12.0) ; (sys_platform == "linux" and platform_machine == "aarch64") and (extra == "ml")
 Requires-Dist: tensorflow-macos (==2.12.0) ; (sys_platform == "darwin" and platform_machine == "arm64") and (extra == "ml")
 Requires-Dist: timeout-decorator (==0.4.1)
 Requires-Dist: tqdm (==4.64.1)
+Requires-Dist: twisted (==22.10.0)
 Description-Content-Type: text/markdown
 
 # SmartApp Framework
 
 **SmartApp Framework** - это Python-фреймворк, который позволяет создавать смартапы для виртуальных ассистентов Салют.
```

## Comparing `smart_app_framework-2.2.0rc7.dist-info/RECORD` & `smart_app_framework-2.2.0rc8.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -324,10 +324,10 @@
 smart_kit/utils/cache.py,sha256=Lut5HMkfoeiRwCCnZoSHw7srWYn3Y0fD-hUJWckDBf8,1325
 smart_kit/utils/diff.py,sha256=UP2Zmp0VW4YZpDPe_lGQ-5L_wF5wd7J4B33kXyUINmQ,3946
 smart_kit/utils/logger_writer/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 smart_kit/utils/logger_writer/logger_formatter.py,sha256=n5N4FHjXyeZAASjVB2zhoOMsbnWiixI0OQsk4KkcDFg,3322
 smart_kit/utils/monitoring.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 smart_kit/utils/object_location.py,sha256=uJmTxBBeeyvwahiA1TMKr2rzDW9R1bh-FwK663zoBe4,332
 smart_kit/utils/picklable_mock.py,sha256=PxrgnKue58GFpVZMBGIQq36LPnITFzfNA21euCbfViE,320
-smart_app_framework-2.2.0rc7.dist-info/METADATA,sha256=H4tt4BBK19TO1GfaiHbChwDsxlN3uTfukmgM5VFBL1o,10823
-smart_app_framework-2.2.0rc7.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-smart_app_framework-2.2.0rc7.dist-info/RECORD,,
+smart_app_framework-2.2.0rc8.dist-info/METADATA,sha256=IwGzi60U0Y1sy4mKvNvxNBdjK0X-jS57bSzzEfCQnR0,10824
+smart_app_framework-2.2.0rc8.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+smart_app_framework-2.2.0rc8.dist-info/RECORD,,
```

