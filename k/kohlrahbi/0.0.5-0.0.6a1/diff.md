# Comparing `tmp/kohlrahbi-0.0.5.tar.gz` & `tmp/kohlrahbi-0.0.6a1.tar.gz`

## Comparing `kohlrahbi-0.0.5.tar` & `kohlrahbi-0.0.6a1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0     6576 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/README.md
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/requirements.in
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/requirements.txt
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/tox.ini
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/.github/dependabot.yml
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/.github/workflows/black.yml
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/.github/workflows/packaging_test.yml
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/.github/workflows/pythonlint.yml
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/.github/workflows/unittests.yml
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/_kohlrahbi_version.py
--rw-r--r--   0        0        0     8370 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/__init__.py
--rw-r--r--   0        0        0     4325 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/ahbfilefinder.py
--rw-r--r--   0        0        0     4299 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/all_known_pruefis.toml
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/collect_pruefis.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/logger.ini
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/logger.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/py.typed
--rw-r--r--   0        0        0     6188 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/read_functions.py
--rw-r--r--   0        0        0     5203 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/row_type_checker.py
--rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/seed.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/ahb/__init__.py
--rw-r--r--   0        0        0     5028 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/ahb/ahbsubtable.py
--rw-r--r--   0        0        0     7849 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/ahb/ahbtable.py
--rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/ahb/ahbtablerow.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/docxtablecells/__init__.py
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/docxtablecells/bedinungscell.py
--rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/docxtablecells/bodycell.py
--rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/docxtablecells/edifactstrukturcell.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/enums/__init__.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/enums/flat_ahb_row_type.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/enums/row_type.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/enums/row_type_color.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/unfoldedahb/__init__.py
--rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/unfoldedahb/unfoldedahbline.py
--rw-r--r--   0        0        0    15722 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/unfoldedahb/unfoldedahbtable.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/unfoldedahb/unfoldedahbtablemetadata.py
--rw-r--r--   0        0        0   861363 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/temp/test-fobar.docx
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/LICENSE
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     7738 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/PKG-INFO
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

### Comparing `kohlrahbi-0.0.5/.pre-commit-config.yaml` & `kohlrahbi-0.0.6a1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.5/README.md` & `kohlrahbi-0.0.6a1/README.md`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.5/requirements.txt` & `kohlrahbi-0.0.6a1/requirements.txt`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 #    pip-compile requirements.in
 #
 attrs==23.1.0
     # via
     #   -r requirements.in
     #   maus
-click==8.1.5
+click==8.1.6
     # via
     #   -r requirements.in
     #   maus
 colorlog==6.7.0
     # via -r requirements.in
 et-xmlfile==1.1.0
     # via openpyxl
```

### Comparing `kohlrahbi-0.0.5/tox.ini` & `kohlrahbi-0.0.6a1/tox.ini`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.5/.github/dependabot.yml` & `kohlrahbi-0.0.6a1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.5/.github/workflows/black.yml` & `kohlrahbi-0.0.6a1/.github/workflows/black.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.5/.github/workflows/coverage.yml` & `kohlrahbi-0.0.6a1/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.5/.github/workflows/packaging_test.yml` & `kohlrahbi-0.0.6a1/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.5/.github/workflows/python-publish.yml` & `kohlrahbi-0.0.6a1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.5/.github/workflows/pythonlint.yml` & `kohlrahbi-0.0.6a1/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.5/.github/workflows/unittests.yml` & `kohlrahbi-0.0.6a1/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.5/src/kohlrahbi/__init__.py` & `kohlrahbi-0.0.6a1/src/kohlrahbi/__init__.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.5/src/kohlrahbi/ahbfilefinder.py` & `kohlrahbi-0.0.6a1/src/kohlrahbi/ahbfilefinder.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.5/src/kohlrahbi/all_known_pruefis.toml` & `kohlrahbi-0.0.6a1/src/kohlrahbi/all_known_pruefis.toml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.5/src/kohlrahbi/collect_pruefis.py` & `kohlrahbi-0.0.6a1/src/kohlrahbi/collect_pruefis.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.5/src/kohlrahbi/read_functions.py` & `kohlrahbi-0.0.6a1/src/kohlrahbi/read_functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -89,42 +89,48 @@
     ahb_table: Optional[AhbTable] = None
     is_ahb_table_initialized: bool = False
     searched_pruefi_is_found: bool = False
 
     # Iterate through the whole word document
     logger.info("Start iterating through paragraphs and tables")
     for item in get_all_paragraphs_and_tables(parent=document):
+        style_name = item.style.name  # this is a bit expensive. we should only call it once per item
         # Check if we reached the end of the current AHB document and stop if it's true.
-        if isinstance(item, Paragraph) and "Heading" in item.style.name and "Änderungshistorie" in item.text:
+        if isinstance(item, Paragraph) and "Änderungshistorie" in item.text and "Heading" in style_name:
+            # checking the style is quite expensive for the CPU because it includes some xpath searches;
+            # we should only check the style if the other (easier/cheap) checks returned True
+            logger.info(
+                "We reached the end of the document before any table containing the searched Prüfi %s was found", pruefi
+            )
             del seed
             return None
 
         # Check if there is just a text paragraph,
-        if isinstance(item, Paragraph) and not "Heading" in item.style.name:
+        if isinstance(item, Paragraph) and not "Heading" in style_name:
             continue
 
         if isinstance(item, Table) and does_the_table_contain_pruefidentifikatoren(table=item):
             # check which pruefis
             seed = Seed.from_table(docx_table=item)
-            logger.info("Found a table with the following pruefis: %s", seed.pruefidentifikatoren)
+            logger.debug("Found a table with the following pruefis (A): %s", seed.pruefidentifikatoren)
 
         we_reached_the_end_of_the_ahb_table_of_the_searched_pruefi: bool = (
             seed is not None and pruefi not in seed.pruefidentifikatoren and searched_pruefi_is_found
         )
 
         if we_reached_the_end_of_the_ahb_table_of_the_searched_pruefi:
             del seed
             seed = None
             logger.info("🏁 We reached the end of the AHB table of the Prüfidentifikator '%s'", pruefi)
             break
 
         if isinstance(item, Table) and does_the_table_contain_pruefidentifikatoren(table=item):
             # check which pruefis
             seed = Seed.from_table(docx_table=item)
-            logger.info("Found a table with the following pruefis: %s", seed.pruefidentifikatoren)
+            logger.debug("Found a table with the following pruefis (B): %s", seed.pruefidentifikatoren)
 
             searched_pruefi_is_found = pruefi in seed.pruefidentifikatoren and not is_ahb_table_initialized
 
             if searched_pruefi_is_found:
                 logger.info("👀 Found the AHB table with the Prüfidentifkator you are looking for %s", pruefi)
                 logger.info("✨ Initializing new ahb table")
```

