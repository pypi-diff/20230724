# Comparing `tmp/kohlrahbi-0.0.6.tar.gz` & `tmp/kohlrahbi-0.0.6a1.tar.gz`

## Comparing `kohlrahbi-0.0.6.tar` & `kohlrahbi-0.0.6a1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0     6576 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6/README.md
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6/requirements.in
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6/requirements.txt
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6/tox.ini
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6/.github/dependabot.yml
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6/.github/workflows/black.yml
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6/.github/workflows/packaging_test.yml
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6/.github/workflows/pythonlint.yml
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6/.github/workflows/unittests.yml
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6/src/_kohlrahbi_version.py
--rw-r--r--   0        0        0     8445 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6/src/kohlrahbi/__init__.py
--rw-r--r--   0        0        0     4325 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6/src/kohlrahbi/ahbfilefinder.py
--rw-r--r--   0        0        0     8770 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6/src/kohlrahbi/all_known_pruefis.toml
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6/src/kohlrahbi/collect_pruefis.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6/src/kohlrahbi/logger.ini
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6/src/kohlrahbi/logger.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6/src/kohlrahbi/py.typed
--rw-r--r--   0        0        0     6650 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6/src/kohlrahbi/read_functions.py
--rw-r--r--   0        0        0     5203 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6/src/kohlrahbi/row_type_checker.py
--rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6/src/kohlrahbi/seed.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6/src/kohlrahbi/ahb/__init__.py
--rw-r--r--   0        0        0     5028 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6/src/kohlrahbi/ahb/ahbsubtable.py
--rw-r--r--   0        0        0     7918 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6/src/kohlrahbi/ahb/ahbtable.py
--rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6/src/kohlrahbi/ahb/ahbtablerow.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6/src/kohlrahbi/docxtablecells/__init__.py
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6/src/kohlrahbi/docxtablecells/bedinungscell.py
--rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6/src/kohlrahbi/docxtablecells/bodycell.py
--rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6/src/kohlrahbi/docxtablecells/edifactstrukturcell.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6/src/kohlrahbi/enums/__init__.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6/src/kohlrahbi/enums/flat_ahb_row_type.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6/src/kohlrahbi/enums/row_type.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6/src/kohlrahbi/enums/row_type_color.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6/src/kohlrahbi/unfoldedahb/__init__.py
--rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6/src/kohlrahbi/unfoldedahb/unfoldedahbline.py
--rw-r--r--   0        0        0    18732 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6/src/kohlrahbi/unfoldedahb/unfoldedahbtable.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6/src/kohlrahbi/unfoldedahb/unfoldedahbtablemetadata.py
--rw-r--r--   0        0        0   861363 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6/temp/test-fobar.docx
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6/LICENSE
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     7738 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6a1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     6576 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6a1/README.md
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6a1/requirements.in
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6a1/requirements.txt
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6a1/tox.ini
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6a1/.github/dependabot.yml
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6a1/.github/workflows/black.yml
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6a1/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6a1/.github/workflows/packaging_test.yml
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6a1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6a1/.github/workflows/pythonlint.yml
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6a1/.github/workflows/unittests.yml
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6a1/src/_kohlrahbi_version.py
+-rw-r--r--   0        0        0     8370 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6a1/src/kohlrahbi/__init__.py
+-rw-r--r--   0        0        0     4325 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6a1/src/kohlrahbi/ahbfilefinder.py
+-rw-r--r--   0        0        0     4299 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6a1/src/kohlrahbi/all_known_pruefis.toml
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6a1/src/kohlrahbi/collect_pruefis.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6a1/src/kohlrahbi/logger.ini
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6a1/src/kohlrahbi/logger.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6a1/src/kohlrahbi/py.typed
+-rw-r--r--   0        0        0     6650 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6a1/src/kohlrahbi/read_functions.py
+-rw-r--r--   0        0        0     5203 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6a1/src/kohlrahbi/row_type_checker.py
+-rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6a1/src/kohlrahbi/seed.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6a1/src/kohlrahbi/ahb/__init__.py
+-rw-r--r--   0        0        0     5028 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6a1/src/kohlrahbi/ahb/ahbsubtable.py
+-rw-r--r--   0        0        0     7918 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6a1/src/kohlrahbi/ahb/ahbtable.py
+-rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6a1/src/kohlrahbi/ahb/ahbtablerow.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6a1/src/kohlrahbi/docxtablecells/__init__.py
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6a1/src/kohlrahbi/docxtablecells/bedinungscell.py
+-rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6a1/src/kohlrahbi/docxtablecells/bodycell.py
+-rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6a1/src/kohlrahbi/docxtablecells/edifactstrukturcell.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6a1/src/kohlrahbi/enums/__init__.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6a1/src/kohlrahbi/enums/flat_ahb_row_type.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6a1/src/kohlrahbi/enums/row_type.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6a1/src/kohlrahbi/enums/row_type_color.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6a1/src/kohlrahbi/unfoldedahb/__init__.py
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6a1/src/kohlrahbi/unfoldedahb/unfoldedahbline.py
+-rw-r--r--   0        0        0    18202 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6a1/src/kohlrahbi/unfoldedahb/unfoldedahbtable.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6a1/src/kohlrahbi/unfoldedahb/unfoldedahbtablemetadata.py
+-rw-r--r--   0        0        0   861363 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6a1/temp/test-fobar.docx
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6a1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6a1/LICENSE
+-rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6a1/pyproject.toml
+-rw-r--r--   0        0        0     7740 2020-02-02 00:00:00.000000 kohlrahbi-0.0.6a1/PKG-INFO
```

### Comparing `kohlrahbi-0.0.6/.pre-commit-config.yaml` & `kohlrahbi-0.0.6a1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.6/README.md` & `kohlrahbi-0.0.6a1/README.md`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.6/requirements.txt` & `kohlrahbi-0.0.6a1/requirements.txt`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.6/tox.ini` & `kohlrahbi-0.0.6a1/tox.ini`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.6/.github/dependabot.yml` & `kohlrahbi-0.0.6a1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.6/.github/workflows/black.yml` & `kohlrahbi-0.0.6a1/.github/workflows/black.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.6/.github/workflows/coverage.yml` & `kohlrahbi-0.0.6a1/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.6/.github/workflows/packaging_test.yml` & `kohlrahbi-0.0.6a1/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.6/.github/workflows/python-publish.yml` & `kohlrahbi-0.0.6a1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.6/.github/workflows/pythonlint.yml` & `kohlrahbi-0.0.6a1/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.6/.github/workflows/unittests.yml` & `kohlrahbi-0.0.6a1/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.6/src/kohlrahbi/__init__.py` & `kohlrahbi-0.0.6a1/src/kohlrahbi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,14 @@
 
 
 def load_all_known_pruefis_from_file(
     path_to_all_known_pruefis: Path = Path(__file__).parent / Path("all_known_pruefis.toml"),
 ) -> list[str]:
     """
     Loads the file which contains all known Prüfidentifikatoren.
-    The file may be manually updated with the script `collect_pruefis.py`.
     """
 
     with open(path_to_all_known_pruefis, "rb") as file:
         state_of_kohlrahbi: dict[str, Any] = tomlkit.load(file)
 
     meta_data_section = state_of_kohlrahbi.get("meta_data")
     content_section = state_of_kohlrahbi.get("content")
```

