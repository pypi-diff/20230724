# Comparing `tmp/dbt-materialize-1.5.0.tar.gz` & `tmp/dbt-materialize-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-materialize-1.5.0.tar", last modified: Thu Jul 13 19:12:06 2023, max compression
+gzip compressed data, was "dbt-materialize-1.5.1.tar", last modified: Mon Jul 24 13:45:46 2023, max compression
```

## Comparing `dbt-materialize-1.5.0.tar` & `dbt-materialize-1.5.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-07-13 19:12:06.656389 dbt-materialize-1.5.0/
--rw-r--r--   0 materialize  (2000) materialize  (1001)     5950 2023-07-13 19:12:06.656389 dbt-materialize-1.5.0/PKG-INFO
--rw-r--r--   0 materialize  (2000) materialize  (1001)     5592 2023-07-13 19:11:38.000000 dbt-materialize-1.5.0/README.md
-drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-07-13 19:12:06.656389 dbt-materialize-1.5.0/dbt/
--rw-r--r--   0 materialize  (2000) materialize  (1001)      729 2023-07-13 19:11:38.000000 dbt-materialize-1.5.0/dbt/__init__.py
-drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-07-13 19:12:06.656389 dbt-materialize-1.5.0/dbt/adapters/
--rw-r--r--   0 materialize  (2000) materialize  (1001)      729 2023-07-13 19:11:38.000000 dbt-materialize-1.5.0/dbt/adapters/__init__.py
-drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-07-13 19:12:06.656389 dbt-materialize-1.5.0/dbt/adapters/materialize/
--rw-r--r--   0 materialize  (2000) materialize  (1001)     1159 2023-07-13 19:11:38.000000 dbt-materialize-1.5.0/dbt/adapters/materialize/__init__.py
--rw-r--r--   0 materialize  (2000) materialize  (1001)      801 2023-07-13 19:11:38.000000 dbt-materialize-1.5.0/dbt/adapters/materialize/__version__.py
--rw-r--r--   0 materialize  (2000) materialize  (1001)     3431 2023-07-13 19:11:38.000000 dbt-materialize-1.5.0/dbt/adapters/materialize/connections.py
--rw-r--r--   0 materialize  (2000) materialize  (1001)     4802 2023-07-13 19:11:38.000000 dbt-materialize-1.5.0/dbt/adapters/materialize/impl.py
--rw-r--r--   0 materialize  (2000) materialize  (1001)     1688 2023-07-13 19:11:38.000000 dbt-materialize-1.5.0/dbt/adapters/materialize/relation.py
-drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-07-13 19:12:06.656389 dbt-materialize-1.5.0/dbt/include/
--rw-r--r--   0 materialize  (2000) materialize  (1001)      729 2023-07-13 19:11:38.000000 dbt-materialize-1.5.0/dbt/include/__init__.py
-drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-07-13 19:12:06.656389 dbt-materialize-1.5.0/dbt/include/materialize/
--rw-r--r--   0 materialize  (2000) materialize  (1001)      782 2023-07-13 19:11:38.000000 dbt-materialize-1.5.0/dbt/include/materialize/__init__.py
--rw-r--r--   0 materialize  (2000) materialize  (1001)      808 2023-07-13 19:11:38.000000 dbt-materialize-1.5.0/dbt/include/materialize/dbt_project.yml
-drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-07-13 19:12:06.656389 dbt-materialize-1.5.0/dbt/include/materialize/macros/
--rw-r--r--   0 materialize  (2000) materialize  (1001)     4808 2023-07-13 19:11:38.000000 dbt-materialize-1.5.0/dbt/include/materialize/macros/adapters.sql
--rw-r--r--   0 materialize  (2000) materialize  (1001)     2222 2023-07-13 19:11:38.000000 dbt-materialize-1.5.0/dbt/include/materialize/macros/catalog.sql
-drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-07-13 19:12:06.656389 dbt-materialize-1.5.0/dbt/include/materialize/macros/materializations/
--rw-r--r--   0 materialize  (2000) materialize  (1001)     1909 2023-07-13 19:11:38.000000 dbt-materialize-1.5.0/dbt/include/materialize/macros/materializations/incremental.sql
--rw-r--r--   0 materialize  (2000) materialize  (1001)     1920 2023-07-13 19:11:38.000000 dbt-materialize-1.5.0/dbt/include/materialize/macros/materializations/materialized_view.sql
--rw-r--r--   0 materialize  (2000) materialize  (1001)     3023 2023-07-13 19:11:38.000000 dbt-materialize-1.5.0/dbt/include/materialize/macros/materializations/seed.sql
--rw-r--r--   0 materialize  (2000) materialize  (1001)     1784 2023-07-13 19:11:38.000000 dbt-materialize-1.5.0/dbt/include/materialize/macros/materializations/sink.sql
--rw-r--r--   0 materialize  (2000) materialize  (1001)     1828 2023-07-13 19:11:38.000000 dbt-materialize-1.5.0/dbt/include/materialize/macros/materializations/source.sql
--rw-r--r--   0 materialize  (2000) materialize  (1001)     1933 2023-07-13 19:11:38.000000 dbt-materialize-1.5.0/dbt/include/materialize/macros/materializations/table.sql
--rw-r--r--   0 materialize  (2000) materialize  (1001)     1960 2023-07-13 19:11:38.000000 dbt-materialize-1.5.0/dbt/include/materialize/macros/materializations/test.sql
--rw-r--r--   0 materialize  (2000) materialize  (1001)     1883 2023-07-13 19:11:38.000000 dbt-materialize-1.5.0/dbt/include/materialize/macros/materializations/view.sql
-drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-07-13 19:12:06.656389 dbt-materialize-1.5.0/dbt/include/materialize/macros/utils/
--rw-r--r--   0 materialize  (2000) materialize  (1001)     1016 2023-07-13 19:11:38.000000 dbt-materialize-1.5.0/dbt/include/materialize/macros/utils/listagg.sql
-drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-07-13 19:12:06.656389 dbt-materialize-1.5.0/dbt_materialize.egg-info/
--rw-r--r--   0 materialize  (2000) materialize  (1001)     5950 2023-07-13 19:12:06.000000 dbt-materialize-1.5.0/dbt_materialize.egg-info/PKG-INFO
--rw-r--r--   0 materialize  (2000) materialize  (1001)     1155 2023-07-13 19:12:06.000000 dbt-materialize-1.5.0/dbt_materialize.egg-info/SOURCES.txt
--rw-r--r--   0 materialize  (2000) materialize  (1001)        1 2023-07-13 19:12:06.000000 dbt-materialize-1.5.0/dbt_materialize.egg-info/dependency_links.txt
--rw-r--r--   0 materialize  (2000) materialize  (1001)       52 2023-07-13 19:12:06.000000 dbt-materialize-1.5.0/dbt_materialize.egg-info/requires.txt
--rw-r--r--   0 materialize  (2000) materialize  (1001)        4 2023-07-13 19:12:06.000000 dbt-materialize-1.5.0/dbt_materialize.egg-info/top_level.txt
--rw-r--r--   0 materialize  (2000) materialize  (1001)       38 2023-07-13 19:12:06.656389 dbt-materialize-1.5.0/setup.cfg
--rw-r--r--   0 materialize  (2000) materialize  (1001)     1768 2023-07-13 19:11:38.000000 dbt-materialize-1.5.0/setup.py
+drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-07-24 13:45:46.870505 dbt-materialize-1.5.1/
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     5958 2023-07-24 13:45:46.870505 dbt-materialize-1.5.1/PKG-INFO
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     5600 2023-07-24 13:45:17.000000 dbt-materialize-1.5.1/README.md
+drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-07-24 13:45:46.870505 dbt-materialize-1.5.1/dbt/
+-rw-r--r--   0 materialize  (2000) materialize  (1001)      729 2023-07-24 13:45:17.000000 dbt-materialize-1.5.1/dbt/__init__.py
+drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-07-24 13:45:46.870505 dbt-materialize-1.5.1/dbt/adapters/
+-rw-r--r--   0 materialize  (2000) materialize  (1001)      729 2023-07-24 13:45:17.000000 dbt-materialize-1.5.1/dbt/adapters/__init__.py
+drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-07-24 13:45:46.870505 dbt-materialize-1.5.1/dbt/adapters/materialize/
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     1159 2023-07-24 13:45:17.000000 dbt-materialize-1.5.1/dbt/adapters/materialize/__init__.py
+-rw-r--r--   0 materialize  (2000) materialize  (1001)      801 2023-07-24 13:45:17.000000 dbt-materialize-1.5.1/dbt/adapters/materialize/__version__.py
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     3431 2023-07-24 13:45:17.000000 dbt-materialize-1.5.1/dbt/adapters/materialize/connections.py
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     4802 2023-07-24 13:45:17.000000 dbt-materialize-1.5.1/dbt/adapters/materialize/impl.py
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     1688 2023-07-24 13:45:17.000000 dbt-materialize-1.5.1/dbt/adapters/materialize/relation.py
+drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-07-24 13:45:46.870505 dbt-materialize-1.5.1/dbt/include/
+-rw-r--r--   0 materialize  (2000) materialize  (1001)      729 2023-07-24 13:45:17.000000 dbt-materialize-1.5.1/dbt/include/__init__.py
+drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-07-24 13:45:46.870505 dbt-materialize-1.5.1/dbt/include/materialize/
+-rw-r--r--   0 materialize  (2000) materialize  (1001)      782 2023-07-24 13:45:17.000000 dbt-materialize-1.5.1/dbt/include/materialize/__init__.py
+-rw-r--r--   0 materialize  (2000) materialize  (1001)      808 2023-07-24 13:45:17.000000 dbt-materialize-1.5.1/dbt/include/materialize/dbt_project.yml
+drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-07-24 13:45:46.870505 dbt-materialize-1.5.1/dbt/include/materialize/macros/
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     4808 2023-07-24 13:45:17.000000 dbt-materialize-1.5.1/dbt/include/materialize/macros/adapters.sql
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     2222 2023-07-24 13:45:17.000000 dbt-materialize-1.5.1/dbt/include/materialize/macros/catalog.sql
+drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-07-24 13:45:46.870505 dbt-materialize-1.5.1/dbt/include/materialize/macros/materializations/
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     1909 2023-07-24 13:45:17.000000 dbt-materialize-1.5.1/dbt/include/materialize/macros/materializations/incremental.sql
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     1920 2023-07-24 13:45:17.000000 dbt-materialize-1.5.1/dbt/include/materialize/macros/materializations/materialized_view.sql
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     3023 2023-07-24 13:45:17.000000 dbt-materialize-1.5.1/dbt/include/materialize/macros/materializations/seed.sql
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     1784 2023-07-24 13:45:17.000000 dbt-materialize-1.5.1/dbt/include/materialize/macros/materializations/sink.sql
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     1828 2023-07-24 13:45:17.000000 dbt-materialize-1.5.1/dbt/include/materialize/macros/materializations/source.sql
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     1973 2023-07-24 13:45:17.000000 dbt-materialize-1.5.1/dbt/include/materialize/macros/materializations/table.sql
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     1960 2023-07-24 13:45:17.000000 dbt-materialize-1.5.1/dbt/include/materialize/macros/materializations/test.sql
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     1883 2023-07-24 13:45:17.000000 dbt-materialize-1.5.1/dbt/include/materialize/macros/materializations/view.sql
+drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-07-24 13:45:46.870505 dbt-materialize-1.5.1/dbt/include/materialize/macros/utils/
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     1016 2023-07-24 13:45:17.000000 dbt-materialize-1.5.1/dbt/include/materialize/macros/utils/listagg.sql
+drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-07-24 13:45:46.870505 dbt-materialize-1.5.1/dbt_materialize.egg-info/
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     5958 2023-07-24 13:45:46.000000 dbt-materialize-1.5.1/dbt_materialize.egg-info/PKG-INFO
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     1155 2023-07-24 13:45:46.000000 dbt-materialize-1.5.1/dbt_materialize.egg-info/SOURCES.txt
+-rw-r--r--   0 materialize  (2000) materialize  (1001)        1 2023-07-24 13:45:46.000000 dbt-materialize-1.5.1/dbt_materialize.egg-info/dependency_links.txt
+-rw-r--r--   0 materialize  (2000) materialize  (1001)       52 2023-07-24 13:45:46.000000 dbt-materialize-1.5.1/dbt_materialize.egg-info/requires.txt
+-rw-r--r--   0 materialize  (2000) materialize  (1001)        4 2023-07-24 13:45:46.000000 dbt-materialize-1.5.1/dbt_materialize.egg-info/top_level.txt
+-rw-r--r--   0 materialize  (2000) materialize  (1001)       38 2023-07-24 13:45:46.870505 dbt-materialize-1.5.1/setup.cfg
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     1768 2023-07-24 13:45:17.000000 dbt-materialize-1.5.1/setup.py
```

### Comparing `dbt-materialize-1.5.0/PKG-INFO` & `dbt-materialize-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-materialize
-Version: 1.5.0
+Version: 1.5.1
 Summary: The Materialize adapter plugin for dbt.
 Home-page: https://github.com/MaterializeInc/materialize/blob/main/misc/dbt-materialize
 Author: Materialize, Inc.
 Author-email: support@materialize.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -70,15 +70,15 @@
 `table`            | YES        | Creates a [materialized view]. (Actual table support pending [#5266].)
 `sink`             | YES        | Creates a [sink].
 `ephemeral`        | YES        | Executes queries using CTEs.
 `incremental`      | NO         | Use the `materializedview` materialization instead! dbt's incremental models are valuable because they only spend your time and money transforming your new data as it arrives. Luckily, this is exactly what Materialize's materialized views were built to do! Better yet, our materialized views will always return up-to-date results without manual or configured refreshes. For more information, check out [our documentation](https://materialize.com/docs/).
 
 ### Indexes
 
-Use the indexes option to define a list of [indexes](/sql/create-index/) on `source`, `view`, or `materialized view` materializations. Each Materialize index can have the following components:
+Use the indexes option to define a list of [indexes](/sql/create-index/) on `source`, `view`, `table` or `materialized view` materializations. Each Materialize index can have the following components:
 
 Component                            | Value     | Description
 -------------------------------------|-----------|--------------------------------------------------
 `columns`                            | `list`    | One or more columns on which the index is defined. To create an index that uses _all_ columns, use the `default` component instead.
 `name`                               | `string`  | The name for the index. If unspecified, Materialize will use the materialization name and column names provided.
 `cluster`                            | `string`  | The cluster to use to create the index. If unspecified, indexes will be created in the cluster used to create the materialization.
 `default`                            | `bool`    | Default: `False`. If set to `True`, creates a default index that uses all columns.
```

### Comparing `dbt-materialize-1.5.0/README.md` & `dbt-materialize-1.5.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 `table`            | YES        | Creates a [materialized view]. (Actual table support pending [#5266].)
 `sink`             | YES        | Creates a [sink].
 `ephemeral`        | YES        | Executes queries using CTEs.
 `incremental`      | NO         | Use the `materializedview` materialization instead! dbt's incremental models are valuable because they only spend your time and money transforming your new data as it arrives. Luckily, this is exactly what Materialize's materialized views were built to do! Better yet, our materialized views will always return up-to-date results without manual or configured refreshes. For more information, check out [our documentation](https://materialize.com/docs/).
 
 ### Indexes
 
-Use the indexes option to define a list of [indexes](/sql/create-index/) on `source`, `view`, or `materialized view` materializations. Each Materialize index can have the following components:
+Use the indexes option to define a list of [indexes](/sql/create-index/) on `source`, `view`, `table` or `materialized view` materializations. Each Materialize index can have the following components:
 
 Component                            | Value     | Description
 -------------------------------------|-----------|--------------------------------------------------
 `columns`                            | `list`    | One or more columns on which the index is defined. To create an index that uses _all_ columns, use the `default` component instead.
 `name`                               | `string`  | The name for the index. If unspecified, Materialize will use the materialization name and column names provided.
 `cluster`                            | `string`  | The cluster to use to create the index. If unspecified, indexes will be created in the cluster used to create the materialization.
 `default`                            | `bool`    | Default: `False`. If set to `True`, creates a default index that uses all columns.
```

### Comparing `dbt-materialize-1.5.0/dbt/__init__.py` & `dbt-materialize-1.5.1/dbt/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.5.0/dbt/adapters/__init__.py` & `dbt-materialize-1.5.1/dbt/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.5.0/dbt/adapters/materialize/__init__.py` & `dbt-materialize-1.5.1/dbt/adapters/materialize/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.5.0/dbt/adapters/materialize/__version__.py` & `dbt-materialize-1.5.1/dbt/adapters/materialize/__version__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # If you bump this version, bump it in setup.py too.
-version = "1.5.0"
+version = "1.5.1"
```

### Comparing `dbt-materialize-1.5.0/dbt/adapters/materialize/connections.py` & `dbt-materialize-1.5.1/dbt/adapters/materialize/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.5.0/dbt/adapters/materialize/impl.py` & `dbt-materialize-1.5.1/dbt/adapters/materialize/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.5.0/dbt/adapters/materialize/relation.py` & `dbt-materialize-1.5.1/dbt/adapters/materialize/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.5.0/dbt/include/__init__.py` & `dbt-materialize-1.5.1/dbt/include/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.5.0/dbt/include/materialize/__init__.py` & `dbt-materialize-1.5.1/dbt/include/materialize/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.5.0/dbt/include/materialize/dbt_project.yml` & `dbt-materialize-1.5.1/dbt/include/materialize/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.5.0/dbt/include/materialize/macros/adapters.sql` & `dbt-materialize-1.5.1/dbt/include/materialize/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.5.0/dbt/include/materialize/macros/catalog.sql` & `dbt-materialize-1.5.1/dbt/include/materialize/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.5.0/dbt/include/materialize/macros/materializations/incremental.sql` & `dbt-materialize-1.5.1/dbt/include/materialize/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.5.0/dbt/include/materialize/macros/materializations/materialized_view.sql` & `dbt-materialize-1.5.1/dbt/include/materialize/macros/materializations/materialized_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.5.0/dbt/include/materialize/macros/materializations/seed.sql` & `dbt-materialize-1.5.1/dbt/include/materialize/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.5.0/dbt/include/materialize/macros/materializations/sink.sql` & `dbt-materialize-1.5.1/dbt/include/materialize/macros/materializations/sink.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.5.0/dbt/include/materialize/macros/materializations/source.sql` & `dbt-materialize-1.5.1/dbt/include/materialize/macros/materializations/source.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.5.0/dbt/include/materialize/macros/materializations/table.sql` & `dbt-materialize-1.5.1/dbt/include/materialize/macros/materializations/table.sql`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
   {{ run_hooks(pre_hooks, inside_transaction=True) }}
 
   {% call statement('main') -%}
     -- Creates a materialized view, not a table, in Materialize
     {{ materialize__create_materialized_view_as(target_relation, sql) }}
   {%- endcall %}
 
+  {{ create_indexes(target_relation) }}
   {% do persist_docs(target_relation, model) %}
 
   {{ run_hooks(post_hooks, inside_transaction=False) }}
   {{ run_hooks(post_hooks, inside_transaction=True) }}
 
   {{ return({'relations': [target_relation]}) }}
 {% endmaterialization %}
```

### Comparing `dbt-materialize-1.5.0/dbt/include/materialize/macros/materializations/test.sql` & `dbt-materialize-1.5.1/dbt/include/materialize/macros/materializations/test.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.5.0/dbt/include/materialize/macros/materializations/view.sql` & `dbt-materialize-1.5.1/dbt/include/materialize/macros/materializations/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.5.0/dbt/include/materialize/macros/utils/listagg.sql` & `dbt-materialize-1.5.1/dbt/include/materialize/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.5.0/dbt_materialize.egg-info/PKG-INFO` & `dbt-materialize-1.5.1/dbt_materialize.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-materialize
-Version: 1.5.0
+Version: 1.5.1
 Summary: The Materialize adapter plugin for dbt.
 Home-page: https://github.com/MaterializeInc/materialize/blob/main/misc/dbt-materialize
 Author: Materialize, Inc.
 Author-email: support@materialize.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -70,15 +70,15 @@
 `table`            | YES        | Creates a [materialized view]. (Actual table support pending [#5266].)
 `sink`             | YES        | Creates a [sink].
 `ephemeral`        | YES        | Executes queries using CTEs.
 `incremental`      | NO         | Use the `materializedview` materialization instead! dbt's incremental models are valuable because they only spend your time and money transforming your new data as it arrives. Luckily, this is exactly what Materialize's materialized views were built to do! Better yet, our materialized views will always return up-to-date results without manual or configured refreshes. For more information, check out [our documentation](https://materialize.com/docs/).
 
 ### Indexes
 
-Use the indexes option to define a list of [indexes](/sql/create-index/) on `source`, `view`, or `materialized view` materializations. Each Materialize index can have the following components:
+Use the indexes option to define a list of [indexes](/sql/create-index/) on `source`, `view`, `table` or `materialized view` materializations. Each Materialize index can have the following components:
 
 Component                            | Value     | Description
 -------------------------------------|-----------|--------------------------------------------------
 `columns`                            | `list`    | One or more columns on which the index is defined. To create an index that uses _all_ columns, use the `default` component instead.
 `name`                               | `string`  | The name for the index. If unspecified, Materialize will use the materialization name and column names provided.
 `cluster`                            | `string`  | The cluster to use to create the index. If unspecified, indexes will be created in the cluster used to create the materialization.
 `default`                            | `bool`    | Default: `False`. If set to `True`, creates a default index that uses all columns.
```

### Comparing `dbt-materialize-1.5.0/dbt_materialize.egg-info/SOURCES.txt` & `dbt-materialize-1.5.1/dbt_materialize.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.5.0/setup.py` & `dbt-materialize-1.5.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from setuptools import find_packages
 
 setup(
     name="dbt-materialize",
     # This adapter's minor version should match the required dbt-postgres version,
     # but patch versions may differ.
     # If you bump this version, bump it in __version__.py too.
-    version="1.5.0",
+    version="1.5.1",
     description="The Materialize adapter plugin for dbt.",
     long_description=(Path(__file__).parent / "README.md").open().read(),
     long_description_content_type="text/markdown",
     author="Materialize, Inc.",
     author_email="support@materialize.com",
     url="https://github.com/MaterializeInc/materialize/blob/main/misc/dbt-materialize",
     packages=find_packages(),
```

