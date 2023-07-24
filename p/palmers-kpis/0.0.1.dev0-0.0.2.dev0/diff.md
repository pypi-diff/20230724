# Comparing `tmp/palmers_kpis-0.0.1.dev0.tar.gz` & `tmp/palmers_kpis-0.0.2.dev0.tar.gz`

## Comparing `palmers_kpis-0.0.1.dev0.tar` & `palmers_kpis-0.0.2.dev0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_kpis-0.0.1.dev0/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_kpis-0.0.1.dev0/kpi/__init__.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 palmers_kpis-0.0.1.dev0/kpi/config.py
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 palmers_kpis-0.0.1.dev0/kpi/main.py
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 palmers_kpis-0.0.1.dev0/kpi/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_kpis-0.0.1.dev0/kpi/miss_sales_kpi/__init__.py
--rw-r--r--   0        0        0    12059 2020-02-02 00:00:00.000000 palmers_kpis-0.0.1.dev0/kpi/miss_sales_kpi/miss_sales_kpi_metric.py
--rw-r--r--   0        0        0    36950 2020-02-02 00:00:00.000000 palmers_kpis-0.0.1.dev0/kpi/notebook/check_simulated_data_for_kpi.ipynb
--rw-r--r--   0        0        0    18235 2020-02-02 00:00:00.000000 palmers_kpis-0.0.1.dev0/kpi/notebook/final_check_kpi.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_kpis-0.0.1.dev0/kpi/stock_kpi/__init__.py
--rw-r--r--   0        0        0     6955 2020-02-02 00:00:00.000000 palmers_kpis-0.0.1.dev0/kpi/stock_kpi/stock_kpi_metric.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_kpis-0.0.1.dev0/kpi/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_kpis-0.0.1.dev0/kpi/tests/kpi/__init__.py
--rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 palmers_kpis-0.0.1.dev0/kpi/tests/kpi/check_kpi_metirc.py
--rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 palmers_kpis-0.0.1.dev0/LICENSE
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 palmers_kpis-0.0.1.dev0/README.md
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 palmers_kpis-0.0.1.dev0/pyproject.toml
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 palmers_kpis-0.0.1.dev0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_kpis-0.0.2.dev0/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_kpis-0.0.2.dev0/kpi/__init__.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 palmers_kpis-0.0.2.dev0/kpi/config.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 palmers_kpis-0.0.2.dev0/kpi/main.py
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 palmers_kpis-0.0.2.dev0/kpi/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_kpis-0.0.2.dev0/kpi/miss_sales_kpi/__init__.py
+-rw-r--r--   0        0        0    12059 2020-02-02 00:00:00.000000 palmers_kpis-0.0.2.dev0/kpi/miss_sales_kpi/miss_sales_kpi_metric.py
+-rw-r--r--   0        0        0    36950 2020-02-02 00:00:00.000000 palmers_kpis-0.0.2.dev0/kpi/notebook/check_simulated_data_for_kpi.ipynb
+-rw-r--r--   0        0        0    18235 2020-02-02 00:00:00.000000 palmers_kpis-0.0.2.dev0/kpi/notebook/final_check_kpi.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_kpis-0.0.2.dev0/kpi/stock_kpi/__init__.py
+-rw-r--r--   0        0        0     6955 2020-02-02 00:00:00.000000 palmers_kpis-0.0.2.dev0/kpi/stock_kpi/stock_kpi_metric.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_kpis-0.0.2.dev0/kpi/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_kpis-0.0.2.dev0/kpi/tests/kpi/__init__.py
+-rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 palmers_kpis-0.0.2.dev0/kpi/tests/kpi/check_kpi_metirc.py
+-rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 palmers_kpis-0.0.2.dev0/LICENSE
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 palmers_kpis-0.0.2.dev0/README.md
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 palmers_kpis-0.0.2.dev0/pyproject.toml
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 palmers_kpis-0.0.2.dev0/PKG-INFO
```

### Comparing `palmers_kpis-0.0.1.dev0/kpi/main.py` & `palmers_kpis-0.0.2.dev0/kpi/main.py`

 * *Files identical despite different names*

### Comparing `palmers_kpis-0.0.1.dev0/kpi/utils.py` & `palmers_kpis-0.0.2.dev0/kpi/utils.py`

 * *Files identical despite different names*

### Comparing `palmers_kpis-0.0.1.dev0/kpi/miss_sales_kpi/miss_sales_kpi_metric.py` & `palmers_kpis-0.0.2.dev0/kpi/miss_sales_kpi/miss_sales_kpi_metric.py`

 * *Files identical despite different names*

### Comparing `palmers_kpis-0.0.1.dev0/kpi/notebook/check_simulated_data_for_kpi.ipynb` & `palmers_kpis-0.0.2.dev0/kpi/notebook/check_simulated_data_for_kpi.ipynb`

 * *Files identical despite different names*

### Comparing `palmers_kpis-0.0.1.dev0/kpi/notebook/final_check_kpi.ipynb` & `palmers_kpis-0.0.2.dev0/kpi/notebook/final_check_kpi.ipynb`

 * *Files identical despite different names*

### Comparing `palmers_kpis-0.0.1.dev0/kpi/stock_kpi/stock_kpi_metric.py` & `palmers_kpis-0.0.2.dev0/kpi/stock_kpi/stock_kpi_metric.py`

 * *Files identical despite different names*

### Comparing `palmers_kpis-0.0.1.dev0/kpi/tests/kpi/check_kpi_metirc.py` & `palmers_kpis-0.0.2.dev0/kpi/tests/kpi/check_kpi_metirc.py`

 * *Files identical despite different names*

### Comparing `palmers_kpis-0.0.1.dev0/LICENSE` & `palmers_kpis-0.0.2.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `palmers_kpis-0.0.1.dev0/pyproject.toml` & `palmers_kpis-0.0.2.dev0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "palmers_kpis"
-version = "0.0.1.dev"
+version = "0.0.2.dev"
 authors = [
   { name="Assaf", email="assafm@sdatta.ai" },
   { name="Roy ", email="roy@sdatta.ai" },
   { name="Guy", email="assafm@sdatta.ai" },
   { name="Oran", email="assafm@sdatta.ai" },
   { name="Yotam", email="assafm@sdatta.ai" },
 ]
```

### Comparing `palmers_kpis-0.0.1.dev0/PKG-INFO` & `palmers_kpis-0.0.2.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: palmers_kpis
-Version: 0.0.1.dev0
+Version: 0.0.2.dev0
 Summary: A package for KPI analysis for Palmer's project
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Assaf <assafm@sdatta.ai>, Roy  <roy@sdatta.ai>, Guy <assafm@sdatta.ai>, Oran <assafm@sdatta.ai>, Yotam <assafm@sdatta.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