### Comparing `kohlrahbi-0.0.6/src/kohlrahbi/ahbfilefinder.py` & `kohlrahbi-0.0.6a1/src/kohlrahbi/ahbfilefinder.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.6/src/kohlrahbi/collect_pruefis.py` & `kohlrahbi-0.0.6a1/src/kohlrahbi/collect_pruefis.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """
 This module collects all Prüfidentifikatoren from the AHB documents.
 You have to define a path where all AHB docx files are.
-Use this script to create an updated version of the all_known_pruefis.toml file.
 """
 from datetime import date
 from pathlib import Path
 
 import docx  # type:ignore[import]
 import tomlkit
 from docx.table import Table  # type:ignore[import]
@@ -17,36 +16,30 @@
 from kohlrahbi.seed import Seed
 
 all_pruefis: list[str] = []
 
 # You have to clone the edi_energy_mirror repository and define the path to the current folder.
 # https://github.com/Hochfrequenz/edi_energy_mirror
 # Just put it next to the kohlrahbi repository.
-edi_energy_mirror_repo_root_path = Path(__file__).parent.parent.parent.parent / "edi_energy_mirror"
-pathes_to_ahb_documents: list[Path] = [
-    edi_energy_mirror_repo_root_path / Path("edi_energy_de/current"),
-    edi_energy_mirror_repo_root_path / Path("edi_energy_de/future"),
-]
-assert all(path.exists() for path in pathes_to_ahb_documents)
-
-
-for path_to_ahb_documents in pathes_to_ahb_documents:
-    for edifact_format in EdifactFormat:
-        ahb_file_finder = AhbFileFinder.from_input_path(input_path=path_to_ahb_documents)
-
-        ahb_file_finder.filter_for_latest_ahb_docx_files()
-
-        for ahb_file_path in ahb_file_finder.paths_to_docx_files:
-            doc = docx.Document(ahb_file_path)
-            for item in get_all_paragraphs_and_tables(parent=doc):
-                if isinstance(item, Table) and does_the_table_contain_pruefidentifikatoren(table=item):
-                    # check which pruefis
-                    seed = Seed.from_table(docx_table=item)
-                    logger.info("Found a table with the following pruefis: %s", seed.pruefidentifikatoren)
-                    all_pruefis = all_pruefis + seed.pruefidentifikatoren
+path_to_ahb_documents: Path = Path.cwd().parent / Path("edi_energy_mirror/edi_energy_de/current")
+
+for edifact_format in EdifactFormat:
+    ahb_file_finder = AhbFileFinder.from_input_path(input_path=path_to_ahb_documents)
+
+    ahb_file_finder.filter_for_latest_ahb_docx_files()
+
+    for ahb_file_path in ahb_file_finder.paths_to_docx_files:
+        doc = docx.Document(ahb_file_path)  # Creating word reader object.
+
+        for item in get_all_paragraphs_and_tables(parent=doc):
+            if isinstance(item, Table) and does_the_table_contain_pruefidentifikatoren(table=item):
+                # check which pruefis
+                seed = Seed.from_table(docx_table=item)
+                logger.info("Found a table with the following pruefis: %s", seed.pruefidentifikatoren)
+                all_pruefis = all_pruefis + seed.pruefidentifikatoren
 
 all_pruefis = sorted(list(set(all_pruefis)))
 
 toml_data = {
     "meta_data": {"updated_on": date.today()},
     "content": {"pruefidentifikatoren": all_pruefis},
 }
```

### Comparing `kohlrahbi-0.0.6/src/kohlrahbi/read_functions.py` & `kohlrahbi-0.0.6a1/src/kohlrahbi/read_functions.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.6/src/kohlrahbi/row_type_checker.py` & `kohlrahbi-0.0.6a1/src/kohlrahbi/row_type_checker.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.6/src/kohlrahbi/seed.py` & `kohlrahbi-0.0.6a1/src/kohlrahbi/seed.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.6/src/kohlrahbi/ahb/ahbsubtable.py` & `kohlrahbi-0.0.6a1/src/kohlrahbi/ahb/ahbsubtable.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.6/src/kohlrahbi/ahb/ahbtable.py` & `kohlrahbi-0.0.6a1/src/kohlrahbi/ahb/ahbtable.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.6/src/kohlrahbi/ahb/ahbtablerow.py` & `kohlrahbi-0.0.6a1/src/kohlrahbi/ahb/ahbtablerow.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.6/src/kohlrahbi/docxtablecells/bedinungscell.py` & `kohlrahbi-0.0.6a1/src/kohlrahbi/docxtablecells/bedinungscell.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.6/src/kohlrahbi/docxtablecells/bodycell.py` & `kohlrahbi-0.0.6a1/src/kohlrahbi/docxtablecells/bodycell.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.6/src/kohlrahbi/docxtablecells/edifactstrukturcell.py` & `kohlrahbi-0.0.6a1/src/kohlrahbi/docxtablecells/edifactstrukturcell.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.6/src/kohlrahbi/enums/row_type.py` & `kohlrahbi-0.0.6a1/src/kohlrahbi/enums/row_type.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.6/src/kohlrahbi/unfoldedahb/unfoldedahbline.py` & `kohlrahbi-0.0.6a1/src/kohlrahbi/unfoldedahb/unfoldedahbline.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.6/src/kohlrahbi/unfoldedahb/unfoldedahbtable.py` & `kohlrahbi-0.0.6a1/src/kohlrahbi/unfoldedahb/unfoldedahbtable.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,68 +1,37 @@
 """
 This module contains the UnfoldedAhbTable class.
 """
-import copy
+
 import json
 import re
 from pathlib import Path
 from uuid import uuid4
 
 import attrs
 import pandas as pd
 from maus.edifact import get_format_of_pruefidentifikator
 from maus.models.anwendungshandbuch import (
     AhbLine,
+    AhbLineSchema,
     AhbMetaInformation,
     FlatAnwendungshandbuch,
     FlatAnwendungshandbuchSchema,
 )
 from maus.reader.flat_ahb_reader import FlatAhbCsvReader
-from more_itertools import first_true, peekable
+from more_itertools import peekable
 
 from kohlrahbi.ahb.ahbtable import AhbTable, _column_letter_width_mapping
 from kohlrahbi.logger import logger
 from kohlrahbi.unfoldedahb.unfoldedahbline import UnfoldedAhbLine
 from kohlrahbi.unfoldedahb.unfoldedahbtablemetadata import UnfoldedAhbTableMetaData
 
 _segment_group_pattern = re.compile(r"^SG\d+$")
 
 
-def _lines_are_equal_when_ignoring_guid(line1: AhbLine, line2: AhbLine) -> bool:
-    """
-    returns true iff the line1 and line2 are equal except for their guid
-    """
-    line1_copy = copy.deepcopy(line1)
-    line2_copy = copy.deepcopy(line2)
-    line1_copy.guid = None
-    line2_copy.guid = None
-    return line1_copy == line2_copy
-
-
-def _keep_guids_of_unchanged_lines_stable(
-    updated_ahb: FlatAnwendungshandbuch, existing_ahb: FlatAnwendungshandbuch
-) -> None:
-    """
-    Modifies the instance of updated_ahb such that the guids of all lines that are unchanged are the same as in the
-    existing_ahb. Only applies if metadata of both AHBs match.
-    """
-    if updated_ahb.meta == existing_ahb.meta:
-        existing_ahb_search_start_index = 0
-        for update_index, updated_line in enumerate(updated_ahb.lines.copy()):
-            if existing_line_match := first_true(  # ⚠ performance wise this goes like O(n^2)
-                existing_ahb.lines[existing_ahb_search_start_index:],
-                pred=lambda x: _lines_are_equal_when_ignoring_guid(
-                    x, updated_line  # pylint:disable=cell-var-from-loop
-                ),
-            ):
-                updated_ahb.lines[update_index].guid = existing_line_match.guid
-                # if we found a line match, we can start the next search at the next line in the next loop iteration
-                existing_ahb_search_start_index = existing_ahb.lines.index(existing_line_match) + 1
-
-
 @attrs.define(auto_attribs=True, kw_only=True)
 class UnfoldedAhb:
     """
     The UnfoldedAhb contains one Prüfidentifikator.
     Some columns in the AHB documents contain multiple information in one column e.g. Segmentname and Segmentgruppe.
     The unfolded classes add new columns/attribues to avoid the duplication of information in one column.
     """
@@ -347,15 +316,31 @@
         flatahb_output_directory_path.mkdir(parents=True, exist_ok=True)
         flat_ahb = self.convert_to_flat_ahb()
 
         file_path = flatahb_output_directory_path / f"{self.meta_data.pruefidentifikator}.json"
         if file_path.exists():
             with open(file_path, "r", encoding="utf-8") as file:
                 existing_flat_ahb = FlatAnwendungshandbuchSchema().load(json.load(file))
-            _keep_guids_of_unchanged_lines_stable(flat_ahb, existing_flat_ahb)
+        dump_equals_existing_file_except_for_guids = flat_ahb.meta == existing_flat_ahb.meta and len(
+            flat_ahb.lines
+        ) == len(existing_flat_ahb.lines)
+        if dump_equals_existing_file_except_for_guids:
+            ahb_line_schema = AhbLineSchema()
+            for line, existing_line in zip(flat_ahb.lines, existing_flat_ahb.lines):
+                line_copy = ahb_line_schema.load(ahb_line_schema.dump(line))
+                existing_line_copy = ahb_line_schema.load(ahb_line_schema.dump(existing_line))
+                line_copy.guid = None
+                existing_line_copy.guid = None
+                if line_copy == existing_line_copy:
+                    # keep the same guid if lines didn't change
+                    line.guid = existing_line.guid
+                else:
+                    dump_equals_existing_file_except_for_guids = False
+        if dump_equals_existing_file_except_for_guids:
+            logger.info("The AHB for Prüfi %s didn't change", self.meta_data.pruefidentifikator)
         dump_data = FlatAnwendungshandbuchSchema().dump(flat_ahb)
         with open(file_path, "w", encoding="utf-8") as file:
             json.dump(dump_data, file, ensure_ascii=False, indent=2, sort_keys=True)
         logger.info(
             "The flatahb file for %s is saved at %s",
             self.meta_data.pruefidentifikator,
             flatahb_output_directory_path / f"{self.meta_data.pruefidentifikator}.json",
```

### Comparing `kohlrahbi-0.0.6/temp/test-fobar.docx` & `kohlrahbi-0.0.6a1/temp/test-fobar.docx`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.6/.gitignore` & `kohlrahbi-0.0.6a1/.gitignore`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.6/LICENSE` & `kohlrahbi-0.0.6a1/LICENSE`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.6/pyproject.toml` & `kohlrahbi-0.0.6a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.6/PKG-INFO` & `kohlrahbi-0.0.6a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kohlrahbi
-Version: 0.0.6
+Version: 0.0.6a1
 Summary: Tool to generate machine readable files from AHB documents
 Project-URL: Changelog, https://github.com/Hochfrequenz/kohlrahbi/releases
 Project-URL: Homepage, https://github.com/Hochfrequenz/kohlrahbi
 Author-email: Kevin Krechan <kevin.krechan@hochfrequenz.de>
 License: GPL
 License-File: LICENSE
 Keywords: ahb,automation,bdew,edi@energy
```

