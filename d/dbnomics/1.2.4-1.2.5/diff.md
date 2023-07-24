# Comparing `tmp/dbnomics-1.2.4.tar.gz` & `tmp/dbnomics-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbnomics-1.2.4.tar", last modified: Wed May 24 15:27:22 2023, max compression
+gzip compressed data, was "dbnomics-1.2.5.tar", last modified: Mon Jul 24 13:21:16 2023, max compression
```

## Comparing `dbnomics-1.2.4.tar` & `dbnomics-1.2.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:27:22.196650 dbnomics-1.2.4/
--rw-rw-rw-   0 root         (0) root         (0)    34461 2023-05-24 14:07:48.000000 dbnomics-1.2.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)    42252 2023-05-24 15:27:22.196650 dbnomics-1.2.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1880 2023-05-24 14:07:48.000000 dbnomics-1.2.4/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2084 2023-05-24 14:07:48.000000 dbnomics-1.2.4/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       88 2023-05-24 15:27:22.196650 dbnomics-1.2.4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:27:22.192650 dbnomics-1.2.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:27:22.192650 dbnomics-1.2.4/src/dbnomics/
--rw-rw-rw-   0 root         (0) root         (0)    22733 2023-05-24 14:07:48.000000 dbnomics-1.2.4/src/dbnomics/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:27:22.196650 dbnomics-1.2.4/src/dbnomics.egg-info/
--rw-r--r--   0 root         (0) root         (0)    42252 2023-05-24 15:27:22.000000 dbnomics-1.2.4/src/dbnomics.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      267 2023-05-24 15:27:22.000000 dbnomics-1.2.4/src/dbnomics.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 15:27:22.000000 dbnomics-1.2.4/src/dbnomics.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       80 2023-05-24 15:27:22.000000 dbnomics-1.2.4/src/dbnomics.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-24 15:27:22.000000 dbnomics-1.2.4/src/dbnomics.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:27:22.196650 dbnomics-1.2.4/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2271 2023-05-24 14:07:48.000000 dbnomics-1.2.4/tests/test_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 13:21:16.206102 dbnomics-1.2.5/
+-rw-rw-rw-   0 root         (0) root         (0)    34461 2023-07-24 13:05:37.000000 dbnomics-1.2.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    42252 2023-07-24 13:21:16.206102 dbnomics-1.2.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1880 2023-07-24 13:05:37.000000 dbnomics-1.2.5/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2149 2023-07-24 13:05:37.000000 dbnomics-1.2.5/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-07-24 13:21:16.206102 dbnomics-1.2.5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 13:21:16.202102 dbnomics-1.2.5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 13:21:16.202102 dbnomics-1.2.5/src/dbnomics/
+-rw-rw-rw-   0 root         (0) root         (0)    22724 2023-07-24 13:05:37.000000 dbnomics-1.2.5/src/dbnomics/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 13:21:16.206102 dbnomics-1.2.5/src/dbnomics.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    42252 2023-07-24 13:21:16.000000 dbnomics-1.2.5/src/dbnomics.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      267 2023-07-24 13:21:16.000000 dbnomics-1.2.5/src/dbnomics.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 13:21:16.000000 dbnomics-1.2.5/src/dbnomics.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       98 2023-07-24 13:21:16.000000 dbnomics-1.2.5/src/dbnomics.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-24 13:21:16.000000 dbnomics-1.2.5/src/dbnomics.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 13:21:16.206102 dbnomics-1.2.5/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     5205 2023-07-24 13:05:37.000000 dbnomics-1.2.5/tests/test_client.py
```

### Comparing `dbnomics-1.2.4/LICENSE` & `dbnomics-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dbnomics-1.2.4/PKG-INFO` & `dbnomics-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnomics
-Version: 1.2.4
+Version: 1.2.5
 Summary: DBnomics Python client
 Author-email: Christophe Benz <christophe.benz@nomics.world>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `dbnomics-1.2.4/README.md` & `dbnomics-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `dbnomics-1.2.4/pyproject.toml` & `dbnomics-1.2.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 [project]
 name = "dbnomics"
-version = "1.2.4"
+version = "1.2.5"
 description = "DBnomics Python client"
 authors = [{ name = "Christophe Benz", email = "christophe.benz@nomics.world" }]
 license = { file = "LICENSE" }
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
   "Operating System :: OS Independent",
 ]
 dependencies = ["httpx", "pandas", "tenacity"]
 
 [project.optional-dependencies]
