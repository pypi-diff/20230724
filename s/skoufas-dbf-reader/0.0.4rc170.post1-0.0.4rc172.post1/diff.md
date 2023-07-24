# Comparing `tmp/skoufas_dbf_reader-0.0.4rc170.post1.tar.gz` & `tmp/skoufas_dbf_reader-0.0.4rc172.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skoufas_dbf_reader-0.0.4rc170.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "skoufas_dbf_reader-0.0.4rc172.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `skoufas_dbf_reader-0.0.4rc170.post1.tar` & `skoufas_dbf_reader-0.0.4rc172.post1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0      358 2023-07-14 13:25:49.357322 skoufas_dbf_reader-0.0.4rc170.post1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     2310 2023-07-14 13:25:49.357322 skoufas_dbf_reader-0.0.4rc170.post1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0       93 2023-07-14 13:25:49.357322 skoufas_dbf_reader-0.0.4rc170.post1/.flake8
--rw-r--r--   0        0        0      239 2023-07-14 13:25:49.357322 skoufas_dbf_reader-0.0.4rc170.post1/.github/dependabot.yml
--rw-r--r--   0        0        0     1552 2023-07-14 13:25:49.357322 skoufas_dbf_reader-0.0.4rc170.post1/.github/workflows/CI.yml
--rw-r--r--   0        0        0     1521 2023-07-14 13:25:49.357322 skoufas_dbf_reader-0.0.4rc170.post1/.github/workflows/jekyll-gh-pages.yml
--rw-r--r--   0        0        0      263 2023-07-14 13:25:49.357322 skoufas_dbf_reader-0.0.4rc170.post1/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1824 2023-07-14 13:25:49.357322 skoufas_dbf_reader-0.0.4rc170.post1/.gitignore
--rw-r--r--   0        0        0     1540 2023-07-14 13:25:49.357322 skoufas_dbf_reader-0.0.4rc170.post1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      158 2023-07-14 13:25:49.357322 skoufas_dbf_reader-0.0.4rc170.post1/.pypirc
--rw-r--r--   0        0        0      129 2023-07-14 13:25:49.357322 skoufas_dbf_reader-0.0.4rc170.post1/.vscode/extensions.json
--rw-r--r--   0        0        0      127 2023-07-14 13:25:49.357322 skoufas_dbf_reader-0.0.4rc170.post1/.vscode/settings.json
--rw-r--r--   0        0        0    34523 2023-07-14 13:25:49.357322 skoufas_dbf_reader-0.0.4rc170.post1/LICENSE
--rw-r--r--   0        0        0     6267 2023-07-14 13:25:49.357322 skoufas_dbf_reader-0.0.4rc170.post1/README.md
--rw-r--r--   0        0        0     5746 2023-07-14 13:25:49.357322 skoufas_dbf_reader-0.0.4rc170.post1/pyproject.toml
--rw-r--r--   0        0        0       95 2023-07-14 13:25:52.629534 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/__init__.py
--rw-r--r--   0        0        0     4563 2023-07-14 13:25:49.357322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/correction_data.py
--rw-r--r--   0        0        0    80900 2023-07-14 13:25:49.357322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/author_corrections.yml
--rw-r--r--   0        0        0 18255023 2023-07-14 13:25:49.417322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/converted_entries.yml
--rw-r--r--   0        0        0   261526 2023-07-14 13:25:49.421322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/editor_corrections.yml
--rw-r--r--   0        0        0  6074952 2023-07-14 13:25:49.445322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/entries.yml
--rw-r--r--   0        0        0     2236 2023-07-14 13:25:49.445322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field04_corrections.yml
--rw-r--r--   0        0        0     1492 2023-07-14 13:25:49.445322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field05_corrections.yml
--rw-r--r--   0        0        0     1662 2023-07-14 13:25:49.445322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field06_corrections.yml
--rw-r--r--   0        0        0     2149 2023-07-14 13:25:49.445322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field07_corrections.yml
--rw-r--r--   0        0        0   133171 2023-07-14 13:25:49.445322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field08_corrections.yml
--rw-r--r--   0        0        0    12404 2023-07-14 13:25:49.445322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field09_corrections.yml
--rw-r--r--   0        0        0      493 2023-07-14 13:25:49.445322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field10_corrections.yml
--rw-r--r--   0        0        0      440 2023-07-14 13:25:49.445322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field11_corrections.yml
--rw-r--r--   0        0        0     1816 2023-07-14 13:25:49.445322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field16_corrections.yml
--rw-r--r--   0        0        0    45765 2023-07-14 13:25:49.449322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field17_corrections.yml
--rw-r--r--   0        0        0     1081 2023-07-14 13:25:49.449322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field18_corrections.yml
--rw-r--r--   0        0        0    38584 2023-07-14 13:25:49.449322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field19_corrections.yml
--rw-r--r--   0        0        0      247 2023-07-14 13:25:49.449322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field20_corrections.yml
--rw-r--r--   0        0        0    24214 2023-07-14 13:25:49.449322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field30_corrections.yml
--rw-r--r--   0        0        0     6773 2023-07-14 13:25:49.449322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/first_names.yml
--rw-r--r--   0        0        0       50 2023-07-14 13:25:49.449322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/language_codes.yml
--rw-r--r--   0        0        0    65691 2023-07-14 13:25:49.449322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/topic_replacements.yml
--rw-r--r--   0        0        0   109074 2023-07-14 13:25:49.449322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/translator_corrections.yml
--rw-r--r--   0        0        0     1192 2023-07-14 13:25:49.449322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/dbf_to_yaml.py
--rw-r--r--   0        0        0    22109 2023-07-14 13:25:49.449322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/field_extractors.py
--rw-r--r--   0        0        0    28054 2023-07-14 13:25:49.449322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/generate_reports.py
--rw-r--r--   0        0        0     6286 2023-07-14 13:25:49.449322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/utilities.py
--rw-r--r--   0        0        0    18910 2023-07-14 13:25:49.449322 skoufas_dbf_reader-0.0.4rc170.post1/tests/test_field_extractors.py
--rw-r--r--   0        0        0    20756 2023-07-14 13:25:49.449322 skoufas_dbf_reader-0.0.4rc170.post1/tests/test_reports.py
--rw-r--r--   0        0        0     1173 2023-07-14 13:25:49.449322 skoufas_dbf_reader-0.0.4rc170.post1/tests/test_utilities.py
--rw-r--r--   0        0        0     7971 1970-01-01 00:00:00.000000 skoufas_dbf_reader-0.0.4rc170.post1/PKG-INFO
+-rw-r--r--   0        0        0      358 2023-07-24 07:05:31.128452 skoufas_dbf_reader-0.0.4rc172.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     2310 2023-07-24 07:05:31.128452 skoufas_dbf_reader-0.0.4rc172.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0       93 2023-07-24 07:05:31.128452 skoufas_dbf_reader-0.0.4rc172.post1/.flake8
+-rw-r--r--   0        0        0      239 2023-07-24 07:05:31.128452 skoufas_dbf_reader-0.0.4rc172.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1552 2023-07-24 07:05:31.128452 skoufas_dbf_reader-0.0.4rc172.post1/.github/workflows/CI.yml
+-rw-r--r--   0        0        0     1521 2023-07-24 07:05:31.128452 skoufas_dbf_reader-0.0.4rc172.post1/.github/workflows/jekyll-gh-pages.yml
+-rw-r--r--   0        0        0      263 2023-07-24 07:05:31.128452 skoufas_dbf_reader-0.0.4rc172.post1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1824 2023-07-24 07:05:31.128452 skoufas_dbf_reader-0.0.4rc172.post1/.gitignore
+-rw-r--r--   0        0        0     1540 2023-07-24 07:05:31.128452 skoufas_dbf_reader-0.0.4rc172.post1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      158 2023-07-24 07:05:31.128452 skoufas_dbf_reader-0.0.4rc172.post1/.pypirc
+-rw-r--r--   0        0        0      129 2023-07-24 07:05:31.128452 skoufas_dbf_reader-0.0.4rc172.post1/.vscode/extensions.json
+-rw-r--r--   0        0        0      127 2023-07-24 07:05:31.128452 skoufas_dbf_reader-0.0.4rc172.post1/.vscode/settings.json
+-rw-r--r--   0        0        0    34523 2023-07-24 07:05:31.128452 skoufas_dbf_reader-0.0.4rc172.post1/LICENSE
+-rw-r--r--   0        0        0     6267 2023-07-24 07:05:31.128452 skoufas_dbf_reader-0.0.4rc172.post1/README.md
+-rw-r--r--   0        0        0     5746 2023-07-24 07:05:31.132453 skoufas_dbf_reader-0.0.4rc172.post1/pyproject.toml
+-rw-r--r--   0        0        0       95 2023-07-24 07:05:37.748873 skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/__init__.py
+-rw-r--r--   0        0        0     4563 2023-07-24 07:05:31.132453 skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/correction_data.py
+-rw-r--r--   0        0        0   121354 2023-07-24 07:05:31.132453 skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/data/author_corrections.yml
+-rw-r--r--   0        0        0 18256098 2023-07-24 07:05:31.204457 skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/data/converted_entries.yml
+-rw-r--r--   0        0        0   261526 2023-07-24 07:05:31.208457 skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/data/editor_corrections.yml
+-rw-r--r--   0        0        0  6074952 2023-07-24 07:05:31.240459 skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/data/entries.yml
+-rw-r--r--   0        0        0     2236 2023-07-24 07:05:31.240459 skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/data/field04_corrections.yml
+-rw-r--r--   0        0        0     1492 2023-07-24 07:05:31.240459 skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/data/field05_corrections.yml
+-rw-r--r--   0        0        0     1662 2023-07-24 07:05:31.240459 skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/data/field06_corrections.yml
+-rw-r--r--   0        0        0     2149 2023-07-24 07:05:31.240459 skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/data/field07_corrections.yml
+-rw-r--r--   0        0        0   133171 2023-07-24 07:05:31.240459 skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/data/field08_corrections.yml
+-rw-r--r--   0        0        0    12404 2023-07-24 07:05:31.240459 skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/data/field09_corrections.yml
+-rw-r--r--   0        0        0      493 2023-07-24 07:05:31.240459 skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/data/field10_corrections.yml
+-rw-r--r--   0        0        0      440 2023-07-24 07:05:31.240459 skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/data/field11_corrections.yml
+-rw-r--r--   0        0        0     1816 2023-07-24 07:05:31.240459 skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/data/field16_corrections.yml
+-rw-r--r--   0        0        0    45765 2023-07-24 07:05:31.240459 skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/data/field17_corrections.yml
+-rw-r--r--   0        0        0     1081 2023-07-24 07:05:31.240459 skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/data/field18_corrections.yml
+-rw-r--r--   0        0        0    38584 2023-07-24 07:05:31.244459 skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/data/field19_corrections.yml
+-rw-r--r--   0        0        0      247 2023-07-24 07:05:31.244459 skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/data/field20_corrections.yml
+-rw-r--r--   0        0        0    24214 2023-07-24 07:05:31.244459 skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/data/field30_corrections.yml
+-rw-r--r--   0        0        0     6773 2023-07-24 07:05:31.244459 skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/data/first_names.yml
+-rw-r--r--   0        0        0       50 2023-07-24 07:05:31.244459 skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/data/language_codes.yml
+-rw-r--r--   0        0        0    65691 2023-07-24 07:05:31.244459 skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/data/topic_replacements.yml
+-rw-r--r--   0        0        0   109074 2023-07-24 07:05:31.244459 skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/data/translator_corrections.yml
+-rw-r--r--   0        0        0     1192 2023-07-24 07:05:31.244459 skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/dbf_to_yaml.py
+-rw-r--r--   0        0        0    22109 2023-07-24 07:05:31.244459 skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/field_extractors.py
+-rw-r--r--   0        0        0    28522 2023-07-24 07:05:31.244459 skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/generate_reports.py
+-rw-r--r--   0        0        0     6286 2023-07-24 07:05:31.244459 skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/utilities.py
+-rw-r--r--   0        0        0    18910 2023-07-24 07:05:31.244459 skoufas_dbf_reader-0.0.4rc172.post1/tests/test_field_extractors.py
+-rw-r--r--   0        0        0    21224 2023-07-24 07:05:31.244459 skoufas_dbf_reader-0.0.4rc172.post1/tests/test_reports.py
+-rw-r--r--   0        0        0     1173 2023-07-24 07:05:31.244459 skoufas_dbf_reader-0.0.4rc172.post1/tests/test_utilities.py
+-rw-r--r--   0        0        0     7971 1970-01-01 00:00:00.000000 skoufas_dbf_reader-0.0.4rc172.post1/PKG-INFO
```

### Comparing `skoufas_dbf_reader-0.0.4rc170.post1/.devcontainer/devcontainer.json` & `skoufas_dbf_reader-0.0.4rc172.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc170.post1/.github/workflows/CI.yml` & `skoufas_dbf_reader-0.0.4rc172.post1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc170.post1/.github/workflows/jekyll-gh-pages.yml` & `skoufas_dbf_reader-0.0.4rc172.post1/.github/workflows/jekyll-gh-pages.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc170.post1/.gitignore` & `skoufas_dbf_reader-0.0.4rc172.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc170.post1/.pre-commit-config.yaml` & `skoufas_dbf_reader-0.0.4rc172.post1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc170.post1/LICENSE` & `skoufas_dbf_reader-0.0.4rc172.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc170.post1/README.md` & `skoufas_dbf_reader-0.0.4rc172.post1/README.md`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc170.post1/pyproject.toml` & `skoufas_dbf_reader-0.0.4rc172.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/correction_data.py` & `skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/correction_data.py`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/author_corrections.yml` & `skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/data/author_corrections.yml`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,69 @@
 ---
 author_corrections:
+## ΟΚ:
+## ΟΡΓΑΝΩΣΗ (ΧΩΡΙΣ ΚΟΜΜΑ)
+## ΕΠΙΘΕΤΟ,ΟΝΟΜΑ
+## ΕΠΙΘΕΤΟ,ΟΝ.
+## ΕΠΙΘΕΤΟ,ΟΝΟΜΑ,ΠΑΤΡΩΝΥΜΟ
+## ΕΠΙΘΕΤΟ,ΟΝΟΜΑ,ΔΕΥΤΕΡΟ
+## ΕΠΙΘΕΤΟ,ΟΝΟΜΑ@ΨΕΥΔΩΝΥΜΟ
+## @ΨΕΥΔΩΝΥΜΟ
 
 #### ΧΡΕΙΑΖΟΝΤΑΙ ΠΑΡΑΠΑΝΩ ΕΛΕΓΧΟ
   ΒΟΚΑΚΙΟΣ: BOCCACCIO,GIOVANNI
   ΒΟΚΚΑΚΚΙΟ,ΤΖΟΒΑΝΝΙ: BOCCACCIO,GIOVANNI
   VIRGILE: VIRGILIO
   ΒΟΛΤΑΙΡΟΣ: VOLTAIRE
 
   ΒΕΛΕΝΣΤΙΝΛΗΣ,ΡΗΓΑΣ: ΒΕΛΕΝΣΤΙΝΛΗΣ,ΡΗΓΑΣ
 
   ΒΥΖΑΝΤΙΟ: ΒΥΖΑΝΤΙΟ
   ΑΡΑΓΚΟΝ: ARAGON,LOUIS
 
+#### ΔΕΝ ΒΡΙΣΚΟΝΤΑΙ ΣΤΟ ΔΙΑΔΥΚΤΙΟ!
+  ΜΠΑΓΙΑΘ,Ζ.: ΜΠΑΓΙΑΘ,Ζ.
+  ΜΠΑΙΡΑΚΤΑΡΗΣ,ΜΕΤΑΞΙΑ: ΜΠΑΙΡΑΚΤΑΡΗΣ,ΜΕΤΑΞΙΑ
+  BARTHOLOY KARI: BARTHOLOY,KARI
+  BAYER ERIGH: BAYER,ERIGH
+  BUHRCHNER L: BUHRCHNER,L.
+
+
 #### ΔΕΝ ΕΙΝΑΙ ΣΥΓΓΡΑΦΕΙΣ, ΧΡΕΙΑΖΕΤΑΙ ΑΛΛΑΓΗ ΟΛΗ Η ΕΓΓΡΑΦΗ ΜΕΤΑ ΤΗΝ
   WACKEL WICKEL: WACKEL WICKEL
   VETUSTA REGENSIO: VETUSTA REGENSIO
+  ANNALES DE LA FACULTE DES: ANNALES DE LA FACULTE DES
+  ANNALES DU MUSEE GUIMET: ANNALES DU MUSEE GUIMET
 
 #### ΠΡΟΒΛΗΜΑΤΙΚΑ
   VICBUHR B: VICBUHR B # https://books.google.it/books?id=YdxTAAAAcAAJ&printsec=frontcover&hl=el&source=gbs_ge_summary_r&cad=0#v=onepage&q&f=false
   VINUS G.: VINUS G.
   WAATZ ALEXANDER: WAATZ,ALEXANDER
   WILLE-MOSSE COUKOWSKY: WILL,EDOUARD!!MOSSE,CLAUDE!!GOUKOWSKY,PAUL
   ΑΝΔΡΙΤΣΟΠΟΥΛΟΥ Σ., ΚΕΝΤΕΠΟΖΙΔΗ Ν, ΠΡΑΠΑ: ΑΝΔΡΙΤΣΟΠΟΥΛΟΥ,Σ.!!ΚΕΝΤΕΠΟΖΙΔΗ,Ν.,ΠΡΑΠΑ,
   ALEXIS,VASILIS: ALEXIS,VASILIS
 
-  ANNALES DE LA FACULTE DES: ANNALES DE LA FACULTE DES
-  ANNALES DU MUSEE GUIMET: ANNALES DU MUSEE GUIMET
-
   ΑΛΙΦΕΡΗ-ΜΑΚΡΟΠΟΥΛΟΥ,ΚΑΙΤΗ: ΑΛΙΦΕΡΗ-ΜΑΚΡΟΠΟΥΛΟΥ,ΚΑΙΤΗ
   ΑΛΙΦΕΡΗ-ΜΑΡΚΟΠΟΥΛΟΥ,ΚΑΙΤΗ: ΑΛΙΦΕΡΗ-ΜΑΡΚΟΠΟΥΛΟΥ,ΚΑΙΤΗ
 
   AOYISTAPACE: AOYISTAPACE
 
   ΑΡΧΑΙΑΙ ΕΛΛΗ: ΑΡΧΑΙΑΙ ΕΛΛΗ
   ΑΡΧΕΙΑ ΓΕΝΙΚΟΥ ΕΠΙΤΕΛΕΙΟΥ ΣΤΡΑΤΟΥ: ΑΡΧΕΙΑ ΓΕΝΙΚΟΥ ΕΠΙΤΕΛΕΙΟΥ ΣΤΡΑΤΟΥ
 
-#### ΨΕΥΔΩΝΥΜΑ
-  AJAR EMILE: AJAR,EMILE
+
+  ΨΑΡΟΜΗΛΙΓΚΟΣ , ΛΑΖΟΥ , ΚΑΡΤΑΛΗΣ: ΨΑΡΟΜΗΛΙΓΚΟΣ,!!ΛΑΖΟΥ,!!ΚΑΡΤΑΛΗΣ,
+  ΚΕΛΕΣΙΔΗΣ, ΤΕΛΗΣ: ΚΕΛΕΣΙΔΗΣ,ΤΕΛΗΣ
+  ΩUENEAU RAYMOND: QUENEAU,RAYMOND
+  FINLAY GEORG: FINLAY,GEORGE
+  FINLAY,GEORGE: FINLAY,GEORGE
+  FINLEY M: FINLEY,M.I.
+  ΦΙΝΛΕΥ,ΓΕΩΡΓΙΟΥ: FINLAY,GEORGE
+  FINLEY,M.I.: FINLEY,M.I.
+
 
 ####
 
   # no author
   .Σ: null
   "X . Σ.": null
   "X,S": null
@@ -61,22 +84,21 @@
   "ΧΣ": null
   Χ,Α: null
   Χ.Ε: null
   χ.Σ.: null
 
   ΑΝΩΝΥΜΟΣ: ΑΝΩΝΥΜΟΣ ΣΥΓΓΡΑΦΕΑΣ
 
-  ΨΑΡΟΜΗΛΙΓΚΟΣ , ΛΑΖΟΥ , ΚΑΡΤΑΛΗΣ: ΨΑΡΟΜΗΛΙΓΚΟΣ,!!ΛΑΖΟΥ,!!ΚΑΡΤΑΛΗΣ,
-  ΚΕΛΕΣΙΔΗΣ, ΤΕΛΗΣ: ΚΕΛΕΣΙΔΗΣ,ΤΕΛΗΣ
-  ΩUENEAU RAYMOND: QUENEAU,RAYMOND
-  FINLAY GEORG: FINLAY,GEORGE
-  FINLAY,GEORGE: FINLAY,GEORGE
-  FINLEY M: FINLEY,M.I.
-  ΦΙΝΛΕΥ,ΓΕΩΡΓΙΟΥ: FINLAY,GEORGE
-  FINLEY,M.I.: FINLEY,M.I.
+#### ΨΕΥΔΩΝΥΜΑ
+  AJAR EMILE: GARY,ROMAIN@EMILE AJAR
+  ΖΑΝΑΝΤΡΙΣ,ΚΑΣ: ΑΝΔΡΙΑΝΟΠΟΥΛΟΥ,ΙΩΑΝΝΑ@ΚΥΡΙΑ ΖΑΝΑΝΤΡΙΣ
+  ΜΠΑΙΡΟΝ: BYRON,GEORGE,GORDON@LORD BYRON
+  ΜΠΑΣΤΑ,ΚΩΣΤΗ: ΜΠΑΣΤΟΥΝΌΠΟΥΛΟΣ,ΑΙΜΊΛΙΟΣ,ΚΩΝΣΤΑΝΤΊΝΟΣ@ΚΩΣΤΗΣ ΜΠΑΣΤΙΑΣ
+  ΜΠΑΣΤΙΑ,ΚΩΣΤΗ: ΜΠΑΣΤΟΥΝΌΠΟΥΛΟΣ,ΑΙΜΊΛΙΟΣ,ΚΩΝΣΤΑΝΤΊΝΟΣ@ΚΩΣΤΗΣ ΜΠΑΣΤΙΑΣ
+  ΜΠΑΣΤΙΑΣ,ΚΩΣΤΑΣ: ΜΠΑΣΤΟΥΝΌΠΟΥΛΟΣ,ΑΙΜΊΛΙΟΣ,ΚΩΝΣΤΑΝΤΊΝΟΣ@ΚΩΣΤΗΣ ΜΠΑΣΤΙΑΣ
 
 #### A
   AYLWEN,AXEL: AYLWEN,AXEL
   AYMARD A: AYMARD,ANDRE
   AYMARD ANDRE: AYMARD,ANDRE
   AYMARD ANDRE-AUBOYER JEAN: AYMARD,ANDRE-AUBOYER,JEANNINE
   AZIZ,PHILIPPE: AZIZ,PHILIPPE
@@ -705,15 +727,14 @@
   ΑΞΙΟΝΟΦ,ΒΑΣΙΛΗ: ΑΞΙΟΝΟΦ,ΒΑΣΙΛΗΣ
   ΑΞΙΩΤΗ,ΜΕΛΠΩ: ΑΞΙΩΤΗ,ΜΕΛΠΩ
   ΑΞΙΩΤΗ,ΠΕΤΡΟΥ: ΑΞΙΩΤΗΣ,ΠΕΤΡΟΣ,Ι.
   ΑΞΙΩΤΗ,ΘΕΟΔΩΡΟΥ: ΑΞΙΩΤΗΣ,ΘΕΟΔΩΡΟΣ
   ΑΞΙΩΤΗΣ,ΠΕΤΡΟΣ Ι: ΑΞΙΩΤΗΣ,ΠΕΤΡΟΣ,Ι.
 #### A
 
-
 #### B
   Β'ΝΕΟΓΝΙΚΟ ΤΜΗΜ.ΝΟΣ.ΠΑΙΔΩΝ ΑΓΙΑ ΣΟΦΙΑ: Β' ΝΕΟΓΝΙΚΟ ΤΜΗΜΑ ΝΟΣΟΚΟΜΕΙΟΥ ΠΑΙΔΩΝ ΑΓΙΑ ΣΟΦΙΑ
   Β. ΚΑΛΦΑΣ ΚΑΙ Γ. ΖΩΓΡΑΦΙΔΗΣ: ΚΑΛΦΑΣ,Β.!!ΖΩΓΡΑΦΙΔΗΣ,Γ.
   ΒΑΦΕΙΑΔΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ Μ.: ΒΑΦΕΙΑΔΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ,Μ.
   ΒΑΦΕΙΑΔΟΥ,ΜΑΡΙΑΣ: ΒΑΦΕΙΑΔΟΥ,ΜΑΡΙΑ
   ΒΑΦΙΑ,ΓΡΗΓΟΡΗ: ΒΑΦΙΑΣ,ΓΡΗΓΟΡΗΣ
   ΒΑΦΙΑΣ ΤΑΚΗΣ: ΒΑΦΙΑΣ,ΤΑΚΗΣ,Γ.
@@ -1044,18 +1065,18 @@
   ΒΛΑΧΟΓΙΑΝΝΗΣ. Ι: ΒΛΑΧΟΓΙΑΝΝΗΣ,ΓΙΑΝΝΗΣ
   ΒΛΑΧΟΠΑΝΟΣ ΔΗΜΗΤΡΗΣ: ΒΛΑΧΟΠΑΝΟΣ,ΔΗΜΗΤΡΗΣ
   ΒΛΑΧΟΠΑΝΟΣ, ΔΗΜΗΤΡΗΣ: ΒΛΑΧΟΠΑΝΟΣ,ΔΗΜΗΤΡΗΣ
   ΒΛΑΧΟΠΑΝΟΣ,ΔΗΜΗΤΡΗΣ: ΒΛΑΧΟΠΑΝΟΣ,ΔΗΜΗΤΡΗΣ
   ΒΛΑΧΟΠΟΥΛΟΣ,ΣΠΥΡΟΣ: ΒΛΑΧΟΠΟΥΛΟΣ,ΣΠΥΡΟΣ
   ΒΛΑΧΟΠΟΥΛΟΥ ΣΤΕΛΛΑ: ΒΛΑΧΟΠΟΥΛΟΥ,ΣΤΕΛΛΑ
   ΒΛΑΧΟΠΟΥΛΟΥ,ΣΤΕΛΛΑ: ΒΛΑΧΟΠΟΥΛΟΥ,ΣΤΕΛΛΑ
-  ΒΛΑΧΟΣ, ΑΓΓΕΛΟΣ: ΒΛΑΧΟΣ,ΑΓΓΕΛΟΣ,ΣΤ,
-  ΒΛΑΧΟΣ,ΑΓΓΕΛΟΣ: ΒΛΑΧΟΣ,ΑΓΓΕΛΟΣ,ΣΤ,
-  ΒΛΑΧΟΣ,ΑΓΓΕΛΟΣ ΣΤ.: ΒΛΑΧΟΣ,ΑΓΓΕΛΟΣ,ΣΤ,
-  ΒΛΑΧΟΣ,ΑΓΓΕΛΟΣ,ΣΤ: ΒΛΑΧΟΣ,ΑΓΓΕΛΟΣ,ΣΤ,
+  ΒΛΑΧΟΣ, ΑΓΓΕΛΟΣ: ΒΛΑΧΟΣ,ΑΓΓΕΛΟΣ,ΣΤ.
+  ΒΛΑΧΟΣ,ΑΓΓΕΛΟΣ: ΒΛΑΧΟΣ,ΑΓΓΕΛΟΣ,ΣΤ.
+  ΒΛΑΧΟΣ,ΑΓΓΕΛΟΣ ΣΤ.: ΒΛΑΧΟΣ,ΑΓΓΕΛΟΣ,ΣΤ.
+  ΒΛΑΧΟΣ,ΑΓΓΕΛΟΣ,ΣΤ: ΒΛΑΧΟΣ,ΑΓΓΕΛΟΣ,ΣΤ.
   ΒΛΑΧΟΣ,ΓΕΡΑΣΙΜΟΣ: ΒΛΑΧΟΣ,ΓΕΡΑΣΙΜΟΣ
   ΒΛΑΧΟΣ,Ι.Δ: ΒΛΑΧΟΣ,Ι.,Δ.
   ΒΛΑΧΟΣ,ΙΕΡΟΘΕΟΣ ΑΡΧΙΜΑΝΔΡΗΤΗΣ: ΒΛΑΧΟΣ,ΙΕΡΟΘΕΟΣ ΑΡΧΙΜΑΝΔΡΗΤΗΣ
   ΒΛΑΧΟΣ,ΙΕΡΟΘΕΟΣ ΙΕΡΟΚΥΡΗΚΑΣ: ΒΛΑΧΟΣ,ΙΕΡΟΘΕΟΣ ΙΕΡΟΚΥΡΗΚΑΣ
   ΒΛΑΧΟΣ,Κ.Π: ΒΛΑΧΟΣ,Κ.,Π.
   VLACHOS,NICOLAS: VLACHOS,NICOLAS
   ΒΛΑΧΟΥ,Α.Σ: ΒΛΑΧΟΣ,ΑΓΓΕΛΟΣ,Σ.
@@ -1269,8 +1290,723 @@
   DR WOOD,M.J: WOOD,M.J.
   WOODHOUSE,C.M: WOODHOUSE,CRISTOPHER,MONTAGUE
   WOODHOYSE,C: WOODHOUSE,CRISTOPHER,MONTAGUE
   WOODS,ALAN: WOODS,ALAN
   WUHST FRITZ: WUST,FRITZ,R.
   WUILLEUMIER PIERRE: WUILLEUMIER,PIERRE
 
-##### B
+##### B V
+
+##### B ΜΠ
+
+  BABELON ERNEST: BABELON,ERNEST
+  BABELON J LAFAURIE J: BABELON,JEAN!!LAFAURIE,JEAN
+  BABELON JEAN: BABELON,JEAN
+  BABELON,J: BABELON,JEAN
+  BACCALARIO,P.D: BACCALARIO,PIERDOMENICO
+  ΜΠΑΧ,Α.Μ: BACH,ANNA,MAGDALENA
+  BACK JOSEF: BACK,JOSEF
+  ΜΠΑΔΑ,ΚΩΝΣΤΑΝΤΙΝΑ: ΜΠΑΔΑ,ΚΩΝΣΤΑΝΤΙΝΑ
+  BADIOU,ALAIN: BADIOU,ALAIN
+  ΜΠΑΕΤΕΝ.ΛΙΒΕ-ΜΠΕΝΚΕ-ΚΟΥΝΤΣΛΕΡ,ΡΟΖΜΑΡΙ: BAETEN,LIEVE!!KUNZLER-BEHNCKE,ROSEMARIE
+  BAGGISH,MICHAEL: BAGGISH,MICHAEL
+  ΜΠΑΓΙΑ-ΑΛΕΞΟΠΟΥΛΟΥ,ΠΟΛΛΥ: ΜΠΑΓΙΑ-ΑΛΕΞΟΠΟΥΛΟΥ,ΠΟΛΛΥ
+  ΜΠΑΓΙΕΡ ΤΟΜΜΥ: BAYER,TOMMY
+  BAHN,PAUL: BAHN,PAUL
+  BAHRDT HANS: BAHRDT,HANS,PAUL
+  ΜΠΑΙΛΑ,ΤΕΣΥ: ΜΠΑΙΛΑ,ΤΕΣΥ
+  ΜΠΑΙΛΗΣ,ΠΑΝΟΣ: ΜΠΑΙΛΗΣ,ΠΑΝΟΣ
+  BAILLEUX,NATHALIE: BAILLEUX,NATHALIE
+  ΜΠΑΙΡΑΚΤΑΡΗ,ΑΝΤΩΝΙΟΥ: ΜΠΑΙΡΑΚΤΑΡΗΣ,ΑΝΤΩΝΙΟΣ
+  ΜΠΑΙΡΑΚΤΑΡΗ,ΣΤΥΛ: ΜΠΑΙΡΑΚΤΑΡΗΣ,ΣΤΥΛ.
+  ΜΠΑΙΡΑΚΤΑΡΗ,ΣΤΥΛ.: ΜΠΑΙΡΑΚΤΑΡΗΣ,ΣΤΥΛ.
+  ΜΠΑΙΡΑΚΤΑΡΗΣ,ΚΩΣΤΑΣ: ΜΠΑΙΡΑΚΤΑΡΗΣ,ΚΩΣΤΑΣ
+  ΜΠΑΙΡΑΚΤΑΡΗΣ,ΣΤΥΛ: ΜΠΑΙΡΑΚΤΑΡΗΣ,ΣΤΥΛ.
+
+  ΜΠΑΗΣ,ΜΙΧΑΗΛ: ΜΠΑΗΣ,ΜΙΧΑΗΛ
+  ΜΠΑΙΤΣΗΣ,ΤΑΚΗΣ: ΜΠΑΙΤΣΗΣ,ΤΑΚΗΣ
+  ΜΠΑΚ ΠΕΡΛ: BUCK,PEARL,S.
+  ΜΠΑΚ,ΠΕΡΛ: BUCK,PEARL,S.
+  ΜΠΑΚΑΓΙΑΝΝΗ-ΚΑΣΙΑΡ,ΠΕΛΛΑ: ΜΠΑΚΑΓΙΑΝΝΗ-ΚΑΣΙΑΡ,ΠΕΛΛΑ
+  ΜΠΑΚΑΛΑΚΗ,Γ.: ΜΠΑΚΑΛΑΚΗ,Γ.
+  ΜΠΑΚΑΛΑΚΗ-ΕΜΠΕΟΓΛΟΥ,ΕΥΔΟΚΙΑ: ΜΠΑΚΑΛΑΚΗ-ΕΜΠΕΟΓΛΟΥ,ΕΥΔΟΚΙΑ
+  ΜΠΑΚΑΟΥΚΑΣ,ΜΙΧΑΗΛ: ΜΠΑΚΑΟΥΚΑΣ,ΜΙΧΑΗΛ
+  BAKARIC,VLADIMIR: BAKARIC,VLADIMIR
+  ΜΠΑΚΑΣ,ΘΩΜΑΣ: ΜΠΑΚΑΣ,ΘΩΜΑΣ
+  ΜΠΑΚΑΤΣΟΥΛΑΣ,ΜΕΝΕΛΑΟΣ: ΜΠΑΚΑΤΣΟΥΛΑΣ,ΜΕΝΕΛΑΟΣ
+  BAKER G: BAKER,GEORGE,PHILIP
+  BAKER,,Q.P: BAKER,GEORGE,PHILIP
+  ΜΠΑΚΟΓΙΑΝΝΗ,ΒΑΣΙΛΕΙΟΣ: ΜΠΑΚΟΓΙΑΝΝΗS,ΒΑΣΙΛΕΙΟΣ
+  ΜΠΑΚΟΓΙΑΝΝΗΣ,ΣΤΕΦΑΝΟΣ: ΜΠΑΚΟΓΙΑΝΝΗΣ,ΣΤΕΦΑΝΟΣ
+  ΜΠΑΚΟΣ,ΗΛΙΑΣ: ΜΠΑΚΟΣ,ΗΛΙΑΣ,Δ.
+  ΜΠΑΚΟΣ,ΗΛΙΑΣ Δ: ΜΠΑΚΟΣ,ΗΛΙΑΣ,Δ.
+  ΜΠΑΚΟΥΡΗ,ΜΙΧΑΗΛ-ΓΕΩΡΓΙΟΥ: ΜΠΑΚΟΥΡΗΣ,ΜΙΧΑΗΛ,ΓΕΩΡΓΙΟΣ
+  ΜΠΑΚΟΥΡΗΣ,ΓΙΩΡΓΟΣ: ΜΠΑΚΟΥΡΗΣ,ΓΙΩΡΓΟΣ
+  ΜΠΑΛΑΦΟΥΣΙΑ-ΓΑΛΑΝΙΔΟΥ,ΕΛΣΑΣ: ΜΠΑΛΑΦΟΥΣΙΑ-ΓΑΛΑΝΙΔΟΥ,ΕΛΣΑ
+  ΜΠΑΛΑΦΟΥΤΗ- ΦΩΤΙΑΔΟΥ ΓΙΩΤΑ: ΜΠΑΛΑΦΟΥΤΗ-ΦΩΤΙΑΔΟΥ,ΓΙΩΤΑ
+  ΜΠΑΛΑΦΟΥΤΗ-ΦΩΤΙΑΔΟΥ,ΓΙΩΤΑ: ΜΠΑΛΑΦΟΥΤΗ-ΦΩΤΙΑΔΟΥ,ΓΙΩΤΑ
+  ΜΠΑΛΑΜΑΤΣΙΑ,ΑΓΓΕΛΙΚΗ: ΜΠΑΛΑΜΑΤΣΙΑ,ΑΓΓΕΛΙΚΗ
+  BALANDIER,GEORGE: BALANDIER,GEORGES
+  ΜΠΑΛΑΣ,Π.: ΜΠΑΛΑΣ,ΠΑΝΑΓΙΏΤΗΣ
+  ΜΠΑΛΑΣΚΑ,ΓΡΗΓΟΡΙΟΥ: ΜΠΑΛΑΣΚΑΣ,ΓΡΗΓΟΡΙΟΣ
+  ΜΠΑΛΑΣΚΑΣ,ΑΛΕΞΑΝΔΡΟΣ Α: ΜΠΑΛΑΣΚΑΣ,ΑΛΕΞΑΝΔΡΟΣ,Α.
+  ΜΠΑΛΑΤΣΟΥΚΑ,ΣΩΤΗΡΙΟΥ: ΜΠΑΛΑΤΣΟΥΚΑΣ,ΣΩΤΗΡΙΟΣ
+  ΜΠΑΛΕΣΤΡΙΝΙ,ΝΑΝΝΙ: BALESTRINI,NANNI
+
+  ΜΠΑΛΦΟΥΣΙΑ-ΓΑΛΑΝΙΔΟΥ,ΕΛΣΑ: ΜΠΑΛΦΟΥΣΙΑ-ΓΑΛΑΝΙΔΟΥ,ΕΛΣΑ
+  ΜΠΑΛΗ,ΤΙΛΛΑ: ΜΠΑΛΗ,ΤΙΛΛΑ
+  ΜΠΑΛΙΔΗ,ΘΕΟΔΩΡΟΥ: ΜΠΑΛΙΔΗΣ,ΘΕΟΔΩΡΟΣ
+  ΜΠΑΛΙΜΠΑΡ,ΕΤΙΕΝ: BALIBAR,ÉTIENNE
+  BALLANTYNE,ANDREW: BALLANTYNE,ANDREW
+  BALLARD,J.G.: BALLARD,JAMES,GRAHAM
+  ΜΠΑΛΟΔΗΜΟΣ,ΠΕΡΙΚΛΗΣ: ΜΠΑΛΟΔΗΜΟΣ,ΠΕΡΙΚΛΗΣ
+  ΜΠΑΛΟΓΛΟΥ,ΧΡΗΣΤΟΣ: ΜΠΑΛΟΓΛΟΥ,ΧΡΗΣΤΟΣ
+  ΜΠΑΛΩΜΕΝΟΥ,ΦΩΤΕΙΝΗ: ΜΠΑΛΩΜΕΝΟΥ,ΦΩΤΕΙΝΗ
+  ΜΠΑΛΟΥΜΗΣ,ΕΠΑΜ.: ΜΠΑΛΟΥΜΗΣ,ΕΠΑΜΕΙΝΩΝΔΑΣ
+  ΜΠΑΛΟΥΜΗΣ,ΕΠΑΜΕΙΝΩΝΔΑΣ: ΜΠΑΛΟΥΜΗΣ,ΕΠΑΜΕΙΝΩΝΔΑΣ
+  ΜΠΑΛΣΟΝ,Ζ: BALSDON,JOHN,PERCY VYVIAN DACRE
+  ΜΠΑΛΤΑ,ΕΥΑΓΓΕΛΙΑ: ΜΠΑΛΤΑ,ΕΥΑΓΓΕΛΙΑ
+  ΜΠΑΛΤΑ,ΕΥΑΓΓΕΛΙΑ-ΚΟΥΡΟΥΠΟΥ,ΜΑΤΟΥΛΑ: ΜΠΑΛΤΑ,ΕΥΑΓΓΕΛΙΑ!!ΚΟΥΡΟΥΠΟΥ,ΜΑΤΟΥΛΑ
+  ΜΠΑΛΤΑ,ΓΑΛΑΤΕΙΑ: ΜΠΑΛΤΑ,ΓΑΛΑΤΕΙΑ
+  ΜΠΑΛΤΑΓΙΑΝΝΗΣ,ΘΑΝΑΣΗΣ: ΜΠΑΛΤΑΓΙΑΝΝΗΣ,ΘΑΝΑΣΗΣ
+  BALZAC,HONORE DE: BALZAC,HONORE DE
+  ΜΠΑΛΖΑΚ: BALZAC,HONORÉ DE
+  ΜΠΑΛΖΑΚ ΟΝΟΡΕ: BALZAC,HONORÉ DE
+  ΜΠΑΛΖΑΚ ΟΝΟΡΕ ΝΤΕ: BALZAC,HONORÉ DE
+  ΜΠΑΛΖΑΚ, ΝΤΕ, ΟΝΟΡΕ: BALZAC,HONORÉ DE
+  ΜΠΑΛΖΑΚ,ΟΝΟΡΕ: BALZAC,HONORÉ DE
+  ΜΠΑΛΖΑΚ,ΟΝΟΡΕΝΤΕ: BALZAC,HONORÉ DE
+  BALZC: BALZAC,HONORÉ DE
+  BAMM PETER: BAMM,PETER
+  ΜΠΑΜΠΑΛΗ ΑΓΓΕΛΙΚΗ: ΜΠΑΜΠΑΛΗ,ΑΓΓΕΛΙΚΗ
+  ΜΠΑΜΠΑΝΑΣΗ, ΣΤΕΡΓΙΟΥ: ΜΠΑΜΠΑΝΑΣΗΣ,ΣΤΕΡΓΙΟΣ
+  ΜΠΑΜΠΕΡΙ ΚΡΙΣ: BAMBERY,CHRIS
+  ΜΠΑΜΠΙΝΙΩΤΗΣ,Γ.: ΜΠΑΜΠΙΝΙΩΤΗΣ,ΓΕΩΡΓΙΟΣ
+  ΜΠΑΜΠΙΝΙΩΤΗΣ,Γ: ΜΠΑΜΠΙΝΙΩΤΗΣ,ΓΕΩΡΓΙΟΣ
+  ΜΠΑΜΠΟΥΝΗΣ,ΧΑΡΗΣ: ΜΠΑΜΠΟΥΝΗΣ,ΧΑΡΗΣ
+  BAND ERSTER: BAND,ERSTER
+  BANKS,OLIVER: BANKS,OLIVER
+  ΜΠΑΝΤΑΛΟΥΚΑ,ΚΛΑΥΔΙΟΣ: ΜΠΑΝΤΑΛΟΥΚΑΣ,ΚΛΑΥΔΙΟΣ
+  ΜΠΑΝΤΑΛΟΥΚΑ,ΠΟΛΥΞΕΝΗ: ΜΠΑΝΤΑΛΟΥΚΑ,ΠΟΛΥΞΕΝΗ
+  ΜΠΑΝΤΑΛΟΥΚΑΣ,ΚΑΛΑΥΔΙΟΣ: ΜΠΑΝΤΑΛΟΥΚΑΣ,ΚΛΑΥΔΙΟΣ
+  ΜΠΑΝΤΑΛΟΥΚΑΣ,ΚΛΑΥΔΙΟΣ: ΜΠΑΝΤΑΛΟΥΚΑΣ,ΚΛΑΥΔΙΟΣ
+  ΜΠΑΡΑ,ΑΛΕΞΑΝΔΡΟΥ: ΜΠΑΡΑΣ,ΑΛΕΞΑΝΔΡΟΣ
+  ΜΠΑΡΑ,ΒΑΣΙΛΕΙΟΣ: ΜΠΑΡΑΣ,ΒΑΣΙΛΕΙΟΣ
+  BARAGLI,SANDRA: BARAGLI,SANDRA
+  ΜΠΑΡΑΜΠΑΣ,ΜΠΕΝΥ: BARBASH,BENNY
+  ΜΠΑΡΑΣ,ΑΛΕΞΑΝΔΡΟΣ: ΜΠΑΡΑΣ,ΑΛΕΞΑΝΔΡΟΣ
+  ΜΠΑΡΑΣΚΑΓΙΑ,ΝΑΤΑΛΙΑ: ΜΠΑΡΑΣΚΑΓΙΑ,ΝΑΤΑΛΙΑ
+  BARBAGALLO,C: BARBAGALLO,CORRADO
+  BARBALO CORRADO: BARBAGALLO,CORRADO
+  BARBER,Α.: BARBER,ERIC,ARTHUR
+  ΜΠΑΡΔΑΝΗ,ΣΟΦΙΑ: ΜΠΑΡΔΑΝΗ,ΣΟΦΙΑ
+  ΜΠΑΡΙΓΕ,ΕΛΙΖΑΜΠΕΤ: BARILLE,ELISABETH
+  ΜΠΑΡΙΓΙΕ,ΠΙΕΡ-ΓΚΡΕΝΤΙ ΖΑΝ-ΠΙΕΡ: BARILLET,PIERRE!!GRÉDY,JEAN-PIERRE
+  ΜΠΑΡΙΤΑΚΗ,ΒΑΓΓΕΛΗ: ΜΠΑΡΙΤΑΚΗΣ,ΒΑΓΓΕΛΗΣ
+  BARKER,PHILLIP: BARKER,PHILLIP
+  BARKS,CARL: BARKS,CARL
+  ΜΠΑΡΛΑΣ,ΦΑΙΔΡΟΣ: ΜΠΑΡΛΑΣ,ΦΑΙΔΡΟΣ
+  ΜΠΑΡΜΠΑ,ΒΑΣΟΥ: ΜΠΑΡΜΠΑΣ,ΒΑΣΟΣ
+  ΜΠΑΡΜΠΑΣ ΒΑΣΟΣ: ΜΠΑΡΜΠΑΣ,ΒΑΣΟΣ
+  ΜΠΑΡΜΠΗΣ,ΚΩΣΤΑΣ: ΜΠΑΡΜΠΗΣ,ΚΩΣΤΑΣ
+  BARNARD & EDWARDS: BARNARD,JOHN,DARRELL!!EDWARDS,LONNIE,J.
+  BARNES,JONATHAN: BARNES,JONATHAN
+  BARNES,JULIAN: BARNES,JULIAN
+  ΜΠΑΡΝΕΤ,Φ.: HODGSON BURNETT,FRANCES
+  ΜΠΑΡΝΕΤ,ΜΑΚ-ΤΖΟΡΙ,ΤΖΟΝ: JORY,JOHN!!BARNETT,MAC
+  ΜΠΑΡΝΣ,ΤΖΟΥΛΙΑΝ: BARNES,JULIAN
+  ΜΠΑΡΟ, ΡΟΥΝΤΟΛΦ: BAHRO,RUDOLPH
+  BARON A: BARON,AUGUSTE
+  ΜΠΑΡΟΥΤΣΟΥ,ΓΕΩΡΓΙΟΥ: ΜΠΑΡΟΥΤΣΟΣ,ΓΕΩΡΓΙΟΣ
+  BARRAL,XAVIER: BARRAL,XAVIER
+  BARROWS,MARJORIE: BARROWS,MARJORIE
+  ΜΠΑΡΡΥ,ΜΠΡΟΥΝΟΝΙΑ: BARRY,BRUNONIA
+  ΜΠΑΡΤ,ΣΒΑΡΤΣ: SCHWARZ-BART,ANDRÉ
+  BARTH PAUL: BARTH,PAUL
+  ΜΠΑΡΘΕΛΟ,ΕΛΙΑ: BARCELÓ,ELIA
+  BARTHOLDN KARL: MENDELSSOHN BARTHOLDY,KARL
+  ΜΠΑΡΤΣΙΩΤΗΣ,ΠΑΝΑΓΙΩΤΗΣ: ΜΠΑΡΤΣΙΩΤΗΣ,ΠΑΝΑΓΙΩΤΗΣ
+  ΜΠΑΡΤΖΩΚΑΣ ΚΙΜΩΝ: ΜΠΑΡΤΖΩΚΑΣ,ΚΙΜΩΝΑΣ
+  ΜΠΑΡΤΖΩΚΑΣ,ΚΙΜΩΝ: ΜΠΑΡΤΖΩΚΑΣ,ΚΙΜΩΝΑΣ
+  ΜΠΑΡΤΖΩΚΑΣ,ΚΙΜΩΝΑΣ: ΜΠΑΡΤΖΩΚΑΣ,ΚΙΜΩΝΑΣ
+  ΜΠΑΡΤΖΟΠΟΥΛΟΣ,ΔΗΜΗΤΡΗΣ: ΜΠΑΡΤΖΟΠΟΥΛΟΣ,ΔΗΜΗΤΡΗΣ
+  ΜΠΑΡΖΟΥΚΑ,ΤΑΣΟ: ΜΠΑΡΖΟΥΚΑΣ,ΤΑΣΟΣ
+  ΜΠΑΣΔΕΚΗΣ,ΓΙΩΡΓΟΣ: ΜΠΑΣΔΕΚΗΣ,ΓΙΩΡΓΟΣ
+  ΜΠΑΣΙΑΚΟΣ ΙΩΑΝΝΗΣ: ΜΠΑΣΙΑΚΟΣ,ΙΩΑΝΝΗΣ
+  BASS,J: BASS,J.
+  BASSETT,BRUCE: BASSETT,BRUCE
+  ΜΠΑΣΤΑ,ΕΥΣΤΑΘΙΟΥ: ΜΠΑΣΤΑΣ,ΕΥΣΤΑΘΙΟΣ
+  ΜΠΑΣΤΑΝΗΣ,ΠΑΝΑΓΙΩΤΗΣ: ΜΠΑΣΤΑΝΗΣ,ΠΑΝΑΓΙΩΤΗΣ
+  BATIFFOL,HENRI: BATIFFOL,HENRI
+  ΜΠΑΤΡΙΝΟΣ: ΜΠΑΤΡΙΝΟΣ,ΜΕΝΕΛΑΟΣ
+  ΜΠΑΤΡΙΝΟΣ,Μ: ΜΠΑΤΡΙΝΟΣ,ΜΕΝΕΛΑΟΣ
+  BATSALIA,FRIEDERIKE: BATSALIA,FRIEDERIKE
+  ΜΠΑΤΣΗ,ΔΗΜ: ΜΠΑΤΣΗΣ,ΔΗΜΗΤΡΙΟΣ
+  ΜΠΑΤΣΙΚΑΝΗΣ,ΝΙΚΟΣ: ΜΠΑΤΣΙΚΑΝΗΣ,ΝΙΚΟΣ
+  BAUD,FRANCIS: BAUD,FRANCIS
+  BAUDELAIRE CHARLES: BAUDELAIRE,CHARLES
+  BAUDIN LOUIS: BAUDIN,LOUIS
+  BAUMGARTEN-POLAND-WAGNER: BAUMGARTEN,FRITZ!!WAGNER,RICHARD,ANTON!!POLAND,FRANZ
+  ΜΠΑΞΕΡ,ΝΟΕΛ: ΜΠΑΞΕΡ,ΝΟΕΛ
+  BAYET C: BAYET,CHARLES,MARIE ADOLPHE LOUIS
+  ΜΠΑΖΑΙΟΣ, ΚΩΣΤΑΣ: ΜΠΑΖΑΙΟΣ,ΚΩΣΤΑΣ
+  ΜΠΑΖΕΝ,ΕΡΒΕ: BAZIN,HERVÉ
+  ΜΠΑΖΙΛΙ,Κ.Μ: BAZILI,KONSTANTIN,M.
+  BEAUX,JEAN: BEAUX,JEAN
+  BEAYFRE: BEAUFRE,ANDRE
+  BEECHER,E.R.: BEECHER,E.,R.
+  BEER-POITEVIN,G.: BEER-POITEVIN,F.
+  ΜΠΕΓΚΕΧΟΛΝΤ,ΜΠΕΤΙ: BOEGEHOLD,BETTY
+  ΜΠΕΓΖΟΣ,ΜΑΡΙΟΣ: ΜΠΕΓΖΟΣ,ΜΑΡΙΟΣ
+  BEHRENDT RICHARD: BEHRENDT,RICHARD
+  ΜΠΕΙΝΜΠΡΙΤΖ,ΜΠΕΡΙΛ: BAINBRIDGE,BERYL
+
+  ΜΠΕΙΟΓΛΟΥ,ΚΥΡΙΑΚΗ: ΜΠΕΙΟΓΛΟΥ,ΚΥΡΙΑΚΗ
+  BEISSIER,F: BEISSIER,FERNAND
+  ΜΠΕΚ,ΠΕΤΕΡ: BECK,PETER
+  ΜΠΕΚΑΤΩΡΟΣ,ΓΕΩΡΓΙΟΣ: ΜΠΕΚΑΤΩΡΟΣ,ΓΕΩΡΓΙΟΣ
+  ΜΠΕΚΑΤΩΡΟΣ,ΣΤΕΦΑΝΟΣ: ΜΠΕΚΑΤΩΡΟΣ,ΣΤΕΦΑΝΟΣ
+  ΜΠΕΚΕ,ΟΜΗΡΟΥ: ΜΠΕΚΕΣ,ΟΜΗΡΟΣ
+  BEKGTSON HERMANN: BENGTSON,HERMANN
+  ΜΠΕΚΟΣ ΔΙΟΝΥΣΙΟΣ: ΜΠΕΚΟΣ,ΔΙΟΝΥΣΙΟΣ
+  ΜΠΕΚΤΑΣ,ΧΑΜΠΙΠ: BEKTAS,HABIB
+  ΜΠΕΛ,Χ-ΚΟΠΕΛΕΒ,Λ-ΦΟΡΜΒΕΓΚ,Χ: BÖLL,HEINRICH!!KOPELEV,LEV,ZALMANOVICH (ZINOVYEVICH)!!VORMWEG,HEINRICH
+  ΜΠΕΛ,ΧΑΙΝΡΙΧ: BÖLL,HEINRICH
+  ΜΠΕΛΑΝΤΗΣ,ΔΗΜΗΤΡΙΟΣ: ΜΠΕΛΑΝΤΗΣ,ΔΗΜΗΤΡΙΟΣ
+  ΜΠΕΛΑΝΤΗΣ,ΔΗΜΗΤΡΗΣ: ΜΠΕΛΑΝΤΗΣ,ΔΗΜΗΤΡΙΟΣ
+  ΜΠΕΛΙΑ,ΕΛΕΝΗ Δ: ΜΠΕΛΙΑ,ΕΛΕΝΗ,Δ.
+  ΜΠΕΛΙΑΕΦ,ΝΙΚΩΝΟΣ ΟΣΙΟΥ ΣΤΑΡΕΤΣ: ΜΠΕΛΙΑΕΦ,ΟΣΙΟΣ ΣΤΑΡΕΤΣ ΝΙΚΩΝ
+  ΜΠΕΛΙΕΣ,ΕΡΡΙΚΟΣ: ΜΠΕΛΙΕΣ,ΕΡΡΙΚΟΣ
+  ΜΠΕΛΙΤΣΟΣ,ΘΕΟΔ.: ΜΠΕΛΙΤΣΟΣ,ΘΕΟΔΩΡΟΣ
+  ΜΠΕΛΛ,ΧΑΙΝΡΙΧ: BÖLL,HEINRIC
+  ΜΠΕΛΛΟΣ,ΚΩΝ/ΝΟΣ: ΜΠΕΛΛΟΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
+  ΜΠΕΛΛΟΥ,ΚΩΝΣΤΑΝΤΙΝΟΥ: ΜΠΕΛΛΟΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
+  BELOCH JULIUS: BELOCH,KARL,JULIUS
+  BELOCH KARL: BELOCH,KARL,JULIUS
+  ΜΠΕΛΟΓΙΑΝΝΗΣ,ΝΙΚΟΣ: ΜΠΕΛΟΓΙΑΝΝΗΣ,ΝΙΚΟΣ
+  ΜΠΕΛΟΟΥΣΟΒΑ,ΛΙΛΙΑ: BELOUSOVA,LILIA
+  BELOT EMILE: BELOT,EMILE
+  ΜΠΕΛΤΟΝ,ΤΖΩΝ: BELTON,JOHN
+  ΜΠΕΝΑΣ,ΤΑΚΗΣ: ΜΠΕΝΑΣ,ΤΑΚΗΣ
+  ΜΠΕΝΑΤΣΗΣ ΑΠΟΣΤΟΛΟΣ: ΜΠΕΝΑΤΣΗΣ,ΑΠΟΣΤΟΛΟΣ
+  BENDALL,SIMON: BENDALL,SIMON
+  BENDIXEN F: BENDIXEN,FRIEDRICH
+  ΜΠΕΝΕΚΟΥ,ΓΙΑΝΝΗ: ΜΠΕΝΕΚΟΣ,ΓΙΑΝΝΗΣ
+  BENES EDOUARD: BENES,EDOUARD
+  ΜΠΕΝΓΙΑΜΙΝ,ΒΑΛΤΕΡ: BENJAMIN,WALTER, BENDIX SCHÖNFLIES
+  ΜΠΕΝΓΚΤΣΟΝ,ΧΕΡΜΑΝ: BENGTSON,HERMANN
+  BENGRSON HERMANN: BENGTSON,HERMANN
+  BENGTSON HERMANN: BENGTSON,HERMANN
+  ΜΠΕΝΓΤΣΟΝ,ΧΕΡΜΑΝ: BENGTSON,HERMANN
+  ΜΠΕΝΙ,ΣΤΕΦΑΝΟ: BENNI,STEFANO
+  BENSON,MARY: BENSON,MARY
+  ΜΠΕΝΤΙΛΛΑ,ΕΛΕΝΗ: ΜΠΕΝΤΙΛΛΑ,ΕΛΕΝΗ
+  ΜΠΕΝΤΙΤ,ΚΟΝ: COHN-BENDIT,GABRIEL
+  BENTON,MIKE: BENTON,MIKE
+  BER HANS: GERBER,HANS
+  BER HUGO: BERGER,ERNST,HUGO
+  ΜΠΕΡ,ΜΑΞ: BEER,MAX
+  BERARD JEAN: BÉRARD,JEAN
+  BERARO VICTOR: BÉRARD,VICTOR
+  ΜΠΕΡΑΤΗ,ΘΕΟΔΩΡΟΥ: ΜΠΕΡΑΤΗΣ,ΘΕΟΔΩΡΟΣ
+  ΜΠΕΡΑΤΗΣ,ΓΙΑΝΝΗΣ: ΜΠΕΡΑΤΗΣ,ΓΙΑΝΝΗΣ
+  ΜΠΕΡΑΤΗΣ,ΘΕΟΔΩΡΟΣ: ΜΠΕΡΑΤΗΣ,ΘΕΟΔΩΡΟΣ
+  ΜΠΕΡΔΕΚΛΗ,ΓΕΩΡΓΙΟΥ: ΜΠΕΡΔΕΚΛΗΣ,ΓΕΩΡΓΙΟΣ
+  ΜΠΕΡΓΑΜΙΝΙ,ΝΤΕΙΒΙΝΤ: BERGAMINI,DAVID
+  ΜΠΕΡΓΕΛΕΣ,ΝΙΚΟΣ: ΜΠΕΡΓΕΛΕΣ,ΝΙΚΟΣ
+  BERGK THEODOR: BERGK,THEODOR
+  ΜΠΕΡΓΚΜΑΝ,ΙΝΓΚΜΑΡ: BERGMAN,INGMAR
+  BERGSON HENDRI: BERGSON,HENRI
+  BERGSON,HENRI: BERGSON,HENRI
+  BERLIN,RICHARD: BERLIN,RICHARD
+  ΜΠΕΡΛΙΝΓΚ,ΠΕΤΕΡ: BERLING,PETER
+  ΜΠΕΡΛΙΝΓΚΟΥΕΡ,ΕΝΡΙΚΟ: BERLINGUER,ENRICO
+  BERLITZ,CHARLES: BERLITZ,CHARLES
+  ΜΠΕΡΝ,Α.Δ: BURN,ANDREW,ROBERT
+  ΜΠΕΡΝ,Α.Ρ: BURN,ANDREW,ROBERT
+  ΜΠΕΡΝ,ΕΡΙΚ: BERNE,ERIC
+  BERNARDO,JOSE-RAUL: BERNARDO,JOSE-RAUL
+  BERNE HELMUT: BERNE,HELMUT
+  ΜΠΕΡΝΕΤ,ΓΟΥΙΛΙΑΜ: BURNETT,WILLIAM
+  BERNOYLLI ZZ: BERNOULLI,JOHANN,JACOB
+  ΜΠΕΡΝΤ,ΛΟΥΙΖΑ: BIRD,LOIS
+  BERRY,JOY: BERRY,JOY
+  BERTINO,SERGE: BERTINO,SERGE
+  ΜΠΕΡΤΩ,ΣΙΜΟΝ: BERTHEAU,SIMONE
+  BERVE HELMUT: BERVE,HELMUT
+  BERVE HELMYT: BERVE,HELMUT
+  ΜΠΕΣΜΠΕΑΣ,ΣΤΑΥΡΟΣ: ΜΠΕΣΜΠΕΑΣ,ΣΤΑΥΡΟΣ
+  BESNIER MAURICE: BESNIER,MAURICE
+  ΜΠΕΤΕΛΕΜ,ΣΑΡΛ: BETTELHEIM,CHARLES
+  BETHMANN-HOLLWEG TH: VON BETHMANN HOLLWEG,THEOBALD
+  ΜΠΕΤΣΑΣ,ΓΙΑΝΝΗΣ: ΜΠΕΤΣΑΣ,ΓΙΑΝΝΗΣ
+  BETSIS ANDREW: BETSIS,ANDREW
+  ΜΠΕΤΤΕΛΕΜ ΣΑΡΛ: BETTELHEIM,CHARLES
+  ΜΠΕΤΤΕΛΕΜ,ΣΑΡΛ: BETTELHEIM,CHARLES
+  BETTELHEIM CH: BETTELHEIM,CHARLES
+  BETTELHEIM CR: BETTELHEIM,CHARLES
+  ΜΠΕΤΤΗ,ΣΤΕΦΑΝΟΥ: ΜΠΕΤΤΗΣ,ΣΤΕΦΑΝΟΣ
+  ΜΠΕΤΤΗΣ,ΣΤΕΦΑΝΟΣ: ΜΠΕΤΤΗΣ,ΣΤΕΦΑΝΟΣ
+  BETTLEHEIM,CH.: BETTELHEIM,CHARLES
+  BEUS,J.G: BEUS,JACOBUS,GIJSBERTUS DE
+  ΜΠΕΒΙΛΑΚΟΥΑ,ΑΛΜΠΕΡΤΟ: BEVILACQUA,ALBERTO
+  ΜΠΙΧΕΛ,ΠΑΟΥΛ: BIEGEL,PAUL
+  BIEFWELD,HORST: BIEFWELD,HORST
+  ΜΠΙΛΑΛΗΣ,ΣΠΥΡΙΔΩΝ: ΜΠΙΛΑΛΗΣ,ΣΠΥΡΙΔΩΝ
+  BILLETDOUX,RAPHAELE: BILLETDOUX,RAPHAËLE
+  ΜΠΙΝΑΡΔΟΠΟΥΛΟΥ,ΝΤΙΝΟΥ: ΜΠΙΝΑΡΔΟΠΟΥΛΟΣ,ΝΤΙΝΟΣ
+  ΜΠΙΝΙΑΡΗ,ΓΚΙΚΑ: ΜΠΙΝΙΑΡΗΣ,ΓΚΙΚΑΣ
+  ΜΠΙΝΙΑΡΗΣ,ΓΚΙΚΑΣ: ΜΠΙΝΙΑΡΗΣ,ΓΚΙΚΑΣ
+  ΜΠΙΝΙΟΥ,ΑΘΗΝΑ: ΜΠΙΝΙΟΥ,ΑΘΗΝΑ
+  ΜΠΙΝΤΣΥ,ΜΕΗΒ: BINCHY,MAEVE
+  BIOT,R.: BIOT,RENÉ
+  ΜΠΙΟΤ,ΡΕΝΕ: BIOT,RENÉ
+  ΜΠΙΟΥΜΠΙ ΦΡΙΝΤΑ: ΜΠΙΟΥΜΠΙ,ΦΡΙΝΤΑ
+  ΜΠΙΡΓΚΕΓΚΟΡ,ΜΙΚΚΕΛ: BIRKEGAARD,MIKKEL
+  ΜΠΙΡΚΑ,ΚΩΣΤΑ: ΜΠΙΡΚΑΣ,ΚΩΣΤΑΣ
+  ΜΠΙΡΜΑΝ ΦΡΑΝΤΖΙΣΚΑ: BIERMANN,FRANZISKA
+  ΜΠΙΡΜΑΝ,ΦΡΑΝΤΣΙΣΚΑ: BIERMANN,FRANZISKA
+  ΜΠΙΡΜΠΙΛΗ ΕΛΕΝΗ: ΜΠΙΡΜΠΙΛΗ,ΕΛΕΝΗ
+  ΜΠΙΡΜΠΙΛΗ,ΕΛΕΝΗ: ΜΠΙΡΜΠΙΛΗ,ΕΛΕΝΗ
+  ΜΠΗΡΣ ΑΜΠΡΟΟΥΖ: BIERCE,AMBROSE
+  BIRT THEODOR: BIRT,THEODOR
+  BISCOTTI,BARBARA: BISCOTTI,BARBARA
+  ΜΠΙΣΚΑ-ΚΑΡΑΚΑΣΙΔΟΥ,ΑΝΝΑ: ΜΠΙΣΚΑ-ΚΑΡΑΚΑΣΙΔΟΥ,ΑΝΝΑ
+  BISMUTH,HENRI-CASAING,DENIS: BISMUTH,HENRI!!CASΤAING,DENIS
+  ΜΠΙΣΟΠ,ΜΑΡΚ: BISHOP,MARK
+  ΜΠΙΣΤΗΣ ΝΙΚΟΣ: ΜΠΙΣΤΗΣ,ΝΙΚΟΣ
+  ΜΠΙΣΤΟΛΑ-ΠΛΑΣΤΟΥΡΓΟΥ,ΦΩΤΙΚΑ: ΜΠΙΣΤΟΛΑ-ΠΛΑΣΤΟΥΡΓΟΥ,ΦΩΤΙΚΑ
+  ΜΠΙΘΑ,ΙΩΑΝΝΑ-ΧΑΤΖΗΔΑΚΗΣ,ΜΑΝΟΛΗΣ: ΜΠΙΘΑ,ΙΩΑΝΝΑ!!ΧΑΤΖΗΔΑΚΗΣ,ΜΑΝΟΛΗΣ
+  ΜΠΙΤΣΑΚΗ,ΕΥΤΥΧΗ: ΜΠΙΤΣΑΚΗΣ,ΕΥΤΥΧΗΣ,Ι.
+  ΜΠΙΤΣΑΚΗ,ΕΥΤΥΧΗ Ι.: ΜΠΙΤΣΑΚΗΣ,ΕΥΤΥΧΗΣ,Ι.
+  ΜΠΙΤΣΑΚΗΣ,ΕΥΤΥΧΗΣ: ΜΠΙΤΣΑΚΗΣ,ΕΥΤΥΧΗΣ,Ι.
+  BJORK,SAMUEL: BJORK,SAMUEL
+  ΜΠΛΑΧΟΥΡΑ,ΚΩΝΣΤΑΝΤΙΝΟΥ: ΜΠΛΑΧΟΥΡΑΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ,.ΧΡ.
+  ΜΠΛΑΧΟΥΡΑΣ,ΚΩΝ: ΜΠΛΑΧΟΥΡΑΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ,.ΧΡ.
+  ΜΠΛΑΧΟΥΡΑΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ.ΧΡ: ΜΠΛΑΧΟΥΡΑΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ,.ΧΡ.
+  BLACKBURN,SIMON: BLACKBURN,SIMON
+  BLACKIE,DUNCAN: BLACKIE,DUNCAN
+  BLACKMORE,SUSAN: BLACKMORE,SUSAN
+  ΜΠΛΑΙΤΟΝ,ΕΝΙΝΤ: BLYTON,ENID
+  ΜΠΛΑΚ,ΜΠΕΝΤΖΑΜΙΝ: BLACK,BENJAMIN
+  ΜΠΛΑΝΑ,ΓΕΩΡΓΙΟΥ: ΜΠΛΑΝΑΣ,ΓΙΩΡΓΟΣ
+  ΜΠΛΑΝΑΣ , ΓΙΩΡΓΟΣ: ΜΠΛΑΝΑΣ,ΓΙΩΡΓΟΣ
+  ΜΠΛΑΝΑΣ ΓΙΩΡΓΟΣ: ΜΠΛΑΝΑΣ,ΓΙΩΡΓΟΣ
+  BLANC ANDRE: BLANC,ANDRE
+  BLASS FRIEDRICH: BLASS,FRIEDRICH
+
+  BLAVATSKAJA-COLYBCOVA-PAVLOVSKAJA: BLAVATSKAJA,TATJANA,V.!!GOLUBCOVA,ELENA,S.!!PAVLOVSKAJA,ALEKSANDRA,I.
+  ΜΠΛΕΤΑΣ,ΑΝΑΣΤΑΣΙΟΣ: ΜΠΛΕΤΑΣ,ΑΝΑΣΤΑΣΙΟΣ
+  ΜΠΛΕΤΑΣ,ΤΑΣΟΣ: ΜΠΛΕΤΑΣ,ΤΑΣΟΣ
+  ΜΠΛΙΞΕΝ,ΚΑΡΕΝ: BLIXEN,KAREN
+  BLOCH GUSTAVE: BLOCH,GUSTAVE
+  BLOCH IWAN: BLOCH,IWAN
+  BLOCH MARC: BLOCH,MARC
+  BLOCH PAYMOND: BLOCH,RAYMOND
+  BLOCH RAUMOND: BLOCH,RAYMOND
+  BLOCH RAYMOND-COYSIN JEAN: BLOCH,RAYMOND!!COUSIN,JEAN
+  BLOCK,LAWRENCE: BLOCK,LAWRENCE
+  ΜΠΛΟΚ,ΛΟΡΕΝΣ: BLOCK,LAWRENCE
+  ΜΠΛΟΥΜ,ΤΖΟΥΝΤΙ: BLOOM,JUDY
+  BLYMENTHAL ALBERT: BLUMENTHAL,ALBERT,H.
+  BLYTON,ENID: BLYTON,ENID
+  BLYTON,ERID: BLYTON,ENID
+  BOARDMAN,JOHN: BOARDMAN,JOHN
+  BOBIN,ROBERT: BOBIN,ROBERT
+  BOEHRIN ERICH: BOEHRIN,ERICH
+  ΜΠΟΓΙΟΠΟΥΛΟΣ,ΝΙΚΟΣ: ΜΠΟΓΙΟΠΟΥΛΟΣ,ΝΙΚΟΣ
+  ΜΠΟΓΚΑ,ΕΥΑΓΓΕΛΟΥ: ΜΠΟΓΚΑΣ,ΕΥΑΓΓΕΛΟΣ
+  BOHCKH AUGUST: BÖCKH,AUGUST
+  BOHLER, BING: BOHLER,BING
+  BOHM-BAWERK: VON BÖHM-BAWERK,EUGEN
+  ΜΠΟΚΟΓΙΑΝΝΗΣ ΧΡΥΣΟΣΤΟΜΟΣ: ΜΠΟΚΟΓΙΑΝΝΗΣ,ΧΡΥΣΟΣΤΟΜΟΣ
+  ΜΠΟΚΟΓΙΑΝΝΗΣ,ΧΡΥΣΟΣΤΟΜΟΣ: ΜΠΟΚΟΓΙΑΝΝΗΣ,ΧΡΥΣΟΣΤΟΜΟΣ
+  ΜΠΟΚΟΒΟΣ,ΠΑΝΑΓΙΩΤΗΣ: ΜΠΟΚΟΒΟΣ,ΠΑΝΑΓΙΩΤΗΣ
+  ΜΠΟΚΟΒΟΥ,ΠΑΝ.: ΜΠΟΚΟΒΟΣ,ΠΑΝΑΓΙΩΤΗΣ
+  ΜΠΟΚΟΒΟΥ,ΠΑΝΑΓΙΩΤΗ: ΜΠΟΚΟΒΟΣ,ΠΑΝΑΓΙΩΤΗΣ
+  ΜΠΟΚΟΒΟΥ,ΠΑΝΑΓΙΩΤΟΥ: ΜΠΟΚΟΒΟΣ,ΠΑΝΑΓΙΩΤΗΣ
+  ΜΠΟΛΕΤΣΗΣ ΣΤΕΦΑΝΟΣ: ΜΠΟΛΕΤΣΗΣ,ΣΤΕΦΑΝΟΣ
+  BOLLACK JEAN: BOLLACK,JEAN
+  BOLTON,JOHN: BOLTON,JOHN
+  BOMMELAER JEAN: BOMMELAER,JEAN
+  ΜΠΟΜΠΑΣ,ΛΕΩΝΙΔΑΣ: ΜΠΟΜΠΑΣ,ΛΕΩΝΙΔΑΣ
+  ΜΠΟΜΠΕΝ,ΚΡΙΣΤΙΑΝ: BOBIN,CHRISTIAN
+  BOMPOIS FERDIANAND: BOMPOIS,FERDINAND
+  ΜΠΟΜΠΟΛΗ,ΧΡΥΣΑΥΓΗ: ΜΠΟΜΠΟΛΗ,ΧΡΥΣΑΥΓΗ
+  ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ: ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
+  ΜΠΟΝΑΡ,ΑΝΤΡΕ: BONNARD,ANDRÉ
+  ΜΠΟΝΗ,ΚΩΝ.: ΜΠΟΝΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
+  ΜΠΟΝΗ,ΚΩΝΣΤΑΝΤΙΝΟΥ: ΜΠΟΝΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
+  ΜΠΟΝΗΣ ΚΩΝ/ΝΟΣ: ΜΠΟΝΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
+  BONIS KONSTANTIN: ΜΠΟΝΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
+  ΜΠΟΝΗΣ ΚΩΝΣΤΑΝΤΙΝΟΣ: ΜΠΟΝΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
+  ΜΠΟΝΗΣ,ΚΩΝ/ΝΟΣ: ΜΠΟΝΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
+  BONNARD ANDRE: BONNARD,ANDRÉ
+  ΜΠΟΝΟΥ,Β.Ν.: ΜΠΌΝΟΣ,Β.,Ν.
+  ΜΠΩΝΤΛΑΙΡ,ΣΑΡΛ: BAUDELAIRE,CHARLES
+  BORDER,ROSEMARY: BORDER,ROSEMARY
+  BORGEAUD WILLY: BORGEAUD,WILLY
+  BORNECOUE HENRI: BORNECQUE,HENRI
+  ΜΠΟΡΝΤΟΝΣ,ΠΑΛΟΜΑ: BORDONS,PALOMA
+  ΜΠΟΡΟΒΙΤΣ,ΜΙΣΕΛ:  BORWICZ,MICHEL
+  ΜΠΟΡΟΒΣΚΙ,ΤΑΝΤΕΟΥΣ: BOROWSKI,TADEUSZ
+  ΜΠΩΣΑΝ,ΚΛΩΝΤΙΝ: BEAUSSANT,CLAUDINE
+  BOSCH GLEMENS: BOSCH,CLEMENS
+  BOSE,PARTHA: BOSE,PARTHA
+  ΜΠΟΣΗ,ΚΩΣΤΑ: ΜΠΟΣΗΣ,ΚΩΣΤΑΣ
+  ΜΠΩΣΩ,ΑΝΡΥ: BAUCHAU,HENRY
+  BOSQUET,MICHEL: BOSQUET,MICHEL
+  BOSSET,C.P.: BOSSET,C.,P.
+  ΜΠΟΣΤ: ΒΟΣΤΑΝΤΖΌΓΛΟΥ,ΧΡΎΣΑΝΘΟΣ@ΜΈΝΤΗΣ ΜΠΟΣΤΑΝΤΖΌΓΛΟΥ Ή ΜΠΟΣΤ
+  BOTH KARL: BOTH,KARL
+  ΜΠΟΤΣΑΡΗ,ΜΑΡΚΟΥ: ΜΠΟΤΣΑΡΗΣ,ΜΑΡΚΟΣ
+  ΜΠΟΤΣΑΡΗ,ΝΟΤΗ: ΜΠΟΤΣΑΡΗΣ,ΝΟΤΗΣ
+  ΜΠΟΤΣΑΡΗΣ ΝΟΤΗΣ: ΜΠΟΤΣΑΡΗΣ,ΝΟΤΗΣ
+  ΜΠΟΤΣΑΡΗΣ,ΔΗΜ  ΝΟΤΗ: ΜΠΟΤΣΑΡΗΣ,ΔΗΜΗΤΡΙΟΣ,ΝΟΤΗ
+  ΜΠΟΤΣΑΡΗΣ,ΔΗΜ Τ ΝΟΤΗ: ΜΠΟΤΣΑΡΗΣ,ΔΗΜΗΤΡΙΟΣ,Τ. ΝΟΤΗ
+  ΜΠΟΤΣΑΡΗΣ,ΔΗΜ.Τ.ΝΟΤΗ: ΜΠΟΤΣΑΡΗΣ,ΔΗΜΗΤΡΙΟΣ,Τ. ΝΟΤΗ
+  BOUCARD,ROBERT: BOUCARD,ROBERT
+  BOUCHE-LEGLERGO A: BOUCHE-LECLERCQ,AUGUSTE
+  BOUET,M: BOUET,M.!!VALLIN,J.
+  ΜΠΟΥΦΙΔΗ,Ν.ΧΑΓΕΡ: ΜΠΟΥΦΙΔΗΣ,ΧΑΓΕΡ
+  ΜΠΟΥΦΙΔΗΣ ΒΑΣΙΛΗΣ: ΜΠΟΥΦΙΔΗΣ,ΒΑΣΙΛΗΣ
+  ΜΠΟΥΦΙΔΗΣ,ΧΑΓΕΡ: ΧΆΓΕΡ-ΜΠΟΥΦΊΔΗΣ,ΝΊΚΟΣ
+  ΜΠΟΥΚΟΦΣΚΙ,ΤΣΑΡΛΣ: BUKOWSKI,HENRY CHARLES
+
+  ΜΠΟΥΛΑΛΑ,ΚΛΕΑΝΘΟΥΣ: ΜΠΟΥΛΑΛΆΣ,ΚΛΕΆΝΘΗΣ,Κ.
+  ΜΠΟΥΛΓΚΑΚΩΦ Μ.: BULGAKOV,MIKHAIL
+  ΜΠΟΥΛΩΤΗΣ,ΧΡΗΣΤΟΣ: ΜΠΟΥΛΩΤΗΣ,ΧΡΗΣΤΟΣ
+  ΜΠΟΥΛΟΥΤΖΑΣ,ΑΝΤΩΝΗΣ: ΜΠΟΥΛΟΥΤΖΑΣ,ΑΝΤΩΝΗΣ
+  ΜΠΟΥΜΗ,ΡΙΤΑ: ΜΠΟΥΜΗ,ΡΙΤΑ
+  ΜΠΟΥΜΗ-ΒΓΟΝΤΖΑ ΟΛΓΑ: ΜΠΟΥΜΗ-ΒΓΟΝΤΖΑ,ΟΛΓΑ
+  ΜΠΟΥΜΠΟΥΓΙΑΤΖΗ,ΕΥΑΓΓΕΛΙΑ: ΜΠΟΥΜΠΟΥΓΙΑΤΖΗ,ΕΥΑΓΓΕΛΙΑ
+  ΜΠΟΥΜΠΟΥΛΙΔΟΥ ΓΛΥΚΕΡΙΑ: ΜΠΟΥΜΠΟΥΛΙΔΟΥ,ΓΛΥΚΕΡΙΑ
+  ΜΠΟΥΝΙΑΣ,ΑΛΚΙΝΟΟΣ: ΜΠΟΥΝΙΑΣ,ΑΛΚΙΝΟΟΣ
+  ΜΠΟΥΝΙΟΥΕΛ,ΛΟΥΙΣ: BUÑUEL,LUIS
+  ΜΠΟΥΡΑΝΤΑ,ΔΗΜΗΤΡΙΟΥ: ΜΠΟΥΡΑΝΤΑΣ,ΔΗΜΗΤΡΗΣ
+  ΜΠΟΥΡΑΝΤΑΣ,ΑΠΟΣΤΟΛΟΣ: ΜΠΟΥΡΑΝΤΑΣ,ΑΠΟΣΤΟΛΟΣ
+  ΜΠΟΥΡΑΝΤΑΣ,ΔΗΜΗΤΡΗΣ: ΜΠΟΥΡΑΝΤΑΣ,ΔΗΜΗΤΡΗΣ
+  ΜΠΟΥΡΑΝΤΑΣ,ΛΑΜΠΡΟΣ Κ: ΜΠΟΥΡΑΝΤΑΣ,ΛΑΜΠΡΟΣ,Κ
+  ΜΠΟΥΡΑΟΥΙ,ΝΙΝΑ: BOURAOUI,NINA
+  ΜΠΟΥΡΑΣ,ΠΑΝΑΓΙΩΤΗΣ: ΜΠΟΥΡΑΣ,ΠΑΝΑΓΙΩΤΗΣ
+  ΜΠΟΥΡΑΣ,ΒΑΣΙΛΗΣ: ΜΠΟΥΡΑΣ,ΒΑΣΙΛΗΣ
+  ΜΠΟΥΡΑΖΕΡΗ,ΝΙΚΟΛΑΟΥ: ΜΠΟΥΡΑΖΕΡΗΣ,ΝΙΚΟΛΑΟΣ
+  ΜΠΟΥΡΑΖΟΠΟΥΛΟΥ,ΙΩΑΝΝΑ: ΜΠΟΥΡΑΖΟΠΟΥΛΟΥ,ΙΩΑΝΝΑ
+  ΜΠΟΥΡΓΟΣ,ΗΛΙΑΣ-ΓΑΤΑ.ΣΤΑΥΡΟΥΛΑ: ΜΠΟΥΡΓΟΣ,ΗΛΙΑΣ!!ΓΑΤΑ,ΣΤΑΥΡΟΥΛΑ
+  # https://www.dancearchive.gr/article.php?id=14
+  ΜΠΟΥΡΗΣ. ΣΤΑΥΡΟΠΟΥΛΟΣ. ΤΕΝΤΖΕΡΑΚΗΣ: ΠΑΠΆ-ΣΈΒΟΥ,ΜΊΚΑ!!ΜΠΟΎΡΗΣ,ΑΝΔΡΈΑΣ!!ΣΤΑΥΡΌΠΟΥΛΟΣ,ΛΕΥΤΈΡΗΣ!!ΤΕΝΤΖΕΡΆΚΗΣ,ΧΡΉΣΤΟΣ
+  ΜΠΟΥΡΙΤΣΑ ΜΟΥΖΑΚΗ ΕΛΕΝΗ: ΜΟΥΖΑΚΗ-ΜΠΟΥΡΙΤΣΑ,ΕΛΕΝΗ
+  ΜΠΟΥΡΛΟΣ,ΓΙΩΡΓΟΣ: ΜΠΟΥΡΛΟΣ,ΓΙΩΡΓΟΣ
+  BOURNIER,ISABELLE: BOURNIER,ISABELLE
+  ΜΠΟΥΡΟΠΟΥΛΟΣ,Λ.: ΜΠΟΥΡΟΠΟΥΛΟΣ,ΑΓΓΕΛΟΣ,ΝΙΚ.
+  ΜΠΟΥΡΟΠΟΥΛΟΥ,ΑΓΓΕΛΟΥ: ΜΠΟΥΡΟΠΟΥΛΟΣ,ΑΓΓΕΛΟΣ,ΝΙΚ.
+  ΜΠΟΥΣΧΟΤΕΝ,ΡΙΚΗ ΒΑΝ: ΒΑΝ ΜΠΟΥΣΧΟΤΕΝ,ΡΙΚΗ
+  ΜΠΟΥΣΙΑ,ΧΑΡΑΛΑΜΠΟΥΣ: ΜΠΟΎΣΙΑΣ,ΧΑΡΆΛΑΜΠΟΣ,Μ.
+  ΜΠΟΥΣΙΑΣ ΠΑΝΑΓΙΩΤΗΣ: ΜΠΟΥΣΙΑΣ,ΠΑΝΑΓΙΩΤΗΣ
+  ΜΠΟΥΣΚΑΛΙΑ ΛΕΟ: BUSCAGLIA,LEO
+  ΜΠΟΥΣΚΑΛΙΑ,ΛΕΟ: BUSCAGLIA,LEO
+  ΜΠΟΥΣΜΠΟΥΡΕΛΗ,ΜΑΙΡΗ: ΜΠΟΥΣΜΠΟΥΡΕΛΗ,ΜΑΙΡΗ
+  BOUSOUET BERNARD: BOUSOUET,BERNARD
+  ΜΠΟΥΣΟΥΛΑ,ΝΙΚΟΛΑΟΥ-ΙΩΑΝΝΟΥ: ΜΠΟΎΣΟΥΛΑΣ,ΝΙΚΌΛΑΟΣ-ΙΩΆΝΝΗΣ,Σ.
+  ΜΠΟΥΣΟΥΝΗ,ΔΗΜΗΤΡΗ: ΜΠΟΥΣΟΥΝΗΣ,ΔΗΜΗΤΡΗΣ
+  ΜΠΟΥΣΟΥΡΗΣ,ΙΩΑΝΝΗΣ: ΜΠΟΥΣΟΥΡΗΣ,ΙΩΑΝΝΗΣ
+  BOUTENEFF,FANN-PATRICIA: FANN BOUTENEFF,PATRICIA
+  BOUTHOUL GASTON: BOUTHOUL,GASTON
+  ΜΠΟΥΤΛΑΣ,ΓΙΩΡΓΟΣ: ΜΠΟΥΤΛΑΣ,ΓΙΩΡΓΟΣ
+  ΜΠΟΥΤΟΣ ΒΑΣΙΛΗΣ: ΜΠΟΥΤΟΣ,ΒΑΣΙΛΗΣ
+  ΜΠΟΥΤΣΙΚΑ,ΑΝΔΡΕΑ: ΜΠΟΥΤΣΙΚΑΣ,ΑΝΔΡΕΑΣ
+  ΜΠΟΥΤΣΙΚΑΣ,ΑΝΔΡΕΑΣ: ΜΠΟΥΤΣΙΚΑΣ,ΑΝΔΡΕΑΣ
+  ΜΠΟΥΤΒΑ,ΝΙΚΟΥ: ΜΠΟΥΤΒΑΣ,ΝΙΚΟΣ
+  ΜΠΟΥΖΑΚΗΣ ΣΗΦΗΣ: ΜΠΟΥΖΑΚΗΣ,ΣΗΦΗΣ
+  ΜΠΟΥΖΑΚΗΣ,ΣΗΦΗΣ: ΜΠΟΥΖΑΚΗΣ,ΣΗΦΗΣ
+  BOVE,TONY: BOVE,TONY
+  BOVET M: DE BOVET,FRANÇOIS
+  BOVET THEODOR: BOVET,THEODOR
+  BOWLER,SUE: BOWLER,SUE
+  BOWRA C.M:  BOWRA,CECIL,MAURICE
+  BOWRA,C,Μ: BOWRA,CECIL,MAURICE
+  BOWRA,C.M: BOWRA,CECIL,MAURICE
+  BOWRA,C.M.: BOWRA,CECIL,MAURICE
+  BOYER,JEAN: BOYER,JEAN
+  ΜΠΟΖΙΟΣ,ΙΩΑΝΝΗΣ Θ: ΜΠΟΖΙΟΣ,ΙΩΑΝΝΗΣ,Θ.
+  ΜΠΡΑΓΚΕΤΙ,ΑΝΝΑ ΛΑΟΥΡΑ: BRAGHETTI,ANNA LAURA
+  BRAHUTIGEM OTTO: BRAUTIGAM,OTTO
+  ΜΠΡΑΙΑΝ,ΠΑΤΡΙΚ: O'BRIAN,PATRICK
+  ΜΠΡΑΚΑΤΣΟΥΛΑΣ,ΒΑΣΙΛΗΣ: ΜΠΡΑΚΑΤΣΟΥΛΑΣ,ΒΑΣΙΛΗΣ
+  ΜΠΡΑΜΟΣ,ΚΩΣΤΑΣ Α: ΜΠΡΑΜΟΣ,ΚΩΣΤΑΣ,Α.
+  BRANDSTAETER: BRANDSTÄTER,FRANZ,AUGUST
+  ΜΠΡΑΝΤΜΠΕΡΥ,ΡΑΙΗ: BRADBURY,RAY
+  ΜΠΡΑΝΤΟΝ: BRANDON,EDGAR EWING
+  ΜΠΡΑΤΣΙΩΤΟΥ,ΝΙΚΟΛΑΟΥ: ΜΠΡΑΤΣΙΩΤΗΣ,ΝΙΚΟΛΑΟΣ
+  BRAUDEL FERNAND: BRAUDEL,FERNAND
+  BRAUDEL,FERNAND: BRAUDEL,FERNAND
+  BRAUDEL,FERNARD: BRAUDEL,FERNAND
+  BRAUND,DAVID: BRAUND,DAVID
+  ΜΠΡΕΧΤ,ΜΠΕΡΤΟΛΝΤ: BRECHT,BERTOLT
+  ΜΠΡΕΧΤ,ΜΠΕΡΤΟΛΤ: BRECHT,BERTOLT
+  ΜΠΡΕΔΗΜΑΣ,ΠΙΝΔΑΡΟΣ: ΜΠΡΕΔΗΜΑΣ,ΠΙΝΔΑΡΟΣ
+  BREHIER,EMILE: BREHIER,EMILE
+  BREITENBACH H: BREITENBACH,HANS,RUDOLF
+  BRELOER BERNHARD: BRELOER,BERNHARD
+  BREMOND,CL.: BREMOND,CLAUDE
+  BRENTANO LUZO: BRENTANO,LUJO
+  ΜΠΡΕΤΟΝ,ΑΝΤΡΕ: BRETON,ANDRÉ,ROBERT
+  BRETON,PHILIPPE: BRETON,PHILIPPE
+  ΜΠΡΕΖΙΝΑ,ΤΟΜΑΣ: BREZINA,THOMAS
+  ΜΠΡΙΑΚΟΥ,ΕΛΕΝΗ: ΜΠΡΙΑΚΟΥ,ΕΛΕΝΗ
+  BRIANT PIERRE: BRIANT,PIERRE
+  BRIANT,PIERRE: BRIANT,PIERRE
+  BRICUSSE,LESLIE: BRICUSSE,LESLIE
+  ΜΠΡΙΚΑ,ΕΛΕΝΗ: ΜΠΡΙΚΑ,ΕΛΕΝΗ
+  ΜΠΡΙΜΠΟ,ΤΖΕΦ-ΓΚΕΙΛ,ΝΤΕ ΜΑΡΚΕΝ: BRUMBEAU,JEFF!!DE MARCKEN,GAIL
+  ΜΠΡΙΝΑ ΣΒΙΤ: SVIT,BRINA
+  ΜΠΡΙΟΝ ΜΑΡΣΕΛ: BRION,MARCEL
+  ΜΠΡΙΟΝ,ΜΑΡ.: BRION,MARCEL
+  ΜΠΡΙΟΝ,ΜΑΡΣΕΛ: BRION,MARCEL
+  ΜΠΡΙΣΚΟΟΥ,ΤΖΟΑΝΑ: BRISCOE,JOANNA
+  BROCARD LUCIEN: BROCARD,LUCIEN
+  BROCKHUS: BROCKHAUS
+  BROHCKER WALTER: BRÖCKER,WALTER
+  ΜΠΡΟΝΤΕ ΕΜΙΛΥ: BRONTË,EMILY
+  BRONTE,CH.: BRONTË,CHARLOTTE
+  BRONTE,CHARLOTTE: BRONTË,CHARLOTTE
+  ΜΠΡΟΝΤΕ,ΚΑΡΛΟΤΤΑ: BRONTË,CHARLOTTE
+  ΜΠΡΟΝΤΕ,ΣΑΡΛΟΤ: BRONTË,CHARLOTTE
+  BROTTON,JERRY: BROTTON,JERRY
+  ΜΠΡΟΥΠΗΣ,ΜΙΧΑΛΗΣ ΒΑΣ: ΜΠΡΟΥΠΗΣ,ΜΙΧΑΛΗΣ,ΒΑΣ.
+  ΜΠΡΟΥΣΚΟΥ Α., ΑΓΓΕΛΟΠΟΥΛΟΥ Α.: ΜΠΡΟΥΣΚΟΥ,ΑΊΓΛΗ!!ΑΓΓΕΛΟΠΟΥΛΟΥ,ΆΝΝΑ
+  BROWN,DAN: BROWN,DAN
+  BROWN,MARC: BROWN,MARC
+  BRUCE,ANDY-LANGDON,KEN: BRUCE,ANDY!!LANGDON,KEN
+  BRUCE,STEVE: BRUCE,STEVE
+  BRULE PIERRE: BRULE,PIERRE
+  BRUNEAU PHILIPPE: BRUNEAU,PHILIPPE
+  ΜΠΡΥΚΝΕΡ,ΠΑΣΚΑΛ: BRUCKNER,PASCAL
+  ΜΠΡΥΝΟΦ ΝΤΕ ΣΟΥΖΑΝ: ΝΤΕ ΜΠΡΥΝΟΦ,ΣΟΥΖΑΝ
+  BUDGE,WALLIS: BUDGE,WALLIS
+  BUFAEUX,RENE: BUFAEUX,RENE
+  BUONO,VITO: BUONO,VITO
+  BURCKHARDT JACOD: BURCKHARDT,JACOB
+  BURKE,PETER: BURKE,PETER
+  BURN,A.R: BURN,ANDREW,ROBERT
+  BURNIE,D.: BURNIE,DAVID
+  BURNIE,DAVID: BURNIE,DAVID
+  BURSIAN CONRAD: BURSIAN,CONRAD
+  BUSCAGLIA,LEO: BUSCAGLIA,LEO
+  BUSCH-ZANTNER RICHARD: BUSCH-ZANTNER,RICHARD
+  BUSCHOR ERNST: BUSCHOR,ERNST
+  BUSHNELL CANDACE: BUSHNELL,CANDACE
+  BUSHNELL,CANDACE: BUSHNELL,CANDACE
+  BUSOLT GEORG: BUSOLT,GEORG
+  BUTTNER HERMANN: BUTTNER,HERMANN
+  ΜΠΥΡΓΚΕΡ,Γ.Α: Bürger,Gottfried,August
+  BYRKHARDT ZACOB: BURCKHARDT,JACOB
+
+##### B ΜΠ
+
+##### Z
+
+  ΖΑΧΑΡΕΑΣ, ΑΙΜΙΛΙΟΣ: ΖΑΧΑΡΕΑΣ,ΑΙΜΙΛΙΟΣ
+  ΖΑΧΑΡΗ,ΕΥΣΤΑΘΙΟΥ: ΖΑΧΑΡΗΣ,ΕΥΣΤΑΘΙΟΣ
+  ΖΑΧΑΡΗ,ΛΑΜΠΡΟΥ: ΖΑΧΑΡΗΣ,ΛΑΜΠΡΟΣ
+  ΖΑΧΑΡΗ-ΜΑΤΣΟΥΚΑ ΠΟΠΗ: ΖΑΧΑΡΗ-ΜΑΤΣΟΥΚΑ,ΠΟΠΗ
+  ΖΑΧΑΡΗ-ΜΑΤΣΟΥΚΑ,ΠΟΠΗ: ΖΑΧΑΡΗ-ΜΑΤΣΟΥΚΑ,ΠΟΠΗ
+  ΖΑΧΑΡΗΣ,ΔΗΜΗΤΡΗΣ: ΖΑΧΑΡΗΣ,ΔΗΜΗΤΡΗΣ
+  ΖΑΧΑΡΗΣ,ΛΑΜΠΡΟΣ: ΖΑΧΑΡΗΣ,ΛΑΜΠΡΟΣ
+  ΖΑΧΑΡΟΠΟΥΛΟΥ,ΙΓΝΑΤΙΟΥ: ΖΑΧΑΡΟΠΟΥΛΟΣ,ΙΓΝΑΤΙΟΣ
+  ΖΑΧΑΡΟΣ,ΚΩΣΤΑΣ: ΖΑΧΑΡΟΣ,ΚΩΣΤΑΣ
+  ΖΑΧΟΣ,Χ-ΤΟΥΜΠΟΥΡΟΣ,Χ.: ΖΑΧΟΣ,Χ.!!ΤΟΥΜΠΟΥΡΟΣ,Χ.
+  ΖΑΧΟΥ-ΒΡΕΛΛΗ,ΜΑΡΙΝΑ: ΖΑΧΟΥ-ΒΡΕΛΛΗ,ΜΑΡΙΝΑ
+  ZACOBY FELIX: JACOBY,FELIX
+  ΖΑΔΕ,ΔΗΜΟΣΘΕΝΗΣ: ΖΑΔΕΣ,ΔΗΜΟΣΘΕΝΗΣ
+  ΖΑΔΕΣ ΔΗΜΟΣΘΕΝΗΣ: ΖΑΔΕΣ,ΔΗΜΟΣΘΕΝΗΣ
+  ΖΑΔΕΣ,ΔΗΜΟΣΘΕΝΗΣ: ΖΑΔΕΣ,ΔΗΜΟΣΘΕΝΗΣ
+
+  # https://www.amazon.de/Demosthenes-Staatsmann-Werden-Werner-Jaeger/dp/3110025272
+  ZAE WERNER: JAEGER,WERNER,WILHELM
+  JAE WERNER: JAEGER,WERNER,WILHELM
+  JAEGER,WERNER: JAEGER,WERNER,WILHELM
+
+  ΖΑΦΕΙΡΗ,ΝΙΚΟΛΑΟΥ: ΖΑΦΕΙΡΗΣ,ΝΙΚΟΛΑΟΣ
+  ΖΑΦΕΙΡΟΠΟΥΛΟΣ,ΔΗΜ Γ: ΖΑΦΕΙΡΟΠΟΥΛΟΣ,ΔΗΜ.,Γ.
+  ΖΑΦΕΙΡΟΠΟΥΛΟΥ: ΖΑΦΕΙΡΟΠΟΥΛΟΣ,ΖΑΦΕΙΡΙΟΣ
+  ΖΑΦΕΙΡΟΠΟΥΛΟΥ,ΣΙΜΟΝΗ: ΖΑΦΕΙΡΟΠΟΥΛΟΥ,ΣΙΜΟΝΗ
+  ΖΑΦΕΙΡΟΠΟΥΛΟΥ,ΒΑΣΩ: ΖΑΦΕΙΡΟΠΟΥΛΟΥ,ΒΑΣΩ
+  ZAFON,RUIZ,CARLOS: ZAFON,CARLOS,RUIZ
+  ΖΑΦΡΑΚΑ-ΣΤΑΥΡΙΔΟΥ,ΑΛΚΜΗΝΗ: ΖΑΦΡΑΚΑ-ΣΤΑΥΡΙΔΟΥ,ΑΛΚΜΗΝΗ
+  ΖΑΦΡΕΙΡΗΣ,ΧΡΥΣΟΣΤΟΜΟΣ: ΖΑΦΕΙΡΗΣ,ΧΡΥΣΟΣΤΟΜΟΣ
+  ΖΑΓΚΑΓΙΕΒΣΚΙ,ΑΝΤΑΜ: ZAGAJEWSKI,ADAM
+  ΖΑΓΚΛΗ,ΔΗΜΗΤΡΙΟΥ: ΖΑΓΚΛΗΣ,ΔΗΜΗΤΡΙΟΣ
+  ΖΑΓΚΛΗΣ,Α.Δ: ΖΑΓΚΛΗΣ,Α.,Δ.
+  ΖΑΓΚΛΗΣ,ΔΗΜΗΤΡΙΟΣ Δ: ΖΑΓΚΛΗΣ,ΔΗΜΗΤΡΙΟΣ
+  ΖΑΓΚΟΥΙΝ,ΚΙΟΥ: JACQUIN,GUY
+  ZAHRNT MICHAEL: ZAHRNT,MICHAEL
+  ΖΑΙΡΗ-ΡΩΣΣΗ,ΡΕΝΑ: ΖΑΙΡΗ-ΡΩΣΣΗ,ΡΕΝΑ
+  ΖΑΚΑΣ ΠΑΝΟΣ: ΖΑΚΑΣ,ΠΑΝΟΣ
+  ΖΑΚΚΑ,ΜΙΛΤΙΑΔΗ: ΖΑΚΚΑΣ,ΜΙΛΤΙΑΔΗΣ
+  ΖΑΚΟΠΟΥΛΟΣ: ΖΑΚΟΠΟΥΛΟΣ,ΝΙΚΟΣ,Ι.
+  ΖΑΚΟΠΟΥΛΟΣ,Ν.Ι: ΖΑΚΟΠΟΥΛΟΣ,ΝΙΚΟΣ,Ι.
+  ΖΑΚΟΠΟΥΛΟΣ,Ν.Ι.: ΖΑΚΟΠΟΥΛΟΣ,ΝΙΚΟΣ,Ι.
+  ΖΑΚΟΠΟΥΛΟΣ,ΝΙΚΟΛΑΟΣ: ΖΑΚΟΠΟΥΛΟΣ,ΝΙΚΟΣ,Ι.
+  ΖΑΚΟΠΟΥΛΟΣ,ΝΙΚΟΣ: ΖΑΚΟΠΟΥΛΟΣ,ΝΙΚΟΣ,Ι.
+  ΖΑΚΟΠΟΥΛΟΣ,ΝΙΚΟΣ.Ι: ΖΑΚΟΠΟΥΛΟΣ,ΝΙΚΟΣ,Ι.
+  ΖΑΚΟΠΟΥΛΟΥ,ΠΑΝΑΓΙΩΤΟΥ: ΖΑΚΟΠΟΥΛΟΣ,ΠΑΝΑΓΙΩΤΗΣ
+
+  ΖΑΚΟΥΕ,ΑΝΤΡΕ: JACQUES,ANDRE
+  ΖΑΚΥΝΘΗΝΟΥ ΔΙΟΝ: ΖΑΚΥΘΗΝΟΣ,ΔΙΟΝΥΣΙΟΣ
+  ΖΑΚΥΘΗΝΟΣ,ΔΙΟΝ Α: ΖΑΚΥΘΗΝΟΣ,ΔΙΟΝΥΣΙΟΣ
+  ΖΑΚΥΘΥΝΟΣ,ΑΛΕΞΗΣ: ΖΑΚΥΘΥΝΟΣ,ΑΛΕΞΗΣ
+  ΖΑΛΙΟΣ ΧΡΗΣΤΟΣ: ΖΑΛΙΟΣ,ΧΡΗΣΤΟΣ
+  ΖΑΛΟΚΩΣΤΑΣ,ΧΡΗΣΤΟΣ: ΖΑΛΟΚΩΣΤΑΣ,ΧΡΗΣΤΟΣ
+  ΖΑΛΩΝΗ,ΠΑΝΑΓΙΩΤΑ: ΖΑΛΩΝΗ-ΧΡΙΣΤΟΠΟΥΛΟΥ,ΠΑΝΑΓΙΩΤΑ
+  ΖΑΛΩΝΗ-ΧΡΙΣΤΟΠΟΥΛΟΥ,ΠΑΝΑΓΙΩΤΑ: ΖΑΛΩΝΗ-ΧΡΙΣΤΟΠΟΥΛΟΥ,ΠΑΝΑΓΙΩΤΑ
+  ΖΑΜΠΑΚΟΣ,ΓΙΑΝΝΗΣ: ΖΑΜΠΑΚΟΣ,ΓΙΑΝΝΗΣ
+  ΖΑΜΠΑΘΑ-ΠΑΓΟΥΛΑΤΟΥ,ΦΑΙΔΡΑ: ΖΑΜΠΑΘΑ-ΠΑΓΟΥΛΑΤΟΥ,ΦΑΙΔΡΑ
+  ΖΑΜΠΑΤΗΣ,ΕΛΕΥΘΕΡΙΟΣ: ΖΑΜΠΑΤΗΣ,ΕΛΕΥΘΕΡΙΟΣ
+  ΖΑΜΠΟΥΝΗΣ ΧΡΗΣΤΟΣ: ΖΑΜΠΟΥΝΗΣ,ΧΡΗΣΤΟΣ
+  ΖΑΜΠΟΥΝΗΣ,ΧΡΗΣΤΟΣ: ΖΑΜΠΟΥΝΗΣ,ΧΡΗΣΤΟΣ
+  ΖΑΜΒΑΛΝΤ,ΑΚΙΜ: SAMWALD,ACHIM
+  ΖΑΝ ΕΛΛΕΝΣΤΕΙΝ: ELLEINSTEIN,JEAN
+  ΖΑΝ,ΡΑΙΜΟΝ: RAYMOND,JEAN
+
+  ZANINI,GIUSEPPE: ZANINI,GIUSEPPE
+  ZANTNER,RICHARD: BUSCH-ZANTNER,RICHARD
+  ΖΑΠΠΑΣ,ΚΩΣΤΑΣ: ΖΑΠΠΑΣ,ΚΩΣΤΑΣ
+  ΖΑΡΑΜΠΟΥΚΑ,ΣΟΦΙΑ: ΖΑΡΑΜΠΟΥΚΑ,ΣΟΦΙΑ
+  ΖΑΡΑΒΕΛΑΣ ΔΗΜΗΤΡΗΣ ΑΘ.: ΖΑΡΑΒΕΛΑΣ,ΔΗΜΗΤΡΗΣ,ΑΘ.
+  ΖΑΡΙΦΟΠΟΥΛΟΣ ΓΡΗΓΟΡΙΟΣ: ΖΑΡΙΦΟΠΟΥΛΟΣ,ΓΡΗΓΟΡΙΟΣ
+  ΖΑΡΚΙΑ ΣΤΑΘΗ: ΖΑΡΚΙΑΣ,ΣΤΑΘΗΣ
+  ΖΑΡΟΚΩΣΤΑ,ΚΑΤΕΡΙΝΑ: ΖΑΡΟΚΩΣΤΑ,ΚΑΤΕΡΙΝΑ
+  ΖΑΡΟΥΚΑ,ΚΩΣΤΑ: ΖΑΡΟΥΚΑΣ,ΚΩΣΤΑΣ
+  ΖΑΡΟΥΚΑΣ,ΚΩΣΤΑΣ: ΖΑΡΟΥΚΑΣ,ΚΩΣΤΑΣ
+  ΖΑΡΡΑΣ ΙΩΑΝΝΗΣ: ΖΑΡΡΑΣ,ΙΩΑΝΝΗΣ
+  ΖΑΤΕΛΗ,ΖΥΡΑΝΝΑ: ΖΑΤΕΛΗ,ΖΥΡΑΝΝΑ
+  ΖΑΤΕΛΗ,ΖΥΡΡΑΝΑ: ΖΑΤΕΛΗ,ΖΥΡΑΝΝΑ
+  ΖΑΤΕΛΛΗ,ΖΥΡΑΝΝΑ: ΖΑΤΕΛΗ,ΖΥΡΑΝΝΑ
+  ΖΑΒΕΡΔΙΝΟΥ,ΛΙΖΑ: ΖΑΒΕΡΔΙΝΟΥ,ΛΙΖΑ-ΠΑΡΑΣΚΕΥΗ
+  ΖΑΒΕΡΔΙΝΟΥ,ΛΙΖΑ-ΠΑΡΑΣΚ.: ΖΑΒΕΡΔΙΝΟΥ,ΛΙΖΑ-ΠΑΡΑΣΚΕΥΗ
+  ΖΑΒΙΤΣΑΝΟΥ,ΔΗΜΟΣΘΕΝΗ: ΖΑΒΙΤΣΑΝΟΣ,ΔΗΜΟΣΘΕΝΗΣ
+  ΖΕΓΚΕΡΣ ΑΝΝΑ: SEGHERS,ANNA
+  ZEHNACKER HUBERT: ZEHNACKER,HUBERT
+  ΖΕΗ,ΑΛΚΗ: ΖΕΗ,ΑΛΚΗ
+  ΖΕΗ,ΕΛΕΥΘΕΡΙΑ: ΖΕΗ,ΕΛΕΥΘΕΡΙΑ
+  ΖΕΛΛΕΚΕ,ΚΙΦΕΛΕΒ: ZELLEKE,KIFELEV
+  ΖΕΜΠΗ,ΧΡΙΣΤΙΝΑ: ΖΕΜΠΗ,ΧΡΙΣΤΙΝΑ
+  ΖΕΝΑΚΟΣ,Λ.: ΖΕΝΑΚΟΣ,ΛΕΩΝΙΔΑΣ
+  ΖΕΝΑΚΟΥ,ΛΕΩΝΙΔΑ:  ΖΕΝΑΚΟΣ,ΛΕΩΝΙΔΑΣ
+  ΖΕΝΕΒΟΥΑ,ΜΩΡΙΣ: GENEVOIX,MAURICE
+  ZERLE,HERBERT: ZERLE,HERBERT
+  ΖΕΡΜΠΙΝΗ,ΔΗΜΗΤΡΙΟΥ: ΖΕΡΜΠΙΝΗΣ,ΔΗΜΗΤΡΙΟΣ
+  ΖΕΡΒΑΝΟΣ,ΑΛΕΞΗΣ: ΖΕΡΒΑΝΟΣ,ΑΛΕΞΗΣ
+  ΖΕΡΒΑΝΟΥ,ΑΛΕΞΗ: ΖΕΡΒΑΝΟΣ,ΑΛΕΞΗΣ
+  ΖΕΡΒΑΣ ΓΙΑΝΝΗΣ: ΖΕΡΒΑΣ,ΓΙΑΝΝΗΣ
+  ΖΕΡΒΑΣ,ΑΝΤΩΝΗΣ: ΖΕΡΒΑΣ,ΑΝΤΩΝΗΣ
+  ΖΕΡΒΟΣ,ΓΙΑΝΝΗΣ: ΖΕΡΒΟΣ,ΓΙΑΝΝΗΣ
+  ΖΕΡΒΟΣ,ΙΩΑΝΝΗΣ: ΖΕΡΒΟΣ,ΙΩΑΝΝΗΣ
+  ΖΕΡΒΟΣ,ΤΑΣΟΣ: ΖΕΡΒΟΣ,ΤΑΣΟΣ
+  ΖΕΡΒΟΣ-ΙΑΚΩΒΑΤΗΣ,ΗΛΙΑΣ: ΖΕΡΒΟΣ-ΙΑΚΩΒΑΤΗΣ,ΗΛΙΑΣ
+  ΖΕΡΖΕΛΙΔΗ Ι. ΓΕΩΡΓΙΟΥ: ΖΕΡΖΕΛΙΔΗΣ,ΓΕΩΡΓΙΟΣ,Ι.
+  ΖΕΡΖΕΛΙΔΗ,ΓΕΩΡΓ.: ΖΕΡΖΕΛΙΔΗΣ,ΓΕΩΡΓΙΟΣ,Ι.
+  ΖΕΡΖΕΛΙΔΗ,ΓΕΩΡΓΙΟΥ: ΖΕΡΖΕΛΙΔΗΣ,ΓΕΩΡΓΙΟΣ,Ι.
+  ΖΕΒΑΚΟ,Μ.: ZEVACO,MICHEL
+  ΖΕΥΓΩΛΗ,ΔΙΑΛΕΧΤΗ: ΖΕΥΓΩΛΗ,ΔΙΑΛΕΧΤΗ
+  ΖΕΥΓΩΛΗΣ,ΓΙΑΝΝΗΣ: ΖΕΥΓΩΛΗΣ,ΓΙΑΝΝΗΣ
+  ΖΙΑΓΚΟΣ,Ν.Γ: ΖΙΑΓΚΟΣ,ΝΙΚΟΣ,Γ.
+  ΖΙΑΓΚΟΣ,ΝΙΚ Γ: ΖΙΑΓΚΟΣ,ΝΙΚΟΣ,Γ.
+  ΖΙΑΓΚΟΣ,ΝΙΚ.Γ: ΖΙΑΓΚΟΣ,ΝΙΚΟΣ,Γ.
+  ΖΙΑΓΚΟΣ,ΝΙΚΟΣ: ΖΙΑΓΚΟΣ,ΝΙΚΟΣ,Γ.
+  ΖΙΑΚΑ,ΓΡΗΓΟΡΙΟΥ: ΖΙΑΚΑΣ,ΓΡΗΓΟΡΙΟΣ
+  ΖΙΑΚΑΣ ΓΡΗΓΟΡΙΟΣ: ΖΙΑΚΑΣ,ΓΡΗΓΟΡΙΟΣ
+  ΖΙΑΝΝΗ,ΔΗΜΗΤΡΑ: ΖΙΑΝΝΗ,ΔΗΜΗΤΡΑ
+  ΖΗΔΡΟΥ,ΝΤΙΝΑ: ΖΗΔΡΟΥ,ΝΤΙΝΑ
+  ZIEGLER,JEAN: ZIEGLER,JEAN
+  ZIELINSKI TH: ZIELINSKI,TADEUSZ
+  ZIELNSKI THADDEE: ZIELINSKI,TADEUSZ
+  ΖΙΓΔΗΣ ΙΩΑΝΝΗΣ: ΖΙΓΔΗΣ,ΙΩΑΝΝΗΣ,Γ.
+  ΖΙΓΔΗΣ,ΙΩΑΝΝΗΣ Γ: ΖΙΓΔΗΣ,ΙΩΑΝΝΗΣ,Γ.
+  ΖΙΓΚΜΑΝ,ΛΩΡΑ: ZIGMAN,LAURA
+  ΖΙΓΚΜΟΝΤ,ΜΟΡΙΤΣ: ZSIGMOND,MORICZ
+  ΖΗΚΟΥ ΜΑΙΡΗ: ΖΗΚΟΥ,ΜΑΙΡΗ
+  ΖΗΛΕΜΕΝΟΣ,ΚΩΣΤΑΣ: ΖΗΛΕΜΕΝΟΣ,ΚΩΣΤΑΣ
+  ΖΙΜΕΡ,ΑΛΦΡΕΤ: ZIMMERN,ALFRED
+  ΖΙΜΕΡΙΝ,ΝΤΜΙΤΡΙ: ΖΙΜΕΡΙΝ,ΝΤΜΙΤΡΙ
+  ΖΙΝΤ,ΑΝΤΡΕ: GIDE,ANDRÉ,PAUL GUILLAUME
+  ΖΙΩΓΑΣ ΘΩΜΑΣ: ΖΙΩΓΑΣ,ΘΩΜΑΣ
+  ΖΙΩΓΑΣ,ΘΩΜΑΣ: ΖΙΩΓΑΣ,ΘΩΜΑΣ
+  ΖΙΟΥΤΟΣ,Γ.Δ: ΖΙΟΥΤΟΣ,ΓΙΩΡΓΟΣ,Δ.
+  ΖΙΟΥΤΟΣ,Γ.Δ.: ΖΙΟΥΤΟΣ,ΓΙΩΡΓΟΣ,Δ.
+  ΖΙΟΥΤΟΣ,ΓΙΩΡΓΟΣ: ΖΙΟΥΤΟΣ,ΓΙΩΡΓΟΣ,Δ.
+  ΖΙΡΑΡ,ΠΑΤΡΙΚ: GIRARD,PATRICK
+  ΖΙΡΩΝΤΟΥ ΖΑΝ: GIRAUDOUX,JEAN
+  ΖΙΡΟΥ,ΦΡΑΝΣΟΥΑ: GIROUD,FRANCOISE
+  ΖΙΡΟΥ,ΦΡΑΝΣΟΥΑΖ: GIROUD,FRANCOISE
+  ΖΗΣΗ,ΘΕΟΔΩΡΟΥ: ΖΗΣΗ,ΘΕΟΔΩΡΟΥ
+  ΖΗΣΙΑΔΗ,ΒΑΣΙΛΕΙΟΥ: ΖΗΣΙΑΔΗΣ,ΒΑΣΙΛΕΙΟΣ
+  ΖΗΣΙΜΟΥ,ΓΙΤΣΑ: ΖΗΣΙΜΟΥ,ΓΙΤΣΑ
+  ΖΙΣΚΙΝΤ,ΠΑΤΡΙΚ: SÜSKIND,PATRICK
+  ΖΙΤΣΑΙΑ ΧΡΥΣΑΝΘΗ: ΖΙΤΣΑΙΑ,ΧΡΥΣΑΝΘΗ
+  ΖΙΤΣΑΙΑ,ΧΡΥΣΑΝΘΗ: ΖΙΤΣΑΙΑ,ΧΡΥΣΑΝΘΗ
+  ZIZEK FRANZ: ZIZEK,FRANZ
+  ΖΩΔΙΑΤΟΥ,ΣΠΥΡΟΥ: ΖΩΔΙΑΤΟΣ,ΣΠΥΡΟΣ
+  ΖΟΓΚΖΑ,ΒΑΣΙΛΙΚΗ: ΖΟΓΚΖΑ,ΒΑΣΙΛΙΚΗ
+  ΖΩΓΡΑΦΑΚΗ,ΓΕΩΡΓΙΟΥ: ΖΩΓΡΑΦΑΚΗΣ,ΓΕΩΡΓΙΟΣ
+  ΖΩΓΡΑΦΟ,ΤΑΣΟ: ΖΩΓΡΑΦΟΣ,ΤΑΣΟΣ
+  ΖΩΓΡΑΦΟΥ ΛΙΛΗ: ΖΩΓΡΑΦΟΥ,ΛΙΛΗ
+  ΖΩΓΡΑΦΟΥ ΜΑΡΙΝΑ: ΖΩΓΡΑΦΟΥ,ΜΑΡΙΝΑ
+  ΖΩΓΡΑΦΟΥ,ΕΥΓΕΝΙΑ: ΖΩΓΡΑΦΟΥ,ΕΥΓΕΝΙΑ
+  ΖΩΓΡΑΦΟΥ,ΛΙΛΗ: ΖΩΓΡΑΦΟΥ,ΛΙΛΗ
+  ΖΩΓΡΑΦΟΥ-ΚΟΡΡΕ,ΚΑΤΕΡΙΝΑ: ΖΩΓΡΑΦΟΥ-ΚΟΡΡΕ,ΚΑΤΕΡΙΝΑ
+  ΖΩΗ,ΑΜΑΛΙΑ: ΖΩΗ,ΑΜΑΛΙΑ
+  ΖΩΙΔΗΣ ΠΑΝΑΓΙΩΤΗΣ: ΖΩΙΔΗΣ,ΠΑΝΑΓΙΩΤΗΣ
+  ΖΩΗΣ,ΙΩΝΑΣ: ΖΩΗΣ,ΙΩΝΑΣ
+  ΖΟΛΑ ΑΙΜ: ZOLA,ÉMILE,ÉDOUARD CHARLES ANTOINE
+  ΖΟΛΑ,ΑΙΜΙΛ: ZOLA,ÉMILE,ÉDOUARD CHARLES ANTOINE
+  ΖΟΛΑ,Ε.: ZOLA,ÉMILE,ÉDOUARD CHARLES ANTOINE
+  ΖΟΛΑ,ΕΜΙΛ: ZOLA,ÉMILE,ÉDOUARD CHARLES ANTOINE
+
+  ΖΟΛΔΕΡ,ΑΝΘΟΥΛΑ: ΖΟΛΔΕΡ,ΑΝΘΟΥΛΑ
+  ZOLLIN WALTER:  ZOLLINGER,WALTER
+  ΖΟΛΩΤΑ,ΑΓΓΕΛΙΚΗ: ΖΟΛΩΤΑ,ΑΓΓΕΛΙΚΗ
+  ΖΟΛΩΤΑΣ ΞΕΝΟΦΩΝ: ΖΟΛΩΤΑΣ,ΞΕΝΟΦΩΝ
+  ΖΟΛΩΤΑΣ,ΞΕΝΟΦ.: ΖΟΛΩΤΑΣ,ΞΕΝΟΦΩΝ
+  ΖΟΛΩΤΑΣ,ΞΕΝΟΦΩΝ: ΖΟΛΩΤΑΣ,ΞΕΝΟΦΩΝ
+  ΖΟΜΠΑΝΑΚΗ,ΑΠ.: ΖΟΜΠΑΝΑΚΗΣ,ΣΠ.
+  ΖΟΜΠΑΝΑΚΗ,ΣΠ.: ΖΟΜΠΑΝΑΚΗΣ,ΣΠ.
+  ΖΟΜΠΟΛΑΣ,ΤΑΣΟΣ: ΖΟΜΠΟΛΑΣ,ΤΑΣΟΣ
+  ΖΟΝΚΕ,ΤΙΕΡΥ: JONQUET,THIERRY
+  ΖΩΝΤΑΝΟΥ,ΚΑΤΕΡΙΝΑ: ΖΩΝΤΑΝΟΥ,ΚΑΤΕΡΙΝΑ
+  ΖΩΡΑ ΠΟΠΗ: ΖΩΡΑ,ΠΟΠΗ
+  ΖΩΡΑ,ΠΟΠΗ: ΖΩΡΑ,ΠΟΠΗ
+  ΖΩΡΑΣ ΓΕΡΑΣΙΜΟΣ: ΖΩΡΑΣ,ΓΕΡΑΣΙΜΟΣ
+  ΖΩΡΑΣ, ΓΕΩΡΓΙΟΣ: ΖΩΡΑΣ,ΓΕΩΡΓΙΟΣ
+  ΖΩΡΑΣ,ΓΕΩΡΓΙΟΣ: ΖΩΡΑΣ,ΓΕΩΡΓΙΟΣ
+  ΖΩΡΑΣ,ΓΕΡΑΣΙΜΟΣ: ΖΩΡΑΣ,ΓΕΡΑΣΙΜΟΣ
+  ΖΟΡΜΠΑ,ΠΑΝΟΥ: ΖΟΡΜΠΑΣ,ΠΑΝΟΣ
+  ΖΟΡΜΠΑΣ,ΑΛΕΞΑΝΔΡΟΣ: ΖΟΡΜΠΑΣ,ΑΛΕΞΑΝΔΡΟΣ
+  ΖΩΡΟΓΙΑΝΝΙΔΗΣ,ΚΩΝ/ΝΟΣ: ΖΩΡΟΓΙΑΝΝΙΔΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
+  ΖΩΡΟΓΙΑΝΝΙΔΗΣ,ΝΙΚΟΣ: ΖΩΡΟΓΙΑΝΝΙΔΗΣ,ΝΙΚΟΣ
+  ΖΩΡΖ ΜΠΟΡΝΤΟΝΟΒ: BORDONOVE,GEORGES
+  ΖΩΡΖΟΣ,ΓΡΗΓΟΡΗΣ: ΖΩΡΖΟΣ,ΓΡΗΓΟΡΗΣ
+  ΖΩΤΙΑΔΗΣ,ΓΕΩΡΓΙΟΣ: ΖΩΤΙΑΔΗΣ,ΓΕΩΡΓΙΟΣ
+  ΖΩΤΙΑΔΟΥ,ΓΕΩΡΓΙΟΥ: ΖΩΤΙΑΔΗΣ,ΓΕΩΡΓΙΟΣ
+  ΖΩΤΟΣ,ΔΗΜ Α: ΖΩΤΟΣ,ΔΗΜΗΤΡΙΟΣ,Α.
+  ΖΩΤΟΣ,ΜΕΝΕΛΑΟΣ Σ: ΖΩΤΟΣ,ΜΕΝΕΛΑΟΣ,Σ.
+  ΖΟΥΜΠΟΥΛΑΚΗ,ΔΗΜΗΤΡΙΑ: ΖΟΥΜΠΟΥΛΑΚΗ,ΔΗΜΗΤΡΙΑ
+  ΖΟΥΜΠΟΥΛΑΚΗ,ΜΑΝΙΝΑ: ΖΟΥΜΠΟΥΛΑΚΗ,ΜΑΝΙΝΑ
+  ΖΟΥΡΑ-ΤΡΙΧΙΑ,ΜΑΡΙΑ: ΖΟΥΡΑ-ΤΡΙΧΙΑ,ΜΑΡΙΑ
+  ΖΟΥΡΑΡΙΣ ΚΩΣΤΑΣ: ΖΟΥΡΑΡΙΣ,ΚΩΣΤΑΣ
+  ΖΟΥΡΑΒΛΙΟΒΑ-ΠΑΠΠΟΥ,ΑΙΚΑΤΕΡΙΝΗ: ΖΟΥΡΑΒΛΙΟΒΑ-ΠΑΠΠΟΥ,ΑΙΚΑΤΕΡΙΝΗ
+  ΖΟΥΡΓΟΣ,ΙΣΙΔΩΡΟΣ: ΖΟΥΡΓΟΣ,ΙΣΙΔΩΡΟΣ
+  ΖΟΥΡΙΔΟΥ-ΛΙΑΠΗ ΜΑΡΙΑ: ΖΟΥΡΙΔΟΥ-ΛΙΑΠΗ,ΜΑΡΙΑ
+  ΖΟΥΡΛΑΣ,ΠΑΝΤ: ΖΟΥΡΛΑΣ,ΠΑΝΤΕΛΗΣ
+  ΖΟΥΡΝΑΤΖΙΔΗΣ,ΝΙΚΟΣ: ΖΟΥΡΝΑΤΖΙΔΗΣ,ΝΙΚΟΣ
+  ΖΟΥΡΝΑΤΖΗΣ,ΣΠ: ΖΟΥΡΝΑΤΖΗΣ,ΣΠΥΡΟΣ
+  ΖΟΥΣΑΚ,ΜΑΡΚΟΥΣ: ZUSAK,MARKUS
+  ZSCHOKKE-HEINRICH,JOHANN: ZSCHOKKE,JOHANN,HEINRICH DANIEL
+  ZWEIG,STEFAN: ZWEIG,STEFAN
+  ΖΥΓΟΥΡΗ,ΣΩΤΗΡΗ: ΖΥΓΟΥΡΗΣ,ΣΩΤΗΡΗΣ
+  ΖΥΓΟΥΡΗΣ ΣΩΤΗΡΗΣ: ΖΥΓΟΥΡΗΣ,ΣΩΤΗΡΗΣ
+  ΖΥΓΟΥΡΗΣ,ΣΩΤΗΡΗΣ: ΖΥΓΟΥΡΗΣ,ΣΩΤΗΡΗΣ
+  ΖΥΚΙΕΝ,ΠΙΕΡ: JUQUIN,PIERRE!!STENGERS,ISABELLE!!ANTUNES,CARLOS!KEMP,PENNY!!TELKAMPER,WILFRID!!WOLF,FRIEDER,OTTO
+  ΖΥΛΙΕΝ,ΚΛΩΝΤ: JULIEN,CLAUDE
+
+##### Z
```

### Comparing `skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/converted_entries.yml` & `skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/data/converted_entries.yml`

 * *Files 0% similar despite different names*

```diff
@@ -6218,15 +6218,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 119
   authors:
-  - ΒΛΑΧΟΣ,ΑΓΓΕΛΟΣ,ΣΤ,
+  - ΒΛΑΧΟΣ,ΑΓΓΕΛΟΣ,ΣΤ.
   language: el
   title: Ο ΚΑΜΠΑΝΟΠΥΡΓΟΣ
   dewey: 886.2 ΒΛΑ
   entry_numbers:
   - '1363'
   editor: ΔΩΔΩΝΗ // ΑΘΗΝΑ
   pages: 83
@@ -6270,15 +6270,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 120
   authors:
-  - ΒΛΑΧΟΣ,ΑΓΓΕΛΟΣ,ΣΤ,
+  - ΒΛΑΧΟΣ,ΑΓΓΕΛΟΣ,ΣΤ.
   language: el
   title: ΔΕΚΑ ΧΡΟΝΙΑ ΚΥΠΡΙΑΚΟΥ
   dewey: 938.497 ΒΛΑ
   entry_numbers:
   - '2232'
   editor: ΕΣΤΙΑ // ΑΘΗΝΑ
   edition_year: 1980
@@ -16400,15 +16400,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 315
   authors:
-  - ΖΑΓΚΛΗΣ,Α.Δ
+  - ΖΑΓΚΛΗΣ,Α.,Δ.
   language: el
   title: ΜΟΜΤΖΙΛΟΣ Ή ΜΟΜΤΖΙΛ ΕΘΝΙΚΟΣ ΗΡΩΣ ΒΟΥΛΓΑΡΩΝ ΚΑΙ ΣΕΡΒΩΝ
   dewey: 938.653 ΖΑΓ
   entry_numbers:
   - '2107'
   editor: None // ΑΘΗΝΑ
   edition_year: 1966
@@ -16452,15 +16452,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 316
   authors:
-  - ΖΑΓΚΛΗΣ,ΔΗΜΗΤΡΙΟΣ Δ
+  - ΖΑΓΚΛΗΣ,ΔΗΜΗΤΡΙΟΣ
   language: el
   title: ΧΑΛΚΙΔΙΚΗ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
   subtitle: ΑΠΟ ΤΩΝ ΑΡΧΑΙΟΤΑΤΩΝ ΧΡΟΝΩΝ ΜΕΧΡΙ ΤΟΥ 1912
   dewey: 914.951 ΖΑΓ
   entry_numbers:
   - '354'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
@@ -16503,15 +16503,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 317
   authors:
-  - ΖΑΚΟΠΟΥΛΟΣ,ΝΙΚΟΣ
+  - ΖΑΚΟΠΟΥΛΟΣ,ΝΙΚΟΣ,Ι.
   language: el
   title: Η ΔΙΚΑΙΩΣΗ ΚΑΙ Ο ΧΟΡΟΣ
   dewey: 880.2 ΖΑΚ
   entry_numbers:
   - '1366'
   editor: ΔΩΔΩΝΗ // ΑΘΗΝΑ
   pages: 148
@@ -16554,15 +16554,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 318
   authors:
-  - ΖΑΚΥΘΗΝΟΣ,ΔΙΟΝ Α
+  - ΖΑΚΥΘΗΝΟΣ,ΔΙΟΝΥΣΙΟΣ
   language: el
   title: Η ΑΛΩΣΙΣ ΤΗΣ ΚΩΝΣΑΝΤΙΝΟΥΠΟΛΕΩΣ ΚΑΙ Η ΤΟΥΡΚΟΚΡΑΤΙΑ
   dewey: 938.389 ΖΑΚ
   entry_numbers:
   - '1834'
   editor: None // ΑΘΗΝΑ
   edition_year: 1954
@@ -16605,15 +16605,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 319
   authors:
-  - ΖΑΚΟΥΕ,ΑΝΤΡΕ
+  - JACQUES,ANDRE
   language: el
   title: ΧΙΛΗ
   subtitle: ΕΝΑΣ ΛΑΟΣ ΚΕΝΤΑ ΤΗ ΖΩΗ ΚΑΙ ΤΟΥΣ ΑΓΩΝΕΣ ΤΟΥ
   dewey: 915 ΖΑΚ
   entry_numbers:
   - '458'
   translators:
@@ -16708,15 +16708,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 321
   authors:
-  - ΖΑΝΑΝΤΡΙΣ,ΚΑΣ
+  - ΑΝΔΡΙΑΝΟΠΟΥΛΟΥ,ΙΩΑΝΝΑ@ΚΥΡΙΑ ΖΑΝΑΝΤΡΙΣ
   language: el
   title: ΕΛΛΗΝΕΣ ΑΔΕΡΦΟΙ ΜΟΥ ΑΣ ΠΟΛΕΜΗΣΩΜΕΝ
   dewey: 938 ΖΑΝ
   entry_numbers:
   - '2558'
   editor: None // ΑΘΗΝΑ
   edition_year: 1948
@@ -16758,15 +16758,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 322
   authors:
-  - ΖΑΦΕΙΡΟΠΟΥΛΟΣ,ΔΗΜ Γ
+  - ΖΑΦΕΙΡΟΠΟΥΛΟΣ,ΔΗΜ.,Γ.
   language: el
   title: Η ΑΦΡΙΚΗ ΤΗΣ ΧΘΕΣ ΚΑΙ ΤΗΣ ΣΗΜΕΡΟΝ
   dewey: 916 ΖΑΦ
   entry_numbers:
   - '2589'
   editor: None // ΑΘΗΝΑ
   edition_year: 1963
@@ -16858,15 +16858,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 324
   authors:
-  - ΖΕΝΕΒΟΥΑ,ΜΩΡΙΣ
+  - GENEVOIX,MAURICE
   language: el
   title: Η ΕΛΛΑΣ ΤΟΥ ΚΑΡΑΜΑΝΛΗ Ή Η ΔΗΜΟΚΡΑΤΙΑ ΔΥΣΧΕΡΗΣ
   dewey: 938.497 ΖΕΝ
   entry_numbers:
   - '2575'
   editor: ΣΙΔΕΡΗΣ // ΑΘΗΝΑ
   edition_year: 1972
@@ -17010,15 +17010,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 327
   authors:
-  - ΖΙΑΓΚΟΣ,ΝΙΚ Γ
+  - ΖΙΑΓΚΟΣ,ΝΙΚΟΣ,Γ.
   language: el
   title: ΤΟΥΡΚΟΚΡΑΤΟΥΜΕΝΗ ΗΠΕΙΡΟΣ
   subtitle: ΤΙΜΑΡΙΩΤΙΣΜΟΣ,ΑΣΤΙΣΜΟΣ,ΝΕΟΕΛΛΗΝΙΚΗ ΑΝΑΓΕΝΝΗΣΗ (1648-1820)
   dewey: 938.492 ΖΙΑ
   entry_numbers:
   - '1727'
   - '2350'
@@ -17066,15 +17066,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 328
   authors:
-  - ΖΙΑΓΚΟΣ,ΝΙΚ.Γ
+  - ΖΙΑΓΚΟΣ,ΝΙΚΟΣ,Γ.
   language: el
   title: ΦΕΟΥΔΑΡΧΙΚΗ ΗΠΕΙΡΟΣ ΚΑΙ ΔΕΣΠΟΤΑΤΟ ΤΗΣ ΕΛΛΑΔΟΣ
   dewey: 938.451 ΖΙΑ
   entry_numbers:
   - '1730'
   - '2174'
   editor: None // ΑΘΗΝΑ
@@ -17118,15 +17118,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 329
   authors:
-  - ΖΙΑΓΚΟΣ,Ν.Γ
+  - ΖΙΑΓΚΟΣ,ΝΙΚΟΣ,Γ.
   language: el
   title: ΜΑΡΚΟΣ ΜΠΟΤΣΑΡΗΣ
   dewey: 938.489 ΖΙΑ
   entry_numbers:
   - '1962'
   editor: None // ΑΘΗΝΑ
   edition_year: 1966
@@ -17168,15 +17168,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 330
   authors:
-  - ΖΙΓΔΗΣ,ΙΩΑΝΝΗΣ Γ
+  - ΖΙΓΔΗΣ,ΙΩΑΝΝΗΣ,Γ.
   language: el
   title: ΓΙΑ ΤΗ ΔΗΜΟΚΡΑΤΙΑ ΚΑΙ ΤΗΝ ΚΥΠΡΟ
   dewey: 938.497 ΖΙΓ
   entry_numbers:
   - '2227'
   - '4179'
   editor: ΠΑΠΑΖΗΣΗ // ΑΘΗΝΑ
@@ -17219,15 +17219,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 331
   authors:
-  - ΖΙΡΩΝΤΟΥ ΖΑΝ
+  - GIRAUDOUX,JEAN
   language: el
   title: Ο ΠΟΛΕΜΟΣ ΤΗΣ ΤΡΟΙΑΣ ΔΕΝ ΘΑ ΓΙΝΕΙ
   dewey: 886.02 ΖΙΡ
   entry_numbers:
   - '1376'
   translators:
   - ΛΑΖΟΥ,ΜΑΡΙΑ
@@ -17591,15 +17591,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 338
   authors:
-  - ΖΩΤΟΣ,ΔΗΜ Α
+  - ΖΩΤΟΣ,ΔΗΜΗΤΡΙΟΣ,Α.
   language: el
   title: Η ΔΙΚΑΙΟΣΥΝΗ ΕΙΣ ΤΟ ΚΡΑΤΟΣ ΤΟΥ ΑΛΗ ΠΑΣΑ
   dewey: 938.503 ΖΩΤ
   entry_numbers:
   - '2597'
   editor: None // ΑΘΗΝΑ
   edition_year: 1938
@@ -17642,15 +17642,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 339
   authors:
-  - ΖΩΤΟΣ,ΜΕΝΕΛΑΟΣ Σ
+  - ΖΩΤΟΣ,ΜΕΝΕΛΑΟΣ,Σ.
   language: el
   title: ΤΟ ΔΗΜΟΤΙΚΟ ΤΡΑΓΟΥΔΙ ΤΗΣ ΒΟΡΕΙΟΥ ΗΠΕΙΡΟΥ
   dewey: 782.42 ΖΩΤ
   entry_numbers:
   - '736'
   - '737'
   editor: None // ΙΩΑΝΝΙΝΑ
@@ -37089,15 +37089,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 713
   authors:
-  - ΜΠΑΚΟΣ,ΗΛΙΑΣ
+  - ΜΠΑΚΟΣ,ΗΛΙΑΣ,Δ.
   language: el
   title: ΣΥΜΒΟΛΗ ΣΤΟ ΠΡΟΒΛΗΜΑ ΤΗΣ ΚΑΤΑΓΩΓΗΣ ΤΟΥ ΓΕΩΡ.ΚΑΡΑΙΣΚΑΚΗ
   dewey: 938.566 ΜΠΑ
   entry_numbers:
   - '2248'
   - '2502'
   - '4302'
@@ -37191,15 +37191,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 715
   authors:
-  - ΜΠΑΡΑ,ΒΑΣΙΛΕΙΟΣ
+  - ΜΠΑΡΑΣ,ΒΑΣΙΛΕΙΟΣ
   language: el
   title: ΤΟ ΔΕΛΒΙΝΟ ΤΗΣ ΒΟΡΕΙΟΥ ΗΠΕΙΡΟΥ ΚΑΙ ΟΙ ΓΕΙΤΟΝΙΚΕΣ ΤΟΥ ΠΕΡΙΟΧΕ
   dewey: 938.751 ΜΠΑ
   entry_numbers:
   - '2066'
   editor: None // ΑΘΗΝΑ
   edition_year: 1966
@@ -37241,15 +37241,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 716
   authors:
-  - ΜΠΑΣΤΙΑΣ,ΚΩΣΤΑΣ
+  - ΜΠΑΣΤΟΥΝΌΠΟΥΛΟΣ,ΑΙΜΊΛΙΟΣ,ΚΩΝΣΤΑΝΤΊΝΟΣ@ΚΩΣΤΗΣ ΜΠΑΣΤΙΑΣ
   language: el
   title: Ο ΠΑΠΑΔΙΑΜΑΝΤΗΣ
   dewey: 889.35 ΜΠΑ
   entry_numbers:
   - '1125'
   editor: None // ΑΘΗΝΑ
   edition_year: 1962
@@ -37292,15 +37292,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 717
   authors:
-  - ΜΠΕΛΤΟΝ,ΤΖΩΝ
+  - BELTON,JOHN
   language: el
   title: ΧΑΟΥΑΡΝΤ ΧΩΚΣ
   dewey: 800.203 ΜΠΕ
   entry_numbers:
   - '1627'
   translators:
   - ΚΟΛΙΟΔΗΜΟΣ,Δ.
@@ -37344,15 +37344,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 718
   authors:
-  - ΜΠΕΡΝ,Α.Δ
+  - BURN,ANDREW,ROBERT
   language: el
   title: Ο ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ ΚΑΙ Η ΕΛΛΗΝΙΣΤΙΚΗ ΑΥΤΟΚΡΑΤΟΡΙΑ
   dewey: 938.174 ΜΠΕ
   entry_numbers:
   - '2193'
   editor: ΓΑΛΑΞΙΑ // ΑΘΗΝΑ
   edition_year: 1947
@@ -37394,15 +37394,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 719
   authors:
-  - ΜΠΕΡΤΩ,ΣΙΜΟΝ
+  - BERTHEAU,SIMONE
   language: el
   title: ΕΝΤΙΘ ΠΙΑΦ
   dewey: 840 ΜΠΕ
   entry_numbers:
   - '2631'
   translators:
   - ΑΞΙΩΤΗ,ΜΕΛΠΩ
@@ -37549,15 +37549,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 722
   authors:
-  - ΜΠΟΤΣΑΡΗΣ,ΔΗΜ  ΝΟΤΗ
+  - ΜΠΟΤΣΑΡΗΣ,ΔΗΜΗΤΡΙΟΣ,ΝΟΤΗ
   language: el
   title: ΜΑΡΚΟΣ ΜΠΟΤΣΑΡΗΣ
   subtitle: Ο ΑΕΤΟΣ ΤΟΥ ΣΟΥΛΙΟΥ (1790-1823)
   dewey: 938.489 ΜΠΟ
   entry_numbers:
   - '2329'
   editor: None // ΙΩΑΝΝΙΝΑ
@@ -37599,15 +37599,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 723
   authors:
-  - ΜΠΟΤΣΑΡΗΣ,ΔΗΜ.Τ.ΝΟΤΗ
+  - ΜΠΟΤΣΑΡΗΣ,ΔΗΜΗΤΡΙΟΣ,Τ. ΝΟΤΗ
   language: el
   title: Η ΑΠΕΛΕΥΘΕΡΩΣΙΣ ΤΩΝ ΙΩΑΝΝΙΝΩΝ
   dewey: 938.684 ΜΠΟ
   entry_numbers:
   - '2025'
   - '2736'
   editor: None // ΑΘΗΝΑ
@@ -37651,15 +37651,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 724
   authors:
-  - ΜΠΟΥΝΙΟΥΕΛ,ΛΟΥΙΣ
+  - BUÑUEL,LUIS
   language: el
   title: ΜΠΟΥΝΙΟΥΕΛΕΛ
   dewey: 800.203 ΜΠΟ
   entry_numbers:
   - '1618'
   editor: ΑΙΓΟΚΕΡΩΣ // ΑΘΗΝΑ
   edition_year: 1983
@@ -37701,15 +37701,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 725
   authors:
-  - ΜΠΟΥΡΑΝΤΑΣ,ΛΑΜΠΡΟΣ Κ
+  - ΜΠΟΥΡΑΝΤΑΣ,ΛΑΜΠΡΟΣ,Κ
   language: el
   title: Ο ΑΜΒΡΑΚΙΚΟΣ ΚΟΛΠΟΣ ΚΑΙ ΑΙ ΓΥΡΩΘΕΝ ΑΥΤΟΥ ΛΙΜΝΟΘΑΛΑΣΣΑ
   dewey: 938 ΜΠΟ
   entry_numbers:
   - '2487'
   - '2524'
   editor: None // ΑΡΤΑ
@@ -37753,15 +37753,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 726
   authors:
-  - ΜΠΟΥΦΙΔΗΣ,ΧΑΓΕΡ
+  - ΧΆΓΕΡ-ΜΠΟΥΦΊΔΗΣ,ΝΊΚΟΣ
   language: el
   title: ΑΔΟΛΦΟΣ ΧΙΤΛΕΡ
   subtitle: Ο ΔΗΜΙΟΥΡΓΟΣ ΤΗΣ ΝΕΑΣ ΓΕΡΜΑΝΙΑΣ
   dewey: 938.755 ΜΠΟ
   entry_numbers:
   - '2015'
   editor: ΑΚΡΟΠΟΛΕΩΣ // ΑΘΗΝΑ
@@ -37911,15 +37911,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 729
   authors:
-  - ΜΠΡΕΧΤ,ΜΠΕΡΤΟΛΤ
+  - BRECHT,BERTOLT
   language: el
   title: Η ΜΑΝΑ ΚΟΥΡΑΓΙΟ ΚΑΙ ΤΑ ΠΑΙΔΙΑ ΤΗΣ
   dewey: 832 ΜΠΡ
   entry_numbers:
   - '1558'
   translators:
   - ΑΡΖΟΓΛΟΥ,ΙΟΡΔΑΝΗΣ
@@ -37965,15 +37965,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 730
   authors:
-  - ΜΠΡΕΧΤ,ΜΠΕΡΤΟΛΤ
+  - BRECHT,BERTOLT
   language: el
   title: ΤΡΟΜΟΣ ΚΑΙ ΑΘΛΙΟΤΗΤΑ ΤΟΥ ΤΡΙΤΟΥ ΡΑΙΧ
   dewey: 832 ΜΠΡ
   entry_numbers:
   - '1575'
   translators:
   - ΒΕΡΥΚΟΚΑΚΗ,ΑΓΓΕΛΑ
@@ -38020,15 +38020,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 731
   authors:
-  - ΜΠΡΕΧΤ,ΜΠΕΡΤΟΛΝΤ
+  - BRECHT,BERTOLT
   language: el
   title: Ο ΚΑΛΟΣ ΑΝΘΡΩΠΟΣ ΤΟΥ ΣΕΤΣΟΥΑΝ
   dewey: 832 ΜΠΡ
   entry_numbers:
   - '1572'
   translators:
   - ΠΛΩΡΙΤΗΣ,ΜΑΡΙΟΣ
@@ -38075,15 +38075,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 732
   authors:
-  - ΜΠΡΕΧΤ,ΜΠΕΡΤΟΛΤ
+  - BRECHT,BERTOLT
   language: el
   title: Ο ΚΑΥΚΑΣΙΑΝΟΣ ΚΥΚΛΟΣ ΜΕ ΤΗ ΚΙΜΩΛΙΑ
   dewey: 832 ΜΠΡ
   entry_numbers:
   - '1573'
   translators:
   - ΒΑΜΒΑΛΗΣ,ΓΙΩΡΓΟΣ
@@ -39560,15 +39560,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 761
   authors:
-  - ΜΠΟΤΣΑΡΗΣ,ΔΗΜ Τ ΝΟΤΗ
+  - ΜΠΟΤΣΑΡΗΣ,ΔΗΜΗΤΡΙΟΣ,Τ. ΝΟΤΗ
   language: el
   title: ΑΓΩΝΕΣ ΕΛΕΥΘΕΡΙΑΣ
   dewey: 938.526 ΜΠΟ
   entry_numbers:
   - '2769'
   - 09260
   editor: None // ΑΘΗΝΑ
@@ -78844,15 +78844,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1523
   authors:
-  - ΖΟΥΡΝΑΤΖΗΣ,ΣΠ
+  - ΖΟΥΡΝΑΤΖΗΣ,ΣΠΥΡΟΣ
   language: el
   title: Η ΠΟΛΙΤΙΚΗ ΤΩΝ ΕΠΙΜΗΘΕΩΝ ΚΑΙ Η ΠΕΡΙΠΤΩΣΙΣ ΜΑΡΚΕΖΙΝΗ
   dewey: 938.772 ΖΟΥ
   entry_numbers:
   - '2792'
   edition: '2'
   editor: None // ΑΘΗΝΑ
@@ -78996,15 +78996,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1526
   authors:
-  - ΖΙΑΓΚΟΣ,ΝΙΚΟΣ
+  - ΖΙΑΓΚΟΣ,ΝΙΚΟΣ,Γ.
   language: el
   title: Η ΑΝΤΙΣΤΑΣΗ ΤΩΝ ΣΟΥΛΙΩΤΩΝ ΚΑΙ Ο ΛΑΜΠΡΟΣ ΤΖΑΒΕΛΛΑΣ
   dewey: 938.526 ΖΙΑ
   entry_numbers:
   - '2841'
   editor: None // ΑΘΗΝΑ
   edition_year: 1964
@@ -79259,15 +79259,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1531
   authors:
-  - ΜΠΑΛΑΣΚΑΣ,ΑΛΕΞΑΝΔΡΟΣ Α
+  - ΜΠΑΛΑΣΚΑΣ,ΑΛΕΞΑΝΔΡΟΣ,Α.
   language: el
   title: ΧΡΟΝΟΓΡΑΦΗΜΑΤΑ
   subtitle: ΕΝΟΣ ΑΘΗΝΑΙΟΥ ΔΗΜΟΣΙΟΓΡΑΦΟΥ
   dewey: 889.21 ΜΠΑ
   entry_numbers:
   - '2886'
   editor: None // ΑΘΗΝΑ
@@ -80171,15 +80171,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1549
   authors:
-  - ΜΠΡΟΥΠΗΣ,ΜΙΧΑΛΗΣ ΒΑΣ
+  - ΜΠΡΟΥΠΗΣ,ΜΙΧΑΛΗΣ,ΒΑΣ.
   language: el
   title: ΑΘΗΝΑΓΟΡΑ Α' ΟΙΚΟΥΜ.ΠΑΤΡΙΑΡΧΗ ΠΡΟΣΤΟ ΒΑΣΙΛΗ ΚΡΑΨΙΤΗ ΑΝΕΚΔΟΤΕ
   subtitle: ΕΠΙΣΤΟΛΕΣ ΤΟΥ
   dewey: 889.40 ΜΠΡ
   entry_numbers:
   - '2871'
   editor: None // ΑΘΗΝΑ
@@ -80276,15 +80276,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1551
   authors:
-  - ΖΩΓΡΑΦΟΥ ΜΑΡΙΝΑ
+  - ΖΩΓΡΑΦΟΥ,ΜΑΡΙΝΑ
   title: TARANTELLE EROTIQUE
   dewey: 889.11 ΖΩΓ
   entry_numbers:
   - '10392'
   editor: ΕΥΣΤΑΘΙΟΥ // ΑΘΗΝΑ
   edition_year: 1991
   pages: 109
@@ -81801,15 +81801,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1580
   authors:
-  - ΜΠΡΑΜΟΣ,ΚΩΣΤΑΣ Α
+  - ΜΠΡΑΜΟΣ,ΚΩΣΤΑΣ,Α.
   language: el
   title: ΣΛΑΒΙΚΗ ΠΡΟΠΑΓΑΝΔΑ ΚΑΙ ΕΠΑΝΑΣΤΑΤΙΚΗ ΔΡΑΣΗ ΣΤΗ ΜΑΚΕΔΟΝΙΑ
   dewey: 938.692 ΜΠΡ
   entry_numbers:
   - '2897'
   editor: None // ΑΘΗΝΑ
   edition_year: 1992
@@ -82265,15 +82265,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1589
   authors:
-  - ΜΠΟΖΙΟΣ,ΙΩΑΝΝΗΣ Θ
+  - ΜΠΟΖΙΟΣ,ΙΩΑΝΝΗΣ,Θ.
   language: el
   title: ΕΙΘΟΣ ΚΑΙ ΑΓΩΓΗ
   dewey: 185.1 ΜΠΟ
   entry_numbers:
   - '2913'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1976
@@ -87272,15 +87272,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1686
   authors:
-  - ΜΠΙΟΤ,ΡΕΝΕ
+  - BIOT,RENÉ
   language: el
   title: Η ΥΓΕΙΑ ΜΑΣ
   dewey: 131.3 ΒΙΟ
   entry_numbers:
   - '2978'
   translators:
   - ΧΑΡΟΚΟΠΟΥ,ΔΗΜΗΤΡΗΣ
@@ -87811,15 +87811,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1696
   authors:
-  - ΖΑΓΚΟΥΙΝ,ΚΙΟΥ
+  - JACQUIN,GUY
   language: el
   title: ΒΑΣΙΚΕΣ ΓΡΑΜΜΕΣ ΑΠΟ ΤΗΝ ΨΥΧΟΛΟΓΙΑ ΤΟΥ ΠΑΙΔΙΟΥ
   dewey: 136.73 ΖΑΓ
   entry_numbers:
   - '2970'
   translators:
   - ΟΛΙΕΒΙΕΡΗ,Χ.
@@ -90076,15 +90076,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1740
   authors:
-  - ΖΙΜΕΡ,ΑΛΦΡΕΤ
+  - ZIMMERN,ALFRED
   language: el
   title: ΑΙ ΠΟΛΙΤΕΙΑΙ ΤΗΣ ΑΡΧΑΙΑΣ ΕΛΛΑΔΟΣ
   dewey: 938.1 ΖΙΜ
   entry_numbers:
   - '3632'
   translators:
   - ΤΣΑΜΑΔΟΣ,ΜΙΧ.
@@ -90129,15 +90129,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1741
   authors:
-  - BROCKHUS
+  - BROCKHAUS
   language: de
   title: ZWEITER BAND F.K
   dewey: 030 BRO
   entry_numbers:
   - '3370'
   editor: BROCKHAUS // LEIPZIG
   edition_year: 1923
@@ -90586,15 +90586,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 1750
   authors:
-  - BELOCH KARL
+  - BELOCH,KARL,JULIUS
   language: de
   title: GRIECHISCHE GESCHICHTE
   dewey: 938 BEL
   entry_numbers:
   - '3066'
   editor: GRUYTER // BERLIN
   edition_year: 1926
@@ -90834,15 +90834,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 1755
   authors:
-  - BERNOYLLI ZZ
+  - BERNOULLI,JOHANN,JACOB
   language: de
   title: GRIECHISCHE IKONOGRAPHIE MIT AYSSCHLYSS ALEXADERYND
   subtitle: DIADOCHEN I-II
   dewey: 938.174 BER
   entry_numbers:
   - '3362'
   editor: BRYCMANN // MUNCHEN
@@ -90885,15 +90885,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1756
   authors:
-  - ZAE WERNER
+  - JAEGER,WERNER,WILHELM
   language: de
   title: DEMOSTHENES DER STAATSMANN UND SEIN WERDEN
   dewey: 938.105 ZAE
   entry_numbers:
   - '3149'
   editor: CRUYTER // BERLIN
   edition_year: 1963
@@ -90984,15 +90984,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1758
   authors:
-  - BENGTSON HERMANN
+  - BENGTSON,HERMANN
   language: de
   title: GRIECHISCHE GESCHICHTE
   dewey: 938.19 BEN
   entry_numbers:
   - '3103'
   editor: BECK'SCHE // MUNCHEN
   edition_year: 1950
@@ -91137,15 +91137,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 1761
   authors:
-  - BERVE HELMYT
+  - BERVE,HELMUT
   language: de
   title: GRIECHISCHE GESCHICHTE
   dewey: 938 BER
   entry_numbers:
   - '3073'
   editor: HERDER // FREIBURG
   edition_year: 1931
@@ -91499,15 +91499,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 1768
   authors:
-  - BYRKHARDT ZACOB
+  - BURCKHARDT,JACOB
   language: de
   title: GRIECHISCHE KYLTYR GESCHICHTE
   dewey: 938.06 BYR
   entry_numbers:
   - '3065'
   editor: GMBH // MUNCHEN
   edition_year: 1977
@@ -91960,15 +91960,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 1777
   authors:
-  - BENGTSON HERMANN
+  - BENGTSON,HERMANN
   language: de
   title: EINFYHHRYNG IN DIE ALTE CESHICHTE
   dewey: 909 BEN
   entry_numbers:
   - '3414'
   editor: BECK // MUNCHEN
   edition_year: 1965
@@ -92368,15 +92368,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 1785
   authors:
-  - BEHRENDT RICHARD
+  - BEHRENDT,RICHARD
   language: de
   title: POLITISCHER AKTIVISMUS
   dewey: 301 BEH
   entry_numbers:
   - '3533'
   editor: HIRSCHFELD // LEIPZIG
   edition_year: 1932
@@ -92473,15 +92473,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 1787
   authors:
-  - BRENTANO LUZO
+  - BRENTANO,LUJO
   language: de
   title: DAS WIRTSCHAFTSLEBEN DER ANTIKEN WELT
   dewey: 330 BRE
   entry_numbers:
   - '3568'
   editor: FISCHER // ZENA
   edition_year: 1929
@@ -92576,15 +92576,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1789
   authors:
-  - BUTTNER HERMANN
+  - BUTTNER,HERMANN
   language: de
   title: GESICHTE DER POLITISCHEN HETAHRIEEN IN ATHEN
   dewey: 938.122 BUT
   entry_numbers:
   - '3578'
   editor: BRADES // LEIPZIG
   edition_year: 1840
@@ -92881,15 +92881,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1795
   authors:
-  - BERVE HELMUT
+  - BERVE,HELMUT
   language: de
   title: DAS NEUE BILD DER ANTIKE-HELLAS
   dewey: 938.1 BER
   entry_numbers:
   - '3619'
   editor: KOEHLER // LEIPZIG
   topics:
@@ -92980,15 +92980,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 1797
   authors:
-  - BLASS FRIEDRICH
+  - BLASS,FRIEDRICH
   language: de
   title: DIE ATTISCHE BEREDSAM KEIT
   dewey: 186.3 BCA
   entry_numbers:
   - '3375'
   editor: TEUBNER // LEIPZIG
   edition_year: 1877
@@ -93031,15 +93031,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1798
   authors:
-  - BLASS FRIEDRICH
+  - BLASS,FRIEDRICH
   language: de
   title: DIE ATTISCHE BEREDSAMKEIT DEMOSTHENES GENOSSEN UND GEGNER
   dewey: 938.105 BLA
   entry_numbers:
   - '3150'
   editor: TEUBNER // LEIPZIG
   edition_year: 1898
@@ -93136,15 +93136,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1800
   authors:
-  - ZAHRNT MICHAEL
+  - ZAHRNT,MICHAEL
   language: de
   title: OLYNTH UND DIE CHALKIDIER
   dewey: 938.946 ZAH
   entry_numbers:
   - '3244'
   editor: BECK // MUNCHEN
   edition_year: 1971
@@ -93286,15 +93286,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1803
   authors:
-  - BAYER ERIGH
+  - BAYER,ERIGH
   language: de
   title: DEMETRIOS PHALERYS DER ATHENER
   dewey: 881.092 BAY
   entry_numbers:
   - '3353'
   editor: KOHLHMMER // BERLIN
   edition_year: 1942
@@ -93592,15 +93592,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 1809
   authors:
-  - BERNE HELMUT
+  - BERNE,HELMUT
   language: de
   title: DIE TYRANNIS BEI GRIECHEN
   dewey: 938.19 BER
   entry_numbers:
   - '3359'
   editor: BECK'SCHE // MUNCHEN
   edition_year: 1967
@@ -94164,15 +94164,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 1820
   authors:
-  - ZACOBY FELIX
+  - JACOBY,FELIX
   language: de
   title: DIE FRACMENTE DER GRIECHI SCHEN HISTORIKE
   dewey: 938.02 ZAC
   entry_numbers:
   - '3372'
   editor: BRILL // LEIDEN
   edition_year: 1954
@@ -95324,15 +95324,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1843
   authors:
-  - BENDIXEN F
+  - BENDIXEN,FRIEDRICH
   title: GELD UND KAPITAL
   dewey: 332 BEN
   entry_numbers:
   - '3397'
   editor: FISCHER // JENA
   edition_year: 1922
   topics:
@@ -95428,15 +95428,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1845
   authors:
-  - BAND ERSTER
+  - BAND,ERSTER
   language: de
   title: HANBYCH DER FINANZWISSEN SCHAFT
   dewey: 336 BAN
   entry_numbers:
   - '3399'
   editor: MOHR // TUBINGEN
   edition_year: 1926
@@ -95534,15 +95534,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1847
   authors:
-  - BONIS KONSTANTIN
+  - ΜΠΟΝΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
   language: de
   title: DIE SLAWENAPOSTEL KYRILLOS UND METHODIOS YND DIE BASILIKA
   subtitle: DES HL DEMETRIOS VON THESSALONIKH
   dewey: 938.2 BON
   entry_numbers:
   - '3401'
   editor: None // ΑΘΗΝΑ
@@ -96399,15 +96399,17 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1864
   authors:
-  - BLAVATSKAJA-COLYBCOVA-PAVLOVSKAJA
+  - BLAVATSKAJA,TATJANA,V.
+  - GOLUBCOVA,ELENA,S.
+  - PAVLOVSKAJA,ALEKSANDRA,I.
   language: de
   title: DIE SKLAVEREI IN HELLEN ISTISCHEN STAATEN IM 3-I JH.VCHR
   dewey: 938.4 BLA
   entry_numbers:
   - '3422'
   editor: STEINER // WIESBADEN
   edition_year: 1972
@@ -97106,15 +97108,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1878
   authors:
-  - BENGTSON HERMANN
+  - BENGTSON,HERMANN
   language: de
   title: DIE STRATEGIE IN DER HELLENISTISCHEN ZEIT
   dewey: 938.035 BEN
   entry_numbers:
   - '3437'
   editor: BECK'SCHE // MUNCHEN
   edition_year: 1964
@@ -97459,15 +97461,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1885
   authors:
-  - BARTHOLOY KARI
+  - BARTHOLOY,KARI
   language: de
   title: GESICHTE GRIECHENLAND
   dewey: 938.42 BAR
   entry_numbers:
   - '3445'
   editor: HIRZEL // LEIPZIG
   edition_year: 1870
@@ -97963,15 +97965,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 1895
   authors:
-  - BER HANS
+  - GERBER,HANS
   language: de
   title: FREIHEIT UNT BINDUNG DER STAATSAGEWALT
   dewey: 320 GER
   entry_numbers:
   - '3455'
   editor: MOHR // TUBINGEN
   edition_year: 1932
@@ -98575,15 +98577,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 1907
   authors:
-  - BOHM-BAWERK
+  - VON BÖHM-BAWERK,EUGEN
   language: de
   title: KAPITAL UND KAPITALZINS POSITIVE TEORIE DES KAPITALES
   dewey: 335 BOH
   entry_numbers:
   - '3470'
   editor: FISCHER // JENA
   edition_year: 1921
@@ -98825,15 +98827,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1912
   authors:
-  - JAE WERNER
+  - JAEGER,WERNER,WILHELM
   language: de
   title: DIOKLES VON KARYSTOS
   dewey: 140 JAE
   entry_numbers:
   - '3473'
   editor: GR UYTER // BERLIN
   edition_year: 1963
@@ -99179,15 +99181,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1919
   authors:
-  - BOHM-BAWERK
+  - VON BÖHM-BAWERK,EUGEN
   language: de
   title: KAPITAL UND KAPITALZINS
   dewey: 335 BOH
   entry_numbers:
   - '3480'
   editor: FISCHER // JENA
   edition_year: 1921
@@ -99330,15 +99332,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1922
   authors:
-  - BUSCHOR ERNST
+  - BUSCHOR,ERNST
   language: de
   title: DIE PLASTIK DER GRIECHEN
   dewey: 938 BUS
   entry_numbers:
   - '3483'
   editor: PIPER // MUNCHEN
   topics:
@@ -100540,15 +100542,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1946
   authors:
-  - BOEHRIN ERICH
+  - BOEHRIN,ERICH
   language: de
   title: DIE MYHNZE VON SYRAKYS TAFELN
   dewey: 938.101 BOE
   entry_numbers:
   - '3511'
   editor: GRUYTER // BERLIN
   edition_year: 1929
@@ -100693,15 +100695,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1949
   authors:
-  - BENGTSON HERMANN
+  - BENGTSON,HERMANN
   language: de
   title: DIE VERTRAHGE DER GRIECHISCH-ROMISCHW WELT VON 700 BIS
   subtitle: 338V CHR
   dewey: 938.192 BEN
   entry_numbers:
   - '3517'
   editor: BECK'SCHE // MUNCHEN
@@ -100897,15 +100899,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1953
   authors:
-  - BRELOER BERNHARD
+  - BRELOER,BERNHARD
   language: de
   title: ALEXANDERS KAMPF GEGEN POROS
   dewey: 938.174 BRE
   entry_numbers:
   - '3522'
   editor: KOHLHAMMER // STUTTGART
   edition_year: 1933
@@ -101248,15 +101250,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1960
   authors:
-  - BONIS KONSTANTIN
+  - ΜΠΟΝΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
   language: de
   title: GREGORIS PALAMAS DER GROSSEN BYZANTINISCHEN THEOLOGEN ATHE
   dewey: 938.3 BON
   entry_numbers:
   - '3530'
   editor: None // ΑΘΗΝΑ
   edition_year: 1979
@@ -102061,15 +102063,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1976
   authors:
-  - BELOCH KARL
+  - BELOCH,KARL,JULIUS
   language: de
   title: ROHMISCHE GESCHICHTE
   dewey: 945 BEL
   entry_numbers:
   - '3550'
   editor: GRUTER // BERLIN
   edition_year: 1926
@@ -102158,15 +102160,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1978
   authors:
-  - BOTH KARL
+  - BOTH,KARL
   language: de
   title: ROHMISCHE GESCHICHTE
   dewey: 945 BOT
   entry_numbers:
   - '3552'
   editor: BECK'SCHE // MUNCHEN
   edition_year: 1922
@@ -102758,15 +102760,17 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1990
   authors:
-  - BAUMGARTEN-POLAND-WAGNER
+  - BAUMGARTEN,FRITZ
+  - WAGNER,RICHARD,ANTON
+  - POLAND,FRANZ
   language: de
   title: DIE HELLENISCHE KULTUR
   dewey: 938.06 BAU
   entry_numbers:
   - '3564'
   editor: TEUBNER // LEIPZIG
   edition_year: 1913
@@ -103919,15 +103923,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2013
   authors:
-  - BELOCH JULIUS
+  - BELOCH,KARL,JULIUS
   language: de
   title: DIE ATTISCHE POLITIK SEIT PERIKLES
   dewey: 938.145 BEL
   entry_numbers:
   - '3590'
   editor: TEUBNER // STUTTGART
   edition_year: 1967
@@ -104070,15 +104074,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2016
   authors:
-  - BELOCH JULIUS
+  - BELOCH,KARL,JULIUS
   language: de
   title: DER ITALISCHE BUND UNTER ROMS HEGEMONIE
   dewey: 938.192 BEL
   entry_numbers:
   - '3596'
   editor: L'ERMA // ROMA
   edition_year: 1964
@@ -104170,15 +104174,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2018
   authors:
-  - BARTH PAUL
+  - BARTH,PAUL
   language: de
   title: DIE PHILOSOPHIE DER GESCHICHTE ALS SOZIOLIGIE
   dewey: 301 BAR
   entry_numbers:
   - '3598'
   editor: REISLAND // LEIPZIG
   edition_year: 1922
@@ -104219,15 +104223,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2019
   authors:
-  - BLOCH IWAN
+  - BLOCH,IWAN
   language: de
   title: DIE PROSTITUTION
   dewey: 390 BLO
   entry_numbers:
   - '3599'
   editor: MARCUS // BERLIN
   edition_year: 1925
@@ -104570,15 +104574,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2026
   authors:
-  - BENGTSON HERMANN
+  - BENGTSON,HERMANN
   language: de
   title: GRUNDRIESS DER ROHMISCHEN GESCHICHTE
   subtitle: REPUBLIK UND KAISERZEIT BIS 284 H CHR
   dewey: 945 BEN
   entry_numbers:
   - '3610'
   editor: BECK // MUNCHEN
@@ -105070,15 +105074,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2036
   authors:
-  - BENGTSON HERMANN
+  - BENGTSON,HERMANN
   language: de
   title: MARCYS ANTONYS TRIYM VIR YND HERRSCHER DES ORIENTS
   dewey: 937 BEN
   entry_numbers:
   - '3134'
   editor: CHBECK // MYHNMUNCHENCHN
   edition_year: 1977
@@ -105381,15 +105385,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2042
   authors:
-  - BURCKHARDT JACOD
+  - BURCKHARDT,JACOB
   language: de
   title: DIE ZEIT KOSTANTINS DES GROSSEN
   dewey: 938.311 BUR
   entry_numbers:
   - '3090'
   editor: KROHNER // LEIPZIG
   edition_year: 1924
@@ -106035,15 +106039,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2055
   authors:
-  - BIRT THEODOR
+  - BIRT,THEODOR
   language: de
   title: ROHMISCHE CHARAKTERKAH SE
   dewey: 938.192 BIR
   entry_numbers:
   - '3115'
   editor: OUELLE // LEIPZIG
   edition_year: 1918
@@ -106442,15 +106446,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2063
   authors:
-  - BARTHOLDN KARL
+  - MENDELSSOHN BARTHOLDY,KARL
   language: de
   title: GESCHICHTE GRIECHENLANS VON DER EROBERNUNG KONSTANTINOPELS
   dewey: 938.389 BAR
   entry_numbers:
   - '3106'
   editor: HIRZEL // LEIPZIG
   edition_year: 1874
@@ -106544,15 +106548,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2065
   authors:
-  - BUSOLT GEORG
+  - BUSOLT,GEORG
   language: de
   title: CRIECHISCHE STAATSKUN DE
   dewey: 938.032 BUS
   entry_numbers:
   - '3102'
   editor: BECK // MUNCHEN
   edition_year: 1920
@@ -106754,15 +106758,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2069
   authors:
-  - BERVE HELMUT
+  - BERVE,HELMUT
   language: de
   title: DAS NEUE BILD DER ANTIKEN
   dewey: 938.1 BER
   entry_numbers:
   - '3070'
   editor: KOEHLER // LEIPZIG
   topics:
@@ -107103,15 +107107,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2076
   authors:
-  - BERNE HELMUT
+  - BERNE,HELMUT
   language: de
   title: DAS ALEXANDERREICH AUF PROSOPOGRAPHISCHER GRUNLAGE
   dewey: 938.174 BER
   entry_numbers:
   - '3091'
   editor: BECK'SCHE // MUNCHEN
   topics:
@@ -107356,15 +107360,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 2081
   authors:
-  - BUSCH-ZANTNER RICHARD
+  - BUSCH-ZANTNER,RICHARD
   language: de
   title: BULGARIEN
   dewey: 949 BUS
   entry_numbers:
   - '3085'
   editor: COLDANN // LEIPZIG
   edition_year: 1941
@@ -107756,15 +107760,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 2089
   authors:
-  - BEKGTSON HERMANN
+  - BENGTSON,HERMANN
   language: de
   title: HERRSCHERGESTALTE DES HELLENISMUS
   dewey: 938 BEK
   entry_numbers: []
   editor: BECK // MUNCHEN
   edition_year: 1975
   topics:
@@ -107855,15 +107859,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2091
   authors:
-  - BERGK THEODOR
+  - BERGK,THEODOR
   language: de
   title: CRIECHISCHE LITERATUR GESCHICHTE
   dewey: 880.09 BER
   entry_numbers:
   - '3121'
   editor: WEIDAMANN // BERLIN
   edition_year: 1883
@@ -108008,15 +108012,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2094
   authors:
-  - BREITENBACH H
+  - BREITENBACH,HANS,RUDOLF
   language: de
   title: XENOPHON VON ATHEN
   dewey: 938.1 BRE
   entry_numbers:
   - '3124'
   editor: DRUCKENMUHLLER // STUTTGART
   edition_year: 1966
@@ -108612,15 +108616,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2106
   authors:
-  - BRANDSTAETER
+  - BRANDSTÄTER,FRANZ,AUGUST
   language: de
   title: GESCHICHTEN AETOLISCHEN LANDES-VOLKES YND BYNDES
   dewey: 838.22 BRA
   entry_numbers:
   - '3143'
   editor: KAIMER // BERLIN
   edition_year: 1844
@@ -109006,15 +109010,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2114
   authors:
-  - BLASS FRIEDRICH
+  - BLASS,FRIEDRICH
   language: de
   title: DIE ATTISCHE BEREDSAMKEIT ISOKRATES UND ISAIOS
   dewey: 881.55 BLA
   entry_numbers:
   - '3153'
   editor: TEUBNER // LEIPZIG
   edition_year: 1892
@@ -111223,15 +111227,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2158
   authors:
-  - BACK JOSEF
+  - BACK,JOSEF
   language: de
   title: DIE ENTWICKLUNG DER REINEN OHKONOMIE
   dewey: 330.1 BAC
   entry_numbers:
   - '3214'
   editor: FISCHER // JENA
   edition_year: 1929
@@ -111321,15 +111325,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2160
   authors:
-  - ZOLLIN WALTER
+  - ZOLLINGER,WALTER
   language: de
   title: DIE INFLATIONS-THEORIE AUF IRRWEGEN
   dewey: 301.3 ZOL
   entry_numbers:
   - '3216'
   editor: HUBER // FRAUENFELD
   edition_year: 1962
@@ -111471,15 +111475,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2163
   authors:
-  - BOHCKH AUGUST
+  - BÖCKH,AUGUST
   language: de
   title: STAATHAUSHALTUNG DER ATHENER
   dewey: 938.122 BOH
   entry_numbers:
   - '3219'
   editor: REIMER // BERLIN
   edition_year: 1886
@@ -112025,15 +112029,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2174
   authors:
-  - BER HUGO
+  - BERGER,ERNST,HUGO
   language: de
   title: GESCHICHTE DER WISSENSCHAFTLICHEN
   subtitle: ERKUNDE DER GRIECHEN
   dewey: 914.95 BER
   entry_numbers:
   - '3629'
   editor: VEIT // LEIPZIG
@@ -112373,15 +112377,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2181
   authors:
-  - BAHRDT HANS
+  - BAHRDT,HANS,PAUL
   language: de
   title: WEGE ZUR SOZIOLOGIE
   dewey: 301 BAH
   entry_numbers:
   - '3224'
   topics:
   - ΚΟΙΝΩΝΙΟΛΟΓΙΑ
@@ -113078,15 +113082,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2195
   authors:
-  - BETHMANN-HOLLWEG TH
+  - VON BETHMANN HOLLWEG,THEOBALD
   language: de
   title: BETRACHTUNGE ZUM WELT KRIEGE
   dewey: 904 BET
   entry_numbers:
   - '3240'
   editor: HOBBING // BERLIN
   edition_year: 1921
@@ -113332,15 +113336,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2200
   authors:
-  - BENGRSON HERMANN
+  - BENGTSON,HERMANN
   language: de
   title: GRIECHEN UND PERSER
   dewey: 938.1 BEN
   entry_numbers:
   - '3246'
   editor: FISCHER // FRANKFURT
   edition_year: 1965
@@ -113383,15 +113387,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2201
   authors:
-  - BUHRCHNER L
+  - BUHRCHNER,L.
   language: de
   title: EPHESOS
   dewey: 938.1 BUH
   entry_numbers:
   - '3247'
   editor: None // MUNCHEN
   edition_year: 1905
@@ -113634,15 +113638,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 2206
   authors:
-  - BOSCH GLEMENS
+  - BOSCH,CLEMENS
   language: de
   title: DIE OUELLEN DES VALERIUS MAXIMUS
   dewey: 938 BOS
   entry_numbers:
   - '3252'
   editor: KOHLHAMMER // STUTTGART
   edition_year: 1929
@@ -113792,15 +113796,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 2209
   authors:
-  - BELOCH JULIUS
+  - BELOCH,KARL,JULIUS
   language: de
   title: CAMPANIEN
   dewey: 945 BEL
   entry_numbers:
   - '3255'
   editor: L'ERMA // ROMA
   edition_year: 1964
@@ -114343,15 +114347,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 2220
   authors:
-  - BIRT THEODOR
+  - BIRT,THEODOR
   language: de
   title: ALEXANDER DER GROSSE UND DAS WELTGRIECHENTUN
   dewey: 938.174 BIR
   entry_numbers:
   - '3266'
   editor: MEYER // LEIPZIG
   edition_year: 1925
@@ -114647,15 +114651,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2226
   authors:
-  - BRAHUTIGEM OTTO
+  - BRAUTIGAM,OTTO
   language: de
   title: DIE LANDWIRTSCHAFT IN DER SOWJETUNION
   dewey: 947 BRA
   entry_numbers:
   - '3272'
   editor: STOLLBERG // BERLIN
   topics:
@@ -115339,15 +115343,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2240
   authors:
-  - BELOCH JULIUS
+  - BELOCH,KARL,JULIUS
   language: de
   title: DIE BEVOHLKERUNG DER GRIECHISCH-ROEMISCHEN WELT
   dewey: 938.19 BEL
   entry_numbers:
   - '3285'
   editor: L'ERMA // ROMA
   edition_year: 1968
@@ -116561,15 +116565,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2264
   authors:
-  - BLYMENTHAL ALBERT
+  - BLUMENTHAL,ALBERT,H.
   language: de
   title: GRIECHISCHE VORBILDE-VERSYCH EINER DEYTYNG HEROISCHEN IM   H
   subtitle: SCHRIFTTYME DER HELLENEN
   dewey: 407 BLY
   entry_numbers:
   - '3312'
   editor: KOHLHAMMER // STUTTGART
@@ -116614,15 +116618,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 2265
   authors:
-  - BEAYFRE
+  - BEAUFRE,ANDRE
   language: de
   title: TOTALE KRIEGSKYNST IM FRIEDEN EIN FHHRYNG IN DIE STRATEGIE
   dewey: 355 BEA
   entry_numbers:
   - '3313'
   editor: PROPYLAHEN // BERLIN
   edition_year: 1963
@@ -117738,15 +117742,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2287
   authors:
-  - ZIZEK FRANZ
+  - ZIZEK,FRANZ
   language: de
   title: GRUNDRISS DER STATISTIK
   dewey: 311 ZIZ
   entry_numbers:
   - '3338'
   editor: DUNCKER // MUNCHEN
   edition_year: 1923
@@ -118092,15 +118096,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2294
   authors:
-  - BURSIAN CONRAD
+  - BURSIAN,CONRAD
   language: de
   title: GEOGRAPHIE VON GRIECHEN LAND
   dewey: 914.95 BUR
   entry_numbers:
   - '3345'
   editor: TEUBNER // LEIPZIG
   edition_year: 1862
@@ -118394,15 +118398,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2300
   authors:
-  - BROHCKER WALTER
+  - BRÖCKER,WALTER
   language: de
   title: DIE GESICHTE DER PHILOSOPHIE VOR SOKRATES
   dewey: 183.2 BRO
   entry_numbers:
   - '3352'
   editor: KLOSTERMANN // FRANKFURT
   edition_year: 1965
@@ -119003,15 +119007,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2312
   authors:
-  - ΜΠΕΛΙΑ,ΕΛΕΝΗ Δ
+  - ΜΠΕΛΙΑ,ΕΛΕΝΗ,Δ.
   language: el
   title: Η ΕΚΠΑΙΔΕΥΣΙΣ ΕΙΣ ΤΗΝ ΛΑΚΩΝΙΑΝ ΚΑΙ ΤΗΝ ΜΕΣΣΗΝΙΑΝ ΚΑΤΑ ΤΗΝ  Α
   subtitle: ΚΑΠΟΔΙΣΤΡΙΑΚΗΝ ΠΕΡΙΟΔΟΝ (1828-1832)
   dewey: 938.572 ΜΠΕ
   entry_numbers:
   - '3660'
   editor: None // ΑΘΗΝΑ
@@ -119774,15 +119778,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2327
   authors:
-  - ΒΛΑΧΟΣ,ΑΓΓΕΛΟΣ,ΣΤ,
+  - ΒΛΑΧΟΣ,ΑΓΓΕΛΟΣ,ΣΤ.
   language: el
   title: ΜΕΡΟΛΗΨΙΕΣ ΤΟΥ ΘΟΥΚΥΔΙΔΗ
   subtitle: ΔΟΚΙΜΙΟ
   dewey: 881.2 ΒΛΑ
   entry_numbers:
   - '2927'
   editor: ΕΣΤΙΑ // ΑΘΗΝΑ
@@ -120080,15 +120084,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2333
   authors:
-  - ΜΠΑΚΟΣ,ΗΛΙΑΣ Δ
+  - ΜΠΑΚΟΣ,ΗΛΙΑΣ,Δ.
   language: el
   title: ΒΥΖΑΝΤΙΝΗ ΠΟΙΗΣΙΣ ΚΑΙ ΕΙΚΟΝΟΜΑΧΙΚΑΙ ΕΡΙΔΕΣ
   dewey: 880.9 ΜΠΑ
   entry_numbers:
   - '3676'
   editor: None // ΑΘΗΝΑ
   edition_year: 1992
@@ -120494,15 +120498,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2341
   authors:
-  - ΖΙΟΥΤΟΣ,Γ.Δ
+  - ΖΙΟΥΤΟΣ,ΓΙΩΡΓΟΣ,Δ.
   language: el
   title: ΤΟ ΔΙΕΘΝΕΣ ΕΡΓΑΤΙΚΟ ΚΙΝΗΜΑ
   subtitle: ΣΤΟΝ 19 ΚΑΙ ΤΙΣ ΑΡΧΕΣ ΤΟΥ 20 ΑΙΩΝΑ
   dewey: 909 ΖΙΟ
   entry_numbers:
   - '3691'
   editor: None // ΑΘΗΝΑ
@@ -121939,15 +121943,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2369
   authors:
-  - BAUDELAIRE CHARLES
+  - BAUDELAIRE,CHARLES
   language: fr
   title: LES FLEURS DU MAL
   dewey: 840 BAU
   entry_numbers: []
   editor: BAUDOIN // PARIS
   topics:
   - ΓΑΛΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -121987,15 +121991,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2370
   authors:
-  - BAUDIN LOUIS
+  - BAUDIN,LOUIS
   language: fr
   title: LA MONNAIE ET LA FORMATION DES PRIX
   dewey: 938.5 BAU
   entry_numbers:
   - '4082'
   editor: RECUEIL SIREY // PARIS
   edition_year: 1936
@@ -122827,15 +122831,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2387
   authors:
-  - BORGEAUD WILLY
+  - BORGEAUD,WILLY
   language: de
   title: LES HLYRIENS EN GRECE ET EN ITALIE
   dewey: 938.1 BOR
   entry_numbers:
   - '4065'
   editor: ROULET // GENEVE
   edition_year: 1943
@@ -122980,15 +122984,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2390
   authors:
-  - BLOCH PAYMOND
+  - BLOCH,RAYMOND
   language: fr
   title: L'ART ET LA CIVILATION ETRUSOUES
   dewey: 945 BLO
   entry_numbers:
   - '4062'
   editor: PLON // PARIS
   edition_year: 1955
@@ -123433,15 +123437,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2399
   authors:
-  - BOLLACK JEAN
+  - BOLLACK,JEAN
   language: fr
   title: EMPEDOCLE-LES ORIGINES
   dewey: 182.5 GAL
   entry_numbers:
   - '4053'
   editor: MINUIT // PARIS
   edition_year: 1969
@@ -123687,15 +123691,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2404
   authors:
-  - BABELON ERNEST
+  - BABELON,ERNEST
   language: fr
   title: MONNAIES GRECOUES ET ROMAINES
   subtitle: DESCRIRTION HISTORIOUE
   dewey: 938.101 BAB
   entry_numbers:
   - '4048'
   editor: FORTI // BOLOGNA
@@ -123988,15 +123992,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2410
   authors:
-  - BABELON JEAN
+  - BABELON,JEAN
   language: fr
   title: LES MONNAIES RACONTET L'HISTORE
   dewey: 900 BAB
   entry_numbers:
   - '4042'
   editor: FAYARD // PARIS
   edition_year: 1963
@@ -124702,15 +124706,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 2424
   authors:
-  - BRAUDEL FERNAND
+  - BRAUDEL,FERNAND
   language: fr
   title: LA MEDITERANEE ET LE MONDE MEDITERRANEEN A L'EPOUE DE
   subtitle: PHILIRRE II
   dewey: 938.171 BRA
   entry_numbers:
   - '4028'
   editor: COLIN // PARIS
@@ -124955,15 +124959,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2429
   authors:
-  - BROCARD LUCIEN
+  - BROCARD,LUCIEN
   language: fr
   title: PRINCIPES D'ECONOMIE NATIOET INTERNATIONALE
   dewey: 330 BRO
   entry_numbers:
   - '4023'
   editor: SIREY // PARIS
   edition_year: 1929
@@ -126115,15 +126119,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2452
   authors:
-  - BOMMELAER JEAN
+  - BOMMELAER,JEAN
   language: fr
   title: LYSANDRE DE SPARTE HISTOIRE ET TRADITIONS
   dewey: 938.16 BOM
   entry_numbers:
   - '4000'
   editor: BOCCARD // PARIS
   edition_year: 1981
@@ -126165,15 +126169,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2453
   authors:
-  - BROCARD LUCIEN
+  - BROCARD,LUCIEN
   language: fr
   title: PRINCIPES D'ECONOMIE
   dewey: 330.1 BRO
   entry_numbers:
   - '3999'
   editor: SIREY // PARIS
   edition_year: 1929
@@ -126216,15 +126220,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2454
   authors:
-  - BOUSOUET BERNARD
+  - BOUSOUET,BERNARD
   language: fr
   title: LA GRECE OCCIDENTALE INTER PRETATION GEOMORPHO LO GIGIUE DE
   subtitle: LA ACARNANIE ET DES ILES IONIENNES
   dewey: 550 BOU
   entry_numbers:
   - '3998'
   editor: CHMPION // PARIS
@@ -126682,15 +126686,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2463
   authors:
-  - BOMPOIS FERDIANAND
+  - BOMPOIS,FERDINAND
   language: fr
   title: OBSERVATIONS SES UN DIDRACHME INEDIT DE LA VILLE DE
   subtitle: GIERIUM EN THESSALIE
   dewey: 938.21 BOM
   entry_numbers:
   - '3989'
   editor: DETAILLE // PARIS
@@ -126935,15 +126939,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2468
   authors:
-  - BORNECOUE HENRI
+  - BORNECQUE,HENRI
   language: fr
   title: SENEOUE LE RHETEUR CONTROVERSES ET SUASOIRES
   dewey: 188.6 BOR
   entry_numbers:
   - '3984'
   editor: CARNIER // PARIS
   edition_year: 1932
@@ -127235,15 +127239,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2474
   authors:
-  - BARON A
+  - BARON,AUGUSTE
   language: fr
   title: CALLINUS ET TYRTEE
   dewey: 937 BAR
   entry_numbers:
   - '3978'
   editor: MENINE // BRUXELLES
   edition_year: 1835
@@ -128538,15 +128542,16 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 2500
   authors:
-  - BLOCH RAYMOND-COYSIN JEAN
+  - BLOCH,RAYMOND
+  - COUSIN,JEAN
   language: fr
   title: ROME ET SON DESTIN
   dewey: 937 BLO
   entry_numbers:
   - '3952'
   editor: COLIN // None
   edition_year: 1960
@@ -128788,15 +128793,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2505
   authors:
-  - BOVET M
+  - DE BOVET,FRANÇOIS
   language: fr
   title: DES DYNASTIES EGYPTIENNES
   dewey: 962 BON
   entry_numbers:
   - '3947'
   editor: BLAISE // PARIS
   edition_year: 1930
@@ -130027,15 +130032,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2530
   authors:
-  - BARBALO CORRADO
+  - BARBAGALLO,CORRADO
   language: fr
   title: LE DECLIN D'UNE CIVILISATION OU LA FIN DE LA GRECE ANTIOUE
   dewey: 938.1 BAR
   entry_numbers:
   - '3922'
   editor: PAYOT // PARIS
   edition_year: 1927
@@ -130828,15 +130833,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2546
   authors:
-  - BRAUDEL FERNAND
+  - BRAUDEL,FERNAND
   language: fr
   title: LA MEDITERANEE ET LEMONDE MEDITERRANEEN AL'EPOΩUE
   subtitle: DE PHILIPPE II
   dewey: 938.296 BRA
   entry_numbers:
   - '3906'
   editor: COLIN // PARIS
@@ -130979,15 +130984,16 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2549
   authors:
-  - BABELON J LAFAURIE J
+  - BABELON,JEAN
+  - LAFAURIE,JEAN
   language: fr
   title: CONGRES INTERNATIONAL DE NUMISMATIOUE
   dewey: 332.4 BAB
   entry_numbers:
   - '3903'
   editor: BIBL NATIONALE // PARIS
   edition_year: 1957
@@ -131080,15 +131086,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 2551
   authors:
-  - ZIELINSKI TH
+  - ZIELINSKI,TADEUSZ
   language: fr
   title: HISTOIRE DE LA CINILISATION ANTIOUE
   dewey: 900 ZIE
   entry_numbers:
   - '3901'
   editor: PAYOT // PARIS
   edition_year: 1931
@@ -131574,15 +131580,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2561
   authors:
-  - BONNARD ANDRE
+  - BONNARD,ANDRÉ
   language: fr
   title: CIVILISATION GREGOUE
   dewey: 938.06 BON
   entry_numbers:
   - '3891'
   editor: LA CUILDE LIVRE // LAUSANNE
   edition_year: 1954
@@ -131626,15 +131632,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2562
   authors:
-  - BONNARD ANDRE
+  - BONNARD,ANDRÉ
   language: fr
   title: CIVILISATION GRECOUE
   dewey: 938.06 BON
   entry_numbers:
   - '3890'
   editor: LA CUILDE DU LIVRE // LAUSANNE
   edition_year: 1956
@@ -132326,15 +132332,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 2576
   authors:
-  - BERARO VICTOR
+  - BÉRARD,VICTOR
   language: fr
   title: ITHAOUE ET LA GRECE DES AHEENS
   dewey: 938.26 BER
   entry_numbers:
   - '3876'
   editor: COLIN // PARIS
   edition_year: 1927
@@ -133334,15 +133340,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2596
   authors:
-  - BETTELHEIM CR
+  - BETTELHEIM,CHARLES
   language: fr
   title: L'ECONOMIE SOVIETIOUE
   dewey: 947 BET
   entry_numbers:
   - '3851'
   editor: RECUEIL // PARIS
   edition_year: 1950
@@ -134033,15 +134039,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2610
   authors:
-  - BESNIER MAURICE
+  - BESNIER,MAURICE
   language: fr
   title: L'EMPIRE ROMAIN DE L'AVENEMENT DES SEVERES AU AU CONCILE DU
   subtitle: NICEE
   dewey: 938.192 BES
   entry_numbers:
   - '3838'
   editor: PRESS UNIVERSITAIRES // PARIS
@@ -134536,15 +134542,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 2620
   authors:
-  - BLANC ANDRE
+  - BLANC,ANDRE
   language: fr
   title: L'ECONOMIE DES BALKANS
   dewey: 330 BLA
   entry_numbers:
   - '3828'
   editor: UNIVERSITAIRE // PARIS
   edition_year: 1965
@@ -134940,15 +134946,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2628
   authors:
-  - BONNARD ANDRE
+  - BONNARD,ANDRÉ
   language: fr
   title: CIVISATION GREGOUE
   dewey: 938.06 BON
   entry_numbers:
   - '3819'
   editor: None // LAUSANNE
   edition_year: 1954
@@ -135190,15 +135196,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2633
   authors:
-  - BOUTHOUL GASTON
+  - BOUTHOUL,GASTON
   language: fr
   title: L'ART DE LA POLITIGUE
   dewey: 329 BOU
   entry_numbers:
   - '3861'
   editor: SECHERS // PARIS
   topics:
@@ -135488,15 +135494,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2639
   authors:
-  - BLOCH GUSTAVE
+  - BLOCH,GUSTAVE
   language: fr
   title: HISTOIRE ROMAINE-LA REPUBLIOUE ROMAINE DE 133 AVANT J LA
   subtitle: MORT DE CESAR DES GRACOUES A SULLA
   dewey: 937 BLO
   entry_numbers:
   - '3813'
   editor: UNIVERSITAIRES // PARIS
@@ -135644,15 +135650,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 2642
   authors:
-  - BELOT EMILE
+  - BELOT,EMILE
   language: fr
   title: LA REPUBLIOUE D'ATHENES
   dewey: 938.122 BEL
   entry_numbers:
   - '3810'
   editor: PEDONE-LAURIEL // PARIS
   edition_year: 1880
@@ -136149,15 +136155,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2652
   authors:
-  - BOWRA C.M
+  - BOWRA,CECIL,MAURICE
   language: fr
   title: L'EXPERIENCE GREGUE
   dewey: 938.1 BOW
   entry_numbers:
   - '3800'
   editor: FAYARD // PARIS
   edition_year: 1969
@@ -136248,15 +136254,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2654
   authors:
-  - BOLLACK JEAN
+  - BOLLACK,JEAN
   language: fr
   title: EMPEDOCLE-LES ORIGINES
   dewey: 881.03 BOL
   entry_numbers:
   - '3798'
   editor: MINUIT // PARIS
   edition_year: 1969
@@ -136798,15 +136804,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2665
   authors:
-  - BAYET C
+  - BAYET,CHARLES,MARIE ADOLPHE LOUIS
   language: fr
   title: L'ART BYZANTIN
   dewey: 938.301 BAY
   entry_numbers:
   - '3788'
   editor: A. QUANTIN // PARIS
   topics:
@@ -136846,15 +136852,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2666
   authors:
-  - ZIELNSKI THADDEE
+  - ZIELINSKI,TADEUSZ
   language: fr
   title: LA RELIGION DE LA GRECE ANTIOUE
   dewey: 938.105 ZIE
   entry_numbers:
   - '3787'
   editor: LES BELLES LETTRES // PARIS
   edition_year: 1928
@@ -137001,15 +137007,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2669
   authors:
-  - BERARD JEAN
+  - BÉRARD,JEAN
   language: fr
   title: L'EXPANSION JUSOU AUX GUERRES MEDIOUES
   dewey: 938.126 BER
   entry_numbers:
   - '3785'
   editor: MONTAIGNE // AUBIER
   edition_year: 1960
@@ -137455,15 +137461,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2678
   authors:
-  - BOUTHOUL GASTON
+  - BOUTHOUL,GASTON
   language: fr
   title: LE PHENOMENE-GUERR
   dewey: 355 BOU
   entry_numbers:
   - '3776'
   editor: PAYOT // PARIS
   topics:
@@ -137605,15 +137611,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 2681
   authors:
-  - BLOCH RAUMOND
+  - BLOCH,RAYMOND
   language: fr
   title: LES ORIGINES DE ROME
   dewey: 945 BLO
   entry_numbers:
   - '3772'
   editor: UNIVERSITAIRES // PARIS
   edition_year: 1971
@@ -138448,15 +138454,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2698
   authors:
-  - BOLLACK JEAN
+  - BOLLACK,JEAN
   language: fr
   title: EMPEDOCLE
   subtitle: INTRODUCTION L'ANCIENNE PHYSIOUE
   dewey: 574 BOL
   entry_numbers:
   - '3758'
   editor: MINUETT // PARIS
@@ -139197,15 +139203,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2713
   authors:
-  - BOUCHE-LEGLERGO A
+  - BOUCHE-LECLERCQ,AUGUSTE
   language: fr
   title: HISTOIRE DES SELEUCIDES
   dewey: 938.194 BOU
   entry_numbers:
   - '3744'
   editor: LEROUX // PARIS
   edition_year: 1913
@@ -139398,15 +139404,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2717
   authors:
-  - ZEHNACKER HUBERT
+  - ZEHNACKER,HUBERT
   language: fr
   title: RECHERCHES SUR L'ORGANISATION ET L'ART DES EMISSIONS
   dewey: 938.192 ZEH
   entry_numbers:
   - '3740'
   editor: ECOLE FRANCAISE // ROMA
   edition_year: 1973
@@ -139552,15 +139558,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2720
   authors:
-  - BERGSON HENDRI
+  - BERGSON,HENRI
   language: fr
   title: L'EVOLUTION GREATRICE
   dewey: 312 BER
   entry_numbers:
   - '3737'
   editor: SKIRA // GENEVE
   topics:
@@ -139601,15 +139607,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2721
   authors:
-  - BRUNEAU PHILIPPE
+  - BRUNEAU,PHILIPPE
   language: fr
   title: RECHERCHES SUR LES CULTES DE DELOS AL'EPOUE HELLENISTIOUE ET
   subtitle: ET A EPOUE IMPERIALE
   dewey: 938.031 BRU
   entry_numbers:
   - '3736'
   editor: BOCCARD // PARIS
@@ -139705,15 +139711,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2723
   authors:
-  - BLOCH MARC
+  - BLOCH,MARC
   language: fr
   title: LES ROIS THAUMATURGES
   dewey: 944 BLO
   entry_numbers:
   - '3733'
   editor: COLIN // PARIS
   edition_year: 1961
@@ -139808,15 +139814,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 2725
   authors:
-  - BRIANT PIERRE
+  - BRIANT,PIERRE
   language: fr
   title: ANTIGONE LE BORGNE
   dewey: 938.182 BRI
   entry_numbers:
   - '3731'
   editor: LES BELLES LETTRS // PARIS
   edition_year: 1973
@@ -139858,15 +139864,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2726
   authors:
-  - BAMM PETER
+  - BAMM,PETER
   language: fr
   title: ALEXAND LE GRAND
   dewey: 938.174 BAM
   entry_numbers:
   - '3730'
   editor: SEOUOIA // PARIS
   edition_year: 1969
@@ -139954,15 +139960,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2728
   authors:
-  - BETTELHEIM CH
+  - BETTELHEIM,CHARLES
   language: fr
   title: L'ECONOMIE SOVIETIOUE
   dewey: 947 BET
   entry_numbers:
   - '3728'
   editor: SIREY // PARIS
   edition_year: 1950
@@ -140006,15 +140012,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2729
   authors:
-  - BENES EDOUARD
+  - BENES,EDOUARD
   language: fr
   title: LA DEMOCAATIE AUJOURD ET DEMAIN
   dewey: 329 BEN
   entry_numbers:
   - '3727'
   editor: SUISSE // None
   edition_year: 1944
@@ -140466,15 +140472,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 2738
   authors:
-  - BAKER G
+  - BAKER,GEORGE,PHILIP
   language: fr
   title: ANNIBAL
   dewey: 840 BAK
   entry_numbers:
   - '3718'
   editor: PAYOT // PARIS
   edition_year: 1952
@@ -141370,15 +141376,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2756
   authors:
-  - ΜΠΑΛΣΟΝ,Ζ
+  - BALSDON,JOHN,PERCY VYVIAN DACRE
   language: el
   title: ΡΩΜΑΙΕΣ ΓΥΝΑΙΚΕΣ
   subtitle: Η ΙΣΤΟΡΙΑ ΚΑΙ ΤΑ ΕΘΙΜΑ ΤΟΥΣ
   dewey: 937 ΒΑΛ
   entry_numbers:
   - '4083'
   editor: None // ΑΘΗΝΑ
@@ -141783,15 +141789,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2764
   authors:
-  - ΖΩΡΟΓΙΑΝΝΙΔΗΣ,ΚΩΝ/ΝΟΣ
+  - ΖΩΡΟΓΙΑΝΝΙΔΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
   language: el
   title: ΗΜΕΡΟΛΟΓΙΟΝ ΠΟΡΕΙΩΝ ΚΑΙ ΠΟΛΕΜΙΚΩΝ ΕΠΙΧΕΙΡΗΣΕΩΝ 1912-13
   dewey: 938.603 ΖΩΡ
   entry_numbers:
   - '3036'
   editor: Ι.Μ.Χ.Α // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1992
@@ -142860,15 +142866,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2785
   authors:
-  - ΜΠΑΙΡΑΚΤΑΡΗ,ΣΤΥΛ
+  - ΜΠΑΙΡΑΚΤΑΡΗΣ,ΣΤΥΛ.
   language: el
   title: ΓΝΩΡΙΜΙΑ ΜΕ ΤΗΝ ΚΑΙΝΗ ΔΙΑΘΗΚΗ
   dewey: 225 ΜΠΑ
   entry_numbers:
   - '601'
   editor: None // ΑΘΗΝΑ
   edition_year: 1958
@@ -143364,15 +143370,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2795
   authors:
-  - ΜΠΑΙΡΑΚΤΑΡΗΣ,ΣΤΥΛ
+  - ΜΠΑΙΡΑΚΤΑΡΗΣ,ΣΤΥΛ.
   language: el
   title: ΤΟ ΨΑΛΤΗΡΙΟΝ ΕΙΣ ΤΗΝ ΑΠΛΟΕΛΛΗΝΙΚΗΝ ΚΑΤΑ ΤΟΥΣ ΧΡΟΝΟΥΣ ΤΗΣ
   subtitle: ΤΟΥΡΚΟΚΡΑΤΙΑΣ
   dewey: 223 ΜΠΑ
   entry_numbers:
   - '527'
   editor: None // ΑΘΗΝΑ
@@ -143416,15 +143422,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2796
   authors:
-  - ΜΠΑΙΡΑΚΤΑΡΗΣ,ΣΤΥΛ
+  - ΜΠΑΙΡΑΚΤΑΡΗΣ,ΣΤΥΛ.
   language: el
   title: ΩΡΑ ΓΑΛΗΝΗΣ
   subtitle: 60 ΕΠΙΚΑΙΡΑ ΚΗΡΥΓΜΑΤΑ ΤΟΥ ΕΝΟΣ ΛΕΠΤΟΥ
   dewey: 251 ΜΠΑ
   entry_numbers:
   - '526'
   editor: None // ΑΘΗΝΑ
@@ -145644,15 +145650,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2840
   authors:
-  - ΜΠΛΑΧΟΥΡΑΣ,ΚΩΝ
+  - ΜΠΛΑΧΟΥΡΑΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ,.ΧΡ.
   language: el
   title: ΘΕΣΕΙΣ ΚΑΙ ΑΠΟΨΕΙΣ ΓΥΡΩ ΑΠΟ ΤΑ ΑΝΘΡΩΠΙΝΑ
   subtitle: ΣΤΟΧΑΣΜΟΙ -ΑΦΟΡΙΣΜΟΙ
   dewey: 265 ΜΠΛ
   entry_numbers:
   - '2941'
   editor: None // ΑΘΗΝΑ
@@ -147797,15 +147803,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2882
   authors:
-  - ΜΠΟΝΗΣ,ΚΩΝ/ΝΟΣ
+  - ΜΠΟΝΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
   language: el
   title: ΧΡΙΣΤΙΑΝΙΚΗ ΓΡΑΜΜΑΤΕΙΑ
   subtitle: ΗΤΟΙ ΦΙΛΟΛΟΓΙΚΗ ΚΑΙ ΚΡΙΤΙΚΗ ΙΣΤΟΡΙΑ ΤΩΝ ΠΑΤΕΡΩΝ ΚΑΙ ΕΚΚΛΗΣ..
   dewey: 270 ΜΠΟ
   entry_numbers:
   - '565'
   editor: None // ΑΘΗΝΑ
@@ -147853,15 +147859,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2883
   authors:
-  - ΜΠΟΝΗΣ ΚΩΝ/ΝΟΣ
+  - ΜΠΟΝΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
   language: el
   title: ΕΙΣΑΓΩΓΗ ΕΙΣ ΤΗΝ ΑΡΧΑΙΑΝ ΧΡΙΣΤΙΑΝΙΚΗ ΓΡΑΜΜΑΤΕΙΑΝ
   dewey: 270 ΜΠΟ
   entry_numbers:
   - '570'
   editor: None // ΑΘΗΝΑ
   edition_year: 1974
@@ -148461,15 +148467,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2895
   authors:
-  - ΜΠΑΣΤΙΑ,ΚΩΣΤΗ
+  - ΜΠΑΣΤΟΥΝΌΠΟΥΛΟΣ,ΑΙΜΊΛΙΟΣ,ΚΩΝΣΤΑΝΤΊΝΟΣ@ΚΩΣΤΗΣ ΜΠΑΣΤΙΑΣ
   language: el
   title: ΝΕΟΝ ΚΥΡΙΑΚΟΔΡΟΜΙΟΝ
   subtitle: ΣΧΟΛΙΑ ΚΑΘΕ ΠΕΡΙΚΟΠΗ
   dewey: 226 ΜΠΑ
   entry_numbers:
   - '536'
   - '538'
@@ -154489,15 +154495,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3015
   authors:
-  - ΜΠΟΣΗ,ΚΩΣΤΑ
+  - ΜΠΟΣΗΣ,ΚΩΣΤΑΣ
   language: el
   title: ΑΝΑΜΝΗΣΕΙΣ
   dewey: 889.21 ΜΠΟ
   entry_numbers:
   - '5711'
   editor: ΣΚΑΡΑΒΑΙΟΣ // ΑΘΗΝΑ
   edition_year: 1978
@@ -159090,15 +159096,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3108
   authors:
-  - ΜΠΑΛΟΥΜΗΣ,ΕΠΑΜ.
+  - ΜΠΑΛΟΥΜΗΣ,ΕΠΑΜΕΙΝΩΝΔΑΣ
   language: el
   title: ΟΙ ΚΑΗΔΕΣ
   dewey: 889.21 ΜΠΑ
   entry_numbers:
   - '4465'
   editor: ΛΩΤΟΣ // ΑΘΗΝΑ
   edition_year: 1987
@@ -160230,15 +160236,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3131
   authors:
-  - ΖΑΔΕ,ΔΗΜΟΣΘΕΝΗΣ
+  - ΖΑΔΕΣ,ΔΗΜΟΣΘΕΝΗΣ
   language: el
   title: ΤΕΛΕΥΤΑΙΟΣ ΚΥΚΛΟΣ
   dewey: 889.21 ΖΑΔ
   entry_numbers:
   - '5528'
   editor: ΜΑΥΡΙΔΗΣ // ΑΘΗΝΑ
   edition_year: 1962
@@ -161267,15 +161273,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3152
   authors:
-  - ΜΠΟΥΤΒΑ,ΝΙΚΟΥ
+  - ΜΠΟΥΤΒΑΣ,ΝΙΚΟΣ
   language: el
   title: ΤΥΡΑΓΝΙΑ
   dewey: 889.21 ΜΠΟ
   entry_numbers:
   - '5712'
   editor: None // ΑΘΗΝΑ
   edition_year: 1966
@@ -164074,15 +164080,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3209
   authors:
-  - ΖΑΒΕΡΔΙΝΟΥ,ΛΙΖΑ-ΠΑΡΑΣΚ.
+  - ΖΑΒΕΡΔΙΝΟΥ,ΛΙΖΑ-ΠΑΡΑΣΚΕΥΗ
   language: el
   title: ΤΟ ΠΡΟΣΩΠΟ ΤΗΣ ΜΟΝΑΞΙΑΣ
   dewey: 889.21 ΖΑΒ
   entry_numbers:
   - '5530'
   editor: None // ΑΘΗΝΑ
   edition_year: 1960
@@ -164123,15 +164129,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3210
   authors:
-  - ΖΑΔΕ,ΔΗΜΟΣΘΕΝΗΣ
+  - ΖΑΔΕΣ,ΔΗΜΟΣΘΕΝΗΣ
   language: el
   title: ΓΙΑ ΣΜΕΡΝΕΣ
   dewey: 889.21 ΖΑΔ
   entry_numbers:
   - '5529'
   editor: ΤΡΙΦΥΛΙΑΚΗ ΕΣΤΙΑ // ΑΘΗΝΑ
   edition_year: 1977
@@ -164715,15 +164721,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3222
   authors:
-  - ΖΑΔΕ,ΔΗΜΟΣΘΕΝΗΣ
+  - ΖΑΔΕΣ,ΔΗΜΟΣΘΕΝΗΣ
   language: el
   title: ΣΤΗ ΘΕΣΗ ΤΟΥ ΑΛΛΟΥ
   dewey: 889.21 ΖΑΔ
   entry_numbers:
   - '4652'
   editor: ΤΡΙΦΥΛΙΑΚΗ ΕΣΤΙΑ // ΑΘΗΝΑ
   edition_year: 1983
@@ -165112,15 +165118,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3230
   authors:
-  - ΖΑΚΟΠΟΥΛΟΣ
+  - ΖΑΚΟΠΟΥΛΟΣ,ΝΙΚΟΣ,Ι.
   language: el
   title: Η ΔΙΚΗ
   dewey: 889.21 ΖΑΚ
   entry_numbers:
   - '4656'
   editor: ΔΩΔΩΝΗ // ΑΘΗΝΑ
   edition_year: 1979
@@ -165363,15 +165369,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3235
   authors:
-  - ΜΠΑΚΟΥΡΗ,ΜΙΧΑΗΛ-ΓΕΩΡΓΙΟΥ
+  - ΜΠΑΚΟΥΡΗΣ,ΜΙΧΑΗΛ,ΓΕΩΡΓΙΟΣ
   language: el
   title: ΤΟ ΛΟΥΛΟΥΔΙ
   dewey: 889.21 ΜΠΑ
   entry_numbers:
   - '5682'
   editor: None // ΠΕΙΡΑΙΑΣ
   edition_year: 1970
@@ -167238,15 +167244,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3273
   authors:
-  - ΜΠΑΚΟΣ,ΗΛΙΑΣ
+  - ΜΠΑΚΟΣ,ΗΛΙΑΣ,Δ.
   language: el
   title: Ο ΚΟΣΜΟΣ ΤΩΝ ΝΕΩΝ
   subtitle: ΑΓΩΓΗ ΚΑΙ ΠΑΡΑΔΟΣΗ
   dewey: 889.21 ΜΠΑ
   entry_numbers:
   - '5698'
   editor: None // ΑΘΗΝΑ
@@ -167784,15 +167790,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3284
   authors:
-  - ΖΑΚΟΠΟΥΛΟΣ,ΝΙΚΟΣ.Ι
+  - ΖΑΚΟΠΟΥΛΟΣ,ΝΙΚΟΣ,Ι.
   language: el
   title: Ο ΣΗΜΕΡΙΝΟΣ ΚΟΣΜΟΣ
   dewey: 889.21 ΖΑΚ
   entry_numbers:
   - '4712'
   editor: ΑΔΕΛΦΟΙ ΒΛΑΣΣΗ // None
   pages: 239
@@ -168273,15 +168279,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3294
   authors:
-  - ΜΠΛΑΧΟΥΡΑΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ.ΧΡ
+  - ΜΠΛΑΧΟΥΡΑΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ,.ΧΡ.
   language: el
   title: ΠΡΟΣΑΝΑΤΟΛΙΣΜΟΙ ΣΤΗΝ ΕΠΟΧΗ ΜΑΣ
   dewey: 889.21 ΜΠΛ
   entry_numbers:
   - '5710'
   editor: None // ΑΘΗΝΑ
   edition_year: 1977
@@ -168915,15 +168921,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3307
   authors:
-  - ΜΠΑΚ,ΠΕΡΛ
+  - BUCK,PEARL,S.
   language: el
   title: Η ΤΕΛΕΥΤΑΙΑ ΑΥΤΟΚΡΑΤΕΙΡΑ ΤΗΣ ΚΙΝΑΣ
   dewey: 810.11 ΜΠΑ
   entry_numbers:
   - '1304'
   translators:
   - ΛΑΜΨΑΣ,ΓΙΑΝΝΗΣ
@@ -170003,15 +170009,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3329
   authors:
-  - ΜΠΑΣΤΙΑ,ΚΩΣΤΗ
+  - ΜΠΑΣΤΟΥΝΌΠΟΥΛΟΣ,ΑΙΜΊΛΙΟΣ,ΚΩΝΣΤΑΝΤΊΝΟΣ@ΚΩΣΤΗΣ ΜΠΑΣΤΙΑΣ
   language: el
   title: Ο ΠΑΠΟΥΛΑΚΟΣ
   dewey: 889.21 ΜΠΑ
   entry_numbers:
   - '5681'
   editor: None // NEW YORK
   edition_year: 1951
@@ -170101,15 +170107,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3331
   authors:
-  - ΜΠΙΝΙΑΡΗ,ΓΚΙΚΑ
+  - ΜΠΙΝΙΑΡΗΣ,ΓΚΙΚΑΣ
   language: el
   title: ΤΕΛΕΥΤΑΙΟΣ ΕΣΠΕΡΙΝΟΣ
   dewey: 889.21 ΜΠΙ
   entry_numbers:
   - '5709'
   editor: None // ΑΘΗΝΑ
   edition_year: 1960
@@ -178552,15 +178558,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3503
   authors:
-  - ΜΠΑΡΟΥΤΣΟΥ,ΓΕΩΡΓΙΟΥ
+  - ΜΠΑΡΟΥΤΣΟΣ,ΓΕΩΡΓΙΟΣ
   language: el
   title: ΒΟΥΒΑΘΗΚΑΝ ΟΙ ΚΑΜΠΑΝΕΣ
   dewey: 889.21 ΜΠΑ
   entry_numbers:
   - '5683'
   editor: None // ΑΘΗΝΑ
   edition_year: 1957
@@ -178848,15 +178854,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3509
   authors:
-  - ΖΩΓΡΑΦΑΚΗ,ΓΕΩΡΓΙΟΥ
+  - ΖΩΓΡΑΦΑΚΗΣ,ΓΕΩΡΓΙΟΣ
   language: el
   title: ΑΦΟΡΙΣΜΟΙ
   dewey: 889.21 ΖΩΓ
   entry_numbers:
   - '5549'
   editor: ΝΙΚΟΛΑΙΔΟΥ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1932
@@ -179393,15 +179399,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3520
   authors:
-  - ΜΠΙΡΚΑ,ΚΩΣΤΑ
+  - ΜΠΙΡΚΑΣ,ΚΩΣΤΑΣ
   language: el
   title: ΕΛΛΗΝΙΚΟΣ ΝΟΣΤΟΣ
   subtitle: ΣΕΛΙΔΕΣ ΤΗΣ ΞΕΝΙΤΕΙΑΣ
   dewey: 889.21 ΜΠΙ
   entry_numbers:
   - '4696'
   editor: ΣΥΓΧΡΟΝΟΣ ΚΟΣΜΟΣ // ΑΘΗΝΑ
@@ -179890,15 +179896,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3530
   authors:
-  - ΖΕΝΑΚΟΣ,Λ.
+  - ΖΕΝΑΚΟΣ,ΛΕΩΝΙΔΑΣ
   language: el
   title: ΑΕΤΟΠΟΥΛΑ
   dewey: 889.21 ΖΕΝ
   entry_numbers:
   - '4691'
   editor: ΙΚΑΡΟΣ // ΑΘΗΝΑ
   edition_year: 1983
@@ -180923,15 +180929,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3551
   authors:
-  - ΒΛΑΧΟΣ,ΑΓΓΕΛΟΣ,ΣΤ,
+  - ΒΛΑΧΟΣ,ΑΓΓΕΛΟΣ,ΣΤ.
   language: el
   title: ΟΙ ΤΕΛΕΥΤΑΙΟΙ ΓΑΛΗΝΟΤΑΤΟΙ
   dewey: 889.21 ΒΛΑ
   entry_numbers:
   - '5447'
   edition: '2'
   editor: ΕΣΤΙΑ // ΑΘΗΝΑ
@@ -181957,15 +181963,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3572
   authors:
-  - ΖΑΔΕ,ΔΗΜΟΣΘΕΝΗΣ
+  - ΖΑΔΕΣ,ΔΗΜΟΣΘΕΝΗΣ
   language: el
   title: ΑΛΒΑΝΙΚΗ ΡΑΨΩΔΙΑ ΤΟ ΒΙΒΛΙΟ ΤΗΣ ΕΙΡΗΝΗΣ
   dewey: 889.21 ΖΑΔ
   entry_numbers:
   - '5537'
   editor: None // ΑΘΗΝΑ
   edition_year: 1975
@@ -182893,15 +182899,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3591
   authors:
-  - ΜΠΑΛΖΑΚ
+  - BALZAC,HONORÉ DE
   language: el
   title: ΕΥΓΕΝΙΑ ΓΚΡΑΝΤΕ
   dewey: 843 ΜΠΑ
   entry_numbers:
   - '1280'
   translators:
   - ΠΑΠΑΛΕΞΑΝΔΡΟΥ,Κ.Θ.
@@ -185923,15 +185929,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3651
   authors:
-  - ΖΑΒΕΡΔΙΝΟΥ,ΛΙΖΑ
+  - ΖΑΒΕΡΔΙΝΟΥ,ΛΙΖΑ-ΠΑΡΑΣΚΕΥΗ
   language: el
   title: ΜΥΣΤΙΚΟΙ ΔΡΟΜΟΙ
   dewey: 889.1 ΖΑΒ
   entry_numbers:
   - '6082'
   editor: ΓΡΗΓΟΡΗΣ // ΑΘΗΝΑ
   edition_year: 1964
@@ -186622,15 +186628,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3665
   authors:
-  - ΖΑΧΑΡΗ,ΛΑΜΠΡΟΥ
+  - ΖΑΧΑΡΗΣ,ΛΑΜΠΡΟΣ
   language: el
   title: ΑΠ'Τ'ΑΝΗΛΙΑ ΠΑΛΑΤΙΑ
   dewey: 889.1 ΖΑΧ
   entry_numbers:
   - '6077'
   edition: Β
   editor: None // ΑΘΗΝΑ
@@ -192265,15 +192271,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3777
   authors:
-  - ΜΠΟΥΦΙΔΗ,Ν.ΧΑΓΕΡ
+  - ΜΠΟΥΦΙΔΗΣ,ΧΑΓΕΡ
   language: el
   title: Η ΔΕΥΤΕΡΗ ΖΩΗ
   dewey: 889.1 ΜΠΟ
   entry_numbers:
   - '6244'
   editor: ΚΥΚΛΟΣ // ΑΘΗΝΑ
   edition_year: 1935
@@ -198518,15 +198524,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3902
   authors:
-  - ΖΕΝΑΚΟΥ,ΛΕΩΝΙΔΑ
+  - ΖΕΝΑΚΟΣ,ΛΕΩΝΙΔΑΣ
   language: el
   title: ΠΗΓΕΣ
   dewey: 889.1 ΖΕΝ
   entry_numbers:
   - '6078'
   editor: ΓΚΟΒΟΣΤΗ // ΑΘΗΝΑ
   edition_year: 1962
@@ -200475,15 +200481,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3941
   authors:
-  - ΜΠΕΚΕ,ΟΜΗΡΟΥ
+  - ΜΠΕΚΕΣ,ΟΜΗΡΟΣ
   language: el
   title: ΤΟ ΤΡΑΓΟΥΔΙ ΤΟΥ ΜΕΓΑΛΕΞΑΝΔΡΟΥ
   dewey: 889.1 ΜΠΕ
   entry_numbers:
   - '6247'
   editor: ΖΩΡΖ // ΑΘΗΝΑ
   edition_year: 1959
@@ -205849,15 +205855,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4048
   authors:
-  - ΖΕΡΒΑΝΟΥ,ΑΛΕΞΗ
+  - ΖΕΡΒΑΝΟΣ,ΑΛΕΞΗΣ
   language: el
   title: 12 ΩΡΑ
   dewey: 889.1 ΖΕΡ
   entry_numbers:
   - '6076'
   editor: None // ΑΘΗΝΑ
   edition_year: 1960
@@ -210865,15 +210871,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4148
   authors:
-  - ΖΥΓΟΥΡΗ,ΣΩΤΗΡΗ
+  - ΖΥΓΟΥΡΗΣ,ΣΩΤΗΡΗΣ
   language: el
   title: ΞΥΛΙΝΑ ΤΡΑΚΤΕΡ
   dewey: 889.1 ΖΥΓ
   entry_numbers:
   - '6060'
   editor: ΣΥΓΧΡΟΝΗ ΕΠΟΧΗ // ΑΘΗΝΑ
   edition_year: 1979
@@ -212114,15 +212120,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4173
   authors:
-  - ΖΑΡΟΥΚΑ,ΚΩΣΤΑ
+  - ΖΑΡΟΥΚΑΣ,ΚΩΣΤΑΣ
   language: el
   title: ΔΕΣΜΩΤΕΣ
   dewey: 889.1 ΖΑΡ
   entry_numbers:
   - '6080'
   editor: None // ΑΘΗΝΑ
   edition_year: 1976
@@ -215069,15 +215075,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4232
   authors:
-  - ΖΙΤΣΑΙΑ ΧΡΥΣΑΝΘΗ
+  - ΖΙΤΣΑΙΑ,ΧΡΥΣΑΝΘΗ
   language: el
   title: ΣΥΝΕΠΕΙΑ
   dewey: 889.1 ΖΙΤ
   entry_numbers:
   - '4586'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1982
@@ -220687,15 +220693,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4344
   authors:
-  - ΜΠΛΑΧΟΥΡΑ,ΚΩΝΣΤΑΝΤΙΝΟΥ
+  - ΜΠΛΑΧΟΥΡΑΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ,.ΧΡ.
   language: el
   title: ΑΤΕΛΗΣ ΚΟΣΜΟΣ
   dewey: 889.1 ΜΠΛ
   entry_numbers:
   - '4593'
   editor: ΜΑΥΡΙΔΗΣ // ΑΘΗΝΑ
   edition_year: 1972
@@ -221689,15 +221695,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4364
   authors:
-  - ΖΑΚΚΑ,ΜΙΛΤΙΑΔΗ
+  - ΖΑΚΚΑΣ,ΜΙΛΤΙΑΔΗΣ
   language: el
   title: Η ΤΑΥΤΟΤΗΤΑ ΤΗΣ ΣΥΝΕΙΔΗΣΗΣ
   dewey: 889.1 ΖΑΚ
   entry_numbers:
   - '6081'
   editor: None // ΑΘΗΝΑ
   edition_year: 1984
@@ -221990,15 +221996,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4370
   authors:
-  - ΜΠΑΙΡΟΝ
+  - BYRON,GEORGE,GORDON@LORD BYRON
   language: el
   title: ΕΒΡΑΙΚΕΣ ΜΕΛΩΔΙΕΣ
   dewey: 889.1 ΜΠΑ
   entry_numbers:
   - '1026'
   editor: None // ΑΘΗΝΑ
   edition_year: 1946
@@ -226339,15 +226345,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4457
   authors:
-  - ΜΠΟΥΡΙΤΣΑ ΜΟΥΖΑΚΗ ΕΛΕΝΗ
+  - ΜΟΥΖΑΚΗ-ΜΠΟΥΡΙΤΣΑ,ΕΛΕΝΗ
   language: el
   title: ΠΑΙΔΙΑ ΠΕΡΙΣΤΕΡΙΑ
   dewey: 786.2 ΜΠΟ
   entry_numbers:
   - '9894'
   editor: ΥΔΡΟΓΕΙΟΣ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2009
@@ -226636,15 +226642,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4463
   authors:
-  - ΜΠΡΕΧΤ,ΜΠΕΡΤΟΛΤ
+  - BRECHT,BERTOLT
   language: el
   title: 76 ΠΟΙΗΜΑΤΑ
   dewey: 831.8 ΜΠΡ
   entry_numbers:
   - '6409'
   translators:
   - ΜΑΡΚΑΡΗΣ,ΠΕΤΡΟΣ
@@ -226943,15 +226949,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4469
   authors:
-  - ΖΑΚΟΠΟΥΛΟΣ,ΝΙΚΟΣ
+  - ΖΑΚΟΠΟΥΛΟΣ,ΝΙΚΟΣ,Ι.
   language: el
   title: ΜΙΑ ΠΑΡΑΞΕΝΗ ΠΟΡΝΗ
   dewey: 889 ΖΑΚ
   entry_numbers:
   - '4333'
   editor: ΦΙΛΙΠΠΟΤΗ // ΑΘΗΝΑ
   edition_year: 1983
@@ -227594,15 +227600,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4482
   authors:
-  - ΜΠΟΝΗ,ΚΩΝΣΤΑΝΤΙΝΟΥ
+  - ΜΠΟΝΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
   language: el
   title: ΜΕΓΑΣ ΑΘΑΝΑΣΙΟΣ ΙΟΥΛΙΑΝΟΣ Ο ΑΠΟΣΤΑΤΗΣ ΚΑΙ ΜΕΓΑΣ ΒΑΣΙΛΕΙΟΣ
   dewey: 230 ΜΠΟ
   entry_numbers:
   - '4270'
   editor: None // ΑΘΗΝΑ
   edition_year: 1979
@@ -227888,15 +227894,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4488
   authors:
-  - ΜΠΟΝΗ,ΚΩΝΣΤΑΝΤΙΝΟΥ
+  - ΜΠΟΝΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
   language: el
   title: ΒΑΣΙΛΕΙΟΣ ΚΑΙΣΑΡΕΙΑΣ Ο ΜΕΓΑΣ
   dewey: 230 ΜΠΟ
   entry_numbers:
   - '961'
   editor: None // ΑΘΗΝΑ
   edition_year: 1975
@@ -228684,15 +228690,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4504
   authors:
-  - ΜΠΟΝΗ,ΚΩΝΣΤΑΝΤΙΝΟΥ
+  - ΜΠΟΝΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
   language: el
   title: ΤΟ ΕΝ ΤΟΡΟΝΤΟ ΤΟΥ ΚΑΝΑΔΑ ΔΙΕΘΝΕΣ ΕΠΙΣΤΗΜΟΝΙΚΟ ΣΥΜΠΟΣΙΟ(10-16
   subtitle: ΙΟΥΝ.1979) ΕΙΣ ΜΝΗΜΗΝ ΤΟΥ ΜΕΓΑΛΟΥ ΒΑΣΙΛΕΙΟΥ
   entry_numbers:
   - '4741'
   editor: None // ΑΘΗΝΑ
   edition_year: 1979
@@ -229028,15 +229034,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4511
   authors:
-  - ΜΠΑΙΡΑΚΤΑΡΗ,ΣΤΥΛ.
+  - ΜΠΑΙΡΑΚΤΑΡΗΣ,ΣΤΥΛ.
   language: el
   title: ΣΕΡΑΦΕΙΜ ΜΥΤΙΛΗΝΑΙΟΣ
   subtitle: Ο ΛΗΣΜΟΝΗΜΕΝΟΣ ΠΡΩΤΟΠΟΡΟΣ (1670-1735)
   dewey: 230 ΜΠΑ
   entry_numbers:
   - '6558'
   editor: None // ΑΘΗΝΑ
@@ -229771,15 +229777,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4526
   authors:
-  - ΜΠΟΝΗ,ΚΩΝ.
+  - ΜΠΟΝΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
   language: el
   title: ΑΜΦΙΛΟΧΙΟΥ ΙΚΟΝΙΟΥ
   subtitle: ΠΕΡΙ ΨΕΥΔΟΥΣ ΑΣΚΗΣΕΩΣ
   dewey: 230 ΜΠΟ
   entry_numbers:
   - '4757'
   editor: None // ΑΘΗΝΑ
@@ -229821,15 +229827,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4527
   authors:
-  - ΜΠΟΝΗ,ΚΩΝΣΤΑΝΤΙΝΟΥ
+  - ΜΠΟΝΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
   language: el
   title: Η ΕΛΛΗΝΙΚΗ ΧΡΙΣΤΙΑΝΙΚΗ ΓΡΑΜΜΑΤΕΙΑ ΕΝ ΣΥΓΚΡΙΣΕΙ ΠΡΟΣ ΤΗΝ ΔΥΤΙ
   dewey: 230 ΜΠΟ
   entry_numbers:
   - '4758'
   editor: None // ΑΘΗΝΑ
   edition_year: 1979
@@ -230758,15 +230764,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4546
   authors:
-  - ΜΠΑΙΡΑΚΤΑΡΗ,ΣΤΥΛ.
+  - ΜΠΑΙΡΑΚΤΑΡΗΣ,ΣΤΥΛ.
   language: el
   title: ΑΓΑΠΙΟΣ ΛΑΝΔΟΣ Ο ΚΡΗΣ
   dewey: 230 ΜΠΑ
   entry_numbers:
   - '6564'
   editor: None // ΑΘΗΝΑ
   edition_year: 1970
@@ -231051,15 +231057,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4552
   authors:
-  - ΖΙΑΚΑ,ΓΡΗΓΟΡΙΟΥ
+  - ΖΙΑΚΑΣ,ΓΡΗΓΟΡΙΟΣ
   language: el
   title: ΠΡΟΦΗΤΕΙΑ ΑΠΟΚΑΛΥΨΗ ΚΑΙ ΙΣΤΟΡΙΑ ΤΗΣ ΣΩΤΗΡΙΑΣ ΚΑΤΑ ΤΟ ΚΟΡΑΝΙΟ
   dewey: 230 ΖΙΑ
   entry_numbers:
   - '6574'
   editor: ΠΟΥΡΝΑΡΑ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1976
@@ -233202,15 +233208,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4596
   authors:
-  - ΖΕΛΛΕΚΕ,ΚΙΦΕΛΕΒ
+  - ZELLEKE,KIFELEV
   language: el
   title: ΠΕΡΙ ΤΗΝ ΙΣΤΟΡΙΑΝ ΤΗΣ ΑΝΕΞΑΡΤΗΣΙΑΣ ΤΗΣ ΑΙΘΙΟΠΙΚΗΣ ΕΚΚΛΗΣΙΑΣ
   dewey: 230 ΖΕΛ
   entry_numbers:
   - '4314'
   editor: None // ΑΘΗΝΑ
   edition_year: 1969
@@ -233886,15 +233892,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4610
   authors:
-  - ΜΠΟΝΗ,ΚΩΝΣΤΑΝΤΙΝΟΥ
+  - ΜΠΟΝΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
   language: el
   title: ΟΙ ΑΓΙΟΙ ΚΥΡΙΛΛΟΣ ΚΑΙ ΜΕΘΟΔΙΟΣ ΟΙ ΤΩΝ ΣΛΑΒΩΝ ΑΠΟΣΤΟΛΟΙ ΚΑΙ Η
   subtitle: ΒΑΣΙΛΙΚΗ ΑΟΥ ΑΓ.ΔΗΜΗΤΡΙΟΥ ΘΕΣΣΑΛΟΝΙΚΗΣ
   dewey: 230 ΜΠΟ
   entry_numbers:
   - '962'
   editor: None // ΑΘΗΝΑ
@@ -233937,15 +233943,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4611
   authors:
-  - ΜΠΑΙΡΑΚΤΑΡΗ,ΣΤΥΛ.
+  - ΜΠΑΙΡΑΚΤΑΡΗΣ,ΣΤΥΛ.
   language: el
   title: ΧΩΡΙΣ ΑΜΦΙΒΟΛΙΑ
   dewey: 230 ΜΠΑ
   entry_numbers:
   - '6607'
   editor: None // ΑΘΗΝΑ
   edition_year: 1975
@@ -235009,15 +235015,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4633
   authors:
-  - ΜΠΑΙΡΑΚΤΑΡΗ,ΣΤΥΛ.
+  - ΜΠΑΙΡΑΚΤΑΡΗΣ,ΣΤΥΛ.
   language: el
   title: Ο ΠΑΤΡΙΑΡΧΗΣ ΓΡΗΓΟΡΙΟΣ Ο Ε' ΚΑΙ Η ΜΕΤΑΦΡΑΣΙΣ ΤΗΣ ΑΓΙΑΣ ΓΡΑΦΗ
   dewey: 230 ΜΠΑ
   entry_numbers:
   - '607'
   editor: None // ΑΘΗΝΑ
   edition_year: 1965
@@ -236153,15 +236159,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4656
   authors:
-  - ΜΠΥΡΓΚΕΡ,Γ.Α
+  - Bürger,Gottfried,August
   language: el
   title: ΟΙ ΠΕΡΙΠΕΤΕΙΕΣ ΤΟΥ ΒΑΡΟΝΟΥ ΜΥΝΧΑΟΥΖΕΝ
   dewey: 808.899 ΜΠΥ
   entry_numbers:
   - '4794'
   editor: ΑΣΤΗΡ // ΑΘΗΝΑ
   edition_year: 1973
@@ -238721,15 +238727,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4707
   authors:
-  - BEECHER,E.R.
+  - BEECHER,E.,R.
   language: el
   title: Η ΣΥΝΤΗΡΗΣΗ ΤΩΝ ΥΦΑΣΜΑΤΩΝ
   dewey: 398 ΒΕΕ
   entry_numbers:
   - '1644'
   editor: None // ΑΘΗΝΑ
   edition_year: 1991
@@ -240253,15 +240259,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4738
   authors:
-  - ΜΠΟΓΚΑ,ΕΥΑΓΓΕΛΟΥ
+  - ΜΠΟΓΚΑΣ,ΕΥΑΓΓΕΛΟΣ
   language: el
   title: ΤΑ ΓΛΩΣΣΙΚΑ ΙΔΙΩΜΑΤΑ ΤΗΣ ΗΠΕΙΡΟΥ
   subtitle: ΒΟΡΕΙΟΥ,ΚΕΝΤΡΙΚΗΣ ΚΑΙ ΝΟΤΙΟΥ
   dewey: 398 ΜΠΟ
   entry_numbers:
   - '4804'
   editor: ΕΤΑΙΡ.ΗΠΕΙΡ.ΜΕΛΕΤΩΝ // ΙΩΑΝΝΙΝΑ
@@ -240305,15 +240311,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4739
   authors:
-  - ΜΠΟΓΚΑ,ΕΥΑΓΓΕΛΟΥ
+  - ΜΠΟΓΚΑΣ,ΕΥΑΓΓΕΛΟΣ
   language: el
   title: ΤΑ ΓΛΩΣΣΙΚΑ ΙΔΙΩΜΑΤΑ ΤΗΣ ΗΠΕΙΡΟΥ
   subtitle: ΒΟΡΕΙΟΥ,ΚΕΝΤΡΙΚΗΣ ΚΑΙ ΝΟΤΙΟΥ
   dewey: 398 ΜΠΟ
   entry_numbers:
   - '4805'
   editor: ΕΤΑΙΡ.ΗΠΕΙΡ.ΜΕΛΕΤΩΝ // ΙΩΑΝΝΙΝΑ
@@ -243601,15 +243607,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4806
   authors:
-  - ΜΠΑΝΤΑΛΟΥΚΑ,ΚΛΑΥΔΙΟΣ
+  - ΜΠΑΝΤΑΛΟΥΚΑΣ,ΚΛΑΥΔΙΟΣ
   language: el
   title: ΤΕΣΣΑΡΑΚΟΝΤΑΕΤΟΥΣ ΣΥΜΒΟΛΗΣ ΤΟΥ ΕΙΣ ΤΗΝ ΟΙΚΟΝΟΜ. ΚΑΙ ΟΡΓΑΝΩΤ.
   entry_numbers:
   - '4218'
   editor: None // ΑΘΗΝΑ
   edition_year: 1976
   pages: 92
@@ -244335,15 +244341,16 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4821
   authors:
-  - BISMUTH,HENRI-CASAING,DENIS
+  - BISMUTH,HENRI
+  - CASΤAING,DENIS
   language: el
   title: ΔΙΕΓΧΕΙΡΗΤΙΚΟ ΥΠΕΡΗΧΟΓΡΑΦΗΜΑ ΗΠΑΤΟΣ ΚΑΙ ΧΟΛΗΦΟΡΩΝ
   entry_numbers:
   - '3052'
   editor: ΒΗΤΑ // ΑΘΗΝΑ
   edition_year: 1992
   pages: 86
@@ -245692,15 +245699,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4849
   authors:
-  - ΖΑΚΟΠΟΥΛΟΣ,Ν.Ι
+  - ΖΑΚΟΠΟΥΛΟΣ,ΝΙΚΟΣ,Ι.
   language: el
   title: Η ΑΤΟΜΙΚΗ ΚΑΘΑΡΙΟΤΗΤΑ Η ΥΓΕΙΑ ΚΑΙ Η ΖΩΗ
   entry_numbers:
   - '5927'
   editor: ΑΘΗΝΑΙΚΕΣ ΕΚΔΟΣΕΙΣ // ΑΘΗΝΑ
   edition_year: 1959
   pages: 80
@@ -246612,15 +246619,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4868
   authors:
-  - ΖΑΧΑΡΗ,ΕΥΣΤΑΘΙΟΥ
+  - ΖΑΧΑΡΗΣ,ΕΥΣΤΑΘΙΟΣ
   language: el
   title: ΓΕΩΡΓΙΚΗ ΟΙΚΟΝΟΜΙΑ
   entry_numbers:
   - '6424'
   editor: ΕΥΓΕΝΙΔΙΟΝ ΙΔΡΥΜΑ // ΑΘΗΝΑ
   edition_year: 1979
   pages: 122
@@ -246999,15 +247006,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4876
   authors:
-  - ΖΑΧΑΡΟΠΟΥΛΟΥ,ΙΓΝΑΤΙΟΥ
+  - ΖΑΧΑΡΟΠΟΥΛΟΣ,ΙΓΝΑΤΙΟΣ
   language: el
   title: ΠΩΣ ΛΙΠΑΙΝΕΙΣ ΟΛΕΣ ΤΙΣ ΚΑΛΛΙΕΡΓΕΙΕΣ ΜΕ ΤΟΝ ΚΑΛΥΤΕΡΟ ΤΡΟΠΟ
   entry_numbers:
   - '6005'
   editor: ΣΠ.ΣΠΥΡΟΥ // ΑΘΗΝΑ
   edition_year: 1953
   pages: 198
@@ -254896,15 +254903,16 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5036
   authors:
-  - BARNARD & EDWARDS
+  - BARNARD,JOHN,DARRELL
+  - EDWARDS,LONNIE,J.
   language: el
   title: ΘΕΜΕΛΙΩΔΕΙΣ ΑΡΧΑΙ ΤΗΣ ΦΥΣΙΚΗΣ
   entry_numbers: []
   editor: ΠΕΧΛΙΒΑΝΙΔΗΣ // ΑΘΗΝΑ
   pages: 704
   topics:
   - ΦΥΣΙΚΗ
@@ -255847,15 +255855,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5056
   authors:
-  - ΖΑΧΑΡΗ,ΕΥΣΤΑΘΙΟΥ
+  - ΖΑΧΑΡΗΣ,ΕΥΣΤΑΘΙΟΣ
   language: el
   title: ΓΕΩΡΓΙΚΟΣ ΠΡΟΣΑΝΑΤΟΛΙΣΜΟΣ
   entry_numbers: []
   editor: ΕΥΓΕΝΙΔΙΟ ΙΔΡΥΜΑ // ΑΘΗΝΑ
   edition_year: 1978
   pages: 126
   topics:
@@ -258405,15 +258413,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5110
   authors:
-  - ΜΠΟΥΛΑΛΑ,ΚΛΕΑΝΘΟΥΣ
+  - ΜΠΟΥΛΑΛΆΣ,ΚΛΕΆΝΘΗΣ,Κ.
   language: el
   title: ΕΘΝΙΚΗ ΑΓΩΓΗ
   subtitle: ΗΘΙΚΗ ΚΑΙ ΠΟΛΙΤΙΚΗ ΑΓΩΓΗ
   entry_numbers:
   - '5915'
   editor: None // ΡΟΔΟΣ
   edition_year: 1955
@@ -263178,15 +263186,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5209
   authors:
-  - ΜΠΕΛΛΟΣ,ΚΩΝ/ΝΟΣ
+  - ΜΠΕΛΛΟΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
   language: el
   title: Η ΠΙΣΤΗ ΜΟΥ ΣΤΟ ΧΡΙΣΤΟ,ΤΟ ΠΡΟΣΚΥΝΗΜΑ ΜΟΥ ΣΤΟΥΣ ΑΓΙΟΥΣ ΤΟΠΟΥΣ
   subtitle: ΚΑΙ Η ΠΟΡΕΙΑ ΤΟΥ ΧΡΙΣΤΙΑΝΙΣΜΟΥ
   entry_numbers:
   - '5228'
   edition_year: 1999
   pages: 124
@@ -267716,15 +267724,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5301
   authors:
-  - ΖΑΔΕ,ΔΗΜΟΣΘΕΝΗΣ
+  - ΖΑΔΕΣ,ΔΗΜΟΣΘΕΝΗΣ
   language: el
   title: ΠΑΝΩ ΑΠ'ΤΟΝ ΞΕΝΟ ΜΟΧΘΟ
   dewey: 880.09 ΖΑΔ
   entry_numbers:
   - '5404'
   editor: ΤΡΙΦΥΛΙΑΚΗΣ ΕΣΤΙΑΣ // ΑΘΗΝΑ
   edition_year: 1987
@@ -271840,15 +271848,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5387
   authors:
-  - ΜΠΩΝΤΛΑΙΡ,ΣΑΡΛ
+  - BAUDELAIRE,CHARLES
   language: el
   title: ΤΑ ΑΝΘΗ ΤΟΥ ΚΑΚΟΥ
   dewey: 841 ΜΠΩ
   entry_numbers:
   - '1297'
   - '8452'
   editor: ΖΗΚΑΚΗ // ΑΘΗΝΑ
@@ -276578,15 +276586,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5485
   authors:
-  - ΖΑΦΕΙΡΟΠΟΥΛΟΥ
+  - ΖΑΦΕΙΡΟΠΟΥΛΟΣ,ΖΑΦΕΙΡΙΟΣ
   language: el
   title: ΑΝΑΣΤΑΣΙΜΑΤΑΡΙΟΝ
   dewey: 781.711 ΖΑΦ
   entry_numbers:
   - '6637'
   - '6640'
   pages: 200
@@ -277107,15 +277115,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5496
   authors:
-  - ΖΩΔΙΑΤΟΥ,ΣΠΥΡΟΥ
+  - ΖΩΔΙΑΤΟΣ,ΣΠΥΡΟΣ
   language: el
   title: Η ΕΝΕΝΘΡΩΠΗΣΙΣ ΤΟΥ ΘΕΟΥ
   dewey: 230 ΖΩΔ
   entry_numbers:
   - '6634'
   editor: Ο ΛΟΓΟΣ // ΑΘΗΝΑ
   edition_year: 1963
@@ -277919,15 +277927,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5513
   authors:
-  - ΜΠΕΛΛΟΥ,ΚΩΝΣΤΑΝΤΙΝΟΥ
+  - ΜΠΕΛΛΟΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
   language: el
   title: Η ΠΙΣΤΗ ΜΟΥ ΣΤΟ ΧΡΙΣΤΟ ΤΟ ΠΡΟΣΚΥΝΗΜΑ ΜΟΥ ΣΤΟΥΣ ΑΓΙΟΥΣ ΤΟΠΟΥΣ
   subtitle: ΚΑΙ Η ΠΟΡΕΙΑ ΤΟΥ ΧΡΙΣΤΙΑΝΙΣΜΟΥ
   dewey: 230 ΜΠΕ
   entry_numbers:
   - '5228'
   editor: None // ΠΡΕΒΕΖΑ
@@ -280254,15 +280262,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5562
   authors:
-  - ΜΠΡΟΝΤΕ,ΚΑΡΛΟΤΤΑ
+  - BRONTË,CHARLOTTE
   language: el
   title: ΤΖΕΗΝ ΕΥΡ
   dewey: 880.899 ΜΠΡ
   entry_numbers:
   - '6671'
   editor: ΑΓΚΥΡΑ // ΑΘΗΝΑ
   edition_year: 1994
@@ -282268,15 +282276,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5602
   authors:
-  - ΜΠΟΥΜΠΟΥΛΙΔΟΥ ΓΛΥΚΕΡΙΑ
+  - ΜΠΟΥΜΠΟΥΛΙΔΟΥ,ΓΛΥΚΕΡΙΑ
   language: el
   title: ΠΕΖΟΓΡΑΦΙΚΑ ΚΕΙΜΕΝΑ ΤΟΥ ΠΟΛΕΜΟΥ ΚΑΙ ΤΗΣ ΚΑΤΟΧΗΣ
   dewey: 889.21 ΜΠΟ
   entry_numbers:
   - '4675'
   editor: ΠΑΝΕΠΙΣΤ.ΙΩΑΝΝΙΝΩΝ // ΙΩΑΝΝΙΝΑ
   edition_year: 1974
@@ -283080,15 +283088,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5618
   authors:
-  - ΖΕΒΑΚΟ,Μ.
+  - ZEVACO,MICHEL
   language: el
   title: Η ΓΕΦΥΡΑ ΤΩΝ ΣΤΕΝΑΓΜΩΝ
   dewey: 889 ΖΕΒ
   entry_numbers:
   - '7239'
   translators:
   - ΒΟΥΡΔΟΥΜΠΑ,ΣΤΕΛΛΑ
@@ -283183,15 +283191,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5620
   authors:
-  - ΜΠΑΣΤΙΑ,ΚΩΣΤΗ
+  - ΜΠΑΣΤΟΥΝΌΠΟΥΛΟΣ,ΑΙΜΊΛΙΟΣ,ΚΩΝΣΤΑΝΤΊΝΟΣ@ΚΩΣΤΗΣ ΜΠΑΣΤΙΑΣ
   language: el
   title: ΜΠΟΥΜΠΟΥΛΙΝΑ
   dewey: 889 ΜΠΑ
   entry_numbers:
   - '7275'
   editor: ΜΠΑΣΤΙΑ // ΑΘΗΝΑ
   edition_year: 1974
@@ -283233,15 +283241,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5621
   authors:
-  - ΜΠΑΣΤΙΑ,ΚΩΣΤΗ
+  - ΜΠΑΣΤΟΥΝΌΠΟΥΛΟΣ,ΑΙΜΊΛΙΟΣ,ΚΩΝΣΤΑΝΤΊΝΟΣ@ΚΩΣΤΗΣ ΜΠΑΣΤΙΑΣ
   language: el
   title: ΑΡΑΧΝΗ 44
   dewey: 889 ΜΠΑ
   entry_numbers:
   - '7278'
   editor: ΜΠΑΣΤΙΑ // ΑΘΗΝΑ
   edition_year: 1974
@@ -283283,15 +283291,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5622
   authors:
-  - ΜΠΑΣΤΑ,ΚΩΣΤΗ
+  - ΜΠΑΣΤΟΥΝΌΠΟΥΛΟΣ,ΑΙΜΊΛΙΟΣ,ΚΩΝΣΤΑΝΤΊΝΟΣ@ΚΩΣΤΗΣ ΜΠΑΣΤΙΑΣ
   language: el
   title: ΠΑΠΑΔΙΑΜΑΝΤΗΣ
   dewey: 889 ΜΠΑ
   entry_numbers:
   - '7277'
   editor: ΜΠΑΣΤΙΑ // ΑΘΗΝΑ
   edition_year: 1974
@@ -283334,15 +283342,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5623
   authors:
-  - ΜΠΑΣΤΙΑ,ΚΩΣΤΗ
+  - ΜΠΑΣΤΟΥΝΌΠΟΥΛΟΣ,ΑΙΜΊΛΙΟΣ,ΚΩΝΣΤΑΝΤΊΝΟΣ@ΚΩΣΤΗΣ ΜΠΑΣΤΙΑΣ
   language: el
   title: ΜΗΝΑΣ Ο ΡΕΜΠΕΛΟΣ
   dewey: 889 ΜΠΑ
   entry_numbers:
   - '7276'
   editor: ΜΠΑΣΤΙΑ // ΑΘΗΝΑ
   edition_year: 1968
@@ -283385,15 +283393,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5624
   authors:
-  - ΜΠΑΣΤΙΑ,ΚΩΣΤΗ
+  - ΜΠΑΣΤΟΥΝΌΠΟΥΛΟΣ,ΑΙΜΊΛΙΟΣ,ΚΩΝΣΤΑΝΤΊΝΟΣ@ΚΩΣΤΗΣ ΜΠΑΣΤΙΑΣ
   language: el
   title: ΠΑΠΟΥΛΑΚΟΣ
   dewey: 889 ΜΠΑ
   entry_numbers:
   - '7274'
   editor: ΜΠΑΣΤΙΑ // ΑΘΗΝΑ
   edition_year: 1973
@@ -284311,15 +284319,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5642
   authors:
-  - BRONTE,CH.
+  - BRONTË,CHARLOTTE
   language: el
   title: ΤΖΕΗΝ ΕΥΡ
   dewey: 889 BRO
   entry_numbers:
   - '7062'
   translators:
   - ΠΑΠΑΓΙΑΝΝΗ,ΝΙΝΙΛΑ
@@ -284978,15 +284986,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5655
   authors:
-  - ΖΟΛΑ,ΕΜΙΛ
+  - ZOLA,ÉMILE,ÉDOUARD CHARLES ANTOINE
   language: el
   title: ΚΑΤΗΓΟΡΩ
   subtitle: Η ΥΠΟΘΕΣΙΣ ΝΤΡΕΥΦΟΥΣ ΚΑΙ Ο ΖΟΛΑ
   dewey: 843 ΖΟΛ
   entry_numbers:
   - '7308'
   translators:
@@ -286316,15 +286324,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 5681
   authors:
-  - ΜΠΑΚ,ΠΕΡΛ
+  - BUCK,PEARL,S.
   language: el
   title: ΠΕΡΗΦΑΝΗ ΚΑΡΔΙΑ
   dewey: 889 ΜΠΑ
   entry_numbers:
   - '7134'
   translators:
   - ΑΛΕΞΑΝΔΡΟΥ,ΑΡΗΣ
@@ -286781,15 +286789,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 5690
   authors:
-  - ΜΠΡΙΟΝ,ΜΑΡΣΕΛ
+  - BRION,MARCEL
   language: el
   title: ΜΙΧΑΗΛ ΑΓΓΕΛΟΣ
   dewey: 741.945 ΜΠΡ
   entry_numbers:
   - '6979'
   translators:
   - ΙΩΑΝΝΙΔΗ,Π.Σ.
@@ -286935,15 +286943,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5693
   authors:
-  - ΖΟΛΑ,ΕΜΙΛ
+  - ZOLA,ÉMILE,ÉDOUARD CHARLES ANTOINE
   language: el
   title: ΤΟ ΟΝΕΙΡΟ
   dewey: 889 ΖΟΛ
   entry_numbers:
   - '7026'
   translators:
   - ΣΩΤΗΡΟΠΟΥΛΟΥ,ΜΑΤΘΑΙΟΣ
@@ -287453,15 +287461,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5703
   authors:
-  - ΜΠΕΛΛ,ΧΑΙΝΡΙΧ
+  - BÖLL,HEINRIC
   language: el
   title: ΜΠΙΛΙΑΡΔΟ ΣΤΙΣ 9:30
   dewey: 889 ΜΠΕ
   entry_numbers:
   - '7234'
   translators:
   - ΛΑΜΨΑΣ,ΓΙΑΝΝΗΣ
@@ -288227,15 +288235,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5718
   authors:
-  - ΜΠΑΚ,ΠΕΡΛ
+  - BUCK,PEARL,S.
   language: el
   title: ΠΕΡΗΦΑΝΗ ΚΑΡΔΙΑ
   dewey: 889 ΜΠΑ
   entry_numbers:
   - '7098'
   translators:
   - ΑΛΕΞΑΝΔΡΟΥ,ΑΡΗΣ
@@ -288330,15 +288338,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5720
   authors:
-  - ΖΟΛΑ,Ε.
+  - ZOLA,ÉMILE,ÉDOUARD CHARLES ANTOINE
   language: el
   title: ΑΜΑΡΤΗΜΑ ΑΒ.ΜΟΥΡΕ
   dewey: 843 ΖΟΛ
   entry_numbers:
   - '7105'
   - '91'
   translators:
@@ -288484,15 +288492,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5723
   authors:
-  - ΖΟΛΑ,ΕΜΙΛ
+  - ZOLA,ÉMILE,ÉDOUARD CHARLES ANTOINE
   language: el
   title: ΝΑΝΑ
   dewey: 889 ΖΟΛ
   entry_numbers:
   - '7182'
   translators:
   - ΠΡΑΤΣΙΚΑΣ,ΓΙΩΡΓΟΣ
@@ -289043,15 +289051,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5734
   authors:
-  - ΖΙΝΤ,ΑΝΤΡΕ
+  - GIDE,ANDRÉ,PAUL GUILLAUME
   language: el
   title: ΓΗΙΝΕΣ ΤΡΟΦΕΣ
   dewey: 889 ΖΙΝ
   entry_numbers:
   - '7190'
   editor: ΦΟΝΤΑΝΑ // ΑΘΗΝΑ
   edition_year: 1971
@@ -289547,15 +289555,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5744
   authors:
-  - ΜΠΑΡΤ,ΣΒΑΡΤΣ
+  - SCHWARZ-BART,ANDRÉ
   language: el
   title: Ο ΤΕΛΕΥΤΑΙΟΣ ΤΩΝ ΔΙΚΑΙΩΝ
   dewey: 889 ΜΠΑ
   entry_numbers:
   - '7178'
   translators:
   - ΠΟΡΦΥΡΗ,Κ.
@@ -290411,15 +290419,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5761
   authors:
-  - ΜΠΑΚ,ΠΕΡΛ
+  - BUCK,PEARL,S.
   language: el
   title: ΟΙ ΓΙΟΙ
   dewey: 889 ΜΠΑ
   entry_numbers:
   - '7136'
   translators:
   - ΑΝΑΓΝΩΣΤΟΠΟΥΛΟΣ,Π.
@@ -290462,15 +290470,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5762
   authors:
-  - ΜΠΑΚ,ΠΕΡΛ
+  - BUCK,PEARL,S.
   language: el
   title: ΚΑΤΩ ΑΠΟ ΤΟ ΒΛΕΜΜΑ ΤΟΥ ΒΟΥΔΑ
   dewey: 810.11 ΜΠΑ
   entry_numbers:
   - '7140'
   translators:
   - ΑΝΑΓΝΩΣΤΟΠΟΥΛΟΥ,Π.
@@ -290720,15 +290728,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5767
   authors:
-  - ΜΠΑΚ,ΠΕΡΛ
+  - BUCK,PEARL,S.
   language: el
   title: ΜΑΝΤΑΜ ΒΟΥ
   dewey: 889 ΜΠΑ
   entry_numbers:
   - '7150'
   translators:
   - ΜΑΡΑΓΚΟΠΟΥΛΟΥ,Ι.
@@ -291128,15 +291136,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5775
   authors:
-  - ΖΑΧΑΡΗ,ΛΑΜΠΡΟΥ
+  - ΖΑΧΑΡΗΣ,ΛΑΜΠΡΟΣ
   language: el
   title: ΓΙΑΤΙ Ο ΠΟΝΟΣ ΣΤΗ ΖΩΗ ΜΑΣ
   dewey: 889 ΖΑΧ
   entry_numbers:
   - '7154'
   editor: None // ΑΘΗΝΑ
   edition_year: 1971
@@ -291640,15 +291648,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5785
   authors:
-  - ΜΠΟΥΡΙΤΣΑ ΜΟΥΖΑΚΗ ΕΛΕΝΗ
+  - ΜΟΥΖΑΚΗ-ΜΠΟΥΡΙΤΣΑ,ΕΛΕΝΗ
   language: el
   title: ΣΤΑΘΜΟΙ ΑΓΑΠΗΣ
   dewey: 786.2 ΜΠΟ
   entry_numbers:
   - '9896'
   editor: ΥΔΡΟΓΕΙΟΣ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2009
@@ -294827,15 +294835,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 5849
   authors:
-  - ΜΠΡΕΤΟΝ,ΑΝΤΡΕ
+  - BRETON,ANDRÉ,ROBERT
   language: el
   title: ΜΑΝΙΦΕΣΤΑ ΣΟΥΡΡΕΑΛΙΣΜΟΥ
   entry_numbers:
   - '7111'
   editor: ΔΩΔΩΔΝΗ // ΑΘΗΝΑ
   edition_year: 1972
   pages: 222
@@ -296434,15 +296442,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5881
   authors:
-  - ΜΠΑΧ,Α.Μ
+  - BACH,ANNA,MAGDALENA
   language: el
   title: ΜΠΑΧ
   dewey: 780.92 ΜΠΑ
   entry_numbers:
   - '7243'
   translators:
   - ΔΡΟΣΟΣ,ΓΙΩΡΓΟΣ
@@ -297052,15 +297060,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5893
   authors:
-  - ΜΠΡΙΟΝ,ΜΑΡ.
+  - BRION,MARCEL
   language: el
   title: ΛΕΟΝΑΡΔΟΣ ΝΤΑ ΒΙΝΤΣΙ
   entry_numbers:
   - '6998'
   translators:
   - ΒΡΕΤΤΑΚΟΥ,ΝΙΚ.
   editor: ΒΙΒΛΙΟΕΚΔΟΤΙΚΗ // ΑΘΗΝΑ
@@ -297406,15 +297414,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5900
   authors:
-  - BIOT,R.
+  - BIOT,RENÉ
   language: el
   title: Η ΥΓΕΙΑ ΜΑΣ
   entry_numbers:
   - '7260'
   translators:
   - ΧΑΡΟΚΟΠΟΥ,ΔΗΜ.
   editor: None // ΑΘΗΝΑ
@@ -299813,15 +299821,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5948
   authors:
-  - JAEGER,WERNER
+  - JAEGER,WERNER,WILHELM
   language: el
   title: ΠΡΩΤΟΧΡΙΣΤΙΑΝΙΚΟΙ ΧΡΟΝΟΙ ΚΑΙ ΕΛΛΗΝΙΚΗ ΠΑΙΔΕΙΑ
   entry_numbers:
   - '7261'
   translators:
   - ΒΕΡΡΟΙΟΣ,ΓΕΩΡΓΙΟΣ
   editor: None // ΑΘΗΝΑ
@@ -300110,15 +300118,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5954
   authors:
-  - ΜΠΟΥΡΟΠΟΥΛΟΣ,Λ.
+  - ΜΠΟΥΡΟΠΟΥΛΟΣ,ΑΓΓΕΛΟΣ,ΝΙΚ.
   language: el
   title: ΚΩΔΙΞ ΠΟΛΙΤΙΚΗΣ ΔΙΚΟΝΟΜΙΑΣ
   entry_numbers:
   - '6986'
   editor: ΤΟ ΝΟΜΙΚΟΝ // ΑΘΗΝΑ
   edition_year: 1956
   pages: 733
@@ -307050,15 +307058,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 6093
   authors:
-  - ΜΠΟΡΟΒΙΤΣ,ΜΙΣΕΛ
+  - BORWICZ,MICHEL
   language: el
   title: ΓΡΑΦΤΑ ΤΩΝ ΜΕΛΛΟΘΑΝΑΤΩΝ ΑΠΟ ΤΗ ΝΑΖΙΣΤΙΚΗ ΚΑΤΟΧΗ
   dewey: 940.547 ΜΠΟ
   entry_numbers:
   - '6959'
   translators:
   - ΤΑΣΚΟΥ,ΔΗΜΗΤΡΑ
@@ -307724,15 +307732,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6106
   authors:
-  - ΖΙΝΤ,ΑΝΤΡΕ
+  - GIDE,ANDRÉ,PAUL GUILLAUME
   language: el
   title: ΠΟΙΜΕΝΙΚΗ ΣΥΜΦΩΝΙΑ
   entry_numbers:
   - '20614'
   translators:
   - ΒΕΖΥΡΟΠΟΥΛΟΥ,Ι.
   editor: ΗΡΙΔΑΝΟΣ // ΑΘΗΝΑ
@@ -308982,15 +308990,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6131
   authors:
-  - ΜΠΡΑΝΤΟΝ
+  - BRANDON,EDGAR EWING
   language: el
   title: ΙΣΤΟΡΙΑ ΤΩΝ ΗΝΩΜΕΝΩΝ ΠΟΛΙΤΕΙΩΝ ΤΗΣ ΑΜΕΡΙΚΗΣ
   dewey: 970 ΜΠΡ
   entry_numbers:
   - '7242'
   - '1278'
   editor: ΑΤΛΑΝΤΙΔΑ // NEW YORK
@@ -309895,15 +309903,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6149
   authors:
-  - ΖΟΛΑ,ΕΜΙΛ
+  - ZOLA,ÉMILE,ÉDOUARD CHARLES ANTOINE
   language: el
   title: Η ΚΟΥΖΙΝΑ
   dewey: 843 ΖΟΛ
   entry_numbers:
   - '6908'
   translators:
   - ΑΓΓΕΛΟΥ,ΓΙΑΝΝΗΣ
@@ -317717,15 +317725,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6308
   authors:
-  - ΜΠΑΡΙΤΑΚΗ,ΒΑΓΓΕΛΗ
+  - ΜΠΑΡΙΤΑΚΗΣ,ΒΑΓΓΕΛΗΣ
   language: el
   title: ΓΟΥΒΕΣ 1940-44
   entry_numbers:
   - '8209'
   editor: None // ΓΟΥΒΕΣ
   edition_year: 2000
   pages: 62
@@ -318208,15 +318216,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6318
   authors:
-  - ΖΗΣΙΑΔΗ,ΒΑΣΙΛΕΙΟΥ
+  - ΖΗΣΙΑΔΗΣ,ΒΑΣΙΛΕΙΟΣ
   language: el
   title: Η ΟΙΚΟΝΟΜΙΚΗ ΕΓΚΛΗΜΑΤΙΚΟΤΗΤΑ
   subtitle: ΤΟ ΟΥΣΙΑΣΤΙΚΟ ΚΑΙ ΔΙΚΟΝΟΜΙΚΟ ΟΙΚΟΝΟΜΙΚΟ ΠΟΙΝΙΚΟ ΔΙΚΑΙΟ
   entry_numbers:
   - '8219'
   editor: ΣΑΚΚΟΥΛΑ // ΑΘΗΝΑ
   edition_year: 2001
@@ -319952,15 +319960,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6353
   authors:
-  - ΖΙΓΚΜΑΝ,ΛΩΡΑ
+  - ZIGMAN,LAURA
   language: el
   title: ΑΡΣΕΝΙΚΟ ΚΑΙ ΠΑΛΙΑ ΓΕΛΑΔΑ
   dewey: 889 ΖΙΓ
   entry_numbers:
   - '8254'
   translators:
   - ΔΗΜΗΤΡΑ,ΜΑΡΙΝΑ
@@ -321427,15 +321435,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6383
   authors:
-  - ΜΠΕΛΛ,ΧΑΙΝΡΙΧ
+  - BÖLL,HEINRIC
   language: el
   title: Ο ΧΛΩΜΟΣ ΣΚΥΛΟΣ
   entry_numbers:
   - '8284'
   editor: ΠΟΛΙΣ // ΑΘΗΝΑ
   edition_year: 1995
   pages: 231
@@ -322176,15 +322184,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6398
   authors:
-  - ΖΟΡΜΠΑ,ΠΑΝΟΥ
+  - ΖΟΡΜΠΑΣ,ΠΑΝΟΣ
   language: el
   title: ΥΠΟΔΕΙΓΜΑ ΠΡΟΣΦΥΓΩΝ
   subtitle: ΣΤΑ ΔΙΟΙΚΗΤΙΚΑ ΔΙΚΑΣΤΗΡΙΑ ΓΙΑ ΥΠΟΘΕΣΕΙΣ ΚΟΙΝΩΝΙΚΗΣ ΑΣΦΑΛΙΣΗΣ
   entry_numbers:
   - '8299'
   editor: ΑΜΑΔΑΡΟΣ // ΑΘΗΝΑ
   edition_year: 1996
@@ -327843,15 +327851,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6514
   authors:
-  - ΜΠΑΛΕΣΤΡΙΝΙ,ΝΑΝΝΙ
+  - BALESTRINI,NANNI
   language: el
   title: ΤΑ ΘΕΛΟΥΜΕ ΟΛΑ
   dewey: 850.11 ΜΠΑ
   entry_numbers:
   - '8669'
   editor: ΣΤΟΧΑΣΤΗΣ // ΑΘΗΝΑ
   edition_year: 1979
@@ -327892,15 +327900,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6515
   authors:
-  - ΜΠΟΡΟΒΣΚΙ,ΤΑΝΤΕΟΥΣ
+  - BOROWSKI,TADEUSZ
   language: el
   title: ΑΠΟ ΔΩ ΓΙΑ ΤΑ ΑΕΡΙΑ ΚΥΡΙΕΣ ΚΑΙ ΚΥΡΙΟΙ
   dewey: 938.87 ΜΠΟ
   entry_numbers:
   - '8645'
   editor: ΣΤΟΧΑΣΤΗΣ // ΑΘΗΝΑ
   edition_year: 1981
@@ -333632,15 +333640,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6633
   authors:
-  - ΜΠΡΙΝΑ ΣΒΙΤ
+  - SVIT,BRINA
   title: CON BRIO Η ΤΟ ΧΡΟΝΙΚΟ ΕΝΟΣ ΕΡΩΤΑ
   dewey: 843 ΣΒΙ
   entry_numbers:
   - '8695'
   translators:
   - ΑΒΑΓΙΑΝΟΥ,ΛΟΙΣΚΑ
   editor: ΠΑΤΑΚΗ // ΑΘΗΝΑ
@@ -333937,15 +333945,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6639
   authors:
-  - ΖΙΡΑΡ,ΠΑΤΡΙΚ
+  - GIRARD,PATRICK
   language: el
   title: ΑΜΙΛΚΑΣ ΤΟ ΛΙΟΝΤΑΡΙ ΤΗΣ ΑΜΜΟΥ
   dewey: 843 ΖΙΡ
   entry_numbers:
   - '8701'
   translators:
   - ΡΑΙΚΟΣ,ΓΙΩΡΓΟΣ
@@ -337445,15 +337453,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6710
   authors:
-  - ΜΠΕΡΛΙΝΓΚ,ΠΕΤΕΡ
+  - BERLING,PETER
   language: el
   title: Ο ΘΡΟΝΟΣ ΤΩΝ ΒΑΣΙΛΕΩΝ
   dewey: 830.11 ΜΠΕ
   entry_numbers:
   - '8842'
   translators:
   - ΑΓΓΕΛΙΔΟΥ,ΜΑΡΙΑ
@@ -337600,15 +337608,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6713
   authors:
-  - ΜΠΙΧΕΛ,ΠΑΟΥΛ
+  - BIEGEL,PAUL
   language: el
   title: ΙΣΤΟΡΙΕΣ ΤΗΣ ΝΥΧΤΑΣ
   dewey: 808.899 ΜΠΙ
   entry_numbers:
   - '8845'
   translators:
   - ΧΟΥΚ-ΑΠΟΣΤΟΛΟΠΟΥΛΟΥ,ΕΛΕΝΗ
@@ -341322,15 +341330,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6789
   authors:
-  - ΜΠΑΡΤΖΩΚΑΣ,ΚΙΜΩΝ
+  - ΜΠΑΡΤΖΩΚΑΣ,ΚΙΜΩΝΑΣ
   language: el
   title: ΕΥΘΥΜΕΣ ΛΑΟΓΡΑΦΙΚΕΣ ΙΣΤΟΡΙΕΣ
   dewey: 398 ΜΠΑ
   entry_numbers:
   - '8914'
   editor: None // ΑΘΗΝΑ
   edition_year: 2006
@@ -341371,15 +341379,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6790
   authors:
-  - ΜΠΑΡΤΖΩΚΑΣ,ΚΙΜΩΝ
+  - ΜΠΑΡΤΖΩΚΑΣ,ΚΙΜΩΝΑΣ
   language: el
   title: ΔΙΑΧΡΟΝΙΚΑ ΕΥΘΥΜΟΓΡΑΦΗΜΑΤΑ
   dewey: 398 ΜΠΑ
   entry_numbers:
   - '8913'
   - '9508'
   editor: None // ΑΘΗΝΑ
@@ -341715,15 +341723,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6797
   authors:
-  - ΜΠΡΑΤΣΙΩΤΟΥ,ΝΙΚΟΛΑΟΥ
+  - ΜΠΡΑΤΣΙΩΤΗΣ,ΝΙΚΟΛΑΟΣ
   language: el
   title: Η ΘΕΣΙΣ ΤΟΥ ΑΤΟΜΟΥ ΕΝ ΤΗ ΠΑΛΑΙΑ ΔΙΑΘΗΚΗ
   dewey: 221 ΜΠΡ
   entry_numbers:
   - '8953'
   editor: None // ΑΘΗΝΑ
   edition_year: 1983
@@ -342055,15 +342063,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6804
   authors:
-  - ΖΩΓΡΑΦΟ,ΤΑΣΟ
+  - ΖΩΓΡΑΦΟΣ,ΤΑΣΟΣ
   language: el
   title: Η ΙΣΤΟΡΙΑ ΤΗΣ ΜΙΚΡΗΣ ΓΑΛΑΖΙΑΣ ΚΟΛΟΚΥΘΑΣ
   entry_numbers:
   - '8907'
   editor: ΠΡΟΣΚΗΝΙΟ // ΑΘΗΝΑ
   edition_year: 2001
   pages: 55
@@ -343485,15 +343493,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6833
   authors:
-  - ΖΟΛΑ,ΑΙΜΙΛ
+  - ZOLA,ÉMILE,ÉDOUARD CHARLES ANTOINE
   language: el
   title: ΑΝΘΡΩΠΙΝΟ ΚΤΗΝΟΣ-ΑΒΒΑ ΜΟΥΡΕ-ΥΠΟΘΕΣΗ ΝΤΡΕΥΦΟΥΣ ΚΑΤΗΓΟΡΩ
   dewey: 843 ΖΟΛ
   entry_numbers:
   - '8926'
   translators:
   - ΠΙΚΡΟΣ,ΠΕΤΡΟΣ
@@ -343535,15 +343543,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6834
   authors:
-  - ΖΟΛΑ,ΑΙΜΙΛ
+  - ZOLA,ÉMILE,ÉDOUARD CHARLES ANTOINE
   language: el
   title: ΤΑΒΕΡΝΑ-ΜΑΓΔΑΛΗΝΗ ΦΕΡΑ-ΤΡΕΙΣ ΘΑΝΑΤΟΙ
   dewey: 843 ΖΟΛ
   entry_numbers:
   - '8927'
   translators:
   - ΠΙΚΡΟΣ,ΠΕΤΡΟΣ
@@ -343685,15 +343693,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6837
   authors:
-  - ΜΠΑΛΖΑΚ
+  - BALZAC,HONORÉ DE
   language: el
   title: ΕΥΓΕΝΙΑ ΓΚΡΑΝΤΕ-ΜΠΑΡΜΠΑ ΓΚΟΡΙΟ-ΜΑΓΙΚΟ ΔΕΡΜΑ
   dewey: 843 ΜΠΑ
   entry_numbers:
   - '8931'
   translators:
   - ΝΙΚΑ,ΑΓΓΕΛΟΣ
@@ -343832,15 +343840,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6840
   authors:
-  - ΜΠΕΡΝΤ,ΛΟΥΙΖΑ
+  - BIRD,LOIS
   language: el
   title: Ο ΕΡΩΤΑΣ ΜΕΤΑ ΤΟ ΓΑΜΟ
   dewey: 170 ΜΠΕ
   entry_numbers:
   - '8972'
   translators:
   - ΚΟΝΤΟΣΙΑΝΟΣ,ΑΝΔΡΕΑΣ
@@ -348017,15 +348025,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6925
   authors:
-  - ΜΠΑΖΙΛΙ,Κ.Μ
+  - BAZILI,KONSTANTIN,M.
   language: el
   title: ΕΝΑΣ ΡΩΣΟΣ ΣΤΗΝ ΕΛΛΑΔΑ ΤΟΥ ΚΑΠΟΔΙΣΤΡΙΑ
   subtitle: ΤΟ ΑΡΧΙΠΕΛΑΓΟΣ ΚΑΙ Η ΕΛΛΑΔΑ ΣΤΑ 1830-1831
   dewey: 938.571 ΜΠΑ
   entry_numbers:
   - '5311'
   editor: ΚΑΛΕΝΤΗΣ // ΑΘΗΝΑ
@@ -352037,15 +352045,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7006
   authors:
-  - ΖΕΓΚΕΡΣ ΑΝΝΑ
+  - SEGHERS,ANNA
   language: el
   title: Ο ΕΒΔΟΜΟΣ ΣΤΑΥΡΟΣ
   dewey: 830.11 ΖΕΓ
   entry_numbers:
   - '9059'
   translators:
   - ΚΑΜΠΟΥΡΙΔΗΣ,ΣΤΑΥΡΟΣ
@@ -353628,15 +353636,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7038
   authors:
-  - ΖΙΣΚΙΝΤ,ΠΑΤΡΙΚ
+  - SÜSKIND,PATRICK
   language: el
   title: ΤΟ ΑΡΩΜΑ
   dewey: 889 ΖΙΣ
   entry_numbers:
   - '9106'
   translators:
   - ΑΓΓΕΛΙΔΟΥ,ΜΑΡΙΑ
@@ -354770,15 +354778,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7061
   authors:
-  - BOSSET,C.P.
+  - BOSSET,C.,P.
   language: el
   title: Η ΠΑΡΓΑ ΚΑΙ ΤΑ ΙΟΝΙΑ ΝΗΣΙΑ
   dewey: 938.93 BOS
   entry_numbers:
   - '9134'
   editor: ΔΩΔΩΝΗ // ΙΩΑΝΝΙΝΑ
   edition_year: 2000
@@ -355963,15 +355971,16 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7085
   authors:
-  - ΖΑΧΟΣ,Χ-ΤΟΥΜΠΟΥΡΟΣ,Χ.
+  - ΖΑΧΟΣ,Χ.
+  - ΤΟΥΜΠΟΥΡΟΣ,Χ.
   language: el
   title: ΑΓΝΑΝΤΙΤΙΚΑ ΛΙΧΝΙΣΜΑΤΑ
   dewey: 398 ΖΑΧ
   entry_numbers:
   - '9150'
   editor: None // ΑΘΗΝΑ
   edition_year: 2007
@@ -357874,15 +357883,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7123
   authors:
-  - ΖΑΧΑΡΗ-ΜΑΤΣΟΥΚΑ ΠΟΠΗ
+  - ΖΑΧΑΡΗ-ΜΑΤΣΟΥΚΑ,ΠΟΠΗ
   language: el
   title: ΔΟΚΙΜΙΑ
   subtitle: ΕΞΕΧΟΥΣΕΣ ΙΣΤΟΡΙΚΕΣ ΚΑΙ ΛΟΓΟΤΕΧΝΙΚΕΣ ΜΟΡΦΕΣ
   dewey: 889.21 ΖΑΧ
   entry_numbers:
   - '6856'
   editor: ΔΩΔΩΝΗ // ΑΘΗΝΑ-ΙΩΑΝΝΙΝΑ
@@ -361021,15 +361030,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7184
   authors:
-  - ΜΠΛΟΚ,ΛΟΡΕΝΣ
+  - BLOCK,LAWRENCE
   language: el
   title: Ο ΔΙΑΡΡΗΚΤΗΣ ΠΟΥ ΖΩΓΡΑΦΙΖΕ ΣΑΝ ΤΟΝ ΜΟΝΤΡΙΑΝ
   dewey: 810.11 ΜΠΛ
   entry_numbers:
   - '9230'
   - '12492'
   - '20617'
@@ -361127,15 +361136,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7186
   authors:
-  - BALLARD,J.G.
+  - BALLARD,JAMES,GRAHAM
   language: el
   title: Η ΜΕΡΑ ΤΗΣ ΔΗΜΙΟΥΡΓΙΑΣ
   dewey: 823 BAL
   entry_numbers:
   - '9239'
   translators:
   - ΜΠΑΡΜΠΗΣ,ΚΩΣΤΑΣ
@@ -361382,15 +361391,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7191
   authors:
-  - ΖΟΛΑ,ΕΜΙΛ
+  - ZOLA,ÉMILE,ÉDOUARD CHARLES ANTOINE
   language: el
   title: ΝΑΝΑ
   dewey: 843 ΖΟΛ
   entry_numbers:
   - '9260'
   translators:
   - ΠΡΑΤΣΙΚΑΣ,ΓΙΩΡΓΟΣ
@@ -366620,15 +366629,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7296
   authors:
-  - ΜΠΕΝΓΤΣΟΝ,ΧΕΡΜΑΝ
+  - BENGTSON,HERMANN
   language: el
   title: ΙΣΤΟΡΙΑ ΤΗΣ ΑΡΧΑΙΑΣ ΕΛΛΑΔΟΣ
   entry_numbers:
   - '9191'
   translators:
   - ΓΑΒΡΙΛΗΣ,ΑΝΤΡΕΑΣ
   editor: ΜΕΛΙΣΣΑ // ΑΘΗΝΑ
@@ -369193,15 +369202,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7348
   authors:
-  - ΜΠΑΛΑΣΚΑ,ΓΡΗΓΟΡΙΟΥ
+  - ΜΠΑΛΑΣΚΑΣ,ΓΡΗΓΟΡΙΟΣ
   language: el
   title: ΤΕΤΡΑΚΩΜΟ ΜΗΓΕΡΙ
   subtitle: ΕΝΑ ΞΕΧΑΣΜΕΝΟ ΧΩΡΙΟ
   dewey: 938.939 ΜΠΑ
   entry_numbers:
   - '5377'
   editor: ΚΑΛΑΜΑΣ // ΑΘΗΝΑ
@@ -370344,15 +370353,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7371
   authors:
-  - ΖΟΛΑ,ΕΜΙΛ
+  - ZOLA,ÉMILE,ÉDOUARD CHARLES ANTOINE
   language: el
   title: ΝΑΝΑ
   dewey: 843 ΖΟΛ
   entry_numbers:
   - '9260'
   editor: ΓΚΟΒΟΣΤΗΣ // None
   pages: 536
@@ -375242,15 +375251,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7468
   authors:
-  - ΜΠΑΛΖΑΚ, ΝΤΕ, ΟΝΟΡΕ
+  - BALZAC,HONORÉ DE
   language: el
   title: Ο ΕΞΑΔΕΛΦΟΣ ΠΟΝΣ
   dewey: 889 ΜΠΑ
   entry_numbers:
   - '9940'
   translators:
   - ΦΡΑΓΚΙΑΣ,ΑΝΔΡΕΑΣ
@@ -375757,15 +375766,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7478
   authors:
-  - ΒΛΑΧΟΣ,ΑΓΓΕΛΟΣ,ΣΤ,
+  - ΒΛΑΧΟΣ,ΑΓΓΕΛΟΣ,ΣΤ.
   language: el
   title: ΤΟ ΜΝΗΜΑ ΤΗΣ ΓΡΗΑΣ ΚΑΙ ΟΙ ΩΡΕΣ ΖΩΗΣ
   dewey: 889.21 ΒΛΑ
   entry_numbers:
   - '9934'
   edition: '2'
   editor: ΓΑΛΑΞΙΑΣ // ΑΘΗΝΑ
@@ -378619,15 +378628,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7535
   authors:
-  - ΜΠΑΡΜΠΑΣ ΒΑΣΟΣ
+  - ΜΠΑΡΜΠΑΣ,ΒΑΣΟΣ
   language: el
   title: ΓΙΑ ΜΙΑ ΧΑΡΟΥΜΕΝΗ ΓΕΝΙΑ
   dewey: 889.1 ΜΠΑ
   entry_numbers:
   - '7775'
   editor: None // ΑΘΗΝΑ
   edition_year: 1997
@@ -378861,15 +378870,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7540
   authors:
-  - ΜΠΙΣΤΗΣ ΝΙΚΟΣ
+  - ΜΠΙΣΤΗΣ,ΝΙΚΟΣ
   language: el
   title: ΛΟΓΙΣΜΟΙ
   entry_numbers:
   - '10098'
   editor: None // ΑΘΗΝΑ
   edition_year: 1965
   pages: 38
@@ -379439,15 +379448,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7552
   authors:
-  - ΖΙΓΔΗΣ ΙΩΑΝΝΗΣ
+  - ΖΙΓΔΗΣ,ΙΩΑΝΝΗΣ,Γ.
   language: el
   title: Η ΣΤΡΑΤΗΓΙΚΗ ΤΗΣ ΕΚΒΙΟΜΗΧΑΝΙΣΕΩΣ
   entry_numbers:
   - '10086'
   editor: None // ΑΘΗΝΑ
   edition_year: 1963
   pages: 31
@@ -380065,15 +380074,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7565
   authors:
-  - ΖΑΡΙΦΟΠΟΥΛΟΣ ΓΡΗΓΟΡΙΟΣ
+  - ΖΑΡΙΦΟΠΟΥΛΟΣ,ΓΡΗΓΟΡΙΟΣ
   language: el
   title: ΔΙΚΟΝΟΜΙΑ ΔΙΟΙΚΗΤΙΚΗΣ ΕΚΤΕΛΕΣΕΩΣ
   entry_numbers:
   - '10058'
   editor: None // ΑΘΗΝΑ
   edition_year: 1931
   pages: 387
@@ -381307,15 +381316,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7591
   authors:
-  - ΖΟΛΩΤΑΣ ΞΕΝΟΦΩΝ
+  - ΖΟΛΩΤΑΣ,ΞΕΝΟΦΩΝ
   language: el
   title: ΟΙ ΣΥΝΤΕΛΕΣΤΑΙ ΤΗΣ ΚΟΙΝΩΝΙΚΗΣ ΕΥΗΜΕΡΙΑΣ
   entry_numbers:
   - '9990'
   editor: ΑΡΓΥΡΗΣ ΠΑΠΑΖΗΣΗΣ // ΑΘΗΝΑ
   edition_year: 1946
   pages: 32
@@ -382316,15 +382325,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7612
   authors:
-  - ΖΑΡΡΑΣ ΙΩΑΝΝΗΣ
+  - ΖΑΡΡΑΣ,ΙΩΑΝΝΗΣ
   language: el
   title: ΤΟ ΣΥΝΕΤΑΙΡΙΣΤΙΚΟΝ ΚΙΝΗΜΑ ΤΗΣ ΠΑΛΑΙΣΤΙΝΗΣ
   entry_numbers:
   - '10012'
   editor: ΠΑΠΑΔΗΜΗΤΡΙΟΥ // ΑΘΗΝΑ
   edition_year: 1945
   pages: 28
@@ -382843,15 +382852,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7623
   authors:
-  - ΖΑΚΑΣ ΠΑΝΟΣ
+  - ΖΑΚΑΣ,ΠΑΝΟΣ
   language: el
   title: ΝΟΜΟΘΕΣΙΑ ΤΩΝ ΔΗΜΟΣΙΩΝ ΕΡΓΩΝ
   entry_numbers:
   - '10041'
   editor: ΜΑΡΖΕΛΟΣ // ΜΥΤΙΛΗΝΗ
   edition_year: 1937
   pages: 284
@@ -384550,15 +384559,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7658
   authors:
-  - ΜΠΑΡΤΖΩΚΑΣ ΚΙΜΩΝ
+  - ΜΠΑΡΤΖΩΚΑΣ,ΚΙΜΩΝΑΣ
   language: el
   title: 60 ΔΙΑΧΡΟΝΙΚΑ ΕΥΘΥΜΟΓΡΑΦΗΜΑΤΑ ΧΡΟΝΟΓΡΑΦΗΜΑΤΑ
   dewey: 398 ΜΕΛ
   entry_numbers:
   - '10529'
   editor: ΧΑΡΗΣ ΠΑΤΣΗΣ // ΑΘΗΝΑ
   edition_year: 2011
@@ -385142,15 +385151,18 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7670
   authors:
-  - ΜΠΟΥΡΗΣ. ΣΤΑΥΡΟΠΟΥΛΟΣ. ΤΕΝΤΖΕΡΑΚΗΣ
+  - ΠΑΠΆ-ΣΈΒΟΥ,ΜΊΚΑ
+  - ΜΠΟΎΡΗΣ,ΑΝΔΡΈΑΣ
+  - ΣΤΑΥΡΌΠΟΥΛΟΣ,ΛΕΥΤΈΡΗΣ
+  - ΤΕΝΤΖΕΡΆΚΗΣ,ΧΡΉΣΤΟΣ
   language: el
   title: Η ΜΟΥΣΙΚΟΧΟΡΕΥΤΙΚΗ ΠΑΡΑΔΟΣΗ ΤΗΣ ΣΚΛΙΒΑΝΗΣ ΙΩΑΝΝΙΝΩΝ
   dewey: 398 ΜΠΟ
   entry_numbers:
   - '10164'
   editor: None // ΙΩΑΝΝΙΝΑ
   edition_year: 2002
@@ -385697,15 +385709,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 7681
   authors:
-  - ΜΠΟΥΣΚΑΛΙΑ ΛΕΟ
+  - BUSCAGLIA,LEO
   language: el
   title: ΛΕΩΦΟΡΕΙΟ 9 ΓΙΑ ΤΟΝ ΠΑΡΑΔΕΙΣΟ
   dewey: 850.11 ΜΠΟ
   entry_numbers:
   - '10178'
   translators:
   - ΚΩΣΤΕΛΕΝΟΣ,ΔΗΜΗΤΡΗΣ
@@ -386307,15 +386319,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7693
   authors:
-  - ΖΕΡΒΑΣ ΓΙΑΝΝΗΣ
+  - ΖΕΡΒΑΣ,ΓΙΑΝΝΗΣ
   language: el
   title: Η ΖΩΗ ΕΙΝΑΙ ΩΡΑΙΑ
   dewey: 610 ΖΕΡ
   entry_numbers:
   - '10189'
   editor: ΕΠΙΓΝΩΣΙΣ // ΑΘΗΝΑ
   edition_year: 2006
@@ -386410,15 +386422,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7695
   authors:
-  - ΖΥΓΟΥΡΗΣ ΣΩΤΗΡΗΣ
+  - ΖΥΓΟΥΡΗΣ,ΣΩΤΗΡΗΣ
   language: el
   title: ΤΟ ΣΩΜΑ ΤΗΣ ΑΝΟΙΞΗΣ
   dewey: 889.1 ΖΥΓ
   entry_numbers:
   - '10187'
   editor: None // ΑΡΤΑ
   edition_year: 1996
@@ -386566,15 +386578,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7698
   authors:
-  - ΜΠΙΟΥΜΠΙ ΦΡΙΝΤΑ
+  - ΜΠΙΟΥΜΠΙ,ΦΡΙΝΤΑ
   language: el
   title: ΔΕΚΑΤΡΙΑ ΦΕΓΓΑΡΙΑ ΜΕΤΑ
   dewey: 889.21 ΜΠΙ
   entry_numbers:
   - '10195'
   edition: '11'
   editor: ΕΞΑΝΤΑΣ // ΑΘΗΝΑ
@@ -387076,15 +387088,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7708
   authors:
-  - ΖΥΓΟΥΡΗΣ ΣΩΤΗΡΗΣ
+  - ΖΥΓΟΥΡΗΣ,ΣΩΤΗΡΗΣ
   language: el
   title: ΤΑ ΠΟΙΗΜΑΤΑ
   subtitle: 1975-2003
   dewey: 889.1 ΖΥΓ
   entry_numbers:
   - '10199'
   editor: ΠΕΤΡΑ // ΑΘΗΝΑ
@@ -388726,15 +388738,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7741
   authors:
-  - ΜΠΟΥΣΙΑΣ ΠΑΝΑΓΙΩΤΗΣ
+  - ΜΠΟΥΣΙΑΣ,ΠΑΝΑΓΙΩΤΗΣ
   language: el
   title: ΠΑΝΑΓΙΑ ΡΟΒΕΛΙΣΤΑ
   dewey: 230 ΜΠΟ
   entry_numbers:
   - '10236'
   editor: None // ΑΘΗΝΑ
   edition_year: 1989
@@ -389025,15 +389037,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7747
   authors:
-  - ΜΠΕΚΟΣ ΔΙΟΝΥΣΙΟΣ
+  - ΜΠΕΚΟΣ,ΔΙΟΝΥΣΙΟΣ
   language: el
   title: ΜΗΝ ΚΑΝΕΙΣ ΚΑΚΟ ΣΤΗΝ ΨΥΧΗ ΣΟΥ
   dewey: 230 ΜΠΕ
   entry_numbers:
   - '10230'
   editor: ΧΡΙΣ.ΣΤΕΓΗ ΚΑΛΑΜΑΤΑΣ // None
   edition_year: 2001
@@ -389516,15 +389528,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7757
   authors:
-  - ΖΩΡΑΣ ΓΕΡΑΣΙΜΟΣ
+  - ΖΩΡΑΣ,ΓΕΡΑΣΙΜΟΣ
   language: el
   title: ΦΙΛΟΛΟΓΙΚΑ ΜΕΛΕΤΗΜΑΤΑ
   dewey: 889 ΖΩΡ
   entry_numbers:
   - '6829'
   editor: ΔΟΜΟΣ // ΑΘΗΝΑ
   edition_year: 1993
@@ -390711,15 +390723,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7781
   authors:
-  - ΖΩΓΡΑΦΟΥ ΛΙΛΗ
+  - ΖΩΓΡΑΦΟΥ,ΛΙΛΗ
   language: el
   title: ΠΑΛΑΙΟΠΩΛΗΣ ΑΝΑΜΝΗΣΕΩΝ
   dewey: 889.21 ΖΩΓ
   entry_numbers:
   - '9462'
   edition: '3'
   editor: ΓΑΒΡΙΗΛΙΔΗΣ // ΑΘΗΝΑ
@@ -390909,15 +390921,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7785
   authors:
-  - ΖΩΓΡΑΦΟΥ ΜΑΡΙΝΑ
+  - ΖΩΓΡΑΦΟΥ,ΜΑΡΙΝΑ
   language: el
   title: ΕΚΣΤΑΣΗ
   dewey: 889.21 ΖΩΓ
   entry_numbers:
   - '7683'
   editor: ΓΚΟΒΟΣΤΗ // ΑΘΗΝΑ
   pages: 133
@@ -392602,15 +392614,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7819
   authors:
-  - ΖΗΚΟΥ ΜΑΙΡΗ
+  - ΖΗΚΟΥ,ΜΑΙΡΗ
   language: el
   title: Η ΠΡΟΣΤΥΧΗ
   dewey: 889.21 ΖΗΚ
   entry_numbers:
   - 09160
   editor: ΜΟΝΤΕΡΝΟΙ ΚΑΙΡΟΙ // ΑΘΗΝΑ
   edition_year: 2007
@@ -393893,15 +393905,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7844
   authors:
-  - ΜΠΑΓΙΕΡ ΤΟΜΜΥ
+  - BAYER,TOMMY
   language: el
   title: ΜΙΑ ΥΠΕΡΒΟΛΙΚΗ ΔΟΣΗ ΕΡΩΤΑ
   dewey: 830.11 ΜΠΑ
   entry_numbers:
   - '10283'
   translators:
   - ΑΓΓΕΛΙΔΟΥ,ΜΑΡΙΑ
@@ -394149,15 +394161,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7849
   authors:
-  - ΜΠΑΛΖΑΚ ΟΝΟΡΕ
+  - BALZAC,HONORÉ DE
   language: el
   title: ΕΥΓΕΝΙΑ ΓΚΡΑΝΤΕ
   dewey: 843 ΜΠΑ
   entry_numbers:
   - '8492'
   translators:
   - ΜΠΙΤΖΙΛΕΚΗ,ΔΙΟΝΥΣΙΑ
@@ -395059,15 +395071,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7867
   authors:
-  - ΖΟΛΑ ΑΙΜ
+  - ZOLA,ÉMILE,ÉDOUARD CHARLES ANTOINE
   language: el
   title: Η ΝΑΝΑ
   dewey: 843 ΖΟΛ
   entry_numbers:
   - '10322'
   editor: Ο ΦΟΙΒΟΣ // ΑΘΗΝΑ
   pages: 223
@@ -395207,15 +395219,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7870
   authors:
-  - BALZC
+  - BALZAC,HONORÉ DE
   language: el
   title: ΟΙ ΓΑΜΟΙ ΤΗΣ ΑΔΕΛΙΑΣ
   dewey: 843 BAL
   entry_numbers:
   - '8106'
   editor: ΤΥΠΟΣ // ΑΘΗΝΑ
   pages: 64
@@ -395907,15 +395919,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7884
   authors:
-  - BOVET THEODOR
+  - BOVET,THEODOR
   language: el
   title: Ο ΓΑΜΟΣ
   dewey: 830.11 BOV
   entry_numbers:
   - '10326'
   translators:
   - ΖΑΝΝΗΣ,ΤΑΣΟΣ
@@ -395959,15 +395971,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7885
   authors:
-  - AJAR,EMILE
+  - GARY,ROMAIN@EMILE AJAR
   language: el
   title: Η ΖΩΗ ΜΠΡΟΣΤΑ ΣΟΥ
   dewey: 843 AJA
   entry_numbers:
   - '10325'
   translators:
   - ΜΟΥΡΕΛΑΤΟΥ,ΡΕΝΑ
@@ -397575,15 +397587,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7917
   authors:
-  - ΜΠΟΥΛΓΚΑΚΩΦ Μ.
+  - BULGAKOV,MIKHAIL
   language: el
   title: ΛΕΥΚΗ ΦΡΟΥΡΑ
   dewey: 891.73 ΜΠΟ
   entry_numbers:
   - '10353'
   translators:
   - ΦΡΑΓΚΙΑΣ,ΑΝΔΡΕΑΣ
@@ -399132,15 +399144,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7948
   authors:
-  - ΖΑΧΑΡΗ-ΜΑΤΣΟΥΚΑ ΠΟΠΗ
+  - ΖΑΧΑΡΗ-ΜΑΤΣΟΥΚΑ,ΠΟΠΗ
   language: el
   title: ΣΤΟΝ ΣΤΕΡΙΣΜΟ ΤΗΣ ΝΟΣΤΑΛΓΙΑΣ
   dewey: 889.1 ΖΑΧ
   entry_numbers:
   - '6811'
   editor: None // ΑΘΗΝΑ
   edition_year: 1994
@@ -400224,15 +400236,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7970
   authors:
-  - ΜΠΕΝΑΤΣΗΣ ΑΠΟΣΤΟΛΟΣ
+  - ΜΠΕΝΑΤΣΗΣ,ΑΠΟΣΤΟΛΟΣ
   language: el
   title: ΚΩΣΤΑΣ ΚΑΡΥΩΤΑΚΗΣ
   dewey: 889.19 ΜΠΕ
   entry_numbers:
   - '9866'
   editor: ΜΕΤΑΙΧΜΙΟ // ΑΘΗΝΑ
   edition_year: 2004
@@ -400768,15 +400780,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7981
   authors:
-  - ΜΠΙΡΜΠΙΛΗ ΕΛΕΝΗ
+  - ΜΠΙΡΜΠΙΛΗ,ΕΛΕΝΗ
   language: el
   title: Η ΝΥΧΤΑ ΤΗΣ ΜΕΓΑΛΗΣ ΟΡΓΗΣ
   subtitle: ΤΟ ΧΡΟΝΙΚΟ ΜΙΑΣ ΕΞΕΓΕΡΣΗΣ
   dewey: 889.21 ΜΠΙ
   entry_numbers:
   - '10397'
   editor: ΜΠΑΡΤΖΟΥΛΙΑΝΟΣ // ΑΘΗΝΑ
@@ -401605,15 +401617,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7998
   authors:
-  - ΖΑΡΚΙΑ ΣΤΑΘΗ
+  - ΖΑΡΚΙΑΣ,ΣΤΑΘΗΣ
   language: el
   title: ΝΑΡΚΙΣΣΟΙ
   dewey: 889.1 ΖΑΡ
   entry_numbers:
   - '8009'
   editor: ΤΟ ΕΛΛΗΝΙΚΟ ΒΙΒΛΙΟ // ΑΘΗΝΑ
   edition_year: 1976
@@ -402350,15 +402362,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8013
   authors:
-  - ΜΠΑΣΙΑΚΟΣ ΙΩΑΝΝΗΣ
+  - ΜΠΑΣΙΑΚΟΣ,ΙΩΑΝΝΗΣ
   language: el
   title: ΤΟ ΑΓΓΙΓΜΑ ΤΗΣ ΨΥΧΗΣ
   dewey: 889.1 ΜΠΑ
   entry_numbers:
   - '7785'
   - '7724'
   editor: None // ΑΘΗΝΑ
@@ -403539,15 +403551,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8037
   authors:
-  - ΜΠΑΜΠΑΛΗ ΑΓΓΕΛΙΚΗ
+  - ΜΠΑΜΠΑΛΗ,ΑΓΓΕΛΙΚΗ
   language: el
   title: Η ΠΝΕΥΜΑΤΙΚΗ ΑΤΡΑΠΟΣ
   dewey: 889.1 ΜΠΑ
   entry_numbers:
   - '7835'
   editor: None // ΑΘΗΝΑ
   edition_year: 1993
@@ -404676,15 +404688,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8060
   authors:
-  - ΜΠΟΛΕΤΣΗΣ ΣΤΕΦΑΝΟΣ
+  - ΜΠΟΛΕΤΣΗΣ,ΣΤΕΦΑΝΟΣ
   language: el
   title: ΔΙΑΔΡΟΜΗ
   subtitle: ΠΟΙΗΣΗ Η ΜΙΑ
   dewey: 889.1 ΜΠΟ
   entry_numbers:
   - '10421'
   editor: ΔΑΜΑΣΚΟΣ // ΑΘΗΝΑ
@@ -404972,15 +404984,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8066
   authors:
-  - ΜΠΟΛΕΤΣΗΣ ΣΤΕΦΑΝΟΣ
+  - ΜΠΟΛΕΤΣΗΣ,ΣΤΕΦΑΝΟΣ
   language: el
   title: ΜΥΣΤΙΚΟΣ ΒΙΟΣ
   dewey: 889.1 ΜΠΟ
   entry_numbers:
   - '10412'
   editor: ΔΑΜΑΣΚΟΣ // ΑΘΗΝΑ
   edition_year: 1989
@@ -405022,15 +405034,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8067
   authors:
-  - ΖΙΤΣΑΙΑ ΧΡΥΣΑΝΘΗ
+  - ΖΙΤΣΑΙΑ,ΧΡΥΣΑΝΘΗ
   language: el
   title: ΕΠΙΣΜΑΝΣΕΙΣ
   subtitle: ΠΟΙΗΜΑΤΑ
   dewey: 889.1 ΖΙΤ
   entry_numbers:
   - '10410'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
@@ -405170,15 +405182,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8070
   authors:
-  - ΖΩΙΔΗΣ ΠΑΝΑΓΙΩΤΗΣ
+  - ΖΩΙΔΗΣ,ΠΑΝΑΓΙΩΤΗΣ
   language: el
   title: ΕΝΑ ΠΑΙΔΙ ΜΙΑ ΙΣΤΟΡΙΑ ΣΕ ΕΝΑΝ ΠΟΛΕΜΟΝ
   dewey: 889.1 ΖΩΙ
   entry_numbers:
   - '10406'
   editor: None // ΑΘΗΝΑ
   edition_year: 1985
@@ -405219,15 +405231,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8071
   authors:
-  - ΜΠΑΡΜΠΑΣ ΒΑΣΟΣ
+  - ΜΠΑΡΜΠΑΣ,ΒΑΣΟΣ
   language: el
   title: ΤΑ ΤΡΑΓΟΥΔΙΑ ΤΗΣ ΕΙΡΗΝΗΣ
   subtitle: ΛΥΡΙΚΗ ΠΟΙΗΣΗ
   dewey: 889.1 ΜΠΑ
   entry_numbers:
   - '10403'
   editor: None // ΑΘΗΝΑ
@@ -405269,15 +405281,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8072
   authors:
-  - ΜΠΑΡΜΠΑΣ ΒΑΣΟΣ
+  - ΜΠΑΡΜΠΑΣ,ΒΑΣΟΣ
   language: el
   title: ΤΑ ΤΡΑΓΟΥΔΙΑ ΤΟΥ ΛΑΟΥ ΜΟΥ
   subtitle: ΛΥΡΙΚΗ ΠΟΙΗΣΗ
   dewey: 889.1 ΜΠΑ
   entry_numbers:
   - '10404'
   editor: None // ΑΘΗΝΑ
@@ -405515,15 +405527,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8077
   authors:
-  - ΜΠΑΡΜΠΑΣ ΒΑΣΟΣ
+  - ΜΠΑΡΜΠΑΣ,ΒΑΣΟΣ
   language: el
   title: ΤΑ ΟΜΟΡΦΑ ΧΡΟΝΙΑ
   subtitle: ΛΥΡΙΚΗ ΠΟΙΗΣΗ
   dewey: 889.1 ΜΠΑ
   entry_numbers:
   - '10425'
   editor: None // ΑΘΗΝΑ
@@ -406507,15 +406519,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8097
   authors:
-  - ΖΑΔΕΣ ΔΗΜΟΣΘΕΝΗΣ
+  - ΖΑΔΕΣ,ΔΗΜΟΣΘΕΝΗΣ
   language: el
   title: ΠΑΝΩ ΑΠ ΤΟΝ ΞΕΝΟΜΟΧΘΟ
   dewey: 880.09 ΖΑΔ
   entry_numbers:
   - '5404'
   edition: Β
   editor: ΤΡΙΦΥΛΙΑΚΗΣ ΕΣΤΙΑΣ // ΑΘΗΝΑ
@@ -408108,15 +408120,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8130
   authors:
-  - ΜΠΛΑΝΑΣ ΓΙΩΡΓΟΣ
+  - ΜΠΛΑΝΑΣ,ΓΙΩΡΓΟΣ
   language: el
   title: ΩΔΗ ΣΤΟΝ ΓΕΩΡΓΙΟ ΚΑΡΑΙΣΚΑΚΗ
   dewey: 889.1 ΜΠΛ
   entry_numbers:
   - '9588'
   editor: ΓΑΒΙΗΛΙΔΗΣ // ΑΘΗΝΑ
   edition_year: 2010
@@ -408156,15 +408168,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8131
   authors:
-  - ΜΠΟΛΕΤΣΗΣ ΣΤΕΦΑΝΟΣ
+  - ΜΠΟΛΕΤΣΗΣ,ΣΤΕΦΑΝΟΣ
   language: el
   title: ΡΑΨΩΔΙΑ 140-1946
   dewey: 889.1 ΜΠΟ
   entry_numbers:
   - '10438'
   editor: ΔΑΜΑΣΚΟΣ // ΑΘΗΝΑ
   edition_year: 1989
@@ -408501,15 +408513,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8138
   authors:
-  - ΜΠΑΜΠΑΛΗ ΑΓΓΕΛΙΚΗ
+  - ΜΠΑΜΠΑΛΗ,ΑΓΓΕΛΙΚΗ
   language: el
   title: Ο ΜΕΓΙΣΤΟΣ ΠΑΤΕΡΑΣ ΤΩΝ ΕΛΛΗΝΩΝ,ΠΟΙΗΤΗΣ ΟΜΗΡΟΣ 1000 Π.Χ.
   dewey: 889.1 ΜΠΑ
   entry_numbers:
   - '5089'
   editor: None // ΑΘΗΝΑ
   edition_year: 1998
@@ -411331,15 +411343,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8196
   authors:
-  - ΜΠΑΚ ΠΕΡΛ
+  - BUCK,PEARL,S.
   language: el
   title: Η ΜΑΝΑ
   dewey: 808.899 ΜΠΑ
   entry_numbers:
   - '10477'
   editor: ΑΛΜΑ // ΑΘΗΝΑ
   pages: 223
@@ -411769,15 +411781,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8205
   authors:
-  - ΜΠΡΟΝΤΕ ΕΜΙΛΥ
+  - BRONTË,EMILY
   language: el
   title: ΑΝΕΜΟΔΑΡΜΕΝΑ ΥΨΗ
   dewey: 808.899 ΜΠΡ
   entry_numbers:
   - '10482'
   editor: ΔΙΚΑΚΗ // None
   pages: 94
@@ -413555,15 +413567,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8242
   authors:
-  - BETSIS ANDREW
+  - BETSIS,ANDREW
   title: CAMBRIDGE PROFICIENCY PAST PAPERS
   dewey: 808.899 BET
   entry_numbers:
   - '10571'
   editor: BETSIS // ΑΘΗΝΑ
   pages: 34
   topics:
@@ -414376,15 +414388,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8259
   authors:
-  - ΖΙΩΓΑΣ ΘΩΜΑΣ
+  - ΖΙΩΓΑΣ,ΘΩΜΑΣ
   language: el
   title: ΜΑΣΤΡΟΧΩΡΙΤΙΚΑ
   dewey: 398 ΖΙΩ
   entry_numbers:
   - '10052'
   editor: ΚΑΠΑ // ΑΘΗΝΑ
   edition_year: 2011
@@ -414714,15 +414726,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8266
   authors:
-  - ΖΩΡΑ ΠΟΠΗ
+  - ΖΩΡΑ,ΠΟΠΗ
   language: el
   title: ΛΑΟΓΡΑΦΙΚΟ ΜΟΥΣΕΙΟ ΣΑΡΑΚΑΤΣΑΝΩΝ ΣΕΡΡΕΣ
   dewey: 398 ΖΩΡ
   entry_numbers:
   - '10533'
   pages: 20
   topics:
@@ -415141,15 +415153,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8275
   authors:
-  - ΜΠΟΤΣΑΡΗΣ ΝΟΤΗΣ
+  - ΜΠΟΤΣΑΡΗΣ,ΝΟΤΗΣ
   language: el
   title: ΣΟΥΛΙ ΚΑΙ ΔΗΜΟΤΙΚΟ ΤΡΑΓΟΥΔΙ
   dewey: 780.42 ΜΠΟ
   entry_numbers:
   - '7804'
   editor: None // ΑΘΗΝΑ
   edition_year: 1970
@@ -415333,15 +415345,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8279
   authors:
-  - ΜΠΟΥΦΙΔΗΣ ΒΑΣΙΛΗΣ
+  - ΜΠΟΥΦΙΔΗΣ,ΒΑΣΙΛΗΣ
   language: el
   title: ΣΑΡΑΚΑΤΣΑΝΟΙ ΚΑΙ ΒΛΑΧΟΙ
   dewey: 398 ΜΠΟ
   entry_numbers:
   - '7959'
   editor: None // ΑΘΗΝΑ
   edition_year: 1995
@@ -415527,15 +415539,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8283
   authors:
-  - ΖΙΩΓΑΣ ΘΩΜΑΣ
+  - ΖΙΩΓΑΣ,ΘΩΜΑΣ
   language: el
   title: ΚΟΥΔΑΡΙΤΙΚΑ
   dewey: 398 ΖΙΩ
   entry_numbers:
   - '9900'
   editor: ΚΑΠΑ // ΑΘΗΝΑ
   edition_year: 2010
@@ -415676,15 +415688,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8286
   authors:
-  - ΖΑΛΙΟΣ ΧΡΗΣΤΟΣ
+  - ΖΑΛΙΟΣ,ΧΡΗΣΤΟΣ
   language: el
   title: ΠΑΡΑΔΟΣΙΑΚΟΙ ΧΟΡΟΙ
   subtitle: ΗΘΗ ΚΑΙ ΕΘΙΜΑ ΤΗΣ ΝΑΟΥΣΑΣ
   dewey: 398 ΖΑΛ
   entry_numbers:
   - '10536'
   editor: ΖΑΛΙΟΣ // ΝΑΟΥΣΑ
@@ -419800,15 +419812,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8371
   authors:
-  - ΜΠΙΡΓΚΕΓΚΟΡ,ΜΙΚΚΕΛ
+  - BIRKEGAARD,MIKKEL
   language: el
   title: ΤΟ ΒΙΒΛΙΟΠΩΛΕΙΟ ΤΩΝ ΣΚΙΩΝ
   dewey: 839.81 ΜΠΙ
   entry_numbers:
   - '10598'
   translators:
   - ΚΑΛΟΒΥΡΝΑΣ,ΛΥΟ
@@ -419853,15 +419865,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8372
   authors:
-  - ΜΠΑΡΘΕΛΟ,ΕΛΙΑ
+  - BARCELÓ,ELIA
   language: el
   title: ΤΟ ΜΥΣΤΙΚΟ ΤΟΥ ΧΡΥΣΟΧΟΟΥ
   dewey: 860.11 ΜΠΑ
   entry_numbers:
   - '10605'
   translators:
   - ΖΑΚΟΠΟΥΛΟΥ,ΓΕΩΡΓΙΑ
@@ -420608,15 +420620,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8387
   authors:
-  - BUSHNELL CANDACE
+  - BUSHNELL,CANDACE
   title: SEX AND THE CITY
   dewey: 810.11 BUS
   entry_numbers:
   - '9627'
   translators:
   - ΛΟΓΟΘΕΤΗ,ΕΛΙΣΩ
   editor: ΛΙΒΑΝΗ // ΑΘΗΝΑ
@@ -422035,15 +422047,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8415
   authors:
-  - ΜΠΙΡΜΑΝ ΦΡΑΝΤΖΙΣΚΑ
+  - BIERMANN,FRANZISKA
   language: el
   title: Η ΦΙΟΝΤΟΡΑ ΔΕΝ ΤΟ ΒΑΖΕΙ ΚΑΤΩ!
   dewey: 808.899 ΜΠΙ
   entry_numbers:
   - '10636'
   translators:
   - ΤΣΙΝΑΡΗ,ΠΕΛΑΓΙΑ
@@ -423027,15 +423039,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8435
   authors:
-  - ΜΠΟΚΟΓΙΑΝΝΗΣ ΧΡΥΣΟΣΤΟΜΟΣ
+  - ΜΠΟΚΟΓΙΑΝΝΗΣ,ΧΡΥΣΟΣΤΟΜΟΣ
   language: el
   title: ΜΗΓΕΡΗ ΚΑΙ ΜΗΓΕΡΙΤΕΣ
   dewey: 938.939 ΜΠΟ
   entry_numbers:
   - '9893'
   editor: None // ΑΡΤΑ
   edition_year: 2010
@@ -424296,15 +424308,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8462
   authors:
-  - ΖΑΚΥΝΘΗΝΟΥ ΔΙΟΝ
+  - ΖΑΚΥΘΗΝΟΣ,ΔΙΟΝΥΣΙΟΣ
   language: el
   title: Η ΒΥΖΑΝΤΙΝΗ ΕΛΛΑΣ 392-1204
   dewey: 938.3 ΖΑΚ
   entry_numbers:
   - '10659'
   editor: ΒΑΓΙΟΝΑΚΗ // None
   pages: 104
@@ -427050,15 +427062,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8518
   authors:
-  - ΒΛΑΧΟΣ,ΑΓΓΕΛΟΣ,ΣΤ,
+  - ΒΛΑΧΟΣ,ΑΓΓΕΛΟΣ,ΣΤ.
   language: el
   title: Ο ΚΥΡΙΟΣ ΜΟΥ ΑΛΚΙΒΙΑΔΗΣ
   dewey: 889.21 ΒΛΑ
   entry_numbers:
   - '10738'
   editor: None // ΑΘΗΝΑ
   edition_year: 2008
@@ -428021,15 +428033,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8537
   authors:
-  - ΜΠΛΑΙΤΟΝ,ΕΝΙΝΤ
+  - BLYTON,ENID
   language: el
   title: ΤΟ ΒΙΒΛΙΟ ΜΕ ΤΙΣ ΝΕΡΑΙΔΕΣ
   dewey: 808.899 ΜΠΛ
   entry_numbers:
   - '10818'
   translators:
   - ΚΟΝΔΑΚΗ,ΜΙΡΚΑ
@@ -428749,15 +428761,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8551
   authors:
-  - ΜΠΑΡΤΖΩΚΑΣ,ΚΙΜΩΝ
+  - ΜΠΑΡΤΖΩΚΑΣ,ΚΙΜΩΝΑΣ
   language: el
   title: ΕΥΘΥΜΕΣ ΗΠΕΙΡΩΤΙΣΕΣ ΛΑΟΓΡΑΦΙΚΕΣ ΙΣΤΟΡΙΕΣ
   subtitle: ΓΝΩΜΙΚΑ,ΠΑΡΟΙΜΙΕΣ,ΑΝΕΚΔΟΤΑ
   dewey: '398'
   entry_numbers:
   - '10826'
   edition: '1'
@@ -431041,15 +431053,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8596
   authors:
-  - ΜΠΩΣΩ,ΑΝΡΥ
+  - BAUCHAU,HENRY
   language: el
   title: Η ΔΙΟΤΙΜΑ ΚΑΙ ΤΑ ΛΙΟΝΤΑΡΙΑ
   dewey: 843 ΜΠΩ
   entry_numbers:
   - '10848'
   translators:
   - ΚΟΡΟΜΗΛΑ,ΕΦΗ
@@ -431202,15 +431214,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8599
   authors:
-  - ΜΠΑΖΕΝ,ΕΡΒΕ
+  - BAZIN,HERVÉ
   language: el
   title: ΜΕ ΤΗΝ ΟΧΙΑ ΣΤΟ ΧΕΡΙ
   dewey: 843 ΜΠΑ
   entry_numbers:
   - '10907'
   translators:
   - ΛΕΙΛΙΝΟΣ,ΔΗΜΗΤΡΗΣ
@@ -431524,15 +431536,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8605
   authors:
-  - BILLETDOUX,RAPHAELE
+  - BILLETDOUX,RAPHAËLE
   language: el
   title: ΟΙ ΝΥΧΤΕΣ ΜΟΥ ΕΙΝΑΙ ΠΙΟ ΟΜΟΡΦΕΣ ΑΠΟ ΤΙΣ ΜΕΡΕΣ ΣΑΣ
   dewey: 843 BIL
   entry_numbers:
   - '10871'
   translators:
   - ΚΟΡΟΜΗΛΑ,ΕΦΗ
@@ -431631,15 +431643,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8607
   authors:
-  - ΜΠΡΕΧΤ,ΜΠΕΡΤΟΛΤ
+  - BRECHT,BERTOLT
   language: el
   title: ΟΙ ΔΟΥΛΕΙΕΣ ΤΟΥ ΚΥΡΙΟΥ ΙΟΥΛΙΟΥ ΚΑΙΣΑΡΟΣ
   dewey: 832 ΜΠΡ
   entry_numbers:
   - '10833'
   translators:
   - ΤΕΡΖΙΑΝ,ΙΩΣΗΦ
@@ -432755,15 +432767,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8628
   authors:
-  - ΜΠΑΡΑΜΠΑΣ,ΜΠΕΝΥ
+  - BARBASH,BENNY
   title: MY FIRST SONY
   dewey: 892.43 ΜΠΑ
   entry_numbers:
   - '10910'
   translators:
   - ΣΙΜΠΗ,ΙΑΚΩΒ
   editor: ΓΑΒΡΙΗΛΙΔΗΣ // ΑΘΗΝΑ
@@ -434468,15 +434480,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8661
   authors:
-  - ΖΙΝΤ,ΑΝΤΡΕ
+  - GIDE,ANDRÉ,PAUL GUILLAUME
   language: el
   title: Ο ΑΝΗΘΙΚΟΛΟΓΟΣ
   dewey: 843 ΖΙΝ
   entry_numbers:
   - '10937'
   editor: ΚΟΡΑΛΙ // ΑΘΗΝΑ
   edition_year: 1968
@@ -434777,15 +434789,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8667
   authors:
-  - ΜΠΡΥΚΝΕΡ,ΠΑΣΚΑΛ
+  - BRUCKNER,PASCAL
   language: el
   title: Η ΤΥΡΑΝΝΙΑ ΤΗΣ ΜΕΤΑΜΕΛΕΙΑΣ
   subtitle: ΔΟΚΙΜΙΟ ΠΑΝΩ ΣΤΟΝ ΔΥΤΙΚΟ ΠΟΛΙΤΙΣΜΟ
   dewey: 843 ΜΠΡ
   entry_numbers:
   - '10919'
   translators:
@@ -437114,15 +437126,19 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8712
   authors:
-  - ΖΥΚΙΕΝ,ΠΙΕΡ
+  - JUQUIN,PIERRE
+  - STENGERS,ISABELLE
+  - ANTUNES,CARLOS!KEMP,PENNY
+  - TELKAMPER,WILFRID
+  - WOLF,FRIEDER,OTTO
   language: el
   title: ΤΟ ΜΑΝΙΦΕΣΤΟ ΤΩΝ ΟΙΚΟΣΟΣΙΑΛΙΣΤΩΝ
   subtitle: Η ΠΡΑΣΙΝΗ ΕΝΑΛΛΑΚΤΙΚΗ ΠΡΟΤΑΣΗ ΓΙΑ ΤΗΝ ΕΥΡΩΠΗ
   dewey: 320 ΖΥΚ
   entry_numbers:
   - '10943'
   translators:
@@ -439293,15 +439309,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8754
   authors:
-  - ΜΠΡΕΧΤ,ΜΠΕΡΤΟΛΤ
+  - BRECHT,BERTOLT
   language: el
   title: ΔΙΟΡΘΩΣΗ ΠΑΛΙΩΝ ΜΥΘΩΝ ΚΑΙ ΑΛΛΕΣ ΙΣΤΟΡΙΕΣ
   dewey: 832 ΜΠΡ
   entry_numbers:
   - '11025'
   translators:
   - ΒΑΛΑΒΑΝΗ,ΝΑΝΤΙΑ
@@ -439403,15 +439419,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8756
   authors:
-  - ΜΠΙΤΣΑΚΗΣ,ΕΥΤΥΧΗΣ
+  - ΜΠΙΤΣΑΚΗΣ,ΕΥΤΥΧΗΣ,Ι.
   language: el
   title: Η ΦΥΣΗ ΣΤΗ ΔΙΑΛΕΚΤΙΚΗ ΦΙΛΟΣΟΦΙΑ
   dewey: 109 ΜΠΙ
   entry_numbers:
   - '11036'
   editor: ΕΛΛΗΝΙΚΑ ΓΡΑΜΜΑΤΑ // ΑΘΗΝΑ
   edition_year: 2003
@@ -440805,15 +440821,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8783
   authors:
-  - ΜΠΡΑΓΚΕΤΙ,ΑΝΝΑ ΛΑΟΥΡΑ
+  - BRAGHETTI,ANNA LAURA
   language: el
   title: Η ΟΜΗΡΙΑ
   dewey: 850.11 ΜΠΡ
   entry_numbers:
   - '11054'
   translators:
   - ΑΠΟΣΤΟΛΑΚΗ,ΜΑΡΙΑ
@@ -442892,15 +442908,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8824
   authors:
-  - ΜΠΕΝΤΙΤ,ΚΟΝ
+  - COHN-BENDIT,GABRIEL
   language: el
   title: ΑΡΙΣΤΕΡΙΣΜΟΣ
   subtitle: ΦΑΡΜΑΚΟ ΣΤΗ ΓΕΡΟΝΤΙΚΗ ΑΡΡΩΣΤΙΑ ΤΟΥ ΚΟΜΜΟΥΝΙΣΜΟΥ
   dewey: 330 ΜΠΕ
   entry_numbers:
   - '11089'
   translators:
@@ -442997,15 +443013,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8826
   authors:
-  - ΖΑΓΚΑΓΙΕΒΣΚΙ,ΑΝΤΑΜ
+  - ZAGAJEWSKI,ADAM
   language: el
   title: ΠΟΛΩΝΙΑ
   subtitle: ΣΤΗ ΣΚΙΑ ΤΗΣ ΣΟΒΙΕΤΙΚΗΣ ΕΝΩΣΗΣ
   dewey: 330 ΖΑΓ
   entry_numbers:
   - '11091'
   translators:
@@ -443801,15 +443817,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8842
   authors:
-  - ΜΠΕΛΑΝΤΗΣ,ΔΗΜΗΤΡΗΣ
+  - ΜΠΕΛΑΝΤΗΣ,ΔΗΜΗΤΡΙΟΣ
   language: el
   title: Η ΟΥΡΛΙΚΕ ΜΕΤΑ ΤΟ ΘΑΝΑΤΟ ΤΗΣ ΜΑΙΝΧΟΦ
   dewey: 889.21 ΜΠΕ
   entry_numbers:
   - '11169'
   editor: ΒΙΒΛΙΟΠΕΛΑΓΟΣ // ΑΘΗΝΑ
   edition_year: 2007
@@ -444013,15 +444029,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8846
   authors:
-  - ΜΠΙΤΣΑΚΗ,ΕΥΤΥΧΗ
+  - ΜΠΙΤΣΑΚΗΣ,ΕΥΤΥΧΗΣ,Ι.
   language: el
   title: ΔΙΑΛΕΚΤΙΚΗ ΚΑΙ ΝΕΩΤΕΡΙΚΗ ΦΥΣΙΚΗ
   dewey: 109 ΜΠΙ
   entry_numbers:
   - '11185'
   edition: Ε
   editor: ΔΑΙΔΑΛΟΣ // ΑΘΗΝΑ
@@ -444223,15 +444239,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8850
   authors:
-  - ΜΠΟΥΖΑΚΗΣ ΣΗΦΗΣ
+  - ΜΠΟΥΖΑΚΗΣ,ΣΗΦΗΣ
   language: el
   title: ΑΝΕΚΔΟΤΑ ΚΕΙΜΕΝΑ ΓΙΑ ΤΗΝ ΠΑΙΔΕΙΑ
   dewey: 370 ΜΠΟ
   entry_numbers:
   - '11188'
   editor: ΠΗΓΕΣ // ΑΘΗΝΑ
   edition_year: 2005
@@ -444275,15 +444291,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8851
   authors:
-  - BALANDIER,GEORGE
+  - BALANDIER,GEORGES
   language: el
   title: ΠΟΛΙΤΙΚΗ ΑΝΘΡΩΠΟΛΟΓΙΑ
   dewey: 320 BAL
   entry_numbers:
   - '11140'
   translators:
   - ΒΛΑΧΟΥ,
@@ -445584,15 +445600,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8877
   authors:
-  - ΜΠΙΤΣΑΚΗΣ,ΕΥΤΥΧΗΣ
+  - ΜΠΙΤΣΑΚΗΣ,ΕΥΤΥΧΗΣ,Ι.
   language: el
   title: ΟΙ ΠΟΛΕΜΟΙ ΤΗΣ ΝΕΑΣ ΤΑΞΗΣ
   dewey: 303.484 ΜΠΙ
   entry_numbers:
   - '11155'
   editor: ΠΡΟΣΚΗΝΙΟ // ΑΘΗΝΑ
   edition_year: 2005
@@ -457241,15 +457257,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9102
   authors:
-  - ΖΑΡΑΒΕΛΑΣ ΔΗΜΗΤΡΗΣ ΑΘ.
+  - ΖΑΡΑΒΕΛΑΣ,ΔΗΜΗΤΡΗΣ,ΑΘ.
   language: el
   title: ΠΕΤΡΙΝΕΣ ΜΝΗΜΕΣ
   subtitle: ΟΔΟΙΠΟΡΙΚΟ ΣΤΙΣ ΧΑΜΕΝΕΣ ΠΑΤΡΙΔΕΣ ΤΟΥ ΠΟΝΤΟΥ
   dewey: 889.21 ΖΑΡ
   entry_numbers:
   - '11401'
   editor: ΔΩΔΩΝΗ // ΑΘΗΝΑ
@@ -457655,15 +457671,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9110
   authors:
-  - ΜΠΑΜΠΕΡΙ ΚΡΙΣ
+  - BAMBERY,CHRIS
   language: el
   title: ΠΟΤΕ ΞΑΝΑ ΦΑΣΙΣΜΟΣ
   dewey: 320 ΜΠΑ
   entry_numbers:
   - '11454'
   translators:
   - ΦΩΤΟΠΟΥΛΟΥ,ΒΙΛΛΥ
@@ -458441,15 +458457,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9125
   authors:
-  - ΜΠΗΡΣ ΑΜΠΡΟΟΥΖ
+  - BIERCE,AMBROSE
   language: el
   title: ΙΣΤΟΡΙΕΣ ΦΑΝΤΑΣΜΑΤΩΝ
   dewey: 810.11 ΜΠΗ
   entry_numbers:
   - '11407'
   translators:
   - ΜΠΛΑΝΑΣ,ΓΙΩΡΓΟΣ
@@ -459916,15 +459932,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9153
   authors:
-  - ΜΠΕΤΤΕΛΕΜ ΣΑΡΛ
+  - BETTELHEIM,CHARLES
   language: el
   title: ΠΟΛΙΤΙΣΤΙΚΗ ΕΠΑΝ/ΣΗ ΚΑΙ ΒΙΟΜ/ΚΗ ΟΡΓΑΝ/ΣΗ ΣΤΗΝ ΚΙΝΑ
   dewey: 951.05 ΜΠΕ
   entry_numbers:
   - '11439'
   translators:
   - ΔΗΜΗΤΡΙΟΥ,ΣΤΕΛΙΟΣ
@@ -461550,15 +461566,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9185
   authors:
-  - ΖΟΥΡΑΡΙΣ ΚΩΣΤΑΣ
+  - ΖΟΥΡΑΡΙΣ,ΚΩΣΤΑΣ
   language: el
   title: ΟΙ ΔΙΑΣΤ/ΣΕΣ ΤΗΣ ΔΟΜΙΚΗΣ ΑΚ/ΣΙΑΣ Η Η ΜΕΤ/ΣΗ ΠΡΟΣ ΤΟ ΣΟΣ/ΣΜΟ
   dewey: 320 ΖΟΥ
   entry_numbers:
   - '11495'
   editor: Ο ΠΟΛΙΤΗΣ // ΑΘΗΝΑ
   edition_year: 1980
@@ -461751,15 +461767,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9189
   authors:
-  - ΜΠΑΡΟ, ΡΟΥΝΤΟΛΦ
+  - BAHRO,RUDOLPH
   language: el
   title: Η ΕΝΝ/ΚΤΙΚΗ ΛΥΣΗ ΣΤΗΝ ΑΝΑΤ/ΚΗ ΕΥΡΩΠΗ
   subtitle: ΣΥΜΒΟΛΗ ΣΤΗΝ ΚΡΙΤΙΚΗ ΤΟΥ ΥΠΑΡΚΤΟΥ ΣΟΣ/ΣΜΟΥ
   dewey: 320 ΜΠΑ
   entry_numbers:
   - '11363'
   editor: ΘΟΥΡΙΟΣ // ΑΘΗΝΑ
@@ -461852,15 +461868,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9191
   authors:
-  - ΖΑΧΑΡΕΑΣ, ΑΙΜΙΛΙΟΣ
+  - ΖΑΧΑΡΕΑΣ,ΑΙΜΙΛΙΟΣ
   language: el
   title: Ο ΣΤΡΑΤ/ΚΟΣ-ΠΟΛ/ΚΟΣ ΠΡΟΓΡ/ΣΜΟΣ ΤΗΣ ΟΙΚΟΝΟΜΙΑΣ
   dewey: 330 ΖΑΧ
   entry_numbers:
   - '11364'
   editor: ΟΔΥΣΣΕΑΣ // ΑΘΗΝΑ
   edition_year: 1978
@@ -464798,15 +464814,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9248
   authors:
-  - ΜΠΡΕΧΤ,ΜΠΕΡΤΟΛΤ
+  - BRECHT,BERTOLT
   language: el
   title: ΓΙΑ ΤΗ ΦΙΛΟΣΟΦΙΑ ΚΑΙ ΤΟΝ ΜΑΡΞΙΣΜΟ
   dewey: 150 ΜΠΡ
   entry_numbers:
   - '11441'
   translators:
   - ΒΕΡΓΩΤΗΣ,ΒΑΣΙΛΗΣ
@@ -465109,15 +465125,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9254
   authors:
-  - ΜΠΑΜΠΑΝΑΣΗ, ΣΤΕΡΓΙΟΥ
+  - ΜΠΑΜΠΑΝΑΣΗΣ,ΣΤΕΡΓΙΟΣ
   language: el
   title: Η ΕΛΛΑΔΑ ΣΤΗΝ ΠΕΡΙΦΕΡΕΙΑ ΤΩΝ ΑΝΑΠΤΥΓΜΕΝΩΝ ΧΩΡΩΝ
   dewey: 338.1 ΜΠΑ
   entry_numbers:
   - '11385'
   editor: ΘΕΜΕΛΙΟ // ΑΘΗΝΑ
   edition_year: 1976
@@ -465422,15 +465438,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9260
   authors:
-  - ΜΠΕΤΕΛΕΜ,ΣΑΡΛ
+  - BETTELHEIM,CHARLES
   language: el
   title: ΟΙ ΤΑΞΙΚΟΙ ΑΓΩΝΕΣ ΣΤΗΝ ΕΛΛΑΔΑ
   subtitle: 1η ΠΕΡΙΟΔΟΣ 1917-1923
   dewey: 320 ΜΠΕ
   entry_numbers:
   - '11395'
   translators:
@@ -467230,15 +467246,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9295
   authors:
-  - ΜΠΟΥΣΚΑΛΙΑ,ΛΕΟ
+  - BUSCAGLIA,LEO
   language: el
   title: ΓΕΝΝΗΜΕΝΟΙ ΓΙΑ ΤΗΝ ΑΓΑΠΗ
   dewey: 170 ΜΠΟ
   entry_numbers:
   - '20599'
   editor: ΓΛΑΡΟΣ // ΑΘΗΝΑ
   edition_year: 1992
@@ -468319,15 +468335,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9316
   authors:
-  - ΜΠΡΥΝΟΦ ΝΤΕ ΣΟΥΖΑΝ
+  - ΝΤΕ ΜΠΡΥΝΟΦ,ΣΟΥΖΑΝ
   language: el
   title: ΚΡΑΤΟΣ ΚΑΙ ΚΕΦΑΛΑΙΟ
   dewey: 320 ΜΠΡ
   entry_numbers:
   - '11584'
   translators:
   - ΕΛΕΦΑΝΤΗΣ,ΑΓΓΕΛΟΣ
@@ -471852,15 +471868,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9385
   authors:
-  - ΜΠΟΥΣΧΟΤΕΝ,ΡΙΚΗ ΒΑΝ
+  - ΒΑΝ ΜΠΟΥΣΧΟΤΕΝ,ΡΙΚΗ
   language: el
   title: ΠΕΡΑΣΑΜΕ ΠΟΛΛΕΣ ΜΠΟΡΕΣ ΚΟΡΙΤΣΙ ΜΟΥ
   dewey: 320 ΜΠΟ
   entry_numbers:
   - '11670'
   editor: ΠΛΕΘΡΟΝ // ΑΘΗΝΑ
   edition_year: 1998
@@ -472764,15 +472780,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9403
   authors:
-  - ΜΠΛΑΝΑ,ΓΕΩΡΓΙΟΥ
+  - ΜΠΛΑΝΑΣ,ΓΙΩΡΓΟΣ
   language: el
   title: Η ΣΤΡΑΤΗΓΙΚΗ ΤΗΣ ΣΩΣΤΗΣ ΕΠΑΝΑΣΤΑΣΗΣ
   dewey: 320 ΜΠΛ
   entry_numbers:
   - '11682'
   editor: None // ΑΘΗΝΑ
   edition_year: 1986
@@ -473865,15 +473881,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9425
   authors:
-  - ΜΠΑΛΙΜΠΑΡ,ΕΤΙΕΝ
+  - BALIBAR,ÉTIENNE
   language: el
   title: Ο ΣΠΙΝΟΖΑ ΚΑΙ Η ΠΟΛΙΤΙΚΗ
   dewey: 320 ΜΠΑ
   entry_numbers:
   - '11718'
   translators:
   - ΣΤΥΛΙΑΝΟΥ,ΑΡΗΣ Ι.
@@ -475963,15 +475979,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 9466
   authors:
-  - ΜΠΑΜΠΙΝΙΩΤΗΣ,Γ
+  - ΜΠΑΜΠΙΝΙΩΤΗΣ,ΓΕΩΡΓΙΟΣ
   language: el
   title: Η ΓΛΩΣΣΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
   subtitle: Η ΑΡΧΑΙΑ ΜΑΚΕΔΟΝΙΚΗ ΚΑΙ Η ΨΕΥΔΩΝΥΜΗ ΓΛΩΣΣΑ ΤΩΝ ΣΚΟΠΙΩΝ
   dewey: 480.09 ΜΠΑ
   entry_numbers:
   - '11755'
   editor: ΟΛΚΟΣ // ΑΘΗΝΑ
@@ -477052,15 +477068,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9487
   authors:
-  - ΜΠΑΛΖΑΚ,ΟΝΟΡΕΝΤΕ
+  - BALZAC,HONORÉ DE
   language: el
   title: ΟΙ ΧΩΡΙΑΤΕΣ
   dewey: 843 ΜΠΑ
   entry_numbers:
   - '11774'
   - '16726'
   translators:
@@ -477307,15 +477323,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9492
   authors:
-  - ΖΟΛΑ,ΕΜΙΛ
+  - ZOLA,ÉMILE,ÉDOUARD CHARLES ANTOINE
   language: el
   title: ΚΑΤΗΓΟΡΩ
   dewey: 843 ΖΟΛ
   entry_numbers:
   - '11775'
   - '16727'
   translators:
@@ -478321,15 +478337,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9512
   authors:
-  - ΜΠΟΣΤ
+  - ΒΟΣΤΑΝΤΖΌΓΛΟΥ,ΧΡΎΣΑΝΘΟΣ@ΜΈΝΤΗΣ ΜΠΟΣΤΑΝΤΖΌΓΛΟΥ Ή ΜΠΟΣΤ
   language: el
   title: 18 ΑΝΤΙ ΚΕΙΜΕΝΑ.Η ΥΠΕΡ ΔΙΚΤΑΚΤΟΡΕΙΑΣ ΛΟΓΟΣ
   dewey: 889.21 ΜΠΟ
   entry_numbers:
   - '11798'
   pages: 57
   topics:
@@ -480867,15 +480883,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9562
   authors:
-  - ΖΙΟΥΤΟΣ,Γ.Δ.
+  - ΖΙΟΥΤΟΣ,ΓΙΩΡΓΟΣ,Δ.
   language: el
   title: ΤΟ ΔΙΕΘΝΕΣ ΕΡΓΑΤΙΚΟ ΚΙΝΗΜΑ
   subtitle: ΣΤΟΝ 19ο ΑΙΩΝΑ ΚΑΙ ΤΙΣ ΑΡΧΕΣ ΤΟΥ 20ου ΑΙΩΝΑ
   dewey: 320 ΖΙΟ
   entry_numbers:
   - '11850'
   editor: ΣΤΟΧΑΣΤΗΣ // ΑΘΗΝΑ
@@ -481434,15 +481450,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9573
   authors:
-  - ΜΠΡΑΝΤΜΠΕΡΥ,ΡΑΙΗ
+  - BRADBURY,RAY
   language: el
   title: ΤΟ ΤΕΛΟΣ ΤΗΣ ΑΡΧΗΣ
   dewey: 810.11 ΜΠΡ
   entry_numbers:
   - '11861'
   translators:
   - ΧΑΤΧΟΥΤ,ΡΕΝΑ
@@ -482286,15 +482302,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9590
   authors:
-  - ΜΠΕΤΤΕΛΕΜ,ΣΑΡΛ
+  - BETTELHEIM,CHARLES
   language: el
   title: Η ΟΙΚΟΔΟΜΗΣΗ ΤΟΥ ΣΟΣΙΑΛΙΣΜΟΥ ΣΤΗ ΚΙΝΑ
   dewey: 335.434 ΜΠΕ
   entry_numbers:
   - '11884'
   editor: ΣΤΟΧΑΣΤΗ // ΑΘΗΝΑ
   edition_year: 1976
@@ -482492,15 +482508,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9594
   authors:
-  - ΜΠΙΤΣΑΚΗ,ΕΥΤΥΧΗ Ι.
+  - ΜΠΙΤΣΑΚΗΣ,ΕΥΤΥΧΗΣ,Ι.
   language: el
   title: ΕΝΑ ΦΑΝΤΑΣΜΑ ΠΛΑΝΙΕΤΑΙ
   dewey: 320 ΜΠΙ
   entry_numbers:
   - '11889'
   editor: ΣΤΑΧΥ // ΑΘΗΝΑ
   edition_year: 1992
@@ -482952,15 +482968,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9603
   authors:
-  - ΜΠΑΤΣΗ,ΔΗΜ
+  - ΜΠΑΤΣΗΣ,ΔΗΜΗΤΡΙΟΣ
   language: el
   title: Η ΒΑΡΕΙΑ ΒΙΟΜΗΧΑΝΙΑ ΣΤΗΝ ΕΛΛΑΔΑ
   dewey: 338.1 ΜΠΑ
   entry_numbers:
   - '11894'
   edition: '2'
   editor: ΚΕΔΡΟΣ // ΑΘΗΝΑ
@@ -485578,15 +485594,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9653
   authors:
-  - ΜΠΙΤΣΑΚΗ,ΕΥΤΥΧΗ
+  - ΜΠΙΤΣΑΚΗΣ,ΕΥΤΥΧΗΣ,Ι.
   language: el
   title: Η ΔΥΝΑΜΙΚΗ ΤΟΥ ΕΛΑΧΙΣΤΟΥ
   dewey: 530.12 ΜΠΙ
   entry_numbers:
   - '11905'
   editor: ΖΑΧΑΡΟΠΟΥΛΟΣ // ΑΘΗΝΑ
   edition_year: 1987
@@ -487307,15 +487323,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9687
   authors:
-  - ΜΠΑΡΖΟΥΚΑ,ΤΑΣΟ
+  - ΜΠΑΡΖΟΥΚΑΣ,ΤΑΣΟΣ
   language: el
   title: ΕΠΑΝΑΣΤΑΤΕΣ ΤΡΟΤΣΚΙΣΤΕΣ ΣΤΙΣ ΦΥΛΑΚΕΣ ΤΟΥ ΚΑΘΕΣΤΩΣ ΤΟΥ ΜΑΟ
   dewey: 320 ΜΠΑ
   entry_numbers:
   - '11974'
   editor: ΕΠΙΤΡΟΠΗ ΠΡΩΤΟΒΟΥΛΙΑ // None
   pages: 39
@@ -488709,15 +488725,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9715
   authors:
-  - ΜΠΙΤΣΑΚΗΣ,ΕΥΤΥΧΗΣ
+  - ΜΠΙΤΣΑΚΗΣ,ΕΥΤΥΧΗΣ,Ι.
   language: el
   title: ΓΟΝΙΔΙΑ ΤΟΥ ΜΕΛΛΟΝΤΟΣ
   dewey: 330 ΜΠΙ
   entry_numbers:
   - '11992'
   editor: ΠΡΟΣΚΗΝΙΟ // ΑΘΗΝΑ
   edition_year: 2001
@@ -488813,15 +488829,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9717
   authors:
-  - ΖΥΛΙΕΝ,ΚΛΩΝΤ
+  - JULIEN,CLAUDE
   language: el
   title: Η ΑΜΕΡΙΚΑΝΙΚΗ ΑΥΤΟΚΡΑΤΟΡΙΑ
   dewey: 330 ΖΥΛ
   entry_numbers:
   - '11997'
   editor: ΔΙΟΓΕΝΗΣ // ΑΘΗΝΑ
   edition_year: 1971
@@ -490510,15 +490526,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9751
   authors:
-  - BETTLEHEIM,CH.
+  - BETTELHEIM,CHARLES
   language: el
   title: ΜΕΤΑΒΑΣΗ ΣΤΗ ΣΟΣΙΑΛΙΣΤΙΚΗ ΟΙΚΟΝΟΜΙΑ
   dewey: 330 BET
   entry_numbers:
   - '12067'
   editor: ΜΠΑΥΡΟΝ // ΑΘΗΝΑ
   edition_year: 1975
@@ -491113,15 +491129,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9763
   authors:
-  - ΖΙΟΥΤΟΣ,ΓΙΩΡΓΟΣ
+  - ΖΙΟΥΤΟΣ,ΓΙΩΡΓΟΣ,Δ.
   language: el
   title: ΕΠΙΣΤΗΜΟΝΙΚΗ ΣΥΝΑΝΤΗΣΗ ΣΤΟ ΒΟΛΟ ΓΙΑ ΤΟΝ ΕΡΕΥΝΗΤΗ,ΤΟ ΔΗΜ/ΦΟ,Τ
   subtitle: ΟΝ ΕΚΔΟΤΗ ΚΑΙ ΤΟΝ ΑΝΑΓΝΩΣΤΗ ΤΗΣ ΑΡΙΣΤΕΡΑΣ ΜΑΡΤΙΟΣ 1997
   dewey: 320 ΖΙΟ
   entry_numbers:
   - '12016'
   editor: ΠΑΡΑΣΚΗΝΙΟ // ΑΘΗΝΑ
@@ -491366,15 +491382,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9768
   authors:
-  - ΜΠΕΡΛΙΝΓΚΟΥΕΡ,ΕΝΡΙΚΟ
+  - BERLINGUER,ENRICO
   language: el
   title: ΙΣΤΟΡΙΚΟΣ ΣΥΜΒΙΒΑΣΜΟΣ
   dewey: 330 ΜΠΕ
   entry_numbers:
   - '12035'
   editor: ΘΕΜΕΛΙΟ // ΑΘΗΝΑ
   edition_year: 1977
@@ -491416,15 +491432,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9769
   authors:
-  - ΜΠΙΣΟΠ,ΜΑΡΚ
+  - BISHOP,MARK
   language: el
   title: ΚΙΝΑ
   subtitle: Ο ΓΙΓΑΝΤΑΣ
   dewey: 330 ΜΠΙ
   entry_numbers:
   - '12023'
   editor: GUTENBERG // ΑΘΗΝΑ
@@ -494008,15 +494024,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9821
   authors:
-  - ΖΟΛΑ,ΕΜΙΛ
+  - ZOLA,ÉMILE,ÉDOUARD CHARLES ANTOINE
   language: el
   title: ΝΑΝΑ
   dewey: 843 ΖΟΛ
   entry_numbers:
   - '12119'
   editor: ΤΕΓΟΠΟΥΛΟΣ // ΑΘΗΝΑ
   edition_year: 2007
@@ -503608,15 +503624,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10027
   authors:
-  - ΜΠΑΤΡΙΝΟΣ
+  - ΜΠΑΤΡΙΝΟΣ,ΜΕΝΕΛΑΟΣ
   language: el
   title: ΣΥΓΧΡΟΝΗ ΕΝΔΟΚΡΙΝΟΛΟΓΙΑ
   dewey: 615.5 ΜΠΑ
   entry_numbers:
   - '10811'
   editor: ΠΑΣΧΑΛΙΔΗΣ // ΑΘΗΝΑ
   edition_year: 1982
@@ -506631,15 +506647,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10088
   authors:
-  - ΖΟΥΡΛΑΣ,ΠΑΝΤ
+  - ΖΟΥΡΛΑΣ,ΠΑΝΤΕΛΗΣ
   language: el
   title: ΜΑΘΗΜΑΤΑ ΜΑΙΕΥΤΙΚΗΣ-ΓΥΝΑΙΚΟΛΟΓΙΑΣ
   dewey: 615.5 ΖΟΥ
   entry_numbers:
   - '12300'
   editor: None // ΑΘΗΝΑ
   edition_year: 1984
@@ -508365,15 +508381,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10123
   authors:
-  - ΖΑΚΟΠΟΥΛΟΣ,ΝΙΚΟΛΑΟΣ
+  - ΖΑΚΟΠΟΥΛΟΣ,ΝΙΚΟΣ,Ι.
   language: el
   title: Ο ΓΙΑΤΡΟΣ ΣΤΟ ΣΠΙΤΙ ΣΑΣ
   dewey: 615.5 ΖΑΚ
   entry_numbers:
   - '12327'
   editor: ΑΦΟΙ ΒΛΑΣΣΗ // ΑΘΗΝΑ
   edition_year: 1980
@@ -513114,15 +513130,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10219
   authors:
-  - ΜΠΟΥΡΑΝΤΑ,ΔΗΜΗΤΡΙΟΥ
+  - ΜΠΟΥΡΑΝΤΑΣ,ΔΗΜΗΤΡΗΣ
   language: el
   title: ΕΙΣΑΓΩΓΗ ΣΤΗ ΔΙΟΙΚΗΣΗ ΕΠΙΧΕΙΡΗΣΕΩΝ
   dewey: 658 ΜΠΟ
   entry_numbers:
   - '12477'
   editor: ΜΠΕΝΟΥ // ΑΘΗΝΑ
   edition_year: 1998
@@ -513597,15 +513613,16 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10229
   authors:
-  - ΜΠΑΡΙΓΙΕ,ΠΙΕΡ-ΓΚΡΕΝΤΙ ΖΑΝ-ΠΙΕΡ
+  - BARILLET,PIERRE
+  - GRÉDY,JEAN-PIERRE
   language: el
   title: ΤΟ ΑΝΘΟΣ ΤΟΥ ΚΑΚΤΟΥ
   dewey: 886.2 ΜΠΑ
   entry_numbers:
   - '12498'
   editor: ΑΙΓΟΚΕΡΩΣ // ΑΘΗΝΑ
   edition_year: 2009
@@ -513989,15 +514006,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10237
   authors:
-  - ΖΙΡΟΥ,ΦΡΑΝΣΟΥΑ
+  - GIROUD,FRANCOISE
   language: el
   title: ΜΕΓΑΛΕ ΜΟΥ ΕΡΩΤΑ
   dewey: 843 ΖΙΡ
   entry_numbers:
   - '12508'
   translators:
   - ΝΤΟΥΖΕ,ΝΙΚΗ
@@ -514938,15 +514955,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10256
   authors:
-  - ΜΠΑΡΘΕΛΟ,ΕΛΙΑ
+  - BARCELÓ,ELIA
   language: el
   title: ΜΕ ΤΟ ΤΑΝΓΚΟ ΣΤΗΝ ΚΑΡΔΙΑ
   dewey: 860.11 ΜΠΑ
   entry_numbers:
   - '12428'
   translators:
   - ΖΑΚΟΠΟΥΛΟΥ,ΓΕΩΡΓΙΑ
@@ -515538,15 +515555,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10268
   authors:
-  - ΜΠΛΟΥΜ,ΤΖΟΥΝΤΙ
+  - BLOOM,JUDY
   language: el
   title: ΑΡΚΕΙ ΝΑ ΕΙΜΑΣΤΕ ΜΑΖΙ
   dewey: 808.899 ΜΠΛ
   entry_numbers:
   - '12625'
   translators:
   - ΒΑΞΕΒΑΝΗ,ΜΟΝΙΚΑ
@@ -517005,15 +517022,16 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10297
   authors:
-  - ΜΠΙΘΑ,ΙΩΑΝΝΑ-ΧΑΤΖΗΔΑΚΗΣ,ΜΑΝΟΛΗΣ
+  - ΜΠΙΘΑ,ΙΩΑΝΝΑ
+  - ΧΑΤΖΗΔΑΚΗΣ,ΜΑΝΟΛΗΣ
   language: el
   title: ΕΥΡΕΤΗΡΙΟ ΒΥΖΑΝΤΙΝΩΝ ΤΟΙΧΟΓΡΑΦΙΩΝ ΚΥΘΗΡΩΝ
   dewey: 751.730 ΜΠΙ
   entry_numbers:
   - '12651'
   editor: ΑΚΑΔΗΜΙΑ ΑΘΗΝΩΝΩ // ΑΘΗΝΑ
   edition_year: 1997
@@ -518942,15 +518960,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10335
   authors:
-  - ΜΠΕΚΤΑΣ,ΧΑΜΠΙΠ
+  - BEKTAS,HABIB
   language: el
   title: Ο ΚΗΠΟΣ ΠΙΣΩ ΑΠΟ ΤΟΝ ΠΑΡΑΔΕΙΣΟ
   dewey: 894.35 ΜΠΕ
   entry_numbers:
   - '12709'
   translators:
   - ΒΡΕΤΟΥ,ΣΤΕΛΛΑ
@@ -520177,15 +520195,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10359
   authors:
-  - ΜΠΑΡΝΕΤ,Φ.
+  - HODGSON BURNETT,FRANCES
   language: el
   title: Ο ΜΙΚΡΟΣ ΛΟΡΔΟΣ
   dewey: 808.899 ΜΠΑ
   entry_numbers:
   - '12725'
   editor: ΑΛΜΑ // ΑΘΗΝΑ
   pages: 164
@@ -521259,15 +521277,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10380
   authors:
-  - ΜΠΕΙΝΜΠΡΙΤΖ,ΜΠΕΡΙΛ
+  - BAINBRIDGE,BERYL
   language: el
   title: ΜΙΑ ΑΠΙΣΤΕΥΤΗ ΜΕΓΑΛΗ ΠΕΡΙΠΕΤΕΙΑ
   dewey: 823 ΜΠΕ
   entry_numbers:
   - '12732'
   translators:
   - ΚΟΒΑΛΕΝΚΟ,ΓΙΟΥΡΙ
@@ -521629,15 +521647,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10387
   authors:
-  - ΖΙΡΟΥ,ΦΡΑΝΣΟΥΑΖ
+  - GIROUD,FRANCOISE
   language: el
   title: ΜΕΓΑΛΕ ΜΟΥ ΕΡΩΤΑ
   dewey: 843 ΖΙΡ
   entry_numbers:
   - '12762'
   translators:
   - ΚΑΡΑΚΙΤΣΟΥ-ΝΤΟΥΖΕ [DOUGE],ΝΙΚΗ
@@ -522884,15 +522902,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10411
   authors:
-  - BILLETDOUX,RAPHAELE
+  - BILLETDOUX,RAPHAËLE
   language: el
   title: ΦΥΛΑΞΟΥ ΑΠΟ ΤΗ ΓΛΥΚΑ ΤΩΝ ΠΡΑΓΜΑΤΩΝ
   dewey: 843 BIL
   entry_numbers:
   - '12772'
   translators:
   - ΜΕΤΑΦΤΣΗ,ΑΓΝΗ
@@ -537289,15 +537307,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 10684
   authors:
-  - BOUTENEFF,FANN-PATRICIA
+  - FANN BOUTENEFF,PATRICIA
   title: EXILES ON STAGE
   subtitle: THE MODERN PONTIC THEATER IN GREECE
   dewey: 886.32 BOU
   entry_numbers:
   - '12606'
   editor: ΕΠΙΤ.ΠΟΝΤΙΑΚΩΝ ΜΕΛΕΤ // ΑΘΗΝΑ
   edition_year: 2002
@@ -538365,15 +538383,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10705
   authors:
-  - ΜΠΕΛ,ΧΑΙΝΡΙΧ
+  - BÖLL,HEINRICH
   language: el
   title: Η ΧΑΜΕΝΗ ΤΙΜΗ ΤΗΣ ΚΑΤΕΡΙΝΑΣ ΜΠΛΟΥΜ
   dewey: 832 ΜΠΕ
   entry_numbers:
   - '12902'
   editor: ΤΟ ΒΗΜΑ // ΑΘΗΝΑ
   edition_year: 2007
@@ -539130,15 +539148,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 10720
   authors:
-  - ΖΕΡΖΕΛΙΔΗ,ΓΕΩΡΓ.
+  - ΖΕΡΖΕΛΙΔΗΣ,ΓΕΩΡΓΙΟΣ,Ι.
   language: el
   title: Η ΣΩΝΙΤΣΑ
   subtitle: ΣΤΟ ΙΔΙΩΜΑ ΤΗΣ ΜΑΤΣΟΥΚΑΣ ΤΟΥ ΠΟΝΤΟΥ
   dewey: 889.21 ΖΕΡ
   entry_numbers:
   - '13166'
   editor: None // ΑΘΗΝΑ
@@ -540119,15 +540137,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 10739
   authors:
-  - ΖΕΡΖΕΛΙΔΗ,ΓΕΩΡΓΙΟΥ
+  - ΖΕΡΖΕΛΙΔΗΣ,ΓΕΩΡΓΙΟΣ,Ι.
   language: el
   title: ΙΩΑΚΕΙΜ Δ. ΣΑΛΤΣΗΣ 1893-1968
   subtitle: ΒΙΟΓΡΑΦΙΚΟ ΛΕΥΚΩΜΑ
   dewey: 938.993 ΖΕΡ
   entry_numbers:
   - '13177'
   editor: ΙΩΛΚΟΣ // ΑΘΗΝΑ
@@ -542179,15 +542197,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10779
   authors:
-  - ΜΠΑΡΜΠΑ,ΒΑΣΟΥ
+  - ΜΠΑΡΜΠΑΣ,ΒΑΣΟΣ
   language: el
   title: ΤΟ ΦΕΓΓΟΒΟΛΗΜΑ ΤΗΣ ΖΩΗΣ
   dewey: 889.1 ΜΠΑ
   entry_numbers:
   - '13269'
   editor: None // ΑΘΗΝΑ
   edition_year: 1976
@@ -542881,15 +542899,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 10793
   authors:
-  - ΜΠΑΛΑΦΟΥΣΙΑ-ΓΑΛΑΝΙΔΟΥ,ΕΛΣΑΣ
+  - ΜΠΑΛΑΦΟΥΣΙΑ-ΓΑΛΑΝΙΔΟΥ,ΕΛΣΑ
   language: el
   title: ΣΑΧΤΑΡΙΤΣΑ ΜΑΡΙΤΣΑ
   subtitle: ΑΠΟ ΤΑ ΠΑΡΑΜΥΘΙΑ ΤΟΥ ΠΟΝΤΙΑΚΟΥ ΕΛΛΗΝΙΣΜΟΥ
   dewey: 398 ΜΠΑ
   entry_numbers:
   - '13306'
   editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
@@ -543491,15 +543509,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10805
   authors:
-  - ΜΠΙΝΤΣΥ,ΜΕΗΒ
+  - BINCHY,MAEVE
   language: el
   title: Η ΓΥΑΛΙΝΗ ΛΙΜΝΗ
   dewey: 823 ΜΠΙ
   entry_numbers:
   - '13319'
   translators:
   - ΜΟΣΧΟΠΟΥΛΟΥ,ΠΟΛΥ
@@ -549968,15 +549986,16 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 10931
   authors:
-  - ΜΠΑΛΤΑ,ΕΥΑΓΓΕΛΙΑ-ΚΟΥΡΟΥΠΟΥ,ΜΑΤΟΥΛΑ
+  - ΜΠΑΛΤΑ,ΕΥΑΓΓΕΛΙΑ
+  - ΚΟΥΡΟΥΠΟΥ,ΜΑΤΟΥΛΑ
   language: el
   title: ΕΛΛΗΝΟΡΘΟΔΟΞΕΣ ΚΟΙΝΟΤΗΤΕΣ ΤΗΣ ΚΑΠΠΑΔΟΚΙΑΣ
   subtitle: ΠΕΡΙΦΕΡΕΙΑ ΠΡΟΚΟΠΙΟΥ
   dewey: 938.699 ΜΠΑ
   entry_numbers:
   - '13503'
   editor: ΚΕΝ.ΜΙΚΡΑΣΙΑΤΙΚΩΝ ΣΠ // ΑΘΗΝΑ
@@ -551938,15 +551957,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10969
   authors:
-  - ΜΠΕΛΙΤΣΟΣ,ΘΕΟΔ.
+  - ΜΠΕΛΙΤΣΟΣ,ΘΕΟΔΩΡΟΣ
   language: el
   title: ΑΡΓΥΡΙΟΣ ΜΟΣΧΙΔΗΣ
   subtitle: Ο ΙΣΤΟΡΙΚΟΣ ΤΗΣ ΛΗΜΝΟΥ ΚΑΙ Η ΕΠΟΧΗ ΤΟΥ
   dewey: 938.993 ΜΠΕ
   entry_numbers:
   - '13533'
   editor: ΑΙΓΕΑΣ // ΑΘΗΝΑ
@@ -558008,15 +558027,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 11086
   authors:
-  - ΜΠΕΛΟΟΥΣΟΒΑ,ΛΙΛΙΑ
+  - BELOUSOVA,LILIA
   language: el
   title: ΤΟ ΓΕΝΟΣ ΤΩΝ ΠΕΤΡΟΚΟΚΚΙΝΩΝ
   dewey: 938.498 ΜΠΕ
   entry_numbers:
   - '13688'
   translators:
   - ΤΙΣΚΕΒΙΤΣ,ΞΕΝΙΑ
@@ -560453,15 +560472,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11134
   authors:
-  - ΖΕΡΖΕΛΙΔΗ Ι. ΓΕΩΡΓΙΟΥ
+  - ΖΕΡΖΕΛΙΔΗΣ,ΓΕΩΡΓΙΟΣ,Ι.
   language: el
   title: ΤΟ ΨΩΜΙΝ
   dewey: 398 ΖΕΡ
   entry_numbers:
   - '13799'
   editor: ΠΑΜΠΟΝΤΙΑΚΗΣ ΕΝΩΣΕΩΣ // ΑΘΗΝΑ
   edition_year: 1972
@@ -561450,15 +561469,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11154
   authors:
-  - ΜΠΟΤΣΑΡΗ,ΝΟΤΗ
+  - ΜΠΟΤΣΑΡΗΣ,ΝΟΤΗΣ
   language: el
   title: ΜΙΚΡΑ ΑΣΙΑ ΘΡΥΛΟΙ-ΘΡΙΑΜΒΟΙ-ΘΡΗΝΟΙ-ΘΥΣΙΑΙ ΑΝΑΜΝΗΣΕΙΣ
   dewey: 938.699 ΜΠΟ
   entry_numbers:
   - '13793'
   editor: None // ΑΘΗΝΑ
   edition_year: 1973
@@ -563407,15 +563426,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11193
   authors:
-  - ΜΠΑΛΑΦΟΥΤΗ- ΦΩΤΙΑΔΟΥ ΓΙΩΤΑ
+  - ΜΠΑΛΑΦΟΥΤΗ-ΦΩΤΙΑΔΟΥ,ΓΙΩΤΑ
   language: el
   title: ΠΕΡΑΣΑΝ ΟΛΟΙ ΟΙ ΚΑΙΡΟΙ ΠΑΝΩ ΜΑΣ, ΜΑΡΘΑ
   dewey: 889.21 ΦΩΤ
   entry_numbers:
   - '13902'
   editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1999
@@ -564300,15 +564319,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11211
   authors:
-  - ΜΠΛΑΝΑΣ , ΓΙΩΡΓΟΣ
+  - ΜΠΛΑΝΑΣ,ΓΙΩΡΓΟΣ
   language: el
   title: ΩΔΗ ΣΤΟΝ ΓΙΩΡΓΟ ΚΑΡΑΙΣΚΑΚΗ
   dewey: 938.993 ΜΠΛ
   entry_numbers:
   - '13923'
   editor: ΓΑΒΡΙΗΛΙΔΗΣ // ΑΘΗΝΑ
   edition_year: 2010
@@ -567328,15 +567347,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11272
   authors:
-  - ΜΠΕΤΤΗ,ΣΤΕΦΑΝΟΥ
+  - ΜΠΕΤΤΗΣ,ΣΤΕΦΑΝΟΣ
   language: el
   title: ΟΙ ΖΩΣΙΜΑΔΕΣ
   subtitle: ΚΑΙ Η ΣΥΜΒΟΛΗ ΤΟΥΣ ΣΤ ΝΕΟΕΛΛΗΝΙΚΗ ΑΝΑΓΕΝΝΗΣΗ
   dewey: 938.939 ΜΠΕ
   entry_numbers:
   - '13559'
   editor: None // ΙΩΑΝΝΙΝΑ
@@ -569109,15 +569128,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11308
   authors:
-  - ΖΑΝ ΕΛΛΕΝΣΤΕΙΝ
+  - ELLEINSTEIN,JEAN
   language: el
   title: ΤΟ ΓΑΛΛΙΚΟ ΚΟΜΜΟΥΝΙΣΤΙΚΟ ΚΟΜΜΑ
   dewey: 330 ΧΣ
   entry_numbers:
   - '11531'
   editor: ΘΕΜΕΛΙΟ // ΑΘΗΝΑ
   edition_year: 1997
@@ -570333,15 +570352,16 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11333
   authors:
-  - ΜΠΡΟΥΣΚΟΥ Α., ΑΓΓΕΛΟΠΟΥΛΟΥ Α.
+  - ΜΠΡΟΥΣΚΟΥ,ΑΊΓΛΗ
+  - ΑΓΓΕΛΟΠΟΥΛΟΥ,ΆΝΝΑ
   language: el
   title: ΕΠΕΞΕΡΓΑΣΙΑ ΠΑΡΑΜΥΘΙΑΚΩΝ ΤΥΠΩΝ ΚΑΙ ΠΑΡΑΛΛΑΓΩΝ
   dewey: 888.95 ΜΠΡ
   entry_numbers:
   - '13541'
   editor: Γ Γ ΝΕΑΣ ΓΕΝΙΑΣ // ΑΘΗΝΑ
   edition_year: 1994
@@ -580398,15 +580418,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 11535
   authors:
-  - BARBER,Α.
+  - BARBER,ERIC,ARTHUR
   title: SEXTI PRORERTI CARMINA
   dewey: 372.65 BAR
   entry_numbers:
   - '15008'
   editor: None // OXFORD
   edition_year: 1960
   pages: 180
@@ -581040,15 +581060,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 11548
   authors:
-  - ΜΠΑΜΠΙΝΙΩΤΗΣ,Γ
+  - ΜΠΑΜΠΙΝΙΩΤΗΣ,ΓΕΩΡΓΙΟΣ
   language: el
   title: ΛΕΞΙΚΟ ΓΙΑ ΤΟ ΣΧΟΛΕΙΟ ΚΑΙ ΤΟ ΓΡΑΦΕΙΟ
   dewey: 489.33 ΜΠΑ
   entry_numbers:
   - '15092'
   editor: None // ΑΘΗΝΑ
   edition_year: 2004
@@ -587805,15 +587825,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11682
   authors:
-  - ΖΩΡΖ ΜΠΟΡΝΤΟΝΟΒ
+  - BORDONOVE,GEORGES
   language: el
   title: ΝΑΙΤΕΣ ΙΠΠΟΤΕΣ Ν
   subtitle: ΜΥΣΤΙΚΑ, ΑΙΡΕΤΙΚΕΣ ΜΥΣΤΑΓΩΓΙΕΣ ΚΑΙ ΑΛΗΘΕΙΑ
   dewey: 230 ΜΠΟ
   entry_numbers:
   - '15179'
   translators:
@@ -589847,15 +589867,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11723
   authors:
-  - ΜΠΙΝΑΡΔΟΠΟΥΛΟΥ,ΝΤΙΝΟΥ
+  - ΜΠΙΝΑΡΔΟΠΟΥΛΟΣ,ΝΤΙΝΟΣ
   language: el
   title: ΛΟΓΑΡΙΘΜΙΚΟΙ ΠΙΝΑΚΕΣ
   dewey: 512.922 ΜΠΙ
   entry_numbers:
   - '15277'
   pages: 159
   topics:
@@ -590654,15 +590674,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11739
   authors:
-  - ΜΠΕΡΝΕΤ,ΓΟΥΙΛΙΑΜ
+  - BURNETT,WILLIAM
   language: el
   title: Ο ΜΙΚΡΟΣ ΚΑΙΣΑΡ
   dewey: 823 ΜΠΕ
   entry_numbers:
   - '15249'
   editor: ΠΑΡΑΤΗΡΗΤΗΣ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1985
@@ -596546,15 +596566,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11856
   authors:
-  - ΖΑΒΙΤΣΑΝΟΥ,ΔΗΜΟΣΘΕΝΗ
+  - ΖΑΒΙΤΣΑΝΟΣ,ΔΗΜΟΣΘΕΝΗΣ
   language: el
   title: ΠΕΛΑΓΙΣΙΕΣ ΑΥΡΕΣ
   dewey: 889.1 ΖΑΒ
   entry_numbers:
   - '15341'
   editor: ΘΟΥΚΥΔΙΔΗΣ // ΑΘΗΝΑ
   edition_year: 1993
@@ -596696,15 +596716,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11859
   authors:
-  - ΜΠΕΡ,ΜΑΞ
+  - BEER,MAX
   language: el
   title: ΟΙ ΚΟΙΝΩΝΙΚΟΙ ΑΓΩΝΕΣ ΣΤΗΝ ΑΡΧΑΙΟΤΗΤΑ
   subtitle: ΠΑΛΑΙΣΤΙΚΗ ΕΛΛΑΣ ΡΩΜΗ
   dewey: 050 ΜΠΕ
   entry_numbers:
   - '15320'
   translators:
@@ -597700,15 +597720,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11879
   authors:
-  - ΖΑΜΠΟΥΝΗΣ ΧΡΗΣΤΟΣ
+  - ΖΑΜΠΟΥΝΗΣ,ΧΡΗΣΤΟΣ
   title: SAVOIR VIVRE
   dewey: 395.094 ΖΑΜ
   entry_numbers:
   - '15375'
   editor: ΦΕΡΕΝΙΚΗ // None
   pages: 512
   topics:
@@ -599057,15 +599077,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11906
   authors:
-  - BARBAGALLO,C
+  - BARBAGALLO,CORRADO
   language: el
   title: ΤΑ ΑΙΤΙΑ ΠΑΡΑΚΜΗΣ ΤΗΣ ΑΡΧΑΙΑΣ ΕΛΛΑΔΟΣ
   dewey: 938.498 BAR
   entry_numbers:
   - '15337'
   editor: ΜΠΑΥΡΟΝ // ΑΘΗΝΑ
   pages: 287
@@ -602028,15 +602048,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11965
   authors:
-  - ΜΠΟΚΟΒΟΥ,ΠΑΝΑΓΙΩΤΗ
+  - ΜΠΟΚΟΒΟΣ,ΠΑΝΑΓΙΩΤΗΣ
   language: el
   title: ΠΟΛΙΤΙΚΑ ΚΑΙ ΟΙΚΟΝΟΜΙΚΑ
   dewey: 330 ΜΠΟ
   entry_numbers:
   - '15431'
   edition_year: 1981
   pages: 176
@@ -604052,15 +604072,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12005
   authors:
-  - BOWRA,C.M
+  - BOWRA,CECIL,MAURICE
   title: THE GREEK EXPERIENCE
   dewey: 372.65 BOW
   entry_numbers:
   - '15462'
   editor: MENTOR BOOK // LONDON
   pages: 223
   topics:
@@ -604885,15 +604905,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12022
   authors:
-  - ΜΠΟΥΣΟΥΝΗ,ΔΗΜΗΤΡΗ
+  - ΜΠΟΥΣΟΥΝΗΣ,ΔΗΜΗΤΡΗΣ
   language: el
   title: ΔΥΟ ΧΙΛΙΑΔΕΣ ΧΡΟΝΙΑ
   dewey: 889.1 ΜΠΟ
   entry_numbers:
   - '15771'
   editor: None // ΚΑΛΑΜΑΤΑ
   edition_year: 1999
@@ -606587,15 +606607,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12056
   authors:
-  - ΜΠΑΡΑ,ΑΛΕΞΑΝΔΡΟΥ
+  - ΜΠΑΡΑΣ,ΑΛΕΞΑΝΔΡΟΣ
   language: el
   title: ΣΥΝΘΕΣΕΙΣ
   dewey: 889.1 ΜΠΑ
   entry_numbers:
   - '15757'
   editor: ΟΙ ΕΚΔΟΣΕΙΣ ΤΩΝ ΦΙΛΩ // ΑΘΗΝΑ
   edition_year: 1973
@@ -608285,15 +608305,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 12090
   authors:
-  - ΜΠΟΥΡΟΠΟΥΛΟΥ,ΑΓΓΕΛΟΥ
+  - ΜΠΟΥΡΟΠΟΥΛΟΣ,ΑΓΓΕΛΟΣ,ΝΙΚ.
   language: el
   title: ΚΩΔΙΞ ΠΟΙΝΙΚΗΣ ΔΙΚΟΝΟΜΙΑΣ
   dewey: 345.04 ΜΠΟ
   entry_numbers:
   - '15534'
   editor: ΣΑΚΚΟΥΛΑ // ΑΘΗΝΑ
   pages: 283
@@ -608638,15 +608658,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 12097
   authors:
-  - BREMOND,CL.
+  - BREMOND,CLAUDE
   language: el
   title: ΘΕΩΡΙΑ ΤΗΣ ΑΦΗΓΗΣΗΣ
   dewey: 809.923 BER
   entry_numbers:
   - '15495'
   editor: ΕΞΑΝΤΑΣ // ΑΘΗΝΑ
   edition_year: 1991
@@ -609489,15 +609509,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12114
   authors:
-  - BEUS,J.G
+  - BEUS,JACOBUS,GIJSBERTUS DE
   language: el
   title: ΤΟ ΜΕΛΛΟΝ ΤΗΣ ΔΥΣΕΩΣ
   dewey: 901 BEU
   entry_numbers:
   - '15516'
   editor: ΕΣΤΙΑ // ΑΘΗΝΑ
   edition_year: 1953
@@ -611623,15 +611643,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12157
   authors:
-  - ΜΠΟΤΣΑΡΗ,ΜΑΡΚΟΥ
+  - ΜΠΟΤΣΑΡΗΣ,ΜΑΡΚΟΣ
   language: el
   title: Η ΕΥΑ ΓΕΩΡΓΙΟΥ ΠΑΠΑΝΔΡΕΟΥ ΑΠΟΚΑΛΥΠΤΕΙ
   dewey: 324.209 ΜΠΟ
   entry_numbers:
   - '15538'
   editor: ΙΣΟΚΡΑΤΗΣ // None
   pages: 195
@@ -612216,15 +612236,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12169
   authors:
-  - ΖΙΑΚΑ,ΓΡΗΓΟΡΙΟΥ
+  - ΖΙΑΚΑΣ,ΓΡΗΓΟΡΙΟΣ
   language: el
   title: ΤΑ ΕΛΛΗΝΙΚΗ ΓΡΑΜΜΑΤΑ ΚΑΙ Ο ΑΡΙΣΤΟΤΕΛΗΣ ΣΤΗΝ ΑΡΑΒΙΚΗ ΠΑΡΑΔΟΣΗ
   dewey: 181.07 ΖΙΑ
   entry_numbers:
   - '15545'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1986
@@ -613117,15 +613137,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12187
   authors:
-  - BOHLER, BING
+  - BOHLER,BING
   title: ARDJIO FUR BURGERLIDJES BEDJT
   dewey: 372.65 BOH
   entry_numbers:
   - '15687'
   editor: BERLAG // BERLIN
   edition_year: 1906
   pages: 418
@@ -613314,15 +613334,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12191
   authors:
-  - ΖΙΑΚΑΣ ΓΡΗΓΟΡΙΟΣ
+  - ΖΙΑΚΑΣ,ΓΡΗΓΟΡΙΟΣ
   language: el
   title: ΘΡΗΣΚΕΙΟΛΟΓΙΑ Η ΘΡΗΣΚΕΙΑ ΤΩΝ ΠΡΟΙΣΤΟΡΙΚΩΝ ΚΟΙΝΩΝΙΩΝ ΚΑΙ ΤΩΝ
   subtitle: ΑΡΧΑΙΩΝ ΛΑΩΝ
   dewey: 230 ΖΙΑ
   entry_numbers:
   - '15560'
   editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
@@ -614065,15 +614085,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12206
   authors:
-  - ΜΠΟΝΗΣ ΚΩΝΣΤΑΝΤΙΝΟΣ
+  - ΜΠΟΝΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
   language: el
   title: ΟΙ ΕΛΛΗΝΕΣ ΙΕΡΑΠΟΣΤΟΛΟΙ ΤΩΝ ΣΛΑΒΩΝ ΚΥΡΙΛΛΟΣ ΚΑΙ ΜΕΘΟΔΙΟΣ ΥΠΟ
   subtitle: ΤΟ ΝΕΟΝ ΦΩΣ ΤΗΣ ΕΠΙΣΤΗΜΗΣ
   dewey: 230 ΜΠΟ
   entry_numbers:
   - '15557'
   editor: None // ΑΘΗΝΑ
@@ -614312,15 +614332,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12211
   authors:
-  - BRULE PIERRE
+  - BRULE,PIERRE
   language: el
   title: ΠΕΡΙΚΛΗΣ ΤΟ ΜΕΣΟΥΡΑΝΗΜΑ ΤΗΣ ΑΘΗΝΑΣ
   subtitle: ΑΚΑΛΥΨΕΙΣ ΔΕΛΗΘΑΝΑΣΗ
   dewey: 938.498 BRU
   entry_numbers:
   - '15592'
   edition_year: 1997
@@ -614768,15 +614788,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12220
   authors:
-  - ΖΑΦΕΙΡΗ,ΝΙΚΟΛΑΟΥ
+  - ΖΑΦΕΙΡΗΣ,ΝΙΚΟΛΑΟΣ
   language: el
   title: ΑΙΣΘΗΤΙΚΗ ΑΞΙΟΛΟΓΗΣΗΣ ΤΗΣ ΒΥΖΑΝΤΙΝΗΣ ΤΕΧΝΗΣ
   dewey: 709.2 ΖΑΦ
   entry_numbers:
   - '15674'
   editor: ΕΤ.ΠΑΡΑΔ.ΣΠΟΥΔΩΝ // ΑΘΗΝΑ
   edition_year: 1981
@@ -614919,15 +614939,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12223
   authors:
-  - ΜΠΑΙΡΑΚΤΑΡΗ,ΑΝΤΩΝΙΟΥ
+  - ΜΠΑΙΡΑΚΤΑΡΗΣ,ΑΝΤΩΝΙΟΣ
   language: el
   title: ΘΕΜΕΛΙΩΔΗ ΠΡΟΒΛΗΜΑΤΑ ΤΗΣ ΔΟΓΜΑΤΙΚΗΣ ΚΑΙ ΗΘΙΚΗΣ
   dewey: 230.19 ΜΠΑ
   entry_numbers:
   - '15588'
   editor: None // ΑΘΗΝΑ
   edition_year: 1960
@@ -616568,15 +616588,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12256
   authors:
-  - ΜΠΟΝΗ,ΚΩΝΣΤΑΝΤΙΝΟΥ
+  - ΜΠΟΝΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
   language: el
   title: ΣΚΕΨΕΙΣ ΕΠΙ ΣΥΓΧΡΟΝΩΝ ΕΚΚΛΗΣΙΑΣΤΙΚΩΝ ΘΕΜΑΤΩΝ
   dewey: 230 ΜΠΟ
   entry_numbers:
   - '15562'
   - '17430'
   editor: None // ΑΘΗΝΑ
@@ -617934,15 +617954,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12283
   authors:
-  - ΜΠΟΚΟΒΟΥ,ΠΑΝΑΓΙΩΤΗ
+  - ΜΠΟΚΟΒΟΣ,ΠΑΝΑΓΙΩΤΗΣ
   language: el
   title: ΠΟΛΙΤΙΚΑ ΚΑΙ ΟΙΚΟΝΟΜΙΚΑ
   dewey: 320 ΜΠΟ
   entry_numbers:
   - '15684'
   edition_year: 1981
   pages: 176
@@ -618383,15 +618403,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12292
   authors:
-  - ΖΑΓΚΛΗ,ΔΗΜΗΤΡΙΟΥ
+  - ΖΑΓΚΛΗΣ,ΔΗΜΗΤΡΙΟΣ
   language: el
   title: Η ΜΑΚΕΔΟΝΙΑ ΤΟΥ ΑΙΓΑΙΟΥ ΚΑΙ ΟΙ ΓΙΟΥΓΚΟΣΛΑΒΟΙ
   dewey: 938.94 ΖΑΓ
   entry_numbers:
   - '15661'
   editor: None // ΑΘΗΝΑ
   edition_year: 1975
@@ -623240,15 +623260,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12389
   authors:
-  - ZSCHOKKE-HEINRICH,JOHANN
+  - ZSCHOKKE,JOHANN,HEINRICH DANIEL
   language: el
   title: ΤΟ ΧΡΥΣΟΧΩΡΙ
   dewey: 701 ZSC
   entry_numbers:
   - '15875'
   translators:
   - ΠΑΝΟΥ,ΔΗΜ.
@@ -623493,15 +623513,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12394
   authors:
-  - ΖΑΚΟΠΟΥΛΟΣ,ΝΙΚΟΣ
+  - ΖΑΚΟΠΟΥΛΟΣ,ΝΙΚΟΣ,Ι.
   language: el
   title: ΔΙΗΓΗΜΑΤΑ
   dewey: 889.21 ΖΑΚ
   entry_numbers:
   - '15941'
   editor: None // ΑΘΗΝΑ
   edition_year: 1972
@@ -629122,15 +629142,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12506
   authors:
-  - ΜΠΟΚΟΒΟΥ,ΠΑΝ.
+  - ΜΠΟΚΟΒΟΣ,ΠΑΝΑΓΙΩΤΗΣ
   language: el
   title: ΠΡΟΤΑΣΕΙΣ ΤΙΝΕΣ ΔΙΑ ΤΗΝ ΘΕΩΡΗΤΙΚΗΝ ΔΙΕΡΕΥΝΗΣΙΝ ΚΑΙ ΤΗΝ ΕΠΑΓΓ
   subtitle: ΕΛΜΑΤΙΚΗΝ ΧΡΗΣΙΜΟΠΟΙΗΣΙΝ ΤΗΣ ΛΕΙΤΟΥΡΓΙΑΣ ΤΩΝ ΔΗΜΟΣΙΩΝ ΣΧΕΣΕ
   dewey: 659.2 ΜΠΟ
   entry_numbers:
   - '15966'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
@@ -629473,15 +629493,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12513
   authors:
-  - ΜΠΟΚΟΒΟΥ,ΠΑΝΑΓΙΩΤΟΥ
+  - ΜΠΟΚΟΒΟΣ,ΠΑΝΑΓΙΩΤΗΣ
   language: el
   title: ΜΕΛΕΤΑΙ ΕΠΙ ΘΕΜΑΤΩΝ ΔΗΜΟΣΙΩΝ ΣΧΕΣΕΩΝ
   dewey: 659.2 ΜΠΟ
   entry_numbers:
   - '15961'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1970
@@ -629523,15 +629543,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12514
   authors:
-  - ΖΟΜΠΑΝΑΚΗ,ΑΠ.
+  - ΖΟΜΠΑΝΑΚΗΣ,ΣΠ.
   language: el
   title: ΣΥΜΒΟΛΗ ΕΙΣ ΤΗΝ ΙΣΤΟΡΙΑΝ ΤΩΝ ΔΗΜΟΣΙΩΝ ΣΧΕΣΕΩΝ
   dewey: 659.2 ΖΟΜ
   entry_numbers:
   - '15962'
   editor: None // ΑΘΗΝΑ
   edition_year: 1965
@@ -629573,15 +629593,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12515
   authors:
-  - ΖΟΜΠΑΝΑΚΗ,ΣΠ.
+  - ΖΟΜΠΑΝΑΚΗΣ,ΣΠ.
   language: el
   title: ΔΗΜΟΣΙΑΙ ΣΧΕΣΕΙΣ
   dewey: 659.2 ΖΟΜ
   entry_numbers:
   - '15960'
   editor: None // ΑΘΗΝΑ
   edition_year: 1968
@@ -629623,15 +629643,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12516
   authors:
-  - ΖΟΜΠΑΝΑΚΗ,ΣΠ.
+  - ΖΟΜΠΑΝΑΚΗΣ,ΣΠ.
   language: el
   title: ΔΗΜΟΣΙΑΙ ΣΧΕΣΕΙΣ
   dewey: 659.2 ΖΟΜ
   entry_numbers:
   - '15959'
   editor: None // ΑΘΗΝΑ
   edition_year: 1974
@@ -631471,15 +631491,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12553
   authors:
-  - ΖΑΛΩΝΗ,ΠΑΝΑΓΙΩΤΑ
+  - ΖΑΛΩΝΗ-ΧΡΙΣΤΟΠΟΥΛΟΥ,ΠΑΝΑΓΙΩΤΑ
   language: el
   title: ΡΙΜΑΤΙΚΗ ΜΕΤΡΙΚΗ ΠΟΙΗΣΗ
   dewey: 889.1 ΖΑΛ
   entry_numbers:
   - '16017'
   editor: ΞΑΣΤΕΡΟΝ // ΑΘΗΝΑ
   edition_year: 2006
@@ -632870,15 +632890,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12581
   authors:
-  - ΜΠΑΛΖΑΚ,ΟΝΟΡΕ
+  - BALZAC,HONORÉ DE
   language: el
   title: ΕΥΓΕΝΙΑ ΓΚΡΑΝΤΕ
   dewey: 889.21 ΜΠΑ
   entry_numbers:
   - '16053'
   translators:
   - ΝΙΚΑΣ,ΑΓΓΕΛΟΣ
@@ -633123,15 +633143,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12586
   authors:
-  - BAKER,,Q.P
+  - BAKER,GEORGE,PHILIP
   language: el
   title: Ο ΑΝΝΙΒΑΣ
   dewey: 889.21 BAK
   entry_numbers:
   - '16050'
   translators:
   - ΑΡΓΥΡΟΠΟΥΛΟΥ,ΟΘ.
@@ -633375,15 +633395,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12591
   authors:
-  - ΜΠΕΡΝ,Α.Ρ
+  - BURN,ANDREW,ROBERT
   language: el
   title: Ο ΠΕΡΙΚΛΗΣ ΚΑΙ Η ΑΘΗΝΑ
   dewey: 938.498 ΜΠΕ
   entry_numbers:
   - '16062'
   editor: ΓΑΛΑΞΙΑΣ // ΑΘΗΝΑ
   edition_year: 1948
@@ -633526,15 +633546,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12594
   authors:
-  - BABELON,J
+  - BABELON,JEAN
   language: el
   title: ΑΛΚΙΒΙΑΔΗΣ
   dewey: 889.21 BAB
   entry_numbers:
   - '16058'
   editor: ΜΠΕΡΓΚΑΔΗ // ΑΘΗΝΑ
   edition_year: 1961
@@ -634078,15 +634098,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12605
   authors:
-  - ΜΠΡΙΟΝ ΜΑΡΣΕΛ
+  - BRION,MARCEL
   language: el
   title: ΜΙΧΑΗΛ ΑΓΓΕΛΟΣ
   subtitle: ΙΩΑΝΝΙΔΗΣ Π. Σ.
   dewey: 920 ΜΠΡ
   entry_numbers:
   - '16084'
   editor: None // ΑΘΗΝΑ
@@ -635372,15 +635392,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12631
   authors:
-  - ΜΠΟΝΑΡ,ΑΝΤΡΕ
+  - BONNARD,ANDRÉ
   language: el
   title: Ο ΑΡΧΑΙΟΣ ΕΛΛΗΝΙΚΟΣ ΠΟΛΙΤΙΣΜΟΣ
   dewey: 938.498 ΜΠΟ
   entry_numbers:
   - '16106'
   translators:
   - ΓΑΡΙΔΗ,ΕΛΕΝΗ
@@ -635528,15 +635548,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12634
   authors:
-  - ΖΩΓΡΑΦΑΚΗ,ΓΕΩΡΓΙΟΥ
+  - ΖΩΓΡΑΦΑΚΗΣ,ΓΕΩΡΓΙΟΣ
   language: el
   title: ΘΕΣΣΑΛΟΝΙΚΗ
   subtitle: ΠΕΡΙΠΑΤΟΣ ΑΝΑΜΕΣΑ ΑΠΟ ΤΗΝ ΙΣΤΟΡΙΑ ΚΑΙ ΤΑ ΜΝΗΜΕΙΑ ΤΗΣ
   dewey: 949.565 ΖΩΓ
   entry_numbers:
   - '16070'
   editor: ΜΑΣΤΟΡΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
@@ -635629,15 +635649,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12636
   authors:
-  - ΜΠΕΝΕΚΟΥ,ΓΙΑΝΝΗ
+  - ΜΠΕΝΕΚΟΣ,ΓΙΑΝΝΗΣ
   language: el
   title: ΚΩΛΕΤΗΣ
   dewey: 938.498 ΜΠΕ
   entry_numbers:
   - '16096'
   editor: ΚΥΨΕΛΗ // ΑΘΗΝΑ
   edition_year: 1961
@@ -636420,15 +636440,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12652
   authors:
-  - BASS,J
+  - BASS,J.
   title: HOMERS ODYSSEE
   dewey: 372.65 BAS
   entry_numbers:
   - '16139'
   editor: None // STUTTGART
   pages: 240
   topics:
@@ -636564,15 +636584,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12655
   authors:
-  - BURN,A.R
+  - BURN,ANDREW,ROBERT
   title: THE PELICAN HISTORY OF GREECE
   dewey: 372.65 BUR
   entry_numbers:
   - '16144'
   editor: PENGUIN BOOKS // GREAT BRITAIN
   edition_year: 1974
   pages: 414
@@ -638173,15 +638193,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12688
   authors:
-  - ΖΙΑΚΑ,ΓΡΗΓΟΡΙΟΥ
+  - ΖΙΑΚΑΣ,ΓΡΗΓΟΡΙΟΣ
   language: el
   title: Η ΠΕΡΙ ΕΣΧΑΤΩΝ ΔΙΔΑΣΚΑΛΙΑ ΤΟΥ ΙΣΛΑΜ
   dewey: 337.405 ΖΙΑ
   entry_numbers:
   - '16077'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1976
@@ -640045,15 +640065,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12725
   authors:
-  - ΜΠΕΡΝ,ΕΡΙΚ
+  - BERNE,ERIC
   language: el
   title: ΠΑΙΧΝΙΔΙΑ ΠΟΥ ΠΑΙΖΟΥΝ ΟΙ ΑΝΘΡΩΠΟΙ
   dewey: 158.2 ΜΠΕ
   entry_numbers:
   - '16230'
   editor: METAGLOT // ΘΕΣΣΑΛΟΝΙΚΗ
   pages: 142
@@ -640400,15 +640420,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12732
   authors:
-  - ΜΠΕΡΝ,Α.Ρ
+  - BURN,ANDREW,ROBERT
   language: el
   title: Ο ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ ΚΑΙ Η ΕΛΛΗΝΙΣΤΙΚΗ ΑΥΤΟΚΡΑΤΟΡΙΑ
   dewey: 938.070 ΜΠΕ
   entry_numbers:
   - '16208'
   translators:
   - ΚΟΤΖΙΑΣ,ΑΛΕΞ.
@@ -642061,15 +642081,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12765
   authors:
-  - ΜΠΟΝΟΥ,Β.Ν.
+  - ΜΠΌΝΟΣ,Β.,Ν.
   language: el
   title: ΑΥΤΟΜΕΛΑ
   dewey: 889.1 ΜΠΟ
   entry_numbers:
   - '16244'
   editor: ΚΟΥΚΟΥΔΑΚΗΣ // ΑΘΗΝΑ
   pages: 222
@@ -643756,15 +643776,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12799
   authors:
-  - ΜΠΡΙΟΝ,ΜΑΡΣΕΛ
+  - BRION,MARCEL
   language: el
   title: ΛΕΟΝΑΡΔΟΣ ΝΤΑ ΒΙΝΤΣΙ
   dewey: 150.195 ΜΠΡ
   entry_numbers:
   - '16255'
   editor: ΣΥΨΗ // ΑΘΗΝΑ
   pages: 316
@@ -645901,15 +645921,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12842
   authors:
-  - ΜΠΑΚ,ΠΕΡΛ
+  - BUCK,PEARL,S.
   language: el
   title: ΕΛΑ ΑΓΑΠΗ ΜΟΥ
   dewey: 889.21 ΜΠΑ
   entry_numbers:
   - '16332'
   translators:
   - ΣΑΡΛΗΣ,ΝΙΚΟΣ
@@ -647809,15 +647829,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12880
   authors:
-  - ΜΠΟΥΣΟΥΛΑ,ΝΙΚΟΛΑΟΥ-ΙΩΑΝΝΟΥ
+  - ΜΠΟΎΣΟΥΛΑΣ,ΝΙΚΌΛΑΟΣ-ΙΩΆΝΝΗΣ,Σ.
   language: el
   title: ΦΥΣΙΚΗ ΚΑΙ ΟΝΤΟΛΟΓΙΑ ΣΤΗΝ ΤΕΛΕΥΤΑΙΑ ΠΛΑΤΩΝΙΚΗ ΔΙΑΛΕΚΤΙΚΗ
   dewey: 184 ΜΠΟ
   entry_numbers:
   - '16364'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1974
@@ -648508,15 +648528,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12894
   authors:
-  - ΖΑΚΟΠΟΥΛΟΣ,ΝΙΚΟΣ
+  - ΖΑΚΟΠΟΥΛΟΣ,ΝΙΚΟΣ,Ι.
   language: el
   title: Ο ΑΥΡΙΑΝΟΣ ΚΟΣΜΟΣ
   dewey: 330.011 ΖΑΚ
   entry_numbers:
   - '16341'
   editor: ΦΙΛΙΠΠΟΤΗ // ΑΘΗΝΑ
   edition_year: 1990
@@ -650251,15 +650271,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12929
   authors:
-  - ΜΠΟΚΟΒΟΥ,ΠΑΝΑΓΙΩΤΗ
+  - ΜΠΟΚΟΒΟΣ,ΠΑΝΑΓΙΩΤΗΣ
   language: el
   title: Η ΝΕΑ ΔΗΜΟΚΡΑΤΙΑ ΟΙ ΜΑΡΞΙΣΤΕΣ ΚΑΙ ΤΟ ΧΡΕΟΣ ΤΟΥ ΠΟΛΙΤΗ
   dewey: 324.249 ΜΠΟ
   entry_numbers:
   - '16408'
   edition_year: 1981
   pages: 19
@@ -650300,15 +650320,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12930
   authors:
-  - ΖΙΑΚΑ,ΓΡΗΓΟΡΙΟΥ
+  - ΖΙΑΚΑΣ,ΓΡΗΓΟΡΙΟΣ
   language: el
   title: Ο ΘΙΒΕΤΙΚΟΣ ΒΟΥΔΙΣΜΟΣ ΚΑΙ Ο ΔΑΛΑΙ ΛΑΜΑ
   dewey: 294.393 ΖΙΑ
   entry_numbers:
   - '16409'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1992
@@ -651848,15 +651868,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12961
   authors:
-  - ΜΠΟΚΟΒΟΥ,ΠΑΝΑΓΙΩΤΟΥ
+  - ΜΠΟΚΟΒΟΣ,ΠΑΝΑΓΙΩΤΗΣ
   language: el
   title: Η ΛΕΙΤΟΥΡΓΙΑ ΤΩΝ ΔΗΜΟΣΙΩΝ ΣΧΕΣΕΩΝ ΕΙΣ ΤΗΝ ΣΥΓΧΡΟΝΟΝ ΟΙΚΟΝΟΜΙ
   dewey: 659.2 ΜΠΟ
   entry_numbers:
   - '16418'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1974
@@ -652201,15 +652221,16 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 12968
   authors:
-  - ΜΠΟΥΡΓΟΣ,ΗΛΙΑΣ-ΓΑΤΑ.ΣΤΑΥΡΟΥΛΑ
+  - ΜΠΟΥΡΓΟΣ,ΗΛΙΑΣ
+  - ΓΑΤΑ,ΣΤΑΥΡΟΥΛΑ
   language: el
   title: Η ΚΑΤΑΣΤΑΣΗ ΤΗΣ ΕΚΠΑΙΔΕΥΣΗΣ ΣΤΟ ΝΟΜΟ ΑΡΤΑΣ
   dewey: 938.939 ΜΠΟ
   entry_numbers:
   - '16459'
   editor: ΕΝΤΥΠΩΣΙΣ // ΑΡΤΑ
   edition_year: 2005
@@ -653863,15 +653884,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13001
   authors:
-  - JAEGER,WERNER
+  - JAEGER,WERNER,WILHELM
   language: el
   title: ΑΝΘΡΩΠΙΣΜΟΣ ΚΑΙ ΘΕΟΛΟΓΙΑ
   subtitle: ΟΙ ΕΛΛΗΝΕΣ ΚΑΙ Η ΑΓΩΓΗ ΤΟΥ ΑΝΘΡΩΠΟΥ
   dewey: 230 JAE
   entry_numbers:
   - '16464'
   translators:
@@ -655808,15 +655829,16 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13040
   authors:
-  - BOUET,M
+  - BOUET,M.
+  - VALLIN,J.
   title: BIOLOGIE 5
   dewey: 372.65 BOU
   entry_numbers:
   - '16509'
   editor: BORDAS // PARIS
   edition_year: 1974
   pages: 222
@@ -660782,15 +660804,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13137
   authors:
-  - ΜΠΡΙΣΚΟΟΥ,ΤΖΟΑΝΑ
+  - BRISCOE,JOANNA
   language: el
   title: ΚΟΙΜΗΣΟΥ ΜΑΖΙ ΜΟΥ
   dewey: 823 ΜΠΡ
   entry_numbers:
   - '16625'
   translators:
   - ΜΑΝΤΟΓΛΟΥ,ΑΡΓΥΡΩ
@@ -661396,15 +661418,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13149
   authors:
-  - ΜΠΑΡΙΤΑΚΗ,ΒΑΓΓΕΛΗ
+  - ΜΠΑΡΙΤΑΚΗΣ,ΒΑΓΓΕΛΗΣ
   language: el
   title: ΓΟΥΒΕΣ 1940-44
   dewey: 949.5 ΜΠΑ
   entry_numbers:
   - '8209'
   editor: None // ΓΟΥΒΕΣ
   edition_year: 2000
@@ -661980,15 +662002,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13161
   authors:
-  - ΜΠΕΡΔΕΚΛΗ,ΓΕΩΡΓΙΟΥ
+  - ΜΠΕΡΔΕΚΛΗΣ,ΓΕΩΡΓΙΟΣ
   language: el
   title: ΜΕΤΑ ΤΗ ΔΟΞΑ ΤΟΥ 40
   dewey: 938.506 ΜΠΕ
   entry_numbers:
   - '16632'
   editor: None // ΚΑΛΑΜΑΤΑ
   edition_year: 2002
@@ -662927,15 +662949,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13180
   authors:
-  - ΖΑΤΕΛΗ,ΖΥΡΡΑΝΑ
+  - ΖΑΤΕΛΗ,ΖΥΡΑΝΝΑ
   language: el
   title: ΠΕΡΣΙΝΗ ΑΡΡΑΒΩΝΙΑΣΤΙΚΙΑ
   dewey: 889.21 ΖΑΤ
   entry_numbers:
   - '16678'
   editor: ΚΑΣΤΑΝΙΩΤΗΣ // ΑΘΗΝΑ
   edition_year: 1994
@@ -663698,15 +663720,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13195
   authors:
-  - ΖΑΜΒΑΛΝΤ,ΑΚΙΜ
+  - SAMWALD,ACHIM
   language: el
   title: ΑΠΟΞΗΡΑΙΝΩ ΚΑΙ ΣΥΝΤΗΡΩ ΜΟΝΟΣ ΜΟΥ
   dewey: 641.4 ΖΑΜ
   entry_numbers:
   - '16657'
   editor: ΤΟ ΒΗΜΑ // ΑΘΗΝΑ
   edition_year: 2012
@@ -668748,15 +668770,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13294
   authors:
-  - ΜΠΑΚ,ΠΕΡΛ
+  - BUCK,PEARL,S.
   language: el
   title: ΚΑΤΩ ΑΠΟ ΤΟ ΒΛΕΜΜΑ ΤΟΥ ΒΟΥΔΑ
   dewey: 810.11 ΜΠΑ
   entry_numbers:
   - '16786'
   translators:
   - ΑΝΑΓΝΩΣΤΟΠΟΥΛΟΣ,Π.
@@ -670272,15 +670294,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13324
   authors:
-  - ΜΠΕΝΓΚΤΣΟΝ,ΧΕΡΜΑΝ
+  - BENGTSON,HERMANN
   language: el
   title: ΙΣΤΟΡΙΑ ΤΗΣ ΑΡΧΑΙΑΣ ΕΛΛΑΔΟΣ
   dewey: 938 ΜΠΕ
   entry_numbers:
   - '16908'
   translators:
   - ΓΑΒΡΙΛΗΣ,ΑΝΤΡΕΑΣ
@@ -671504,15 +671526,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13348
   authors:
-  - ΜΠΕΡΓΑΜΙΝΙ,ΝΤΕΙΒΙΝΤ
+  - BERGAMINI,DAVID
   language: el
   title: ΜΑΘΗΜΑΤΙΚΑ
   dewey: 030 ΜΠΕ
   entry_numbers:
   - '16912'
   editor: ΤΑΙΜ // None
   edition_year: 1975
@@ -672568,15 +672590,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13369
   authors:
-  - ΜΠΡΙΟΝ,ΜΑΡΣΕΛ
+  - BRION,MARCEL
   language: el
   title: ΜΙΧΑΗΛ ΑΓΓΕΛΟΣ
   dewey: 808.838 ΜΠΡ
   entry_numbers:
   - '16864'
   translators:
   - ΙΩΑΝΝΙΔΗ,Π.Σ.
@@ -675439,15 +675461,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13426
   authors:
-  - BEISSIER,F
+  - BEISSIER,FERNAND
   title: LES MEMOIRES D'UN MOINEAU
   dewey: 372.65 BEI
   entry_numbers:
   - '16891'
   editor: HACHETTE ET // PARIS
   edition_year: 1895
   pages: 69
@@ -678252,15 +678274,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 13482
   authors:
-  - ΜΠΡΙΣΚΟΟΥ,ΤΖΟΑΝΑ
+  - BRISCOE,JOANNA
   language: el
   title: ΚΟΙΜΗΣΟΥ ΜΑΖΙ ΜΟΥ
   dewey: 823 ΜΠΡ
   entry_numbers:
   - '17042'
   translators:
   - ΜΑΝΤΟΓΛΟΥ,ΑΡΓΥΡΩ
@@ -678863,15 +678885,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13494
   authors:
-  - ΜΠΕΒΙΛΑΚΟΥΑ,ΑΛΜΠΕΡΤΟ
+  - BEVILACQUA,ALBERTO
   language: el
   title: Ο ΕΡΩΣ
   dewey: 850.11 ΜΠΕ
   entry_numbers:
   - '20598'
   translators:
   - ΤΣΑΚΟΥ-ΚΟΝΒΕΡΤΙ,ΤΟΤΑ
@@ -680416,15 +680438,16 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13524
   authors:
-  - ΜΠΡΙΜΠΟ,ΤΖΕΦ-ΓΚΕΙΛ,ΝΤΕ ΜΑΡΚΕΝ
+  - BRUMBEAU,JEFF
+  - DE MARCKEN,GAIL
   language: el
   title: ΤΟ ΔΩΡΟ ΤΗΣ ΠΑΠΛΩΜΑΤΟΥΣ
   dewey: 808.899 ΜΠΡ
   entry_numbers:
   - '13679'
   editor: ΑΓΚΥΡΑ // ΑΘΗΝΑ
   edition_year: 2013
@@ -683056,15 +683079,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 13578
   authors:
-  - ΖΟΛΑ,ΕΜΙΛ
+  - ZOLA,ÉMILE,ÉDOUARD CHARLES ANTOINE
   language: el
   title: ΤΕΡΕΖΑ ΡΑΚΕΝ
   dewey: 843 ΖΟΛ
   entry_numbers:
   - '17088'
   translators:
   - ΡΟΔΟΠΟΥΛΟΥ,ΑΝΘΗ
@@ -684445,15 +684468,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13606
   authors:
-  - ΜΠΑΡΝΣ,ΤΖΟΥΛΙΑΝ
+  - BARNES,JULIAN
   language: el
   title: ΕΝΑ ΚΑΠΟΙΟ ΤΕΛΟΣ
   dewey: 823 ΜΠΑ
   entry_numbers:
   - '17111'
   translators:
   - ΣΚΑΣΣΗΣ,ΘΩΜΑΣ
@@ -688000,15 +688023,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13676
   authors:
-  - ΜΠΑΛΙΔΗ,ΘΕΟΔΩΡΟΥ
+  - ΜΠΑΛΙΔΗΣ,ΘΕΟΔΩΡΟΣ
   language: el
   title: ΤΟ ΕΓΚΛΗΜΑ ΤΗΣ ΑΥΤΟΔΙΚΙΑΣ ΕΙΣ ΤΗΝ ΠΕΡΙΦΕΡΕΙΑΝ ΤΟΥ ΠΡΩΤΟΔΙΚΕΙ
   subtitle: ΟΥ ΘΕΣ/ΝΙΚΗΣ
   dewey: 345.04 ΜΠΑ
   entry_numbers:
   - '17153'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
@@ -689157,15 +689180,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13699
   authors:
-  - ΖΩΤΙΑΔΟΥ,ΓΕΩΡΓΙΟΥ
+  - ΖΩΤΙΑΔΗΣ,ΓΕΩΡΓΙΟΣ
   language: el
   title: Η ΔΙ ΕΙΔΙΚΗΣ ΣΥΜΒΑΣΕΩΣ ΠΡΟΒΛΕΠΟΜΕΝΗ ΕΠΕΜΒΑΣΙΣ ΩΣ ΠΡΟΒΛΗΜΑ
   subtitle: ΔΙΕΘΝΟΥΣ ΝΟΜΙΜΟΤΗΤΟΣ
   dewey: 346 ΖΩΤ
   entry_numbers:
   - '17202'
   edition_year: 1965
@@ -698277,15 +698300,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13882
   authors:
-  - ΜΠΑΛΑΤΣΟΥΚΑ,ΣΩΤΗΡΙΟΥ
+  - ΜΠΑΛΑΤΣΟΥΚΑΣ,ΣΩΤΗΡΙΟΣ
   language: el
   title: ΟΙ ΑΓΙΟΙ ΚΑΙ ΤΟ ΦΥΣΙΚΟ ΠΕΡΙΒΑΛΛΟΝ
   dewey: 230 ΜΠΑ
   entry_numbers:
   - '17423'
   editor: ΜΥΓΔΟΝΙΑ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1996
@@ -701388,15 +701411,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13944
   authors:
-  - JAEGER,WERNER
+  - JAEGER,WERNER,WILHELM
   language: el
   title: ΠΑΙΔΕΙΑ ΤΟΜΟΣ Γ
   dewey: 378 JAE
   entry_numbers:
   - '17464'
   editor: None // ΑΘΗΝΑ
   edition_year: 1974
@@ -701588,15 +701611,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13948
   authors:
-  - ΜΠΟΥΣΙΑ,ΧΑΡΑΛΑΜΠΟΥΣ
+  - ΜΠΟΎΣΙΑΣ,ΧΑΡΆΛΑΜΠΟΣ,Μ.
   language: el
   title: ΠΑΝΑΓΙΑ Η ΡΟΒΕΛΙΣΤΑ
   dewey: 230 ΜΠΟ
   entry_numbers:
   - '17473'
   editor: None // ΑΘΗΝΑ
   pages: 53
@@ -701830,15 +701853,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13953
   authors:
-  - ΜΠΟΥΡΑΖΕΡΗ,ΝΙΚΟΛΑΟΥ
+  - ΜΠΟΥΡΑΖΕΡΗΣ,ΝΙΚΟΛΑΟΣ
   language: el
   title: ΙΗΣΟΥΣ ΧΡΙΣΤΟΣ Η ΠΡΟΣΔΟΚΙΑ ΤΩΝ ΕΘΝΩΝ
   dewey: 230 ΜΠΟ
   entry_numbers:
   - '17476'
   editor: ΚΑΛΑΜΟΣ // ΑΘΗΝΑ
   edition_year: 2000
@@ -706683,15 +706706,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14050
   authors:
-  - ΖΑΚΟΠΟΥΛΟΥ,ΠΑΝΑΓΙΩΤΟΥ
+  - ΖΑΚΟΠΟΥΛΟΣ,ΠΑΝΑΓΙΩΤΗΣ
   language: el
   title: ΤΑ ΕΘΝΙΚΑ ΚΛΗΡΟΔΟΤΗΜΑΤΑ ΚΑΙ ΑΙ ΠΡΟΣ ΑΥΤΑ ΥΠΟΧΡΕΩΣΕΙΣ ΤΗΣ ΠΟΛ
   subtitle: ΙΤΕΙΑΣ
   dewey: 658.153 ΖΑΚ
   entry_numbers:
   - '17563'
   editor: ΕΘΝΙΚΟΥ ΤΥΠΟΓΡΑΦΕΙΟΥ // ΑΘΗΝΑ
@@ -707133,15 +707156,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14059
   authors:
-  - ΖΑΚΟΠΟΥΛΟΥ,ΠΑΝΑΓΙΩΤΟΥ
+  - ΖΑΚΟΠΟΥΛΟΣ,ΠΑΝΑΓΙΩΤΗΣ
   language: el
   title: ΤΑ ΕΘΝΙΚΑ ΚΛΗΡΟΔΟΤΗΜΑΤΑ ΚΑΙ ΑΙ ΠΡΟΣ ΑΥΤΑ ΥΠΟΧΡΕΩΣΕΙΣ ΤΗΣ ΠΟΛ
   subtitle: ΙΤΕΙΑΣ
   dewey: 658.153 ΖΑΚ
   entry_numbers:
   - '17553'
   editor: ΕΘΝΙΚΟ ΤΥΠΟΓΡΑΦΕΙΟ // ΑΘΗΝΑ
@@ -707645,15 +707668,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 14069
   authors:
-  - ΖΕΡΖΕΛΙΔΗ,ΓΕΩΡΓΙΟΥ
+  - ΖΕΡΖΕΛΙΔΗΣ,ΓΕΩΡΓΙΟΣ,Ι.
   language: el
   title: ΤΟ ΚΑΛΑΝΤΟΝΕΡΟΝ
   dewey: 889.21 ΖΕΡ
   entry_numbers:
   - '17582'
   editor: None // ΑΘΗΝΑ
   edition_year: 1950
@@ -710941,15 +710964,17 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14135
   authors:
-  - ΜΠΕΛ,Χ-ΚΟΠΕΛΕΒ,Λ-ΦΟΡΜΒΕΓΚ,Χ
+  - BÖLL,HEINRICH
+  - KOPELEV,LEV,ZALMANOVICH (ZINOVYEVICH)
+  - VORMWEG,HEINRICH
   language: el
   title: ΑΝΤΙΚΟΜΜΟΥΝΙΣΜΟΣ ΣΕ ΑΝΑΤΟΛΗ ΚΑΙ ΔΥΣΗ
   dewey: 330 ΜΠΕ
   entry_numbers:
   - '12780'
   translators:
   - ΧΑΤΖΗ,ΚΑΤΕΡΙΝΑ
@@ -712314,15 +712339,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14162
   authors:
-  - ΖΕΡΜΠΙΝΗ,ΔΗΜΗΤΡΙΟΥ
+  - ΖΕΡΜΠΙΝΗΣ,ΔΗΜΗΤΡΙΟΣ
   language: el
   title: ΩΡΑΙΑΙ ΣΚΕΨΕΙΣ ΑΡΧΑΙΩΝ ΕΛΛΗΝΩΝ ΚΑΙ ΑΛΛΩΝ ΣΥΓΓΡΑΦΕΩΝ
   dewey: 101 ΖΕΡ
   entry_numbers: []
   editor: Η ΠΡΟΟΔΟΣ // ΑΘΗΝΑ
   edition_year: 1958
   pages: 430
@@ -715999,15 +716024,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14236
   authors:
-  - ΜΠΑΡΡΥ,ΜΠΡΟΥΝΟΝΙΑ
+  - BARRY,BRUNONIA
   language: el
   title: Η ΑΝΑΓΝΩΣΤΡΙΑ ΤΗΣ ΔΑΝΤΕΛΑΣ
   dewey: 810.11 ΜΠΑ
   entry_numbers:
   - '17707'
   translators:
   - ΜΟΙΡΑ,ΜΑΡΑ
@@ -717703,15 +717728,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14269
   authors:
-  - ΜΠΑΜΠΙΝΙΩΤΗΣ,Γ.
+  - ΜΠΑΜΠΙΝΙΩΤΗΣ,ΓΕΩΡΓΙΟΣ
   language: el
   title: ΤΟ ΓΛΩΣΣΙΚΟ ΖΗΤΗΜΑ
   subtitle: ΣΥΓΧΡΟΝΕΣ ΠΡΟΣΕΓΓΙΣΕΙΣ
   dewey: 489.3 ΜΠΑ
   entry_numbers:
   - '17724'
   editor: ΙΔΡ.ΒΟΥΛΗ ΤΩΝ ΕΛΛΗΝΩ // ΑΘΗΝΑ
@@ -723823,15 +723848,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14391
   authors:
-  - ΜΠΟΥΤΣΙΚΑ,ΑΝΔΡΕΑ
+  - ΜΠΟΥΤΣΙΚΑΣ,ΑΝΔΡΕΑΣ
   language: el
   title: ΠΑΝΑΓΙΑ ΣΟΥΜΕΛΑ
   subtitle: ΒΑΣΙΛΙΣΣΑ ΤΟΥ ΠΟΝΤΟΥ ΚΑΙ ΤΟΥ ΒΕΡΜΙΟΥ
   dewey: 230 ΜΠΟ
   entry_numbers:
   - '9330'
   editor: ΑΠΟΣΤΟΛΙΚΗΣ ΔΙΑΚΟΝΙΑ // ΑΘΗΝΑ
@@ -724818,15 +724843,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14412
   authors:
-  - ΜΠΕΡΑΤΗ,ΘΕΟΔΩΡΟΥ
+  - ΜΠΕΡΑΤΗΣ,ΘΕΟΔΩΡΟΣ
   language: el
   title: ΠΡΟΣΕΛΘΕΤΕ ΜΕΤΑ ΦΟΒΟΥ ΘΕΟΥ ΠΙΣΤΕΩΣ ΚΑΙ ΑΓΑΠΗΣ
   dewey: 230 ΜΠΕ
   entry_numbers:
   - '12833'
   editor: ΣΩΤΗΡ // ΑΘΗΝΑ
   edition_year: 2000
@@ -726539,15 +726564,16 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 14446
   authors:
-  - ΜΠΑΕΤΕΝ.ΛΙΒΕ-ΜΠΕΝΚΕ-ΚΟΥΝΤΣΛΕΡ,ΡΟΖΜΑΡΙ
+  - BAETEN,LIEVE
+  - KUNZLER-BEHNCKE,ROSEMARIE
   language: el
   title: ΑΛΛΟΣ ΓΙΑ ΤΟ ΝΗΠΙΑΓΩΓΕΙΟ
   dewey: 808.899 ΜΠΑ
   entry_numbers:
   - '17880'
   translators:
   - ΑΓΓΕΛΙΔΟΥ,ΜΑΡΙΑ
@@ -727102,15 +727128,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14457
   authors:
-  - ZAFON,RUIZ,CARLOS
+  - ZAFON,CARLOS,RUIZ
   language: el
   title: Η ΣΚΙΑ ΤΟΥ ΑΝΕΜΟΥ
   dewey: 860.11 ZAF
   entry_numbers:
   - '17883'
   translators:
   - ΡΟΥΦΟΥ,ΚΑΤΕΡΙΝΑ
@@ -734438,15 +734464,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14603
   authors:
-  - ΖΟΥΣΑΚ,ΜΑΡΚΟΥΣ
+  - ZUSAK,MARKUS
   language: el
   title: Η ΚΛΕΦΤΡΑ ΤΩΝ ΒΙΒΛΙΩΝ
   dewey: 810.11 ΖΟΥ
   entry_numbers:
   - '19203'
   editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
   edition_year: 2008
@@ -736900,15 +736926,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14653
   authors:
-  - ΖΑΝ,ΡΑΙΜΟΝ
+  - RAYMOND,JEAN
   language: el
   title: Η ΑΝΑΓΝΩΣΤΡΙΑ
   dewey: 843 ΖΑΝ
   entry_numbers:
   - '19503'
   translators:
   - ΣΑΡΑΦΕΙΔΟΥ,ΔΕΣΠΟΙΝΑ
@@ -737152,15 +737178,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14658
   authors:
-  - ΜΠΟΜΠΕΝ,ΚΡΙΣΤΙΑΝ
+  - BOBIN,CHRISTIAN
   language: el
   title: ΚΙΣΣΑ
   dewey: 843 ΜΠΟ
   entry_numbers:
   - '19500'
   translators:
   - ΣΑΡΑΦΕΙΔΟΥ,ΔΕΣΠΟΙΝΑ
@@ -737750,15 +737776,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14670
   authors:
-  - ΜΠΟΥΚΟΦΣΚΙ,ΤΣΑΡΛΣ
+  - BUKOWSKI,HENRY CHARLES
   language: el
   title: ΙΣΤΟΡΙΕΣ ΜΙΑΣ ΘΑΜΜΕΝΗΣ ΖΩΗΣ
   dewey: 810.11 ΜΠΟ
   entry_numbers:
   - '19530'
   translators:
   - ΦΡΥΔΑ,ΕΦΗ
@@ -739142,15 +739168,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14698
   authors:
-  - ΜΠΩΣΑΝ,ΚΛΩΝΤΙΝ
+  - BEAUSSANT,CLAUDINE
   language: el
   title: ΚΟΜΙΣΣΑ ΝΤΕ ΣΕΓΚΥΡ Η ΠΑΙΔΙΚΗ ΗΛΙΚΙΑ ΤΗΣ ΤΕΧΝΗΣ
   dewey: 920 ΜΠΩ
   entry_numbers:
   - '19495'
   translators:
   - ΜΙΚΟΓΛΟΥ,ΧΑΡΗΣ
@@ -739849,15 +739875,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14712
   authors:
-  - ΖΟΝΚΕ,ΤΙΕΡΥ
+  - JONQUET,THIERRY
   language: el
   title: ΜΥΓΑΛΗ Η ΔΗΛΗΤΗΡΙΩΔΗΣ ΑΡΑΧΝΗ
   dewey: 843 ΖΟΝ
   entry_numbers:
   - '19547'
   translators:
   - ΜΡΝΤΖΟΥ,ΜΑΡΙΝΑ
@@ -745467,15 +745493,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14826
   authors:
-  - ΜΠΕΡΓΚΜΑΝ,ΙΝΓΚΜΑΡ
+  - BERGMAN,INGMAR
   language: el
   title: Ο ΜΑΓΙΚΟΣ ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ
   dewey: 791.430 ΜΠΕ
   entry_numbers:
   - '19653'
   translators:
   - ΚΟΝΔΥΛΗΣ,ΓΡΗΓΟΡΗΣ
@@ -745617,15 +745643,16 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14829
   authors:
-  - ΜΠΑΡΝΕΤ,ΜΑΚ-ΤΖΟΡΙ,ΤΖΟΝ
+  - JORY,JOHN
+  - BARNETT,MAC
   language: el
   title: ΤΟ ΤΡΟΜΕΡΟ ΔΙΔΥΜΟ
   dewey: 808.899 ΜΠΑ
   entry_numbers:
   - '19656'
   translators:
   - ΚΟΛΥΔΑ,ΕΥΓΕΝΙΑ
@@ -747557,15 +747584,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14868
   authors:
-  - BACCALARIO,P.D
+  - BACCALARIO,PIERDOMENICO
   title: CENTURY. ΤΟ ΔΑΧΤΥΛΙΔΙ ΤΗΣ ΦΩΤΙΑΣ
   dewey: 808.899 BAC
   entry_numbers:
   - '19686'
   translators:
   - ΔΑΡΒΙΡΗ,ΘΕΟΔΩΡΑ
   editor: ΔΙΟΠΤΡΑ // ΑΘΗΝΑ
@@ -748703,15 +748730,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14891
   authors:
-  - ΜΠΡΟΝΤΕ,ΣΑΡΛΟΤ
+  - BRONTË,CHARLOTTE
   language: el
   title: ΤΖΕΙΝ ΕΙΡ
   dewey: 808.899 ΜΠΡ
   entry_numbers:
   - '19814'
   translators:
   - ΚΑΝΤΖΟΛΑ,ΒΕΑΤΡΙΚΗ
@@ -751895,15 +751922,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14955
   authors:
-  - ΜΠΕΓΚΕΧΟΛΝΤ,ΜΠΕΤΙ
+  - BOEGEHOLD,BETTY
   language: el
   title: Ο ΜΠΑΜΠΑΣ ΔΕΝ ΜΕΝΕΙ ΠΙΑ ΜΑΖΙ ΜΑΣ
   dewey: 808.899 ΜΠΕ
   entry_numbers:
   - '19924'
   translators:
   - ΒΡΑΝΑΣ,ΡΟΥΣΣΟΣ
@@ -752585,15 +752612,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14969
   authors:
-  - ΜΠΡΕΖΙΝΑ,ΤΟΜΑΣ
+  - BREZINA,THOMAS
   language: el
   title: ΠΟΙΟΣ ΜΠΟΡΕΙ ΝΑ ΣΩΣΕΙ ΤΟ ΧΑΜΕΝΟ ΘΗΣΑΥΡΟ
   dewey: 808.899 ΜΠΡ
   entry_numbers:
   - '19935'
   editor: ΕΛΛΗΝΙΚΑ ΓΡΑΜΜΑΤΑ // ΑΘΗΝΑ
   pages: 95
@@ -754726,15 +754753,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15011
   authors:
-  - ΜΠΛΙΞΕΝ,ΚΑΡΕΝ
+  - BLIXEN,KAREN
   language: el
   title: ΠΕΡΑ ΑΠΟ ΤΗΝ ΑΦΡΙΚΗ
   dewey: 839.81 ΜΠΛ
   entry_numbers:
   - '20006'
   translators:
   - ΦΡΥΔΑ,ΕΦΗ
@@ -755075,15 +755102,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15018
   authors:
-  - ΜΠΑΛΖΑΚ,ΟΝΟΡΕ
+  - BALZAC,HONORÉ DE
   language: el
   title: ΓΚΑΜΠΑΡΑ Η Η ΑΝΘΡΩΠΙΝΗ ΦΩΝΗ
   dewey: 843 ΜΠΑ
   entry_numbers:
   - '20008'
   translators:
   - ΝΕΟΦΥΤΙΔΗΣ,ΑΝΔΡΕΑΣ
@@ -756747,15 +756774,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15051
   authors:
-  - ΜΠΛΑΚ,ΜΠΕΝΤΖΑΜΙΝ
+  - BLACK,BENJAMIN
   language: el
   title: Ο ΛΕΜΟΥΡΙΟΣ
   dewey: 891.62 ΜΠΛ
   entry_numbers:
   - '20057'
   translators:
   - ΦΑΚΙΝΟΥ,ΜΑΡΙΑ
@@ -757204,15 +757231,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15060
   authors:
-  - ΖΑΤΕΛΛΗ,ΖΥΡΑΝΝΑ
+  - ΖΑΤΕΛΗ,ΖΥΡΑΝΝΑ
   language: el
   title: ΗΔΟΝΗ ΣΤΟΝ ΚΡΟΤΑΦΟ
   dewey: 889.21 ΖΑΤ
   entry_numbers:
   - '20044'
   editor: ΚΑΣΤΑΝΙΩΤΗΣ // ΑΘΗΝΑ
   edition_year: 2011
@@ -757713,15 +757740,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15070
   authors:
-  - ΜΠΕΝΙ,ΣΤΕΦΑΝΟ
+  - BENNI,STEFANO
   language: el
   title: ΚΩΜΙΚΟΙ ΤΡΟΜΑΓΜΕΝΟΙ ΜΑΧΗΤΕΣ
   dewey: 850.11 ΜΠΕ
   entry_numbers: []
   translators:
   - ΚΟΝΒΕΡΤΙΝΟ,ΤΟΤΑ
   editor: ΚΑΣΤΑΝΙΩΤΗΣ // ΑΘΗΝΑ
@@ -759897,15 +759924,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15114
   authors:
-  - ΒΛΑΧΟΣ,ΑΓΓΕΛΟΣ,ΣΤ,
+  - ΒΛΑΧΟΣ,ΑΓΓΕΛΟΣ,ΣΤ.
   language: el
   title: Ο ΚΥΡΙΟΣ ΑΛΚΙΒΙΑΔΗΣ
   dewey: 889.21 ΒΛΑ
   entry_numbers:
   - '20112'
   editor: ΤΟ ΒΗΜΑ // ΑΘΗΝΑ
   edition_year: 2008
@@ -760695,15 +760722,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15130
   authors:
-  - BURNIE,D.
+  - BURNIE,DAVID
   language: el
   title: Ο ΠΛΑΝΗΤΗΣ ΣΕ ΚΙΝΔΥΝΟ
   dewey: 363.7 BUR
   entry_numbers:
   - '19979'
   translators:
   - ΓΚΑΝΑ,ΑΓΓΕΛΙΚΗ
@@ -763277,15 +763304,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15182
   authors:
-  - BLYTON,ERID
+  - BLYTON,ENID
   language: el
   title: ΑΛΛΗ ΜΙΑ ΠΕΡΙΠΕΤΕΙΑ ΓΙΑ ΤΟΥΣ ΜΥΣΤΙΚΟΥΣ ΕΦΤΑ
   dewey: 808.899 BLY
   entry_numbers:
   - '20150'
   translators:
   - ΚΟΝΙΔΙΑΡΗ,ΕΛΛΗ
@@ -763482,15 +763509,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15186
   authors:
-  - BLYTON,ERID
+  - BLYTON,ENID
   language: el
   title: ΤΑ ΠΕΝΤΕ ΛΑΓΩΝΙΚΑ ΤΟ ΜΥΣΤΗΡΙΟ ΤΗΣ ΧΑΜΕΝΗΣ ΓΑΤΑΣ
   dewey: 808.899 BLY
   entry_numbers:
   - '20171'
   translators:
   - ΒΙΚΥΛΑΔΗ,
@@ -763843,15 +763870,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15193
   authors:
-  - BLYTON,ERID
+  - BLYTON,ENID
   language: el
   title: ΤΑ ΠΕΝΤΕ ΛΑΓΩΝΙΚΑ ΤΟ ΜΥΣΤΗΡΙΟ ΤΟΥ ΠΥΡΓΟΥ
   dewey: 808.899 BLY
   entry_numbers:
   - '20164'
   translators:
   - ΓΙΟΥΡΓΟΣ,ΚΩΣΤΑΣ
@@ -764410,15 +764437,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15204
   authors:
-  - BLYTON,ERID
+  - BLYTON,ENID
   language: el
   title: ΤΑ ΠΕΝΤΕ ΛΑΓΩΝΙΚΑ ΤΟ ΜΥΣΤΗΡΙΟ ΤΟΥ ΜΥΣΤΙΚΟΥ ΔΩΜΑΤΙΟΥ
   dewey: 808.899 BLY
   entry_numbers:
   - '20153'
   translators:
   - ΚΑΡΑΓΙΑΝΝΗ,ΒΑΛΙΑ
@@ -764462,15 +764489,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15205
   authors:
-  - BLYTON,ERID
+  - BLYTON,ENID
   language: el
   title: ΤΑ ΠΕΝΤΕ ΛΑΓΩΝΙΚΑ ΤΟ ΜΥΣΤΗΡΙΟ ΤΩΝ ΑΝΩΝΥΜΩΝ ΓΡΑΜΜΑΤΩΝ
   dewey: 808.899 BLY
   entry_numbers:
   - '20197'
   translators:
   - ΚΑΡΑΓΙΑΝΝΗ,ΒΑΛΙΑ
@@ -764616,15 +764643,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15208
   authors:
-  - BLYTON,ERID
+  - BLYTON,ENID
   language: el
   title: ΤΑ ΠΕΝΤΕ ΛΑΓΩΝΙΚΑ ΤΟ ΜΥΣΤΗΡΙΟ ΤΟΥ ΚΑΜΕΝΟΥ ΣΠΙΤΙΟΥ
   dewey: 808.899 BLY
   entry_numbers:
   - '20194'
   translators:
   - ΠΑΠΑΜΙΧΑΗΛ,ΚΛΑΙΡΗ
@@ -764668,15 +764695,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15209
   authors:
-  - BLYTON,ERID
+  - BLYTON,ENID
   language: el
   title: ΤΑ ΠΕΝΤΕ ΛΑΓΩΝΙΚΑ ΤΟ ΜΥΣΤΗΡΙΟ ΤΟΥ ΜΟΝΟΠΑΤΙΟΥ
   dewey: 808.899 BLY
   entry_numbers:
   - '20193'
   translators:
   - ΚΑΡΑΓΙΑΝΝΗ,ΒΑΛΙΑ
@@ -765117,15 +765144,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15218
   authors:
-  - ΜΠΛΑΙΤΟΝ,ΕΝΙΝΤ
+  - BLYTON,ENID
   language: el
   title: ΟΙ ΜΥΣΤΙΚΟΙ ΕΦΤΑ ΚΙ Ο ΣΤΟΙΧΕΙΩΜΕΝΟΣ ΠΥΡΓΟΣ
   dewey: 808.899 ΜΠΛ
   entry_numbers:
   - '20185'
   translators:
   - ΒΑΣΙΛΕΙΟΥ,ΑΛΕΞΑΝΔΡΑ
@@ -768743,15 +768770,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15290
   authors:
-  - ΜΠΟΣΗ,ΚΩΣΤΑ
+  - ΜΠΟΣΗΣ,ΚΩΣΤΑΣ
   language: el
   title: ΚΑΙ ΤΟ ΤΡΕΝΟ ΤΡΑΒΟΥΣΕ ΓΙΑ ΤΑ ΞΕΧΕΡΣΩΜΑΤΑ
   dewey: 889.21 ΜΠΟ
   entry_numbers:
   - '20227'
   editor: ΣΥΓΧΡΟΝΗ ΕΠΟΧΗ // ΑΘΗΝΑ
   edition_year: 1998
@@ -773911,15 +773938,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15392
   authors:
-  - ΜΠΟΥΡΑΟΥΙ,ΝΙΝΑ
+  - BOURAOUI,NINA
   language: el
   title: ΤΟ ΑΠΑΓΟΡΕΥΜΕΝΟ ΒΛΕΜΜΑ
   dewey: 843 ΜΠΟ
   entry_numbers:
   - '20346'
   translators:
   - ΣΙΔΕΡΗ,ΝΤΙΝΑ
@@ -774018,15 +774045,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15394
   authors:
-  - ΜΠΑΡΙΓΕ,ΕΛΙΖΑΜΠΕΤ
+  - BARILLE,ELISABETH
   language: el
   title: ΑΝΑΙΣ ΝΙΝ. ΤΟΣΟ ΓΥΜΝΗ ΠΙΣΩ ΑΠΟ ΤΗ ΜΑΣΚΑ ΤΗΣ
   dewey: 843 ΜΠΑ
   entry_numbers:
   - '20336'
   translators:
   - ΖΕΡΒΟΥ,ΡΕΓΓΙΝΑ
@@ -774600,15 +774627,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15405
   authors:
-  - ΜΠΡΑΙΑΝ,ΠΑΤΡΙΚ
+  - O'BRIAN,PATRICK
   language: el
   title: ΑΙΧΜΑΛΩΤΟΙ ΤΩΝ ΩΚΕΑΝΩΝ
   dewey: 843 ΜΠΡ
   entry_numbers:
   - '20337'
   translators:
   - ΣΠΑΝΔΩΝΗΣ,ΓΙΑΝΝΗΣ
@@ -775104,15 +775131,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15415
   authors:
-  - ΜΠΕΝΓΙΑΜΙΝ,ΒΑΛΤΕΡ
+  - BENJAMIN,WALTER, BENDIX SCHÖNFLIES
   language: el
   title: ΗΜΕΡΟΛΟΓΙΟ ΜΟΣΧΑΣ
   dewey: 830 ΜΠΕ
   entry_numbers:
   - '20409'
   translators:
   - ΒΑΙΚΟΥΣΗ,ΕΜΗ
@@ -775366,15 +775393,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15420
   authors:
-  - ΜΠΑΣΤΑ,ΕΥΣΤΑΘΙΟΥ
+  - ΜΠΑΣΤΑΣ,ΕΥΣΤΑΘΙΟΣ
   language: el
   title: ΗΤΑΝ ΖΕΣΤΟ ΤΟ ΣΠΙΤΙ
   dewey: 808.899 ΜΠΑ
   entry_numbers:
   - '12828'
   editor: Ο ΣΩΤΗΡ // ΑΘΗΝΑ
   edition_year: 1999
@@ -777630,15 +777657,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15466
   authors:
-  - ΜΠΟΥΤΟΣ ΒΑΣΙΛΗΣ
+  - ΜΠΟΥΤΟΣ,ΒΑΣΙΛΗΣ
   language: el
   title: ΝΥΧΤΕΡΙΝΗ ΑΠΟΣΤΑΣΙΑ
   dewey: 889.21 ΜΠΟ
   entry_numbers:
   - '20431'
   editor: ΚΑΣΤΑΝΙΩΤΗ // ΑΘΗΝΑ
   edition_year: 1988
@@ -778419,15 +778446,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15482
   authors:
-  - ΜΠΑΛΖΑΚ ΟΝΟΡΕ ΝΤΕ
+  - BALZAC,HONORÉ DE
   language: el
   title: ΕΝΑ ΠΑΘΟΣ ΣΤΗΝ ΕΡΗΜΟ
   dewey: 843 ΜΠΑ
   entry_numbers:
   - '16960'
   translators:
   - ΚΥΡΙΑΚΙΔΗΣ,ΑΧ.
@@ -782441,15 +782468,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15564
   authors:
-  - ΜΠΟΡΝΤΟΝΣ,ΠΑΛΟΜΑ
+  - BORDONS,PALOMA
   language: el
   title: Η ΔΕΣΠΟΙΝΙΔΑ ΠΕΠΟΤΑ
   dewey: 808.899 ΜΠΟ
   entry_numbers:
   - '19457'
   translators:
   - ΓΑΒΑΛΑΚΗ,ΤΖΕΝΗ
@@ -782927,15 +782954,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15574
   authors:
-  - BRONTE,CHARLOTTE
+  - BRONTË,CHARLOTTE
   language: el
   title: ΤΖΕΙΝ ΕΙΡ
   dewey: 823 BRO
   entry_numbers:
   - '20602'
   translators:
   - ΛΑΙΝΑ,ΚΛΑΙΡΗ
@@ -786460,15 +786487,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15644
   authors:
-  - ΜΠΩΣΑΝ,ΚΛΩΝΤΙΝ
+  - BEAUSSANT,CLAUDINE
   language: el
   title: Η ΚΟΜΙΣΣΑ ΝΤΕ ΣΕΓΚΥΡ ;Η Η ΠΑΙΔΙΚΗ ΗΛΙΚΙΑ ΤΗΣ ΤΕΧΝΗΣ
   entry_numbers:
   - '19495'
   translators:
   - ΜΙΚΟΓΛΟΥ,ΧΑΡΗΣ
   editor: ΖΑΧΑΡΟΠΟΥΛΟΣ // ΑΘΗΝΑ
@@ -789471,15 +789498,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15706
   authors:
-  - ΖΩΡΑΣ, ΓΕΩΡΓΙΟΣ
+  - ΖΩΡΑΣ,ΓΕΩΡΓΙΟΣ
   language: el
   title: Η ΞΕΝΙΤΕΙΑ ΕΝ ΤΗ ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΕΙ
   dewey: 880.08 ΖΩΡ
   entry_numbers:
   - '20911'
   editor: ΕΛΛΗΝΙΚΗ ΔΗΜΙΟΥΡΓΙΑ // ΑΘΗΝΑ
   edition_year: 1953
@@ -790284,15 +790311,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15723
   authors:
-  - BOWRA,C,Μ
+  - BOWRA,CECIL,MAURICE
   title: AΡΧΑΙΑ ΕΛΛΗΝΙΚΗ ΛΥΡΙΚΗ ΠΟΙΗΣΗ
   dewey: 884 BOW
   entry_numbers:
   - '20924'
   editor: ΜΟΡ.ΙΔΡ.ΕΘΝ.ΤΡΑΠΕΖΗΣ // ΑΘΗΝΑ
   edition_year: 2008
   pages: 403
@@ -790331,15 +790358,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15724
   authors:
-  - BOWRA,C.M.
+  - BOWRA,CECIL,MAURICE
   language: el
   title: ΑΡΧΑΙΑ ΕΛΛΗΝΙΚΗ ΛΥΡΙΚΗ ΠΟΙΗΣΗ
   dewey: 884 BOW
   entry_numbers:
   - '20924'
   editor: ΜΟΡ.ΙΔ.ΕΘΝ.ΤΡΑΠΕΖΗΣ // ΑΘΗΝΑ
   edition_year: 1999
@@ -794921,15 +794948,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15822
   authors:
-  - ΜΠΑΜΠΙΝΙΩΤΗΣ,Γ.
+  - ΜΠΑΜΠΙΝΙΩΤΗΣ,ΓΕΩΡΓΙΟΣ
   language: el
   title: ΛΕΞΙΚΟ ΤΩΝ ΠΑΡΑΓΩΓΩΝ ΚΑΙ ΣΥΝΘΕΤΩΝ ΤΗΣ ΝΕΑΣ ΕΛΛΗΝΙΚΗΣ
   dewey: 489.33 ΜΠΑ
   entry_numbers:
   - '21007'
   editor: ΤΟ ΒΗΜΑ // ΑΘΗΝΑ
   edition_year: 2016
@@ -795607,15 +795634,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15836
   authors:
-  - ΜΠΑΜΠΙΝΙΩΤΗΣ,Γ
+  - ΜΠΑΜΠΙΝΙΩΤΗΣ,ΓΕΩΡΓΙΟΣ
   language: el
   title: ΛΕΞΙΚΟ ΤΩΝ ΔΥΣΚΟΛΙΩΝ ΚΑΙ ΤΩΝ ΛΑΘΩΝ ΣΤΗ ΧΡΗΣΗ ΤΗΣ ΕΛΛΗΝΙΚΗΣ Γ
   subtitle: ΛΩΣΣΑΣ-ΓΛΩΣΣΙΚΟ ΣΥΜΒΟΥΛΟΣ
   dewey: 489.3 ΜΠΑ
   entry_numbers:
   - '21008'
   editor: ΤΟ ΒΗΜΑ // ΑΘΗΝΑ
@@ -804870,15 +804897,16 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 16019
   authors:
-  - BRUCE,ANDY-LANGDON,KEN
+  - BRUCE,ANDY
+  - LANGDON,KEN
   language: el
   title: ΣΥΜΒΟΥΛΟΣ ΜΑΝΑΤΖΕΡ
   subtitle: Ο ΣΤΡΑΤΗΓΙΚΟΣ ΣΧΕΔΙΑΣΜΟΣ
   dewey: 658.4 BRU
   entry_numbers:
   - '21293'
   translators:
@@ -814166,15 +814194,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 16204
   authors:
-  - ΖΑΚΟΠΟΥΛΟΣ,ΝΙΚΟΣ
+  - ΖΑΚΟΠΟΥΛΟΣ,ΝΙΚΟΣ,Ι.
   language: el
   title: ΩΡΑ ΠΛΗΝ ΔΥΟ
   dewey: 889.21 ΖΑΚ
   entry_numbers:
   - '21411'
   editor: ΦΙΛΙΠΠΟΤΗ // ΑΘΗΝΑ
   edition_year: 1986
@@ -831565,15 +831593,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 16557
   authors:
-  - ΖΑΦΡΕΙΡΗΣ,ΧΡΥΣΟΣΤΟΜΟΣ
+  - ΖΑΦΕΙΡΗΣ,ΧΡΥΣΟΣΤΟΜΟΣ
   language: el
   title: Ο ΙΕΡΟΜΑΡΤΥΡΑΣ-ΕΘΝΟΜΑΡΤΥΡΑΣ-ΟΠΛΑΡΧΗΓΟΣ ΠΑΠΑΣΠΥΡΟΣ ΖΑΦΕΙΡΗΣ
   dewey: 230 ΖΑΦ
   entry_numbers:
   - '21990'
   editor: ΠΕΛΑΣΓΟΣ // ΑΘΗΝΑ
   edition_year: 2018
@@ -834524,15 +834552,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 16619
   authors:
-  - ΜΠΟΥΜΗ-ΒΓΟΝΤΖΑ ΟΛΓΑ
+  - ΜΠΟΥΜΗ-ΒΓΟΝΤΖΑ,ΟΛΓΑ
   language: el
   title: ΠΑΛΑΙΑ ΔΙΑΘΗΚΗ
   dewey: 230 ΜΠΟ
   entry_numbers:
   - '22057'
   editor: ΛΥΧΝΙΑ // ΑΘΗΝΑ
   pages: 340
@@ -835291,15 +835319,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 16635
   authors:
-  - ΜΠΑΣΤΑ,ΕΥΣΤΑΘΙΟΥ
+  - ΜΠΑΣΤΑΣ,ΕΥΣΤΑΘΙΟΣ
   language: el
   title: ΟΙ ΤΡΕΙΣ ΦΙΛΟΙ
   dewey: 230 ΜΠΑ
   entry_numbers:
   - '22044'
   editor: Ο ΣΩΤΗΡ // ΑΘΗΝΑ
   edition_year: 1969
@@ -835387,15 +835415,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 16637
   authors:
-  - ΜΠΑΚΟΓΙΑΝΝΗ,ΒΑΣΙΛΕΙΟΣ
+  - ΜΠΑΚΟΓΙΑΝΝΗS,ΒΑΣΙΛΕΙΟΣ
   language: el
   title: ΧΑΙΡΕ ΚΕΧΑΡΙΤΩΜΕΝΗ
   dewey: 230 ΜΠΑ
   entry_numbers:
   - '22041'
   editor: ΘΑΒΩΡ // ΠΑΤΡΑ
   edition_year: 2005
@@ -835768,15 +835796,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 16645
   authors:
-  - ΜΠΕΛΙΑΕΦ,ΝΙΚΩΝΟΣ ΟΣΙΟΥ ΣΤΑΡΕΤΣ
+  - ΜΠΕΛΙΑΕΦ,ΟΣΙΟΣ ΣΤΑΡΕΤΣ ΝΙΚΩΝ
   language: el
   title: ΡΗΜΑΤΑ ΖΩΗΣ
   dewey: 230 ΜΠΕ
   entry_numbers:
   - '12790'
   editor: Ι.Μ.Μ.ΝΙΚΟΠΟΛΕΟΣ // ΠΡΕΒΕΖΑ
   edition_year: 2006
@@ -844703,15 +844731,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 16828
   authors:
-  - ΖΙΓΚΜΟΝΤ,ΜΟΡΙΤΣ
+  - ZSIGMOND,MORICZ
   language: el
   title: ΝΑ ΕΙΣΑΙ ΚΑΛΟΣ ΩΣ ΤΟ ΘΑΝΑΤΟ
   dewey: 832 ΜΟΡ
   entry_numbers:
   - '22186'
   editor: ΣΥΓΧΡΟΝΗ ΕΠΟΧΗ // ΑΘΗΝΑ
   edition_year: 1986
@@ -847413,15 +847441,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 16884
   authors:
-  - ΖΟΛΩΤΑΣ,ΞΕΝΟΦ.
+  - ΖΟΛΩΤΑΣ,ΞΕΝΟΦΩΝ
   language: el
   title: ΠΕΡΙΦΕΡΕΙΑΚΟΣ ΠΡΟΓΡΑΜΜΑΤΙΣΜΟΣ ΚΑΙ ΟΙΚΟΝΟΜΙΚΗ ΑΝΑΠΤΥΞΙΣ
   dewey: 338.9 ΖΟΛ
   entry_numbers:
   - '22230'
   editor: None // ΑΘΗΝΑ
   edition_year: 1961
@@ -850294,15 +850322,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 16943
   authors:
-  - ΜΠΑΝΤΑΛΟΥΚΑΣ,ΚΑΛΑΥΔΙΟΣ
+  - ΜΠΑΝΤΑΛΟΥΚΑΣ,ΚΛΑΥΔΙΟΣ
   language: el
   title: ΕΙΣΑΓΩΓΗ ΕΙΣ ΤΗΝ ΜΕΘΟΔΟΛΟΓΙΑΝ ΤΗΣ ΟΙΚΟΝΟΜΙΚΗΣ ΕΡΕΥΝΗΣ
   dewey: 330.1 ΜΠΑ
   entry_numbers:
   - '22280'
   editor: ΑΝ.ΒΙΟΜ.ΣΧΟΛΗ // ΠΕΙΡΑΙΑΣ
   edition_year: 1963
@@ -854437,15 +854465,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 17028
   authors:
-  - BEER-POITEVIN,G.
+  - BEER-POITEVIN,F.
   language: el
   title: ΜΕΓΑΛΗ ΙΑΤΡΙΚΗ ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ
   dewey: 615.5 BEE
   entry_numbers:
   - '22411'
   translators:
   - ΛΟΓΑΡΑ,Ε.
@@ -855789,15 +855817,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 17055
   authors:
-  - ΖΑΚΟΠΟΥΛΟΣ,Ν.Ι.
+  - ΖΑΚΟΠΟΥΛΟΣ,ΝΙΚΟΣ,Ι.
   language: el
   title: Η ΑΤΟΜΙΚΗ ΚΑΘΑΡΙΟΤΗΤΑ Η ΥΓΕΙΑ ΚΑΙ Η ΖΩΗ
   dewey: 610 ΖΑΚ
   entry_numbers:
   - '22454'
   editor: ΑΘΗΝΑΙΚΑΙ // ΑΘΗΝΑ
   edition_year: 1959
@@ -856189,15 +856217,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 17063
   authors:
-  - ΜΠΑΛΑΣ,Π.
+  - ΜΠΑΛΑΣ,ΠΑΝΑΓΙΏΤΗΣ
   language: el
   title: ΧΕΙΡΟΥΡΓΙΚΗ
   dewey: 617 ΜΠΑ
   entry_numbers:
   - '22464'
   editor: ΛΙΤΣΑΣ // ΑΘΗΝΑ
   edition_year: 1990
@@ -864094,15 +864122,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 17220
   authors:
-  - ΖΟΥΡΙΔΟΥ-ΛΙΑΠΗ ΜΑΡΙΑ
+  - ΖΟΥΡΙΔΟΥ-ΛΙΑΠΗ,ΜΑΡΙΑ
   language: el
   title: ΝΕΑ ΜΕΘΟΔΟΣ ΟΛΙΚΗΣ ΣΥΝΘΕΣΕΩΣ ΤΩΝ ΣΕΣΚΙΤΕΡΠΕΝΙΩΝ ΔΡΙΜΕΝΙΝΗΣ..
   dewey: 540 ΖΟΥ
   entry_numbers:
   - '22532'
   editor: None // ΑΘΗΝΑ
   edition_year: 1984
@@ -864992,15 +865020,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 17238
   authors:
-  - ΜΠΑΖΑΙΟΣ, ΚΩΣΤΑΣ
+  - ΜΠΑΖΑΙΟΣ,ΚΩΣΤΑΣ
   language: el
   title: ΟΙ ΤΡΟΦΕΣ ΠΟΥ ΧΑΡΙΖΟΥΝ ΥΓΕΙΑ
   subtitle: ΟΔΗΓΟΣ ΓΙΑ ΟΛΗ ΤΗΝ ΟΙΚΟΓΕΝΕΙΑ
   dewey: 613.7 ΜΠΑ
   entry_numbers:
   - '22490'
   editor: ΜΠΑΖΑΙΟΣ // ΑΘΗΝΑ
@@ -866933,15 +866961,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 17277
   authors:
-  - ΜΠΑΤΡΙΝΟΣ,Μ
+  - ΜΠΑΤΡΙΝΟΣ,ΜΕΝΕΛΑΟΣ
   language: el
   title: ΣΥΓΧΡΟΝΟΣ ΕΝΔΟΚΡΙΝΟΛΟΓΙΑ
   dewey: 615.5 ΜΠΑ
   entry_numbers:
   - '22670'
   editor: ΠΑΡΙΣΙΑΝΟΥ // ΑΘΗΝΑ
   edition_year: 1974
@@ -867454,15 +867482,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 17287
   authors:
-  - ΜΠΕΚ,ΠΕΤΕΡ
+  - BECK,PETER
   language: el
   title: ΜΙΣΘΟΦΟΡΟΙ ΤΟΥ ΧΡΗΜΑΤΟΣ
   dewey: 832 ΜΠΕ
   entry_numbers:
   - '22684'
   translators:
   - ΚΑΝΕΛΟΠΟΥΛΟΥ,ΔΕΣ.
@@ -868903,15 +868931,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 17315
   authors:
-  - ΜΠΙΡΜΑΝ,ΦΡΑΝΤΣΙΣΚΑ
+  - BIERMANN,FRANZISKA
   language: el
   title: Ο ΒΙΒΛΙΟΦΑΓΟΣ ΚΥΡΙΟΣ ΑΛΕΠΟΥΔΗΣ
   dewey: 808.899 ΜΠΙ
   entry_numbers:
   - '22695'
   editor: ΠΑΤΑΚΗΣ // ΑΘΗΝΑ
   edition_year: 2019
@@ -876077,15 +876105,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 17459
   authors:
-  - ΜΠΛΑΙΤΟΝ,ΕΝΙΝΤ
+  - BLYTON,ENID
   language: el
   title: ΣΩΣΤΕ ΤΟΝ ΣΚΑΜΠΕΡΜΥΣΤΙΚΟΙ ΕΦΤΑ
   dewey: 808.899 ΜΠΛ
   entry_numbers:
   - '22845'
   translators:
   - ΒΑΣΙΛΕΙΟΥ,ΑΛΕΞΑΝΔΡΑ
@@ -876129,15 +876157,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 17460
   authors:
-  - ΜΠΛΑΙΤΟΝ,ΕΝΙΝΤ
+  - BLYTON,ENID
   language: el
   title: ΟΙ ΜΥΣΤΙΚΟΙ ΕΦΤΑ ΣΕ ΜΙΑ ΔΙΑΣΚΕΔΑΣΤΙΚΗ ΠΕΡΙΠΕΤΕΙΑ
   dewey: 808.899 ΜΠΛ
   entry_numbers:
   - '22844'
   translators:
   - ΒΑΣΙΛΕΙΟΥ,ΑΛΕΞΑΝΔΡΑ
@@ -880295,15 +880323,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 17543
   authors:
-  - BRAUDEL,FERNARD
+  - BRAUDEL,FERNAND
   language: el
   title: ΜΕΣΟΓΕΙΟΣ
   dewey: 909.982 BRA
   entry_numbers:
   - '22941'
   editor: ΜΟΡΦ.ΙΔΡ.ΕΘΝ.ΤΡΑΠ. // ΑΘΗΝΑ
   edition_year: 1997
```

### Comparing `skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/editor_corrections.yml` & `skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/data/editor_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/entries.yml` & `skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/data/entries.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field04_corrections.yml` & `skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/data/field04_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field05_corrections.yml` & `skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/data/field05_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field06_corrections.yml` & `skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/data/field06_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field07_corrections.yml` & `skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/data/field07_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field08_corrections.yml` & `skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/data/field08_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field09_corrections.yml` & `skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/data/field09_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field16_corrections.yml` & `skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/data/field16_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field17_corrections.yml` & `skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/data/field17_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field18_corrections.yml` & `skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/data/field18_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field19_corrections.yml` & `skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/data/field19_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field30_corrections.yml` & `skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/data/field30_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/first_names.yml` & `skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/data/first_names.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/topic_replacements.yml` & `skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/data/topic_replacements.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/translator_corrections.yml` & `skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/data/translator_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/dbf_to_yaml.py` & `skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/dbf_to_yaml.py`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/field_extractors.py` & `skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/field_extractors.py`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/generate_reports.py` & `skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/generate_reports.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,24 +224,32 @@
 def report_weird_names(reports_directory: str):
     os.makedirs(os.path.join(reports_directory, "checks"), exist_ok=True)
     weird_translators: list[str] = []
     weird_authors: list[str] = []
     weird_curators: list[str] = []
     weird_donors: list[str] = []
     valid_name_re = re.compile(r"[A-ZΑ-Ω\-]+,[A-ZΑ-Ω\.]*\.?")
+    valid_name2_re = re.compile(r"[A-ZΑ-Ω\-]+,[A-ZΑ-Ω\.]*,[A-ZΑ-Ω\.]*\.?")
+    valid_name3_re = re.compile(r"[A-ZΑ-Ω\-]+,[A-ZΑ-Ω\.]*\.?@[A-ZΑ-Ω\-]+")
+    valid_name4_re = re.compile(r"[A-ZΑ-Ω\-]+,[A-ZΑ-Ω\.]*,[A-ZΑ-Ω\.]*\.?@[A-ZΑ-Ω\-]+")
     for entry in all_entries():
         translator = translator_from_a06(entry[6])
         if translator:
             translators = translator.split("!!")
             for translator in translators:
                 if not valid_name_re.fullmatch(translator):
                     weird_translators.append(translator)
         authors = authors_from_a01(entry[1])
         for author in authors:
-            if not valid_name_re.fullmatch(author):
+            if (
+                (not valid_name_re.fullmatch(author))
+                and (not valid_name2_re.fullmatch(author))
+                and (not valid_name3_re.fullmatch(author))
+                and (not valid_name4_re.fullmatch(author))
+            ):
                 weird_authors.append(author)
         curator = curator_from_a16(entry[16])
         if curator:
             curators = curator.split("!!")
             for curator in curators:
                 if not valid_name_re.fullmatch(curator):
                     weird_curators.append(curator)
```

### Comparing `skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/utilities.py` & `skoufas_dbf_reader-0.0.4rc172.post1/src/skoufas_dbf_reader/utilities.py`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc170.post1/tests/test_field_extractors.py` & `skoufas_dbf_reader-0.0.4rc172.post1/tests/test_field_extractors.py`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc170.post1/tests/test_reports.py` & `skoufas_dbf_reader-0.0.4rc172.post1/tests/test_reports.py`

 * *Files 4% similar despite different names*

```diff
@@ -208,24 +208,32 @@
 
 def test_report_weird_names(reports_directory: str):
     weird_translators: list[str] = []
     weird_authors: list[str] = []
     weird_curators: list[str] = []
     weird_donors: list[str] = []
     valid_name_re = re.compile(r"[A-ZΑ-Ω\-]+,[A-ZΑ-Ω\.]*\.?")
+    valid_name2_re = re.compile(r"[A-ZΑ-Ω\-]+,[A-ZΑ-Ω\.]*,[A-ZΑ-Ω\.]*\.?")
+    valid_name3_re = re.compile(r"[A-ZΑ-Ω\-]+,[A-ZΑ-Ω\.]*\.?@[A-ZΑ-Ω\-]+")
+    valid_name4_re = re.compile(r"[A-ZΑ-Ω\-]+,[A-ZΑ-Ω\.]*,[A-ZΑ-Ω\.]*\.?@[A-ZΑ-Ω\-]+")
     for entry in all_entries():
         translator = translator_from_a06(entry[6])
         if translator:
             translators = translator.split("!!")
             for translator in translators:
                 if not valid_name_re.fullmatch(translator):
                     weird_translators.append(translator)
         authors = authors_from_a01(entry[1])
         for author in authors:
-            if not valid_name_re.fullmatch(author):
+            if (
+                (not valid_name_re.fullmatch(author))
+                and (not valid_name2_re.fullmatch(author))
+                and (not valid_name3_re.fullmatch(author))
+                and (not valid_name4_re.fullmatch(author))
+            ):
                 weird_authors.append(author)
         curator = curator_from_a16(entry[16])
         if curator:
             curators = curator.split("!!")
             for curator in curators:
                 if not valid_name_re.fullmatch(curator):
                     weird_curators.append(curator)
```

### Comparing `skoufas_dbf_reader-0.0.4rc170.post1/tests/test_utilities.py` & `skoufas_dbf_reader-0.0.4rc172.post1/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc170.post1/PKG-INFO` & `skoufas_dbf_reader-0.0.4rc172.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skoufas-dbf-reader
-Version: 0.0.4rc170.post1
+Version: 0.0.4rc172.post1
 Summary: Library for reading legacy DBF file with library data
 Author-email: Claudio Bantaloukas <rockreamer@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

