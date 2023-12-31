# Comparing `tmp/pysigma_backend_cortexxdr-0.1.0.tar.gz` & `tmp/pysigma_backend_cortexxdr-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysigma_backend_cortexxdr-0.1.0.tar", max compression
+gzip compressed data, was "pysigma_backend_cortexxdr-0.1.1.tar", max compression
```

## Comparing `pysigma_backend_cortexxdr-0.1.0.tar` & `pysigma_backend_cortexxdr-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1067 2023-07-01 16:30:37.865496 pysigma_backend_cortexxdr-0.1.0/LICENSE
--rw-r--r--   0        0        0      569 2023-07-01 16:30:37.869496 pysigma_backend_cortexxdr-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      363 2023-07-01 16:30:37.869496 pysigma_backend_cortexxdr-0.1.0/sigma/backends/cortexxdr/__init__.py
--rw-r--r--   0        0        0    11085 2023-07-01 16:30:37.869496 pysigma_backend_cortexxdr-0.1.0/sigma/backends/cortexxdr/cortexxdr.py
--rw-r--r--   0        0        0      265 2023-07-01 16:30:37.869496 pysigma_backend_cortexxdr-0.1.0/sigma/pipelines/cortexxdr/__init__.py
--rw-r--r--   0        0        0    11740 2023-07-01 16:30:37.869496 pysigma_backend_cortexxdr-0.1.0/sigma/pipelines/cortexxdr/cortexxdr.py
--rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 pysigma_backend_cortexxdr-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-24 20:27:17.500359 pysigma_backend_cortexxdr-0.1.1/LICENSE
+-rw-r--r--   0        0        0      569 2023-07-24 20:27:17.500359 pysigma_backend_cortexxdr-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      363 2023-07-24 20:27:17.500359 pysigma_backend_cortexxdr-0.1.1/sigma/backends/cortexxdr/__init__.py
+-rw-r--r--   0        0        0    10727 2023-07-24 20:27:17.500359 pysigma_backend_cortexxdr-0.1.1/sigma/backends/cortexxdr/cortexxdr.py
+-rw-r--r--   0        0        0      265 2023-07-24 20:27:17.500359 pysigma_backend_cortexxdr-0.1.1/sigma/pipelines/cortexxdr/__init__.py
+-rw-r--r--   0        0        0    11740 2023-07-24 20:27:17.500359 pysigma_backend_cortexxdr-0.1.1/sigma/pipelines/cortexxdr/cortexxdr.py
+-rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 pysigma_backend_cortexxdr-0.1.1/PKG-INFO
```

### Comparing `pysigma_backend_cortexxdr-0.1.0/LICENSE` & `pysigma_backend_cortexxdr-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pysigma_backend_cortexxdr-0.1.0/pyproject.toml` & `pysigma_backend_cortexxdr-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pySigma-backend-cortexxdr"
-version = "0.1.0"
+version = "0.1.1"
 description = "pySigma CortexXDR backend"
 authors = ["Cori Smith <cs2718281@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/7RedViolin/pySigma-backend-cortexxdr"
 packages = [
     { include = "sigma" }
 ]
```

### Comparing `pysigma_backend_cortexxdr-0.1.0/sigma/backends/cortexxdr/cortexxdr.py` & `pysigma_backend_cortexxdr-0.1.1/sigma/backends/cortexxdr/cortexxdr.py`

 * *Files 5% similar despite different names*

```diff
@@ -124,35 +124,31 @@
     #unbound_value_re_expression : ClassVar[str] = '_=~{value}'   # Expression for regular expression not bound to a field as format string with placeholder {value} and {flag_x} as described for re_expression
 
     # Query finalization: appending and concatenating deferred query part
     deferred_start : ClassVar[str] = "\n| "               # String used as separator between main query and deferred parts
     deferred_separator : ClassVar[str] = "\n| "           # String used to join multiple deferred query parts
     #deferred_only_query : ClassVar[str] = "*"            # String used as query if final query only contains deferred expression
 
-    def convert_condition_field_eq_val_num(self, cond : ConditionFieldEqualsValueExpression, state : ConversionState) -> Union[str, DeferredQueryExpression]:
-        """
-        Conversion of field = number value expressions
-        In Cortex XDR, number fields must be treated as strings and quoted
-        """
-        try:
-            return self.escape_and_quote_field(cond.field) + self.eq_token + '"' + str(cond.value) + '"'
-        except TypeError:       # pragma: no cover
-            raise NotImplementedError("Field equals numeric value expressions are not supported by the backend.")
-
     def finalize_query_default(self, rule: SigmaRule, query: str, index: int, state: ConversionState) -> Any:
         """
         Finalize conversion result of a query
         This will add the dataset name to the beginning of the query based on the rule category.
         The dataset name is generated by the ProcessingPipeline state which is why the pipeline is automatically applied.
         """
-        query_dataset = 'dataset=xdr_data | filter '
-        return query_dataset + query
+        query_dataset = 'xdr_data'
+        full_query = f'dataset={query_dataset} | filter {query}'
+        full_query += f' | fields {",".join(rule.fields)}' if rule.fields else ''
+
+        return full_query
 
     def finalize_output_default(self, queries: List[str]) -> Any:
         return queries
     
     def finalize_query_json(self, rule: SigmaRule, query: str, index: int, state: ConversionState) -> Any:
-        query_dataset = 'dataset=xdr_data | filter '
-        return {"query":query_dataset + query, "title":rule.title, "id":rule.id, "description": rule.description}
+        query_dataset = 'xdr_data'
+        full_query = f'dataset={query_dataset} | filter {query}'
+        full_query += f' | fields {",".join(rule.fields)}' if rule.fields else ''
+
+        return {"query":full_query, "title":rule.title, "id":rule.id, "description": rule.description}
 
     def finalize_output_json(self, queries: List[str]) -> Any:
         return {"queries":queries}
```

### Comparing `pysigma_backend_cortexxdr-0.1.0/sigma/pipelines/cortexxdr/cortexxdr.py` & `pysigma_backend_cortexxdr-0.1.1/sigma/pipelines/cortexxdr/cortexxdr.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_cortexxdr-0.1.0/PKG-INFO` & `pysigma_backend_cortexxdr-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysigma-backend-cortexxdr
-Version: 0.1.0
+Version: 0.1.1
 Summary: pySigma CortexXDR backend
 Home-page: https://github.com/7RedViolin/pySigma-backend-cortexxdr
 License: MIT
 Author: Cori Smith
 Author-email: cs2718281@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