### Comparing `kohlrahbi-0.0.5/src/kohlrahbi/row_type_checker.py` & `kohlrahbi-0.0.6a1/src/kohlrahbi/row_type_checker.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.5/src/kohlrahbi/seed.py` & `kohlrahbi-0.0.6a1/src/kohlrahbi/seed.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.5/src/kohlrahbi/ahb/ahbsubtable.py` & `kohlrahbi-0.0.6a1/src/kohlrahbi/ahb/ahbsubtable.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.5/src/kohlrahbi/ahb/ahbtable.py` & `kohlrahbi-0.0.6a1/src/kohlrahbi/ahb/ahbtable.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         """
         In some cases there is the content of one cell splitted in two.
         We need to merge the content into one cell and delete the deprecated cell afterwards.
         """
         index_of_lines_to_drop: list[int] = []
 
         iterable_ahb_table = peekable(self.table.iterrows())
-
+        self.table.reset_index(drop=True, inplace=True)
         for _, row in iterable_ahb_table:
             index_of_next_row, next_row = iterable_ahb_table.peek(
                 (
                     0,
                     pd.Series(
                         {
                             "Segment Gruppe": "",
@@ -141,15 +141,15 @@
 
                 if index_of_next_row == 0:
                     # this case is only for the first and last row. These lines should not get deleted.
                     continue
                 index_of_lines_to_drop.append(index_of_next_row)
 
         self.table.drop(index_of_lines_to_drop, inplace=True)
-        self.table.reset_index(drop=True)
+        self.table.reset_index(drop=True, inplace=True)
 
     def to_csv(self, pruefi: str, path_to_output_directory: Path) -> None:
         """
         Dump an AHB table of a given pruefi into a csv file.
         The csv file will be saved in the following directory structure:
             <path_to_output_directory>/csv/<edifact_format>/<pruefi>.csv
         """
```

### Comparing `kohlrahbi-0.0.5/src/kohlrahbi/ahb/ahbtablerow.py` & `kohlrahbi-0.0.6a1/src/kohlrahbi/ahb/ahbtablerow.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.5/src/kohlrahbi/docxtablecells/bedinungscell.py` & `kohlrahbi-0.0.6a1/src/kohlrahbi/docxtablecells/bedinungscell.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.5/src/kohlrahbi/docxtablecells/bodycell.py` & `kohlrahbi-0.0.6a1/src/kohlrahbi/docxtablecells/bodycell.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.5/src/kohlrahbi/docxtablecells/edifactstrukturcell.py` & `kohlrahbi-0.0.6a1/src/kohlrahbi/docxtablecells/edifactstrukturcell.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.5/src/kohlrahbi/enums/row_type.py` & `kohlrahbi-0.0.6a1/src/kohlrahbi/enums/row_type.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.5/src/kohlrahbi/unfoldedahb/unfoldedahbline.py` & `kohlrahbi-0.0.6a1/src/kohlrahbi/unfoldedahb/unfoldedahbline.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.5/src/kohlrahbi/unfoldedahb/unfoldedahbtable.py` & `kohlrahbi-0.0.6a1/src/kohlrahbi/unfoldedahb/unfoldedahbtable.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,14 +8,15 @@
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
 from more_itertools import peekable
 
@@ -160,14 +161,29 @@
                         qualifier="",
                         beschreibung=description,
                         bedinung_ausdruck=row[pruefi] or None,
                         bedingung=row["Beschreibung"],
                     )
                 )
                 continue
+            if any(unfolded_ahb_lines) and UnfoldedAhb._is_just_value_pool_entry(ahb_row=row):
+                unfolded_ahb_lines.append(
+                    UnfoldedAhbLine(
+                        index=index,
+                        segment_name=current_section_name,
+                        segment_gruppe=unfolded_ahb_lines[-1].segment_gruppe,
+                        segment=unfolded_ahb_lines[-1].segment,
+                        datenelement=unfolded_ahb_lines[-1].datenelement,
+                        code=row["Codes und Qualifier"],
+                        qualifier="",
+                        beschreibung=row["Beschreibung"],
+                        bedinung_ausdruck=row[pruefi] or None,
+                        bedingung=row["Bedingung"],
+                    )
+                )
 
         return cls(
             unfolded_ahb_lines=unfolded_ahb_lines,
             meta_data=UnfoldedAhbTableMetaData(
                 pruefidentifikator=pruefi,
             ),
         )
@@ -239,14 +255,26 @@
         """
         Checks if the given AHB row is a dataelement
         """
         if ahb_row["Datenelement"]:
             return True
         return False
 
+    @staticmethod
+    def _is_just_value_pool_entry(ahb_row: pd.Series) -> bool:
+        """
+        Checks if the given AHB row contains only a value pool entry (w/o Segment (group) and data element)
+        """
+        return (
+            (not ahb_row["Segment Gruppe"])
+            and (not ahb_row["Segment"])
+            and (not ahb_row["Datenelement"])
+            and ahb_row["Codes und Qualifier"]
+        )
+
     def convert_to_flat_ahb(self) -> FlatAnwendungshandbuch:
         """
         Converts the unfolded AHB to a flat AHB.
         """
         meta = AhbMetaInformation(pruefidentifikator=self.meta_data.pruefidentifikator)
         lines: list[AhbLine] = []
 
@@ -282,20 +310,39 @@
         edifact_format = get_format_of_pruefidentifikator(self.meta_data.pruefidentifikator)
         if edifact_format is None:
             logger.warning("'%s' is not a pruefidentifikator", self.meta_data.pruefidentifikator)
             return
 
         flatahb_output_directory_path = output_directory_path / str(edifact_format) / "flatahb"
         flatahb_output_directory_path.mkdir(parents=True, exist_ok=True)
+        flat_ahb = self.convert_to_flat_ahb()
 
-        dump_data = FlatAnwendungshandbuchSchema().dump(self.convert_to_flat_ahb())
-
-        with open(
-            flatahb_output_directory_path / f"{self.meta_data.pruefidentifikator}.json", "w", encoding="utf-8"
-        ) as file:
+        file_path = flatahb_output_directory_path / f"{self.meta_data.pruefidentifikator}.json"
+        if file_path.exists():
+            with open(file_path, "r", encoding="utf-8") as file:
+                existing_flat_ahb = FlatAnwendungshandbuchSchema().load(json.load(file))
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
+        dump_data = FlatAnwendungshandbuchSchema().dump(flat_ahb)
+        with open(file_path, "w", encoding="utf-8") as file:
             json.dump(dump_data, file, ensure_ascii=False, indent=2, sort_keys=True)
         logger.info(
             "The flatahb file for %s is saved at %s",
             self.meta_data.pruefidentifikator,
             flatahb_output_directory_path / f"{self.meta_data.pruefidentifikator}.json",
         )
```

### Comparing `kohlrahbi-0.0.5/temp/test-fobar.docx` & `kohlrahbi-0.0.6a1/temp/test-fobar.docx`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.5/.gitignore` & `kohlrahbi-0.0.6a1/.gitignore`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.5/LICENSE` & `kohlrahbi-0.0.6a1/LICENSE`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.5/pyproject.toml` & `kohlrahbi-0.0.6a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.5/PKG-INFO` & `kohlrahbi-0.0.6a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kohlrahbi
-Version: 0.0.5
+Version: 0.0.6a1
 Summary: Tool to generate machine readable files from AHB documents
 Project-URL: Changelog, https://github.com/Hochfrequenz/kohlrahbi/releases
 Project-URL: Homepage, https://github.com/Hochfrequenz/kohlrahbi
 Author-email: Kevin Krechan <kevin.krechan@hochfrequenz.de>
 License: GPL
 License-File: LICENSE
 Keywords: ahb,automation,bdew,edi@energy
```

