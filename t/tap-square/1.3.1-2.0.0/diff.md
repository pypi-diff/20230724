# Comparing `tmp/tap-square-1.3.1.tar.gz` & `tmp/tap-square-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tap-square-1.3.1.tar", last modified: Thu Jun 10 18:07:07 2021, max compression
+gzip compressed data, was "tap-square-2.0.0.tar", last modified: Mon Jul 24 10:55:42 2023, max compression
```

## Comparing `tap-square-1.3.1.tar` & `tap-square-2.0.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2021-06-10 18:07:07.488882 tap-square-1.3.1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32393 2021-06-08 20:48:34.000000 tap-square-1.3.1/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       50 2021-06-08 20:48:34.000000 tap-square-1.3.1/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      292 2021-06-10 18:07:07.488882 tap-square-1.3.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5849 2021-06-08 20:48:34.000000 tap-square-1.3.1/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2021-06-10 18:07:07.488882 tap-square-1.3.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      888 2021-06-10 18:06:56.000000 tap-square-1.3.1/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2021-06-10 18:07:07.484882 tap-square-1.3.1/tap_square/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      628 2021-06-08 20:48:34.000000 tap-square-1.3.1/tap_square/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12123 2021-06-08 20:48:34.000000 tap-square-1.3.1/tap_square/client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1902 2021-06-08 20:48:34.000000 tap-square-1.3.1/tap_square/discover.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2021-06-10 18:07:07.488882 tap-square-1.3.1/tap_square/schemas/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1179 2021-06-08 20:48:34.000000 tap-square-1.3.1/tap_square/schemas/bank_accounts.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1186 2021-06-08 20:48:34.000000 tap-square-1.3.1/tap_square/schemas/cash_drawer_shifts.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1005 2021-06-08 20:48:34.000000 tap-square-1.3.1/tap_square/schemas/categories.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2220 2021-06-08 20:48:34.000000 tap-square-1.3.1/tap_square/schemas/customers.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2081 2021-06-08 20:48:34.000000 tap-square-1.3.1/tap_square/schemas/discounts.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      954 2021-06-08 20:48:34.000000 tap-square-1.3.1/tap_square/schemas/employees.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      613 2021-06-08 20:48:34.000000 tap-square-1.3.1/tap_square/schemas/inventories.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8268 2021-06-08 20:48:34.000000 tap-square-1.3.1/tap_square/schemas/items.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5003 2021-06-08 20:48:34.000000 tap-square-1.3.1/tap_square/schemas/locations.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3871 2021-06-08 20:48:34.000000 tap-square-1.3.1/tap_square/schemas/modifier_lists.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    35425 2021-06-10 13:50:46.000000 tap-square-1.3.1/tap_square/schemas/orders.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7100 2021-06-08 20:48:34.000000 tap-square-1.3.1/tap_square/schemas/payments.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2037 2021-06-08 20:48:34.000000 tap-square-1.3.1/tap_square/schemas/refunds.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      705 2021-06-08 20:48:34.000000 tap-square-1.3.1/tap_square/schemas/roles.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1322 2021-06-08 20:48:34.000000 tap-square-1.3.1/tap_square/schemas/settlements.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2722 2021-06-08 20:48:34.000000 tap-square-1.3.1/tap_square/schemas/shifts.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1785 2021-06-08 20:48:34.000000 tap-square-1.3.1/tap_square/schemas/taxes.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15240 2021-06-08 20:48:34.000000 tap-square-1.3.1/tap_square/streams.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1168 2021-06-08 20:48:34.000000 tap-square-1.3.1/tap_square/sync.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2021-06-10 18:07:07.484882 tap-square-1.3.1/tap_square.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      292 2021-06-10 18:07:07.000000 tap-square-1.3.1/tap_square.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      942 2021-06-10 18:07:07.000000 tap-square-1.3.1/tap_square.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2021-06-10 18:07:07.000000 tap-square-1.3.1/tap_square.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       72 2021-06-10 18:07:07.000000 tap-square-1.3.1/tap_square.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      112 2021-06-10 18:07:07.000000 tap-square-1.3.1/tap_square.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2021-06-10 18:07:07.000000 tap-square-1.3.1/tap_square.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-24 10:55:42.073953 tap-square-2.0.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32393 2023-06-02 15:01:54.000000 tap-square-2.0.0/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       50 2023-06-02 15:01:54.000000 tap-square-2.0.0/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      258 2023-07-24 10:55:42.073953 tap-square-2.0.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5851 2023-07-24 10:47:44.000000 tap-square-2.0.0/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-07-24 10:55:42.073953 tap-square-2.0.0/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      883 2023-07-24 10:47:44.000000 tap-square-2.0.0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-24 10:55:42.069953 tap-square-2.0.0/tap_square/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      648 2023-07-24 10:47:44.000000 tap-square-2.0.0/tap_square/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12224 2023-07-24 10:47:44.000000 tap-square-2.0.0/tap_square/client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1902 2023-07-12 08:46:24.000000 tap-square-2.0.0/tap_square/discover.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-24 10:55:42.073953 tap-square-2.0.0/tap_square/schemas/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1475 2023-07-24 10:47:44.000000 tap-square-2.0.0/tap_square/schemas/bank_accounts.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1929 2023-07-24 10:47:44.000000 tap-square-2.0.0/tap_square/schemas/cash_drawer_shifts.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1005 2023-06-02 15:01:54.000000 tap-square-2.0.0/tap_square/schemas/categories.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3979 2023-07-24 10:47:44.000000 tap-square-2.0.0/tap_square/schemas/customers.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2081 2023-06-02 15:01:54.000000 tap-square-2.0.0/tap_square/schemas/discounts.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      613 2023-07-06 17:35:22.000000 tap-square-2.0.0/tap_square/schemas/inventories.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8268 2023-06-02 15:01:54.000000 tap-square-2.0.0/tap_square/schemas/items.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5055 2023-07-24 10:47:44.000000 tap-square-2.0.0/tap_square/schemas/locations.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3871 2023-06-02 15:01:54.000000 tap-square-2.0.0/tap_square/schemas/modifier_lists.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    67306 2023-07-24 10:47:44.000000 tap-square-2.0.0/tap_square/schemas/orders.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22812 2023-07-24 10:47:44.000000 tap-square-2.0.0/tap_square/schemas/payments.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8501 2023-07-24 10:47:44.000000 tap-square-2.0.0/tap_square/schemas/refunds.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      705 2023-06-02 15:01:54.000000 tap-square-2.0.0/tap_square/schemas/roles.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1322 2023-07-12 08:46:24.000000 tap-square-2.0.0/tap_square/schemas/settlements.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2829 2023-07-24 10:47:44.000000 tap-square-2.0.0/tap_square/schemas/shifts.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1785 2023-06-02 15:01:54.000000 tap-square-2.0.0/tap_square/schemas/taxes.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1419 2023-07-24 10:47:44.000000 tap-square-2.0.0/tap_square/schemas/team_members.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15191 2023-07-24 10:47:44.000000 tap-square-2.0.0/tap_square/streams.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1168 2023-06-02 15:01:54.000000 tap-square-2.0.0/tap_square/sync.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-24 10:55:42.069953 tap-square-2.0.0/tap_square.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      258 2023-07-24 10:55:41.000000 tap-square-2.0.0/tap_square.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      945 2023-07-24 10:55:42.000000 tap-square-2.0.0/tap_square.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-24 10:55:41.000000 tap-square-2.0.0/tap_square.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       47 2023-07-24 10:55:41.000000 tap-square-2.0.0/tap_square.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      107 2023-07-24 10:55:41.000000 tap-square-2.0.0/tap_square.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2023-07-24 10:55:41.000000 tap-square-2.0.0/tap_square.egg-info/top_level.txt
```

### Comparing `tap-square-1.3.1/LICENSE` & `tap-square-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tap-square-1.3.1/README.md` & `tap-square-2.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 This tap:
 * Downloads data from [Square API](https://developer.squareup.com/reference/square)
 * Extracts from the following sources to produce [streams](https://github.com/singer-io/tap-square/blob/master/tap_square/streams.py). Below is a list of all the streams available. See the [streams file](https://github.com/singer-io/tap-square/blob/master/tap_square/streams.py) for a list of classes where each one has a constant indiciating if the stream's replication_method is INCREMENTAL or FULL_TABLE and what the replication_key is, usually `updated_at` field if it's incremental.
     * Items
     * Categories
     * Discounts
     * Taxes
-    * Employees
+    * TeamMembers
     * Locations
     * BankAccounts
     * Refunds
     * Payments
     * ModifierLists
     * Inventories
     * Orders
```

### Comparing `tap-square-1.3.1/setup.py` & `tap-square-2.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 #!/usr/bin/env python
 
 from setuptools import setup
 
 setup(name='tap-square',
-      version='1.3.1',
+      version='2.0.0',
       description='Singer.io tap for extracting data from the Square API',
       author='Stitch',
       url='http://singer.io',
       classifiers=['Programming Language :: Python :: 3 :: Only'],
       py_modules=['tap_square'],
       install_requires=[
           'singer-python==5.9.0',
-          'squareup==5.3.0.20200528',
+          'squareup==28.0.0.20230608',
           'backoff==1.8.0',
           'methodtools==0.4.2',
       ],
       extras_require={
           'dev': [
-              'ipdb==0.11',
+              'ipdb',
               'pylint==2.5.3',
           ]
       },
       entry_points='''
           [console_scripts]
           tap-square=tap_square:main
       ''',
```

### Comparing `tap-square-1.3.1/tap_square/__init__.py` & `tap-square-2.0.0/tap_square/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 import json
 
 import singer
 from singer.catalog import write_catalog
-from .discover import discover
-from .sync import sync
+from tap_square.discover import discover
+from tap_square.sync import sync
 
 LOGGER = singer.get_logger()
 
 @singer.utils.handle_top_exception(LOGGER)
 def main():
     args = singer.utils.parse_args([])
```

### Comparing `tap-square-1.3.1/tap_square/client.py` & `tap-square-2.0.0/tap_square/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -123,28 +123,14 @@
 
         yield from self._get_v2_objects(
             object_type,
             lambda bdy: self._client.catalog.search_catalog_objects(body=bdy),
             body,
             'objects')
 
-    def get_employees(self, bookmarked_cursor):
-        body = {
-            'limit': 50,
-        }
-
-        if bookmarked_cursor:
-            body['cursor'] = bookmarked_cursor
-
-        yield from self._get_v2_objects(
-            'employees',
-            lambda bdy: self._client.employees.list_employees(**bdy),
-            body,
-            'employees')
-
     def get_locations(self):
         body = {}
 
         yield from self._get_v2_objects(
             'locations',
             lambda bdy: self._client.locations.list_locations(**bdy),
             body,
@@ -198,14 +184,30 @@
 
         yield from self._get_v2_objects(
             'orders',
             lambda bdy: self._client.orders.search_orders(body=bdy),
             body,
             'orders')
 
+    def get_team_members(self, location_ids):
+        body = {
+            "query": {
+                "filter": {
+                    "location_ids": location_ids,
+                    "status": "ACTIVE"
+                }
+            },
+            "limit": 200
+        }
+        yield from self._get_v2_objects(
+            'team_members',
+            lambda bdy: self._client.team.search_team_members(body=bdy),
+            body,
+            'team_members')
+
     def get_inventories(self, start_time, bookmarked_cursor):
         body = {'updated_after': start_time}
 
         if bookmarked_cursor:
             body['cursor'] = bookmarked_cursor
 
         yield from self._get_v2_objects(
```

### Comparing `tap-square-1.3.1/tap_square/discover.py` & `tap-square-2.0.0/tap_square/discover.py`

 * *Files identical despite different names*

### Comparing `tap-square-1.3.1/tap_square/schemas/bank_accounts.json` & `tap-square-2.0.0/tap_square/schemas/bank_accounts.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.953125%*

 * *Differences: {"'properties'": "{'secondary_bank_identification_number': OrderedDict([('type', ['null', "*

 * *                 "'string'])]), 'debit_mandate_reference_id': OrderedDict([('type', ['null', "*

 * *                 "'string'])]), 'reference_id': OrderedDict([('type', ['null', 'string'])])}"}*

```diff
@@ -32,14 +32,20 @@
         },
         "currency": {
             "type": [
                 "null",
                 "string"
             ]
         },
+        "debit_mandate_reference_id": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
         "debitable": {
             "type": [
                 "null",
                 "boolean"
             ]
         },
         "holder_name": {
@@ -62,14 +68,26 @@
         },
         "primary_bank_identification_number": {
             "type": [
                 "null",
                 "string"
             ]
         },
+        "reference_id": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "secondary_bank_identification_number": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
         "status": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "version": {
```

### Comparing `tap-square-1.3.1/tap_square/schemas/cash_drawer_shifts.json` & `tap-square-2.0.0/tap_square/schemas/categories.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.515625%*

 * *Differences: {"'properties'": "{'category_data': OrderedDict([('type', ['null', 'object']), ('properties', "*

 * *                 "OrderedDict([('name', OrderedDict([('type', ['null', 'string'])]))]))]), "*

 * *                 "'is_deleted': OrderedDict([('type', ['null', 'boolean'])]), "*

 * *                 "'absent_at_location_ids': OrderedDict([('type', ['null', 'array']), ('items', "*

 * *                 "OrderedDict([('type', ['null', 'string'])]))]), 'present_at_all_locations': "*

 * *                 "OrderedDict([('type', ['null',  […]*

```diff
@@ -1,104 +1,71 @@
 {
     "properties": {
-        "closed_at": {
-            "format": "date-time",
+        "absent_at_location_ids": {
+            "items": {
+                "type": [
+                    "null",
+                    "string"
+                ]
+            },
             "type": [
                 "null",
-                "string"
+                "array"
             ]
         },
-        "closed_cash_money": {
+        "category_data": {
             "properties": {
-                "amount": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
-                },
-                "currency": {
+                "name": {
                     "type": [
                         "null",
                         "string"
                     ]
                 }
             },
             "type": [
                 "null",
                 "object"
             ]
         },
-        "description": {
+        "id": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "ended_at": {
-            "format": "date-time",
+        "is_deleted": {
             "type": [
                 "null",
-                "string"
+                "boolean"
             ]
         },
-        "expected_cash_money": {
-            "properties": {
-                "amount": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
-                },
-                "currency": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                }
-            },
+        "present_at_all_locations": {
             "type": [
                 "null",
-                "object"
+                "boolean"
             ]
         },
-        "id": {
+        "type": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "opened_at": {
+        "updated_at": {
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "opened_cash_money": {
-            "properties": {
-                "amount": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
-                },
-                "currency": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                }
-            },
-            "type": [
-                "null",
-                "object"
-            ]
-        },
-        "state": {
+        "version": {
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         }
     },
-    "type": "object"
+    "type": [
+        "null",
+        "object"
+    ]
 }
```

### Comparing `tap-square-1.3.1/tap_square/schemas/categories.json` & `tap-square-2.0.0/tap_square/schemas/team_members.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7794117647058824%*

 * *Differences: {"'properties'": "{'reference_id': OrderedDict([('type', ['null', 'string'])]), 'is_owner': "*

 * *                 "OrderedDict([('type', ['null', 'boolean'])]), 'status': OrderedDict([('type', "*

 * *                 "['null', 'string'])]), 'given_name': OrderedDict([('type', ['null', "*

 * *                 "'string'])]), 'family_name': OrderedDict([('type', ['null', 'string'])]), "*

 * *                 "'email_address': OrderedDict([('type', ['null', 'string'])]), 'phone_number': "*

 * *                 "OrderedDict([('type',  […]*

```diff
@@ -1,70 +1,95 @@
 {
     "properties": {
-        "absent_at_location_ids": {
-            "items": {
-                "type": [
-                    "null",
-                    "string"
-                ]
-            },
-            "type": [
-                "null",
-                "array"
-            ]
-        },
-        "category_data": {
+        "assigned_locations": {
             "properties": {
-                "name": {
+                "assignment_type": {
                     "type": [
                         "null",
                         "string"
                     ]
+                },
+                "location_ids": {
+                    "items": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "type": [
+                        "null",
+                        "array"
+                    ]
                 }
             },
             "type": [
                 "null",
                 "object"
             ]
         },
+        "created_at": {
+            "format": "date-time",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "email_address": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "family_name": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "given_name": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
         "id": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "is_deleted": {
+        "is_owner": {
             "type": [
                 "null",
                 "boolean"
             ]
         },
-        "present_at_all_locations": {
+        "phone_number": {
             "type": [
                 "null",
-                "boolean"
+                "string"
             ]
         },
-        "type": {
+        "reference_id": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "updated_at": {
-            "format": "date-time",
+        "status": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "version": {
+        "updated_at": {
+            "format": "date-time",
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         }
     },
     "type": [
         "null",
         "object"
     ]
```

### Comparing `tap-square-1.3.1/tap_square/schemas/customers.json` & `tap-square-2.0.0/tap_square/schemas/taxes.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.775%*

 * *Differences: {"'properties'": "{'is_deleted': OrderedDict([('type', ['null', 'boolean'])]), "*

 * *                 "'absent_at_location_ids': OrderedDict([('type', ['null', 'array']), ('items', "*

 * *                 "OrderedDict([('type', ['null', 'string'])]))]), 'present_at_all_locations': "*

 * *                 "OrderedDict([('type', ['null', 'boolean'])]), 'tax_data': OrderedDict([('type', "*

 * *                 "['null', 'object']), ('properties', OrderedDict([('applies_to_custom_amounts', "*

 * *                 "OrderedDict([('type' […]*

```diff
@@ -1,144 +1,112 @@
 {
     "properties": {
-        "address": {
+        "absent_at_location_ids": {
+            "items": {
+                "type": [
+                    "null",
+                    "string"
+                ]
+            },
+            "type": [
+                "null",
+                "array"
+            ]
+        },
+        "id": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "is_deleted": {
+            "type": [
+                "null",
+                "boolean"
+            ]
+        },
+        "present_at_all_locations": {
+            "type": [
+                "null",
+                "boolean"
+            ]
+        },
+        "tax_data": {
             "properties": {
-                "address_line_1": {
+                "applies_to_custom_amounts": {
                     "type": [
                         "null",
-                        "string"
+                        "boolean"
                     ]
                 },
-                "administrative_district_level_1": {
+                "calculation_phase": {
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "country": {
+                "enabled": {
+                    "type": [
+                        "null",
+                        "boolean"
+                    ]
+                },
+                "inclusion_type": {
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "locality": {
+                "name": {
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "postal_code": {
+                "percentage": {
                     "type": [
                         "null",
                         "string"
                     ]
-                }
-            },
-            "type": [
-                "null",
-                "object"
-            ]
-        },
-        "birthday": {
-            "anyOf": [
-                {
-                    "format": "date-time",
+                },
+                "tax_type_id": {
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                {
+                "tax_type_name": {
                     "type": [
                         "null",
                         "string"
                     ]
                 }
-            ]
-        },
-        "company_name": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "created_at": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "creation_source": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "email_address": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "family_name": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "given_name": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "id": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "nickname": {
+            },
             "type": [
                 "null",
-                "string"
+                "object"
             ]
         },
-        "note": {
+        "type": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "phone_number": {
+        "updated_at": {
+            "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "preferences": {
-            "properties": {
-                "email_unsubscribed": {
-                    "type": [
-                        "null",
-                        "boolean"
-                    ]
-                }
-            },
+        "version": {
             "type": [
                 "null",
-                "object"
-            ]
-        },
-        "updated_at": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
+                "integer"
             ]
         }
     },
     "type": [
         "null",
         "object"
     ]
```

### Comparing `tap-square-1.3.1/tap_square/schemas/discounts.json` & `tap-square-2.0.0/tap_square/schemas/discounts.json`

 * *Files identical despite different names*

### Comparing `tap-square-1.3.1/tap_square/schemas/employees.json` & `tap-square-2.0.0/tap_square/schemas/inventories.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'properties'": "{replace: OrderedDict([('calculated_at', OrderedDict([('type', ['null', "*

 * *                 "'string']), ('format', 'date-time')])), ('catalog_object_type', "*

 * *                 "OrderedDict([('type', ['null', 'string'])])), ('state', OrderedDict([('type', "*

 * *                 "['null', 'string'])])), ('location_id', OrderedDict([('type', ['null', "*

 * *                 "'string'])])), ('quantity', OrderedDict([('type', ['null', 'string'])])), "*

 * *                 "('catalog_object_id', OrderedDict([ […]*

```diff
@@ -1,66 +1,41 @@
 {
     "properties": {
-        "created_at": {
+        "calculated_at": {
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "email": {
+        "catalog_object_id": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "first_name": {
+        "catalog_object_type": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "id": {
+        "location_id": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "is_owner": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
-        "last_name": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "location_ids": {
-            "items": {
-                "type": [
-                    "null",
-                    "string"
-                ]
-            },
-            "type": [
-                "null",
-                "array"
-            ]
-        },
-        "status": {
+        "quantity": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "updated_at": {
-            "format": "date-time",
+        "state": {
             "type": [
                 "null",
                 "string"
             ]
         }
     },
     "type": [
```

### Comparing `tap-square-1.3.1/tap_square/schemas/inventories.json` & `tap-square-2.0.0/tap_square/schemas/roles.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'properties'": "{replace: OrderedDict([('permissions', OrderedDict([('type', ['null', 'array']), "*

 * *                 "('items', OrderedDict([('type', ['null', 'string'])]))])), ('id', "*

 * *                 "OrderedDict([('type', ['null', 'string'])])), ('name', OrderedDict([('type', "*

 * *                 "['null', 'string'])])), ('is_owner', OrderedDict([('type', ['null', "*

 * *                 "'boolean'])])), ('updated_at', OrderedDict([('type', ['null', 'string']), "*

 * *                 "('format', 'date-time')])),  […]*

```diff
@@ -1,41 +1,48 @@
 {
     "properties": {
-        "calculated_at": {
+        "created_at": {
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "catalog_object_id": {
+        "id": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "catalog_object_type": {
+        "is_owner": {
             "type": [
                 "null",
-                "string"
+                "boolean"
             ]
         },
-        "location_id": {
+        "name": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "quantity": {
+        "permissions": {
+            "items": {
+                "type": [
+                    "null",
+                    "string"
+                ]
+            },
             "type": [
                 "null",
-                "string"
+                "array"
             ]
         },
-        "state": {
+        "updated_at": {
+            "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         }
     },
     "type": [
```

### Comparing `tap-square-1.3.1/tap_square/schemas/items.json` & `tap-square-2.0.0/tap_square/schemas/items.json`

 * *Files identical despite different names*

### Comparing `tap-square-1.3.1/tap_square/schemas/locations.json` & `tap-square-2.0.0/tap_square/schemas/locations.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9710737179487179%*

 * *Differences: {"'properties'": "{'address': {'properties': {delete: ['organization']}}, 'logo_url': "*

 * *                 "OrderedDict([('type', ['null', 'string'])]), 'pos_background_url': "*

 * *                 "OrderedDict([('type', ['null', 'string'])]), 'full_format_logo_url': "*

 * *                 "OrderedDict([('type', ['null', 'string'])])}"}*

```diff
@@ -58,20 +58,14 @@
                 },
                 "locality": {
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "organization": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
                 "postal_code": {
                     "type": [
                         "null",
                         "string"
                     ]
                 },
                 "sublocality": {
@@ -211,14 +205,20 @@
         },
         "facebook_url": {
             "type": [
                 "null",
                 "string"
             ]
         },
+        "full_format_logo_url": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
         "id": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "instagram_username": {
@@ -229,14 +229,20 @@
         },
         "language_code": {
             "type": [
                 "null",
                 "string"
             ]
         },
+        "logo_url": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
         "mcc": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "merchant_id": {
@@ -253,14 +259,20 @@
         },
         "phone_number": {
             "type": [
                 "null",
                 "string"
             ]
         },
+        "pos_background_url": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
         "status": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "timezone": {
```

### Comparing `tap-square-1.3.1/tap_square/schemas/modifier_lists.json` & `tap-square-2.0.0/tap_square/schemas/modifier_lists.json`

 * *Files identical despite different names*

### Comparing `tap-square-1.3.1/tap_square/schemas/orders.json` & `tap-square-2.0.0/tap_square/schemas/payments.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8253039370990332%*

 * *Differences: {"'properties'": "{'processing_fee': {'items': {'properties': {'effective_at': {'format': "*

 * *                 "'date-time'}}}}, 'card_details': {'properties': {'card': {'properties': {'id': "*

 * *                 "OrderedDict([('type', ['null', 'string'])]), 'cardholder_name': "*

 * *                 "OrderedDict([('type', ['null', 'string'])]), 'billing_address': "*

 * *                 "OrderedDict([('type', ['null', 'object']), ('properties', "*

 * *                 "OrderedDict([('address_line_1', OrderedDict([('type', ['n […]*

```diff
@@ -16,480 +16,674 @@
                 }
             },
             "type": [
                 "null",
                 "object"
             ]
         },
-        "card_details": {
+        "app_fee_money": {
             "properties": {
-                "avs_status": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "card": {
-                    "properties": {
-                        "bin": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "card_brand": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "card_type": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "exp_month": {
-                            "type": [
-                                "null",
-                                "integer"
-                            ]
-                        },
-                        "exp_year": {
-                            "type": [
-                                "null",
-                                "integer"
-                            ]
-                        },
-                        "fingerprint": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "last_4": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "prepaid_type": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        }
-                    },
-                    "type": [
-                        "null",
-                        "object"
-                    ]
-                },
-                "cvv_status": {
+                "amount": {
                     "type": [
                         "null",
-                        "string"
+                        "integer"
                     ]
                 },
-                "entry_method": {
+                "currency": {
                     "type": [
                         "null",
                         "string"
                     ]
-                },
-                "statement_description": {
+                }
+            },
+            "type": [
+                "null",
+                "object"
+            ]
+        },
+        "application_details": {
+            "properties": {
+                "application_id": {
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "status": {
+                "square_product": {
                     "type": [
                         "null",
                         "string"
                     ]
                 }
             },
             "type": [
                 "null",
                 "object"
             ]
         },
-        "category_data": {
+        "approved_money": {
             "properties": {
-                "name": {
+                "amount": {
+                    "type": [
+                        "null",
+                        "integer"
+                    ]
+                },
+                "currency": {
                     "type": [
                         "null",
                         "string"
                     ]
                 }
             },
             "type": [
                 "null",
                 "object"
             ]
         },
-        "closed_at": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "created_at": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "delay_action": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "delay_duration": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "delayed_until": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "discount_data": {
+        "bank_account_details": {
             "properties": {
-                "amount_money": {
+                "account_ownership_type": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "ach_details": {
                     "properties": {
-                        "amount": {
+                        "account_number_suffix": {
                             "type": [
                                 "null",
-                                "integer"
+                                "string"
                             ]
                         },
-                        "currency": {
+                        "account_type": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "routing_number": {
                             "type": [
                                 "null",
                                 "string"
                             ]
                         }
                     },
                     "type": [
                         "null",
                         "object"
                     ]
                 },
-                "discount_type": {
+                "bank_name": {
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "name": {
+                "country": {
                     "type": [
                         "null",
                         "string"
                     ]
-                }
-            },
-            "type": [
-                "null",
-                "object"
-            ]
-        },
-        "fulfillments": {
-            "items": {
-                "properties": {
-                    "pickup_details": {
+                },
+                "errors": {
+                    "items": {
                         "properties": {
-                            "canceled_at": {
-                                "format": "date-time",
+                            "category": {
                                 "type": [
                                     "null",
                                     "string"
                                 ]
                             },
-                            "expired_at": {
-                                "format": "date-time",
+                            "code": {
                                 "type": [
                                     "null",
                                     "string"
                                 ]
                             },
-                            "expires_at": {
-                                "format": "date-time",
+                            "detail": {
                                 "type": [
                                     "null",
                                     "string"
                                 ]
                             },
-                            "note": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "pickup_at": {
-                                "format": "date-time",
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "recipient": {
-                                "properties": {
-                                    "display_name": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    }
-                                },
-                                "type": [
-                                    "null",
-                                    "object"
-                                ]
-                            },
-                            "rejected_at": {
-                                "format": "date-time",
+                            "field": {
                                 "type": [
                                     "null",
                                     "string"
                                 ]
                             }
                         },
                         "type": [
                             "null",
                             "object"
                         ]
                     },
-                    "state": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "type": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
+                    "type": [
+                        "null",
+                        "array"
+                    ]
+                },
+                "fingerprint": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "statement_description": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "transfer_type": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                }
+            },
+            "type": [
+                "null",
+                "object"
+            ]
+        },
+        "billing_address": {
+            "properties": {
+                "address_line_1": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "address_line_2": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "address_line_3": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "administrative_district_level_1": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "administrative_district_level_2": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "administrative_district_level_3": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "country": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "first_name": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "last_name": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "locality": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "postal_code": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "sublocality": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "sublocality_2": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "sublocality_3": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                }
+            },
+            "type": [
+                "null",
+                "object"
+            ]
+        },
+        "buy_now_pay_later_details": {
+            "properties": {
+                "afterpay_details": {
+                    "properties": {
+                        "email_address": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        }
                     },
-                    "uid": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    }
+                    "type": [
+                        "null",
+                        "object"
+                    ]
                 },
-                "type": [
-                    "null",
-                    "object"
-                ]
+                "brand": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "clearpay_details": {
+                    "properties": {
+                        "email_address": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        }
+                    },
+                    "type": [
+                        "null",
+                        "object"
+                    ]
+                }
             },
             "type": [
                 "null",
-                "array"
+                "object"
             ]
         },
-        "id": {
+        "buyer_email_address": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "is_deleted": {
+        "capabilities": {
+            "items": {
+                "type": [
+                    "null",
+                    "string"
+                ]
+            },
             "type": [
                 "null",
-                "boolean"
+                "array"
             ]
         },
-        "line_items": {
-            "items": {
-                "properties": {
-                    "base_price_money": {
-                        "properties": {
-                            "amount": {
-                                "type": [
-                                    "null",
-                                    "integer"
-                                ]
+        "card_details": {
+            "properties": {
+                "application_cryptogram": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "application_identifier": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "application_name": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "auth_result_code": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "avs_status": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "card": {
+                    "properties": {
+                        "billing_address": {
+                            "properties": {
+                                "address_line_1": {
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                },
+                                "address_line_2": {
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                },
+                                "address_line_3": {
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                },
+                                "administrative_district_level_1": {
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                },
+                                "administrative_district_level_2": {
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                },
+                                "administrative_district_level_3": {
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                },
+                                "country": {
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                },
+                                "first_name": {
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                },
+                                "last_name": {
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                },
+                                "locality": {
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                },
+                                "postal_code": {
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                },
+                                "sublocality": {
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                },
+                                "sublocality_2": {
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                },
+                                "sublocality_3": {
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                }
                             },
-                            "currency": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            }
+                            "type": [
+                                "null",
+                                "object"
+                            ]
                         },
-                        "type": [
-                            "null",
-                            "object"
-                        ]
-                    },
-                    "catalog_object_id": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "gross_sales_money": {
-                        "properties": {
-                            "amount": {
-                                "type": [
-                                    "null",
-                                    "integer"
-                                ]
-                            },
-                            "currency": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            }
+                        "bin": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
                         },
-                        "type": [
-                            "null",
-                            "object"
-                        ]
-                    },
-                    "name": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "note": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "quantity": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
+                        "card_brand": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "card_co_brand": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "card_type": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "cardholder_name": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "customer_id": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "enabled": {
+                            "type": [
+                                "null",
+                                "boolean"
+                            ]
+                        },
+                        "exp_month": {
+                            "type": [
+                                "null",
+                                "integer"
+                            ]
+                        },
+                        "exp_year": {
+                            "type": [
+                                "null",
+                                "integer"
+                            ]
+                        },
+                        "fingerprint": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "id": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "last_4": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "merchant_id": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "prepaid_type": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "reference_id": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "version": {
+                            "type": [
+                                "null",
+                                "integer"
+                            ]
+                        }
                     },
-                    "total_discount_money": {
-                        "properties": {
-                            "amount": {
-                                "type": [
-                                    "null",
-                                    "integer"
-                                ]
-                            },
-                            "currency": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            }
+                    "type": [
+                        "null",
+                        "object"
+                    ]
+                },
+                "card_payment_timeline": {
+                    "properties": {
+                        "authorized_at": {
+                            "format": "date-time",
+                            "type": [
+                                "null",
+                                "string"
+                            ]
                         },
-                        "type": [
-                            "null",
-                            "object"
-                        ]
+                        "captured_at": {
+                            "format": "date-time",
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "voided_at": {
+                            "format": "date-time",
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        }
                     },
-                    "total_money": {
+                    "type": [
+                        "null",
+                        "object"
+                    ]
+                },
+                "cvv_status": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "entry_method": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "errors": {
+                    "items": {
                         "properties": {
-                            "amount": {
+                            "category": {
                                 "type": [
                                     "null",
-                                    "integer"
+                                    "string"
                                 ]
                             },
-                            "currency": {
+                            "code": {
                                 "type": [
                                     "null",
                                     "string"
                                 ]
-                            }
-                        },
-                        "type": [
-                            "null",
-                            "object"
-                        ]
-                    },
-                    "total_tax_money": {
-                        "properties": {
-                            "amount": {
-                                "type": [
-                                    "null",
-                                    "integer"
-                                ]
                             },
-                            "currency": {
+                            "detail": {
                                 "type": [
                                     "null",
                                     "string"
                                 ]
-                            }
-                        },
-                        "type": [
-                            "null",
-                            "object"
-                        ]
-                    },
-                    "uid": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "variation_name": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "variation_total_price_money": {
-                        "properties": {
-                            "amount": {
-                                "type": [
-                                    "null",
-                                    "integer"
-                                ]
                             },
-                            "currency": {
+                            "field": {
                                 "type": [
                                     "null",
                                     "string"
                                 ]
                             }
                         },
                         "type": [
                             "null",
                             "object"
                         ]
-                    }
+                    },
+                    "type": [
+                        "null",
+                        "array"
+                    ]
                 },
-                "type": [
-                    "null",
-                    "object"
-                ]
+                "statement_description": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "status": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "verification_method": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "verification_results": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                }
             },
             "type": [
                 "null",
-                "array"
-            ]
-        },
-        "location_id": {
-            "type": [
-                "null",
-                "string"
+                "object"
             ]
         },
-        "net_amounts": {
+        "cash_details": {
             "properties": {
-                "discount_money": {
+                "buyer_supplied_money": {
                     "properties": {
                         "amount": {
                             "type": [
                                 "null",
                                 "integer"
                             ]
                         },
@@ -501,15 +695,15 @@
                         }
                     },
                     "type": [
                         "null",
                         "object"
                     ]
                 },
-                "service_charge_money": {
+                "change_back_money": {
                     "properties": {
                         "amount": {
                             "type": [
                                 "null",
                                 "integer"
                             ]
                         },
@@ -520,56 +714,88 @@
                             ]
                         }
                     },
                     "type": [
                         "null",
                         "object"
                     ]
+                }
+            },
+            "type": [
+                "null",
+                "object"
+            ]
+        },
+        "created_at": {
+            "format": "date-time",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "customer_id": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "delay_action": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "delay_duration": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "delayed_until": {
+            "format": "date-time",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "device_details": {
+            "properties": {
+                "device_id": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
                 },
-                "tax_money": {
-                    "properties": {
-                        "amount": {
-                            "type": [
-                                "null",
-                                "integer"
-                            ]
-                        },
-                        "currency": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        }
-                    },
+                "device_installation_id": {
                     "type": [
                         "null",
-                        "object"
+                        "string"
                     ]
                 },
-                "tip_money": {
-                    "properties": {
-                        "amount": {
-                            "type": [
-                                "null",
-                                "integer"
-                            ]
-                        },
-                        "currency": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        }
-                    },
+                "device_name": {
                     "type": [
                         "null",
-                        "object"
+                        "string"
+                    ]
+                }
+            },
+            "type": [
+                "null",
+                "object"
+            ]
+        },
+        "external_details": {
+            "properties": {
+                "source": {
+                    "type": [
+                        "null",
+                        "string"
                     ]
                 },
-                "total_money": {
+                "source_fee_money": {
                     "properties": {
                         "amount": {
                             "type": [
                                 "null",
                                 "integer"
                             ]
                         },
@@ -580,43 +806,55 @@
                             ]
                         }
                     },
                     "type": [
                         "null",
                         "object"
                     ]
+                },
+                "source_id": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "type": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
                 }
             },
             "type": [
                 "null",
                 "object"
             ]
         },
-        "note": {
+        "id": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "order_id": {
+        "location_id": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "payment_id": {
+        "note": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "present_at_all_locations": {
+        "order_id": {
             "type": [
                 "null",
-                "boolean"
+                "string"
             ]
         },
         "processing_fee": {
             "items": {
                 "properties": {
                     "amount_money": {
                         "properties": {
@@ -635,14 +873,15 @@
                         },
                         "type": [
                             "null",
                             "object"
                         ]
                     },
                     "effective_at": {
+                        "format": "date-time",
                         "type": [
                             "null",
                             "string"
                         ]
                     },
                     "type": {
                         "type": [
@@ -657,27 +896,27 @@
                 ]
             },
             "type": [
                 "null",
                 "array"
             ]
         },
-        "reason": {
+        "receipt_number": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "receipt_number": {
+        "receipt_url": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "receipt_url": {
+        "reference_id": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "refund_ids": {
             "items": {
@@ -707,658 +946,116 @@
                 }
             },
             "type": [
                 "null",
                 "object"
             ]
         },
-        "refunds": {
-            "items": {
-                "properties": {
-                    "amount_money": {
-                        "properties": {
-                            "amount": {
-                                "type": [
-                                    "null",
-                                    "integer"
-                                ]
-                            },
-                            "currency": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            }
-                        },
-                        "type": [
-                            "null",
-                            "object"
-                        ]
-                    },
-                    "created_at": {
-                        "format": "date-time",
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "id": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "location_id": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "reason": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "status": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "tender_id": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "transaction_id": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    }
+        "risk_evaluation": {
+            "properties": {
+                "created_at": {
+                    "format": "date-time",
+                    "type": [
+                        "null",
+                        "string"
+                    ]
                 },
-                "type": [
-                    "null",
-                    "object"
-                ]
+                "risk_level": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                }
             },
             "type": [
                 "null",
-                "array"
+                "object"
             ]
         },
-        "return_amounts": {
+        "shipping_address": {
             "properties": {
-                "discount_money": {
-                    "properties": {
-                        "amount": {
-                            "type": [
-                                "null",
-                                "integer"
-                            ]
-                        },
-                        "currency": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        }
-                    },
+                "address_line_1": {
                     "type": [
                         "null",
-                        "object"
+                        "string"
                     ]
                 },
-                "service_charge_money": {
-                    "properties": {
-                        "amount": {
-                            "type": [
-                                "null",
-                                "integer"
-                            ]
-                        },
-                        "currency": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        }
-                    },
+                "address_line_2": {
                     "type": [
                         "null",
-                        "object"
+                        "string"
                     ]
                 },
-                "tax_money": {
-                    "properties": {
-                        "amount": {
-                            "type": [
-                                "null",
-                                "integer"
-                            ]
-                        },
-                        "currency": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        }
-                    },
+                "address_line_3": {
                     "type": [
                         "null",
-                        "object"
+                        "string"
                     ]
                 },
-                "tip_money": {
-                    "properties": {
-                        "amount": {
-                            "type": [
-                                "null",
-                                "integer"
-                            ]
-                        },
-                        "currency": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        }
-                    },
+                "administrative_district_level_1": {
                     "type": [
                         "null",
-                        "object"
+                        "string"
                     ]
                 },
-                "total_money": {
-                    "properties": {
-                        "amount": {
-                            "type": [
-                                "null",
-                                "integer"
-                            ]
-                        },
-                        "currency": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        }
-                    },
+                "administrative_district_level_2": {
                     "type": [
                         "null",
-                        "object"
+                        "string"
                     ]
-                }
-            },
-            "type": [
-                "null",
-                "object"
-            ]
-        },
-        "returns": {
-            "items": {
-                "properties": {
-                    "return_line_items": {
-                        "items": {
-                            "properties": {
-                                "applied_discounts": {
-                                    "items": {
-                                        "properties": {
-                                            "applied_money": {
-                                                "properties": {
-                                                    "amount": {
-                                                        "type": [
-                                                            "null",
-                                                            "integer"
-                                                        ]
-                                                    },
-                                                    "currency": {
-                                                        "type": [
-                                                            "null",
-                                                            "string"
-                                                        ]
-                                                    }
-                                                },
-                                                "type": [
-                                                    "null",
-                                                    "object"
-                                                ]
-                                            },
-                                            "discount_uid": {
-                                                "type": [
-                                                    "null",
-                                                    "string"
-                                                ]
-                                            },
-                                            "uid": {
-                                                "type": [
-                                                    "null",
-                                                    "string"
-                                                ]
-                                            }
-                                        },
-                                        "type": [
-                                            "null",
-                                            "object"
-                                        ]
-                                    },
-                                    "type": [
-                                        "null",
-                                        "array"
-                                    ]
-                                },
-                                "applied_taxes": {
-                                    "items": {
-                                        "properties": {
-                                            "applied_money": {
-                                                "properties": {
-                                                    "amount": {
-                                                        "type": [
-                                                            "null",
-                                                            "integer"
-                                                        ]
-                                                    },
-                                                    "currency": {
-                                                        "type": [
-                                                            "null",
-                                                            "string"
-                                                        ]
-                                                    }
-                                                },
-                                                "type": [
-                                                    "null",
-                                                    "object"
-                                                ]
-                                            },
-                                            "tax_uid": {
-                                                "type": [
-                                                    "null",
-                                                    "string"
-                                                ]
-                                            },
-                                            "uid": {
-                                                "type": [
-                                                    "null",
-                                                    "string"
-                                                ]
-                                            }
-                                        },
-                                        "type": [
-                                            "null",
-                                            "object"
-                                        ]
-                                    },
-                                    "type": [
-                                        "null",
-                                        "array"
-                                    ]
-                                },
-                                "base_price_money": {
-                                    "properties": {
-                                        "amount": {
-                                            "type": [
-                                                "null",
-                                                "integer"
-                                            ]
-                                        },
-                                        "currency": {
-                                            "type": [
-                                                "null",
-                                                "string"
-                                            ]
-                                        }
-                                    },
-                                    "type": [
-                                        "null",
-                                        "object"
-                                    ]
-                                },
-                                "catalog_object_id": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                },
-                                "gross_return_money": {
-                                    "properties": {
-                                        "amount": {
-                                            "type": [
-                                                "null",
-                                                "integer"
-                                            ]
-                                        },
-                                        "currency": {
-                                            "type": [
-                                                "null",
-                                                "string"
-                                            ]
-                                        }
-                                    },
-                                    "type": [
-                                        "null",
-                                        "object"
-                                    ]
-                                },
-                                "name": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                },
-                                "note": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                },
-                                "quantity": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                },
-                                "quantity_unit": {
-                                    "properties": {
-                                        "measurement_unit": {
-                                            "properties": {
-                                                "area_unit": {
-                                                    "type": [
-                                                        "null",
-                                                        "string"
-                                                    ]
-                                                },
-                                                "custom_unit": {
-                                                    "properties": {
-                                                        "abbreviation": {
-                                                            "type": [
-                                                                "null",
-                                                                "string"
-                                                            ]
-                                                        },
-                                                        "name": {
-                                                            "type": [
-                                                                "null",
-                                                                "string"
-                                                            ]
-                                                        }
-                                                    },
-                                                    "type": [
-                                                        "null",
-                                                        "object"
-                                                    ]
-                                                },
-                                                "generic_unit": {
-                                                    "type": [
-                                                        "null",
-                                                        "string"
-                                                    ]
-                                                },
-                                                "length_unit": {
-                                                    "type": [
-                                                        "null",
-                                                        "string"
-                                                    ]
-                                                },
-                                                "time_unit": {
-                                                    "type": [
-                                                        "null",
-                                                        "string"
-                                                    ]
-                                                },
-                                                "type": {
-                                                    "type": [
-                                                        "null",
-                                                        "string"
-                                                    ]
-                                                },
-                                                "volume_unit": {
-                                                    "type": [
-                                                        "null",
-                                                        "string"
-                                                    ]
-                                                },
-                                                "weight_unit": {
-                                                    "type": [
-                                                        "null",
-                                                        "string"
-                                                    ]
-                                                }
-                                            },
-                                            "type": [
-                                                "null",
-                                                "object"
-                                            ]
-                                        },
-                                        "precision": {
-                                            "type": [
-                                                "null",
-                                                "integer"
-                                            ]
-                                        }
-                                    },
-                                    "type": [
-                                        "null",
-                                        "object"
-                                    ]
-                                },
-                                "return_modifiers": {
-                                    "items": {
-                                        "properties": {
-                                            "base_price_money": {
-                                                "properties": {
-                                                    "amount": {
-                                                        "type": [
-                                                            "null",
-                                                            "integer"
-                                                        ]
-                                                    },
-                                                    "currency": {
-                                                        "type": [
-                                                            "null",
-                                                            "string"
-                                                        ]
-                                                    }
-                                                },
-                                                "type": [
-                                                    "null",
-                                                    "object"
-                                                ]
-                                            },
-                                            "catalog_object_id": {
-                                                "type": [
-                                                    "null",
-                                                    "string"
-                                                ]
-                                            },
-                                            "name": {
-                                                "type": [
-                                                    "null",
-                                                    "string"
-                                                ]
-                                            },
-                                            "source_modifier_uid": {
-                                                "type": [
-                                                    "null",
-                                                    "string"
-                                                ]
-                                            },
-                                            "total_price_money": {
-                                                "properties": {
-                                                    "amount": {
-                                                        "type": [
-                                                            "null",
-                                                            "integer"
-                                                        ]
-                                                    },
-                                                    "currency": {
-                                                        "type": [
-                                                            "null",
-                                                            "string"
-                                                        ]
-                                                    }
-                                                },
-                                                "type": [
-                                                    "null",
-                                                    "object"
-                                                ]
-                                            },
-                                            "uid": {
-                                                "type": [
-                                                    "null",
-                                                    "string"
-                                                ]
-                                            }
-                                        },
-                                        "type": [
-                                            "null",
-                                            "object"
-                                        ]
-                                    },
-                                    "type": [
-                                        "null",
-                                        "array"
-                                    ]
-                                },
-                                "source_line_item_uid": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                },
-                                "total_discount_money": {
-                                    "properties": {
-                                        "amount": {
-                                            "type": [
-                                                "null",
-                                                "integer"
-                                            ]
-                                        },
-                                        "currency": {
-                                            "type": [
-                                                "null",
-                                                "string"
-                                            ]
-                                        }
-                                    },
-                                    "type": [
-                                        "null",
-                                        "object"
-                                    ]
-                                },
-                                "total_money": {
-                                    "properties": {
-                                        "amount": {
-                                            "type": [
-                                                "null",
-                                                "integer"
-                                            ]
-                                        },
-                                        "currency": {
-                                            "type": [
-                                                "null",
-                                                "string"
-                                            ]
-                                        }
-                                    },
-                                    "type": [
-                                        "null",
-                                        "object"
-                                    ]
-                                },
-                                "total_tax_money": {
-                                    "properties": {
-                                        "amount": {
-                                            "type": [
-                                                "null",
-                                                "integer"
-                                            ]
-                                        },
-                                        "currency": {
-                                            "type": [
-                                                "null",
-                                                "string"
-                                            ]
-                                        }
-                                    },
-                                    "type": [
-                                        "null",
-                                        "object"
-                                    ]
-                                },
-                                "uid": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                },
-                                "variation_name": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                },
-                                "variation_total_price_money": {
-                                    "properties": {
-                                        "amount": {
-                                            "type": [
-                                                "null",
-                                                "integer"
-                                            ]
-                                        },
-                                        "currency": {
-                                            "type": [
-                                                "null",
-                                                "string"
-                                            ]
-                                        }
-                                    },
-                                    "type": [
-                                        "null",
-                                        "object"
-                                    ]
-                                }
-                            },
-                            "type": [
-                                "null",
-                                "object"
-                            ]
-                        },
-                        "type": [
-                            "null",
-                            "array"
-                        ]
-                    },
-                    "source_order_id": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "uid": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    }
                 },
-                "type": [
-                    "null",
-                    "object"
-                ]
-            },
-            "type": [
-                "null",
-                "array"
-            ]
-        },
-        "source": {
-            "properties": {
-                "name": {
+                "administrative_district_level_3": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "country": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "first_name": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "last_name": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "locality": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "postal_code": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "sublocality": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "sublocality_2": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "sublocality_3": {
                     "type": [
                         "null",
                         "string"
                     ]
                 }
             },
             "type": [
@@ -1368,194 +1065,33 @@
         },
         "source_type": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "state": {
+        "statement_description_identifier": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "status": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "tax_data": {
-            "properties": {
-                "name": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                }
-            },
-            "type": [
-                "null",
-                "object"
-            ]
-        },
-        "tenders": {
-            "items": {
-                "properties": {
-                    "amount_money": {
-                        "properties": {
-                            "amount": {
-                                "type": [
-                                    "null",
-                                    "integer"
-                                ]
-                            },
-                            "currency": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            }
-                        },
-                        "type": [
-                            "null",
-                            "object"
-                        ]
-                    },
-                    "card_details": {
-                        "properties": {
-                            "card": {
-                                "properties": {
-                                    "bin": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "card_brand": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "card_type": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "exp_month": {
-                                        "type": [
-                                            "null",
-                                            "integer"
-                                        ]
-                                    },
-                                    "exp_year": {
-                                        "type": [
-                                            "null",
-                                            "integer"
-                                        ]
-                                    },
-                                    "fingerprint": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "last_4": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "prepaid_type": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    }
-                                },
-                                "type": [
-                                    "null",
-                                    "object"
-                                ]
-                            },
-                            "entry_method": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "status": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            }
-                        },
-                        "type": [
-                            "null",
-                            "object"
-                        ]
-                    },
-                    "created_at": {
-                        "format": "date-time",
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "id": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "location_id": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "note": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "payment_id": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "transaction_id": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "type": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    }
-                },
-                "type": [
-                    "null",
-                    "object"
-                ]
-            },
+        "team_member_id": {
             "type": [
                 "null",
-                "array"
+                "string"
             ]
         },
-        "total_discount_money": {
+        "tip_money": {
             "properties": {
                 "amount": {
                     "type": [
                         "null",
                         "integer"
                     ]
                 },
@@ -1587,92 +1123,72 @@
                 }
             },
             "type": [
                 "null",
                 "object"
             ]
         },
-        "total_service_charge_money": {
-            "properties": {
-                "amount": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
-                },
-                "currency": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                }
-            },
+        "updated_at": {
+            "format": "date-time",
             "type": [
                 "null",
-                "object"
+                "string"
             ]
         },
-        "total_tax_money": {
-            "properties": {
-                "amount": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
-                },
-                "currency": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                }
-            },
+        "version_token": {
             "type": [
                 "null",
-                "object"
+                "string"
             ]
         },
-        "total_tip_money": {
+        "wallet_details": {
             "properties": {
-                "amount": {
+                "brand": {
                     "type": [
                         "null",
-                        "integer"
+                        "string"
                     ]
                 },
-                "currency": {
+                "cash_app_details": {
+                    "properties": {
+                        "buyer_cashtag": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "buyer_country_code": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "buyer_full_name": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        }
+                    },
+                    "type": [
+                        "null",
+                        "object"
+                    ]
+                },
+                "status": {
                     "type": [
                         "null",
                         "string"
                     ]
                 }
             },
             "type": [
                 "null",
                 "object"
             ]
-        },
-        "type": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "updated_at": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "version": {
-            "type": [
-                "null",
-                "integer"
-            ]
         }
     },
     "type": [
         "null",
         "object"
     ]
 }
```

### Comparing `tap-square-1.3.1/tap_square/schemas/payments.json` & `tap-square-2.0.0/tap_square/schemas/refunds.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8189655172413793%*

 * *Differences: {"'properties'": "{'unlinked': OrderedDict([('type', ['null', 'boolean'])]), 'destination_type': "*

 * *                 "OrderedDict([('type', ['null', 'string'])]), 'destination_details': "*

 * *                 "OrderedDict([('type', ['null', 'object']), ('properties', "*

 * *                 "OrderedDict([('card_details', OrderedDict([('type', ['null', 'object']), "*

 * *                 "('properties', OrderedDict([('card', OrderedDict([('type', ['null', 'object']), "*

 * *                 "('properties', OrderedDict([('id', O […]*

```diff
@@ -16,173 +16,260 @@
                 }
             },
             "type": [
                 "null",
                 "object"
             ]
         },
-        "card_details": {
+        "app_fee_money": {
             "properties": {
-                "auth_result_code": {
+                "amount": {
                     "type": [
                         "null",
-                        "string"
+                        "integer"
                     ]
                 },
-                "avs_status": {
+                "currency": {
                     "type": [
                         "null",
                         "string"
                     ]
-                },
-                "card": {
+                }
+            },
+            "type": [
+                "null",
+                "object"
+            ]
+        },
+        "created_at": {
+            "format": "date-time",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "destination_details": {
+            "properties": {
+                "card_details": {
                     "properties": {
-                        "bin": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "card_brand": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "card_type": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "cardholder_name": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "exp_month": {
-                            "type": [
-                                "null",
-                                "integer"
-                            ]
-                        },
-                        "exp_year": {
-                            "type": [
-                                "null",
-                                "integer"
-                            ]
-                        },
-                        "fingerprint": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "last_4": {
+                        "card": {
+                            "properties": {
+                                "billing_address": {
+                                    "properties": {
+                                        "address_line_1": {
+                                            "type": [
+                                                "null",
+                                                "string"
+                                            ]
+                                        },
+                                        "address_line_2": {
+                                            "type": [
+                                                "null",
+                                                "string"
+                                            ]
+                                        },
+                                        "address_line_3": {
+                                            "type": [
+                                                "null",
+                                                "string"
+                                            ]
+                                        },
+                                        "administrative_district_level_1": {
+                                            "type": [
+                                                "null",
+                                                "string"
+                                            ]
+                                        },
+                                        "administrative_district_level_2": {
+                                            "type": [
+                                                "null",
+                                                "string"
+                                            ]
+                                        },
+                                        "administrative_district_level_3": {
+                                            "type": [
+                                                "null",
+                                                "string"
+                                            ]
+                                        },
+                                        "country": {
+                                            "type": [
+                                                "null",
+                                                "string"
+                                            ]
+                                        },
+                                        "first_name": {
+                                            "type": [
+                                                "null",
+                                                "string"
+                                            ]
+                                        },
+                                        "last_name": {
+                                            "type": [
+                                                "null",
+                                                "string"
+                                            ]
+                                        },
+                                        "locality": {
+                                            "type": [
+                                                "null",
+                                                "string"
+                                            ]
+                                        },
+                                        "postal_code": {
+                                            "type": [
+                                                "null",
+                                                "string"
+                                            ]
+                                        },
+                                        "sublocality": {
+                                            "type": [
+                                                "null",
+                                                "string"
+                                            ]
+                                        },
+                                        "sublocality_2": {
+                                            "type": [
+                                                "null",
+                                                "string"
+                                            ]
+                                        },
+                                        "sublocality_3": {
+                                            "type": [
+                                                "null",
+                                                "string"
+                                            ]
+                                        }
+                                    },
+                                    "type": [
+                                        "null",
+                                        "object"
+                                    ]
+                                },
+                                "bin": {
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                },
+                                "card_brand": {
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                },
+                                "card_co_brand": {
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                },
+                                "card_type": {
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                },
+                                "cardholder_name": {
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                },
+                                "customer_id": {
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                },
+                                "enabled": {
+                                    "type": [
+                                        "null",
+                                        "boolean"
+                                    ]
+                                },
+                                "exp_month": {
+                                    "type": [
+                                        "null",
+                                        "integer"
+                                    ]
+                                },
+                                "exp_year": {
+                                    "type": [
+                                        "null",
+                                        "integer"
+                                    ]
+                                },
+                                "fingerprint": {
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                },
+                                "id": {
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                },
+                                "last_4": {
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                },
+                                "merchant_id": {
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                },
+                                "prepaid_type": {
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                },
+                                "reference_id": {
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                },
+                                "version": {
+                                    "type": [
+                                        "null",
+                                        "integer"
+                                    ]
+                                }
+                            },
                             "type": [
                                 "null",
-                                "string"
+                                "object"
                             ]
                         },
-                        "prepaid_type": {
+                        "entry_method": {
                             "type": [
                                 "null",
                                 "string"
                             ]
                         }
                     },
                     "type": [
                         "null",
                         "object"
                     ]
-                },
-                "cvv_status": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "entry_method": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "errors": {
-                    "items": {
-                        "category": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "code": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "detail": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        }
-                    },
-                    "type": [
-                        "null",
-                        "array"
-                    ]
-                },
-                "statement_description": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "status": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
                 }
             },
             "type": [
                 "null",
                 "object"
             ]
         },
-        "created_at": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "customer_id": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "delay_action": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "delay_duration": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "delayed_until": {
-            "format": "date-time",
+        "destination_type": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "id": {
             "type": [
@@ -192,21 +279,21 @@
         },
         "location_id": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "note": {
+        "order_id": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "order_id": {
+        "payment_id": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "processing_fee": {
             "items": {
@@ -251,115 +338,36 @@
                 ]
             },
             "type": [
                 "null",
                 "array"
             ]
         },
-        "receipt_number": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "receipt_url": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "reference_id": {
+        "reason": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "refund_ids": {
-            "items": {
-                "type": [
-                    "null",
-                    "string"
-                ]
-            },
-            "type": [
-                "null",
-                "array"
-            ]
-        },
-        "refunded_money": {
-            "properties": {
-                "amount": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
-                },
-                "currency": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                }
-            },
-            "type": [
-                "null",
-                "object"
-            ]
-        },
-        "risk_evaluation": {
-            "properties": {
-                "created_at": {
-                    "format": "date-time",
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "risk_level": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                }
-            },
-            "type": [
-                "null",
-                "object"
-            ]
-        },
-        "source_type": {
+        "status": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "status": {
+        "team_member_id": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "total_money": {
-            "properties": {
-                "amount": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
-                },
-                "currency": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                }
-            },
+        "unlinked": {
             "type": [
                 "null",
-                "object"
+                "boolean"
             ]
         },
         "updated_at": {
             "format": "date-time",
             "type": [
                 "null",
                 "string"
```

### Comparing `tap-square-1.3.1/tap_square/schemas/refunds.json` & `tap-square-2.0.0/tap_square/schemas/shifts.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8235294117647058%*

 * *Differences: {"'properties'": "{'version': OrderedDict([('type', ['null', 'integer'])]), 'end_at': "*

 * *                 "OrderedDict([('type', ['null', 'string']), ('format', 'date-time')]), "*

 * *                 "'start_at': OrderedDict([('type', ['null', 'string']), ('format', "*

 * *                 "'date-time')]), 'breaks': OrderedDict([('items', OrderedDict([('properties', "*

 * *                 "OrderedDict([('expected_duration', OrderedDict([('type', ['null', 'string'])])), "*

 * *                 "('id', OrderedDict([('type', ['n […]*

```diff
@@ -1,125 +1,170 @@
 {
     "properties": {
-        "amount_money": {
-            "properties": {
-                "amount": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
+        "breaks": {
+            "items": {
+                "properties": {
+                    "break_type_id": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "end_at": {
+                        "format": "date-time",
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "expected_duration": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "id": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "is_paid": {
+                        "type": [
+                            "null",
+                            "boolean"
+                        ]
+                    },
+                    "name": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "start_at": {
+                        "format": "date-time",
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    }
                 },
-                "currency": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                }
+                "type": [
+                    "null",
+                    "object"
+                ]
             },
             "type": [
                 "null",
-                "object"
+                "array"
             ]
         },
         "created_at": {
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "id": {
+        "end_at": {
+            "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "location_id": {
+        "id": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "order_id": {
+        "location_id": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "payment_id": {
+        "start_at": {
+            "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "processing_fee": {
-            "items": {
-                "properties": {
-                    "amount_money": {
-                        "properties": {
-                            "amount": {
-                                "type": [
-                                    "null",
-                                    "integer"
-                                ]
-                            },
-                            "currency": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            }
-                        },
-                        "type": [
-                            "null",
-                            "object"
-                        ]
-                    },
-                    "effective_at": {
-                        "format": "date-time",
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "type": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    }
-                },
-                "type": [
-                    "null",
-                    "object"
-                ]
-            },
+        "status": {
             "type": [
                 "null",
-                "array"
+                "string"
             ]
         },
-        "reason": {
+        "team_member_id": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "status": {
+        "timezone": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "updated_at": {
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
+        },
+        "version": {
+            "type": [
+                "null",
+                "integer"
+            ]
+        },
+        "wage": {
+            "properties": {
+                "hourly_rate": {
+                    "properties": {
+                        "amount": {
+                            "type": [
+                                "null",
+                                "integer"
+                            ]
+                        },
+                        "currency": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        }
+                    },
+                    "type": [
+                        "null",
+                        "object"
+                    ]
+                },
+                "job_id": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "title": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                }
+            },
+            "type": [
+                "null",
+                "object"
+            ]
         }
     },
     "type": [
         "null",
         "object"
     ]
 }
```

### Comparing `tap-square-1.3.1/tap_square/schemas/settlements.json` & `tap-square-2.0.0/tap_square/schemas/settlements.json`

 * *Files identical despite different names*

### Comparing `tap-square-1.3.1/tap_square/schemas/shifts.json` & `tap-square-2.0.0/tap_square/schemas/cash_drawer_shifts.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.55%*

 * *Differences: {"'properties'": "{'closed_at': OrderedDict([('type', ['null', 'string']), ('format', "*

 * *                 "'date-time')]), 'closed_cash_money': OrderedDict([('type', ['null', 'object']), "*

 * *                 "('properties', OrderedDict([('amount', OrderedDict([('type', ['null', "*

 * *                 "'integer'])])), ('currency', OrderedDict([('type', ['null', 'string'])]))]))]), "*

 * *                 "'description': OrderedDict([('type', ['null', 'string'])]), 'ended_at': "*

 * *                 "OrderedDict([('type', [' […]*

```diff
@@ -1,164 +1,124 @@
 {
     "properties": {
-        "breaks": {
-            "items": {
-                "properties": {
-                    "break_type_id": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "end_at": {
-                        "format": "date-time",
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "expected_duration": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "id": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "is_paid": {
-                        "type": [
-                            "null",
-                            "boolean"
-                        ]
-                    },
-                    "name": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "start_at": {
-                        "format": "date-time",
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    }
-                },
-                "type": [
-                    "null",
-                    "object"
-                ]
-            },
-            "type": [
-                "null",
-                "array"
-            ]
-        },
-        "created_at": {
+        "closed_at": {
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "employee_id": {
+        "closed_cash_money": {
+            "properties": {
+                "amount": {
+                    "type": [
+                        "null",
+                        "integer"
+                    ]
+                },
+                "currency": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                }
+            },
             "type": [
                 "null",
-                "string"
+                "object"
             ]
         },
-        "end_at": {
+        "created_at": {
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "id": {
+        "description": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "location_id": {
+        "ended_at": {
+            "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "start_at": {
-            "format": "date-time",
+        "expected_cash_money": {
+            "properties": {
+                "amount": {
+                    "type": [
+                        "null",
+                        "integer"
+                    ]
+                },
+                "currency": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                }
+            },
             "type": [
                 "null",
-                "string"
+                "object"
             ]
         },
-        "status": {
+        "id": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "timezone": {
+        "location_id": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "updated_at": {
+        "opened_at": {
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "version": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "wage": {
+        "opened_cash_money": {
             "properties": {
-                "hourly_rate": {
-                    "properties": {
-                        "amount": {
-                            "type": [
-                                "null",
-                                "integer"
-                            ]
-                        },
-                        "currency": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        }
-                    },
+                "amount": {
                     "type": [
                         "null",
-                        "object"
+                        "integer"
                     ]
                 },
-                "title": {
+                "currency": {
                     "type": [
                         "null",
                         "string"
                     ]
                 }
             },
             "type": [
                 "null",
                 "object"
             ]
+        },
+        "state": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "updated_at": {
+            "format": "date-time",
+            "type": [
+                "null",
+                "string"
+            ]
         }
     },
-    "type": [
-        "null",
-        "object"
-    ]
+    "type": "object"
 }
```

### Comparing `tap-square-1.3.1/tap_square/streams.py` & `tap-square-2.0.0/tap_square/streams.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,44 +122,14 @@
     key_properties = ['id']
     replication_method = 'INCREMENTAL'
     valid_replication_keys = ['updated_at']
     replication_key = 'updated_at'
     object_type = 'TAX'
 
 
-class Employees(FullTableStream):
-    tap_stream_id = 'employees'
-    key_properties = ['id']
-    replication_method = 'FULL_TABLE'
-    valid_replication_keys = []
-    replication_key = None
-
-    def get_pages(self, bookmarked_cursor, start_time):
-        yield from self.client.get_employees(bookmarked_cursor)
-
-    def sync(self, state, stream_schema, stream_metadata, config, transformer):
-        start_time = config['start_date']
-        bookmarked_cursor = singer.get_bookmark(state, self.tap_stream_id, 'cursor')
-
-        for page, cursor in self.get_pages_safe(state, bookmarked_cursor, start_time):
-            for record in page:
-                if record['updated_at'] >= start_time:
-                    transformed_record = transformer.transform(record, stream_schema, stream_metadata)
-                    singer.write_record(
-                        self.tap_stream_id,
-                        transformed_record,
-                    )
-            singer.write_bookmark(state, self.tap_stream_id, 'cursor', cursor)
-            singer.write_state(state)
-
-        state = singer.clear_bookmark(state, self.tap_stream_id, 'cursor')
-        singer.write_state(state)
-        return state
-
-
 class ModifierLists(CatalogStream):
     tap_stream_id = 'modifier_lists'
     key_properties = ['id']
     replication_method = 'INCREMENTAL'
     valid_replication_keys = ['updated_at']
     replication_key = 'updated_at'
     object_type = 'MODIFIER_LIST'
@@ -369,14 +339,38 @@
     replication_key = None
 
     def get_pages(self, bookmarked_cursor, start_time):
         for location_id in Locations.get_all_location_ids(self.client):
             # Settlements requests can only take up to 1 location_id at a time
             yield from self.client.get_settlements(location_id, start_time, bookmarked_cursor)
 
+class TeamMembers(Stream):
+    tap_stream_id = 'team_members'
+    key_properties = ['id']
+    replication_method = 'INCREMENTAL'
+    valid_replication_keys = ['updated_at']
+    replication_key = 'updated_at'
+    object_type = 'team_members'
+
+    def sync(self, state, stream_schema, stream_metadata, config, transformer):
+        start_time = singer.get_bookmark(state, self.tap_stream_id, self.replication_key, config['start_date'])
+        max_record_value = start_time
+        all_location_ids = Locations.get_all_location_ids(self.client)
+
+        for page, _ in self.client.get_team_members(all_location_ids):
+            for record in page:
+                transformed_record = transformer.transform(record, stream_schema, stream_metadata)
+
+                if record[self.replication_key] > max_record_value:
+                    singer.write_record(self.tap_stream_id, transformed_record,)
+                    max_record_value = transformed_record[self.replication_key]
+
+            state = singer.write_bookmark(state, self.tap_stream_id, self.replication_key, max_record_value)
+            singer.write_state(state)
+        return state
 
 class Customers(Stream):
     tap_stream_id = 'customers'
     key_properties = ['id']
     replication_method = 'INCREMENTAL'
     valid_replication_keys = ['updated_at']
     replication_key = 'updated_at'
@@ -397,21 +391,21 @@
         return state
 
 STREAMS = {
     'items': Items,
     'categories': Categories,
     'discounts': Discounts,
     'taxes': Taxes,
-    'employees': Employees,
     'locations': Locations,
     'bank_accounts': BankAccounts,
     'refunds': Refunds,
     'payments': Payments,
     'modifier_lists': ModifierLists,
     'inventories': Inventories,
     'orders': Orders,
     'roles': Roles,
     'shifts': Shifts,
     'cash_drawer_shifts': CashDrawerShifts,
     'settlements': Settlements,
+    'team_members': TeamMembers,
     'customers': Customers
 }
```

### Comparing `tap-square-1.3.1/tap_square/sync.py` & `tap-square-2.0.0/tap_square/sync.py`

 * *Files identical despite different names*

### Comparing `tap-square-1.3.1/tap_square.egg-info/SOURCES.txt` & `tap-square-2.0.0/tap_square.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 tap_square.egg-info/requires.txt
 tap_square.egg-info/top_level.txt
 tap_square/schemas/bank_accounts.json
 tap_square/schemas/cash_drawer_shifts.json
 tap_square/schemas/categories.json
 tap_square/schemas/customers.json
 tap_square/schemas/discounts.json
-tap_square/schemas/employees.json
 tap_square/schemas/inventories.json
 tap_square/schemas/items.json
 tap_square/schemas/locations.json
 tap_square/schemas/modifier_lists.json
 tap_square/schemas/orders.json
 tap_square/schemas/payments.json
 tap_square/schemas/refunds.json
 tap_square/schemas/roles.json
 tap_square/schemas/settlements.json
 tap_square/schemas/shifts.json
-tap_square/schemas/taxes.json
+tap_square/schemas/taxes.json
+tap_square/schemas/team_members.json
```

