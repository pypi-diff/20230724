# Comparing `tmp/geci_janitor-0.2.0.tar.gz` & `tmp/geci_janitor-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geci_janitor-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "geci_janitor-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `geci_janitor-0.2.0.tar` & `geci_janitor-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1037 2023-07-24 17:12:42.650118 geci_janitor-0.2.0/README.md
--rw-r--r--   0        0        0       81 2023-07-24 17:12:42.650118 geci_janitor-0.2.0/geci_janitor/__init__.py
--rw-r--r--   0        0        0      759 2023-07-24 17:12:42.650118 geci_janitor-0.2.0/geci_janitor/cli.py
--rw-r--r--   0        0        0      451 2023-07-24 17:12:42.650118 geci_janitor-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1448 1970-01-01 00:00:00.000000 geci_janitor-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1037 2023-07-24 18:01:38.021177 geci_janitor-0.3.0/README.md
+-rw-r--r--   0        0        0       81 2023-07-24 18:01:38.021177 geci_janitor-0.3.0/geci_janitor/__init__.py
+-rw-r--r--   0        0        0     1367 2023-07-24 18:01:38.021177 geci_janitor-0.3.0/geci_janitor/cli.py
+-rw-r--r--   0        0        0      451 2023-07-24 18:01:38.021177 geci_janitor-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1448 1970-01-01 00:00:00.000000 geci_janitor-0.3.0/PKG-INFO
```

### Comparing `geci_janitor-0.2.0/README.md` & `geci_janitor-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `geci_janitor-0.2.0/geci_janitor/cli.py` & `geci_janitor-0.3.0/geci_janitor/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,11 +16,19 @@
 
 @janitor.command(help="Clean and check IG_POSICION_TRAMPAS and IG_MORFOMETRIA")
 def transform_cat_data():
     command = "docker run --rm --volume $PWD:/data islasgeci/diferencias_morfometria_posicion_trampas:latest ./src/verify_data.sh /data"
     os.system(command)
 
 
+@janitor.command(help="Generate tidy and weekly effort tables for socorro monthly cat data")
+def clean_socorro_week_data(week: int, data_file: str):
+    command = f"docker run -v $PWD/results:/workdir/results -v $PWD:/workdir/data islasgeci/datatools python src/get_weekly_summary_socorro_from_excell.py {week} data/{data_file}"
+    os.system(command)
+    command = f"docker run -v $PWD/results:/workdir/results -v $PWD:/workdir/data islasgeci/diferencias_morfometria_posicion_trampas src/make_table_tidy.R --data results/socorro_cleaned_format.csv --salida results/tidy_{week}.csv"
+    os.system(command)
+
+
 @janitor.command()
 def version():
     version = jn.__version__
     print(version)
```

### Comparing `geci_janitor-0.2.0/PKG-INFO` & `geci_janitor-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geci_janitor
-Version: 0.2.0
+Version: 0.3.0
 Summary: A template Python module
 Home-page: https://github.com/IslasGECI/janitor
 Author: Ciencia de Datos • GECI
 Author-email: ciencia.datos@islas.org.mx
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: geci_janitor Version: 0.2.0 Summary: A template
+Metadata-Version: 2.1 Name: geci_janitor Version: 0.3.0 Summary: A template
 Python module Home-page: https://github.com/IslasGECI/janitor Author: Ciencia
 de Datos â¢ GECI Author-email: ciencia.datos@islas.org.mx Requires-Python:
 >=3.9 Description-Content-Type: text/markdown Classifier: License :: OSI
 Approved :: GNU General Public License v3 or later (GPLv3+) Requires-Dist:
 typer Requires-Dist: typer-cli [https://www.islas.org.mx/img/logo.svg] # Dummy
 Transformations Para usar este repo como plantilla debemos hacer lo siguiente:
 1. Presiona el botÃ³n verde que dice _Use this template_ 1. Selecciona como
```

