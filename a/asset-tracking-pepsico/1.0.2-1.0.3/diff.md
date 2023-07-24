# Comparing `tmp/asset_tracking_pepsico-1.0.2.tar.gz` & `tmp/asset_tracking_pepsico-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asset_tracking_pepsico-1.0.2.tar", last modified: Tue Jul 11 10:51:07 2023, max compression
+gzip compressed data, was "asset_tracking_pepsico-1.0.3.tar", last modified: Mon Jul 24 08:34:03 2023, max compression
```

## Comparing `asset_tracking_pepsico-1.0.2.tar` & `asset_tracking_pepsico-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-07-11 10:51:07.833849 asset_tracking_pepsico-1.0.2/
--rw-r--r--   0 jatintalati   (501) staff       (20)     1070 2023-01-19 18:18:48.000000 asset_tracking_pepsico-1.0.2/LICENSE
--rw-r--r--   0 jatintalati   (501) staff       (20)     1593 2023-07-11 10:51:07.833459 asset_tracking_pepsico-1.0.2/PKG-INFO
--rw-r--r--   0 jatintalati   (501) staff       (20)     1015 2023-05-31 14:48:14.000000 asset_tracking_pepsico-1.0.2/README.md
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-07-11 10:51:07.828903 asset_tracking_pepsico-1.0.2/asset_tracking_pepsico/
--rw-r--r--   0 jatintalati   (501) staff       (20)     6750 2023-07-11 10:47:36.000000 asset_tracking_pepsico-1.0.2/asset_tracking_pepsico/asset_tracking_devicelogs.py
--rw-r--r--   0 jatintalati   (501) staff       (20)     4877 2023-07-11 10:45:08.000000 asset_tracking_pepsico-1.0.2/asset_tracking_pepsico/asset_tracking_ingest.py
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-07-11 10:51:07.832953 asset_tracking_pepsico-1.0.2/asset_tracking_pepsico/dto/
--rw-r--r--   0 jatintalati   (501) staff       (20)     6794 2023-07-11 10:46:24.000000 asset_tracking_pepsico-1.0.2/asset_tracking_pepsico/dto/PostgresSchema.py
--rw-r--r--   0 jatintalati   (501) staff       (20)     1332 2023-07-03 06:34:17.000000 asset_tracking_pepsico-1.0.2/asset_tracking_pepsico/utilities.py
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-07-11 10:51:07.832435 asset_tracking_pepsico-1.0.2/asset_tracking_pepsico.egg-info/
--rw-r--r--   0 jatintalati   (501) staff       (20)     1593 2023-07-11 10:51:07.000000 asset_tracking_pepsico-1.0.2/asset_tracking_pepsico.egg-info/PKG-INFO
--rw-r--r--   0 jatintalati   (501) staff       (20)      442 2023-07-11 10:51:07.000000 asset_tracking_pepsico-1.0.2/asset_tracking_pepsico.egg-info/SOURCES.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)        1 2023-07-11 10:51:07.000000 asset_tracking_pepsico-1.0.2/asset_tracking_pepsico.egg-info/dependency_links.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)       35 2023-07-11 10:51:07.000000 asset_tracking_pepsico-1.0.2/asset_tracking_pepsico.egg-info/requires.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)       23 2023-07-11 10:51:07.000000 asset_tracking_pepsico-1.0.2/asset_tracking_pepsico.egg-info/top_level.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)      748 2023-07-11 10:48:26.000000 asset_tracking_pepsico-1.0.2/pyproject.toml
--rw-r--r--   0 jatintalati   (501) staff       (20)       38 2023-07-11 10:51:07.834030 asset_tracking_pepsico-1.0.2/setup.cfg
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-07-24 08:34:03.077003 asset_tracking_pepsico-1.0.3/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1070 2023-01-19 18:18:48.000000 asset_tracking_pepsico-1.0.3/LICENSE
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1593 2023-07-24 08:34:03.076281 asset_tracking_pepsico-1.0.3/PKG-INFO
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1015 2023-05-31 14:48:14.000000 asset_tracking_pepsico-1.0.3/README.md
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-07-24 08:34:03.070009 asset_tracking_pepsico-1.0.3/asset_tracking_pepsico/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     6750 2023-07-11 10:47:36.000000 asset_tracking_pepsico-1.0.3/asset_tracking_pepsico/asset_tracking_devicelogs.py
+-rw-r--r--   0 jatintalati   (501) staff       (20)     5304 2023-07-24 08:26:52.000000 asset_tracking_pepsico-1.0.3/asset_tracking_pepsico/asset_tracking_ingest.py
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-07-24 08:34:03.075353 asset_tracking_pepsico-1.0.3/asset_tracking_pepsico/dto/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     6794 2023-07-11 10:46:24.000000 asset_tracking_pepsico-1.0.3/asset_tracking_pepsico/dto/PostgresSchema.py
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1332 2023-07-03 06:34:17.000000 asset_tracking_pepsico-1.0.3/asset_tracking_pepsico/utilities.py
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-07-24 08:34:03.074567 asset_tracking_pepsico-1.0.3/asset_tracking_pepsico.egg-info/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1593 2023-07-24 08:34:03.000000 asset_tracking_pepsico-1.0.3/asset_tracking_pepsico.egg-info/PKG-INFO
+-rw-r--r--   0 jatintalati   (501) staff       (20)      442 2023-07-24 08:34:03.000000 asset_tracking_pepsico-1.0.3/asset_tracking_pepsico.egg-info/SOURCES.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)        1 2023-07-24 08:34:03.000000 asset_tracking_pepsico-1.0.3/asset_tracking_pepsico.egg-info/dependency_links.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)       35 2023-07-24 08:34:03.000000 asset_tracking_pepsico-1.0.3/asset_tracking_pepsico.egg-info/requires.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)       23 2023-07-24 08:34:03.000000 asset_tracking_pepsico-1.0.3/asset_tracking_pepsico.egg-info/top_level.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)      748 2023-07-24 08:32:48.000000 asset_tracking_pepsico-1.0.3/pyproject.toml
+-rw-r--r--   0 jatintalati   (501) staff       (20)       38 2023-07-24 08:34:03.077343 asset_tracking_pepsico-1.0.3/setup.cfg
```

### Comparing `asset_tracking_pepsico-1.0.2/LICENSE` & `asset_tracking_pepsico-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `asset_tracking_pepsico-1.0.2/PKG-INFO` & `asset_tracking_pepsico-1.0.3/asset_tracking_pepsico.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: asset_tracking_pepsico
-Version: 1.0.2
+Name: asset-tracking-pepsico
+Version: 1.0.3
 Summary: An asset tracking package where the device logs can be read and the location information can be extracted from the log file provided in the parameters.
 Author-email: Jatin Talati <jatalati@in.ibm.com>
 Keywords: asset,tracking,pepsico,location,latitude,longitude,store,events
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `asset_tracking_pepsico-1.0.2/README.md` & `asset_tracking_pepsico-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `asset_tracking_pepsico-1.0.2/asset_tracking_pepsico/asset_tracking_devicelogs.py` & `asset_tracking_pepsico-1.0.3/asset_tracking_pepsico/asset_tracking_devicelogs.py`

 * *Files identical despite different names*