-dev = ["black", "mypy", "pip-tools", "pre-commit", "pytest", "ruff", "vermin"]
+dev = [
+  "black",
+  "mypy",
+  "pip-tools",
+  "pre-commit",
+  "pytest",
+  "pytest-httpserver",
+  "ruff",
+  "vermin",
+]
 
 [project.urls]
 "Homepage" = "https://git.nomics.world/dbnomics/dbnomics-python-client"
 "Bug Tracker" = "https://git.nomics.world/dbnomics/dbnomics-python-client/-/issues"
 
 [tool.black]
 line-length = 120
@@ -95,12 +104,13 @@
 #   "classmethod",
 #   "pydantic.root_validator",
 #   "pydantic.validator",
 # ]
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F403"]
+"tests/**" = ["PLR2004"]
 
 [tool.ruff.pylint]
 max-args = 10
 max-branches = 20
 max-statements = 60
```

### Comparing `dbnomics-1.2.4/src/dbnomics/__init__.py` & `dbnomics-1.2.5/src/dbnomics/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -316,20 +316,19 @@
         for dimension_code in datasets_dimensions[complete_dataset_code]["dimensions_codes_order"]:
             dimensions_codes_columns_names.append(dimension_code)
             # We only add dimensions labels column if this information is present
             if "dimensions_labels" in dataset_dimensions and "dimensions_values_labels" in dataset_dimensions:
                 dimensions_labels_columns_names.append(
                     datasets_dimensions[complete_dataset_code]["dimensions_labels"][dimension_code]
                 )
-            else:
-                if "dimensions_values_labels" in dataset_dimensions:  # noqa: PLR5501
-                    # No dimensions labels but dimensions_values_labels -> we add " (label)" to the end
-                    # of dimension code
-                    dimensions_labels_columns_names.append(f"{dimension_code} (label)")
-                # In the case there's no dimension_label nor dimensions_values_labels, we do not add any column
+            elif "dimensions_values_labels" in dataset_dimensions:
+                # No dimensions labels but dimensions_values_labels -> we add " (label)" to the end
+                # of dimension code
+                dimensions_labels_columns_names.append(f"{dimension_code} (label)")
+            # In the case there's no dimension_label nor dimensions_values_labels, we do not add any column
 
     # In the DataFrame we want to display the dimension columns at the right so we reorder them.
     ordered_columns_names = common_columns + dimensions_codes_columns_names + dimensions_labels_columns_names
 
     # Build dataframe
     dataframes = (pd.DataFrame(data=series, columns=ordered_columns_names) for series in flat_series_list)
     return pd.concat(objs=dataframes, sort=False)
@@ -374,19 +373,21 @@
                 "frequency": series["@frequency"],
                 "period_start_day": series["period_start_day"],
                 "value": series["value"],
             }
             for series in series_group
         ]
         response = httpx.post(
-            apply_endpoint_url, json={"filters": filters, "series": posted_series_list}, timeout=timeout
+            apply_endpoint_url,
+            json={"filters": filters, "series": posted_series_list},
+            timeout=timeout,
         )
         try:
             response_json = response.json()
-        except ValueError:
+        except ValueError:  # noqa: PERF203
             log.error("Invalid response from Time Series Editor (JSON expected)")  # noqa: TRY400
             continue
         if not response.is_success:
             log.error("Error with series filters: %s", json.dumps(response_json, indent=2))
             continue
 
         filter_results = response_json.get("filter_results")
@@ -493,21 +494,19 @@
     series = {
         **without_keys(series, keys={"dimensions", "indexed_at"}),
         **dimensions,
     }
 
     # Flatten observations attributes.
     observations_attributes = series.get("observations_attributes") or []
-    series = {
+    return {
         **without_keys(series, keys={"observations_attributes"}),
         **dict(observations_attributes),
     }
 
-    return series
-
 
 def flatten_editor_series(series, dbnomics_series):
     """Adapt Time Series Editor series attributes to ease DataFrame construction."""
     series = normalize_period(series)
     series = normalize_value(series)
 
     series = {
@@ -566,15 +565,15 @@
     stop=stop_after_attempt(3),
     wait=wait_random_exponential(max=60),
 )
 def _fetch_response(url, timeout=None):
     if timeout is None:
         timeout = default_timeout
 
-    response = httpx.get(url, timeout=timeout)
+    response = httpx.get(url, follow_redirects=True, timeout=timeout)
 
     if response.status_code in {429, 500, 502, 503, 504}:
         raise TryAgain
 
     response.raise_for_status()
 
     return response
```

### Comparing `dbnomics-1.2.4/src/dbnomics.egg-info/PKG-INFO` & `dbnomics-1.2.5/src/dbnomics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnomics
-Version: 1.2.4
+Version: 1.2.5
 Summary: DBnomics Python client
 Author-email: Christophe Benz <christophe.benz@nomics.world>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