### Comparing `asset_tracking_pepsico-1.0.2/asset_tracking_pepsico/asset_tracking_ingest.py` & `asset_tracking_pepsico-1.0.3/asset_tracking_pepsico/asset_tracking_ingest.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,14 +76,24 @@
             except KeyError:
                 route = None
             version = properties['Version']
             return object_id, emp_name, lat, long, acc, event_desc, transition, route, version, loc_desc, loc_id
         except KeyError:
             traceback.print_exc()
 
+    def filter_properties(self, properties_dict):
+        try:
+            for key in properties_dict:
+                item = properties_dict[key]
+                item = item.replace("'", "").replace(":", "").replace(",", "")
+                properties_dict[key] = item
+        except:
+            traceback.print_exc()
+        return properties_dict
+
     def create_schema_list(self, df, object_type, data_source, schema_version):
         try:
             schema_list = []
             for idx, item in df.iterrows():
                 if item['EventName'] == 'CrashDiagnostics' or item['EventName'] == '':
                     continue
                 object_id, emp_name, lat, long, acc, event_desc, transition, route, version, loc_desc, loc_id = \
@@ -102,14 +112,16 @@
                     'OsVersion': item['OsVersion'],
                     'Transition': transition,
                     'Version': version,
                     'EventId': item['EventId'],
                     'Description': event_desc
                 }
 
+                properties_dict = self.filter_properties(properties_dict)
+
                 schema = PostgresSchemaDto(schema_version=schema_version, object_id=object_id, object_type=object_type, event_type=event,
                                            location_hint=loc_desc, location_id=loc_id, object_latitude=lat, object_longitude=long,
                                            created_ts=times, lat_long_acc=acc, datasource=data_source,
                                            properties_dict=str(properties_dict), routeid=route)
                 schema_list.append(schema)
             return schema_list
         except:
```

### Comparing `asset_tracking_pepsico-1.0.2/asset_tracking_pepsico/dto/PostgresSchema.py` & `asset_tracking_pepsico-1.0.3/asset_tracking_pepsico/dto/PostgresSchema.py`

 * *Files identical despite different names*

### Comparing `asset_tracking_pepsico-1.0.2/asset_tracking_pepsico/utilities.py` & `asset_tracking_pepsico-1.0.3/asset_tracking_pepsico/utilities.py`

 * *Files identical despite different names*

### Comparing `asset_tracking_pepsico-1.0.2/asset_tracking_pepsico.egg-info/PKG-INFO` & `asset_tracking_pepsico-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: asset-tracking-pepsico
-Version: 1.0.2
+Name: asset_tracking_pepsico
+Version: 1.0.3
 Summary: An asset tracking package where the device logs can be read and the location information can be extracted from the log file provided in the parameters.
 Author-email: Jatin Talati <jatalati@in.ibm.com>
 Keywords: asset,tracking,pepsico,location,latitude,longitude,store,events
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `asset_tracking_pepsico-1.0.2/pyproject.toml` & `asset_tracking_pepsico-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "asset_tracking_pepsico"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Jatin Talati", email="jatalati@in.ibm.com" },
 ]
 description = "An asset tracking package where the device logs can be read and the location information can be extracted from the log file provided in the parameters."
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["asset", "tracking", "pepsico", "location", "latitude", "longitude", "store", "events"]
```

