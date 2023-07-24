# Comparing `tmp/document_merge_service-6.2.1.tar.gz` & `tmp/document_merge_service-6.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "document_merge_service-6.2.1.tar", max compression
+gzip compressed data, was "document_merge_service-6.2.2.tar", max compression
```

## Comparing `document_merge_service-6.2.1.tar` & `document_merge_service-6.2.2.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0    11511 2023-07-19 13:15:19.469111 document_merge_service-6.2.1/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2023-07-19 13:15:19.469111 document_merge_service-6.2.1/LICENSE
--rw-r--r--   0        0        0     2243 2023-07-19 13:15:19.469111 document_merge_service-6.2.1/README.md
--rw-r--r--   0        0        0        0 2023-07-19 13:15:19.469111 document_merge_service-6.2.1/document_merge_service/__init__.py
--rw-r--r--   0        0        0        0 2023-07-19 13:15:19.469111 document_merge_service-6.2.1/document_merge_service/api/__init__.py
--rw-r--r--   0        0        0      405 2023-07-19 13:15:19.469111 document_merge_service-6.2.1/document_merge_service/api/apps.py
--rw-r--r--   0        0        0     3159 2023-07-19 13:15:19.469111 document_merge_service-6.2.1/document_merge_service/api/authentication.py
--rw-r--r--   0        0        0      504 2023-07-19 13:15:19.469111 document_merge_service-6.2.1/document_merge_service/api/data/__init__.py
--rw-r--r--   0        0        0      559 2023-07-19 13:15:19.469111 document_merge_service-6.2.1/document_merge_service/api/data/black.png
--rw-r--r--   0        0        0     9125 2023-07-19 13:15:19.469111 document_merge_service-6.2.1/document_merge_service/api/data/docx-mailmerge-syntax.docx
--rw-r--r--   0        0        0    11489 2023-07-19 13:15:19.469111 document_merge_service-6.2.1/document_merge_service/api/data/docx-mailmerge.docx
--rw-r--r--   0        0        0     5735 2023-07-19 13:15:19.469111 document_merge_service-6.2.1/document_merge_service/api/data/docx-template-filters.docx
--rw-r--r--   0        0        0     6087 2023-07-19 13:15:19.469111 document_merge_service-6.2.1/document_merge_service/api/data/docx-template-loopcontrols.docx
--rw-r--r--   0        0        0     5952 2023-07-19 13:15:19.469111 document_merge_service-6.2.1/document_merge_service/api/data/docx-template-placeholdercheck.docx
--rw-r--r--   0        0        0     5091 2023-07-19 13:15:19.469111 document_merge_service-6.2.1/document_merge_service/api/data/docx-template-syntax.docx
--rw-r--r--   0        0        0     5490 2023-07-19 13:15:19.469111 document_merge_service-6.2.1/document_merge_service/api/data/docx-template.docx
--rw-r--r--   0        0        0  1127936 2023-07-19 13:15:19.473111 document_merge_service-6.2.1/document_merge_service/api/data/loadtest/1.doc
--rw-r--r--   0        0        0   175922 2023-07-19 13:15:19.473111 document_merge_service-6.2.1/document_merge_service/api/data/loadtest/2.docx
--rw-r--r--   0        0        0   163307 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/data/loadtest/3.docx
--rw-r--r--   0        0        0   141498 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/data/loadtest/4.docx
--rw-r--r--   0        0        0       22 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/data/test.txt
--rw-r--r--   0        0        0        5 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/data/xlsx-not-valid.xlsx
--rw-r--r--   0        0        0     6467 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/data/xlsx-structure.xlsx
--rw-r--r--   0        0        0     6432 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/data/xlsx-syntax.xlsx
--rw-r--r--   0        0        0     4750 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/data/xlsx-template.xlsx
--rw-r--r--   0        0        0     9772 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/engines.py
--rw-r--r--   0        0        0      389 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/factories.py
--rw-r--r--   0        0        0     2841 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/filters.py
--rw-r--r--   0        0        0     2546 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/jinja.py
--rw-r--r--   0        0        0        0 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/management/__init__.py
--rw-r--r--   0        0        0        0 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/management/commands/__init__.py
--rw-r--r--   0        0        0     1628 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/management/commands/clean_dangling_files.py
--rw-r--r--   0        0        0     1354 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/management/commands/upload_local_templates.py
--rw-r--r--   0        0        0     1248 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/migrations/0001_initial.py
--rw-r--r--   0        0        0      488 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/migrations/0002_template_group.py
--rw-r--r--   0        0        0      374 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/migrations/0003_template_meta.py
--rw-r--r--   0        0        0      145 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/migrations/0004_cleanup_files.py
--rw-r--r--   0        0        0     1004 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/migrations/0005_xlsx_template_engine.py
--rw-r--r--   0        0        0      327 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/migrations/0006_remove_template_group.py
--rw-r--r--   0        0        0        0 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/migrations/__init__.py
--rw-r--r--   0        0        0     1845 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/models.py
--rw-r--r--   0        0        0      231 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/pagination.py
--rw-r--r--   0        0        0      289 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/permissions.py
--rw-r--r--   0        0        0     4651 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/serializers.py
--rw-r--r--   0        0        0        0 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/tests/snapshots/__init__.py
--rw-r--r--   0        0        0    29399 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/tests/snapshots/snap_test_template.py
--rw-r--r--   0        0        0     2270 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/tests/test_authentication.py
--rw-r--r--   0        0        0      942 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/tests/test_clean_dangling_files.py
--rw-r--r--   0        0        0     1963 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/tests/test_excel.py
--rw-r--r--   0        0        0     1372 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/tests/test_filters.py
--rw-r--r--   0        0        0     1300 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/tests/test_jinja.py
--rw-r--r--   0        0        0      749 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/tests/test_pagination.py
--rw-r--r--   0        0        0    25634 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/tests/test_template.py
--rw-r--r--   0        0        0     3425 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/tests/test_unoconv.py
--rw-r--r--   0        0        0      597 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/tests/test_upload_local_templates.py
--rw-r--r--   0        0        0     6947 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/unoconv.py
--rw-r--r--   0        0        0      356 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/urls.py
--rw-r--r--   0        0        0     3570 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/views.py
--rw-r--r--   0        0        0     2909 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/conftest.py
--rw-r--r--   0        0        0        0 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/extensions/__init__.py
--rw-r--r--   0        0        0       52 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/extensions/permissions.py
--rw-r--r--   0        0        0       52 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/extensions/visibilities.py
--rw-r--r--   0        0        0      789 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/sentry.py
--rw-r--r--   0        0        0     8818 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/settings.py
--rw-r--r--   0        0        0        0 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/tests/__init__.py
--rw-r--r--   0        0        0      434 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/tests/test_sentry.py
--rw-r--r--   0        0        0      615 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/tests/test_settings.py
--rw-r--r--   0        0        0      225 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/urls.py
--rw-r--r--   0        0        0      412 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/wsgi.py
--rw-r--r--   0        0        0     3571 2023-07-19 13:15:19.481111 document_merge_service-6.2.1/pyproject.toml
--rw-r--r--   0        0        0     4191 1970-01-01 00:00:00.000000 document_merge_service-6.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11721 2023-07-24 09:43:27.598401 document_merge_service-6.2.2/CHANGELOG.md
+-rw-r--r--   0        0        0    35149 2023-07-24 09:43:27.598401 document_merge_service-6.2.2/LICENSE
+-rw-r--r--   0        0        0     2243 2023-07-24 09:43:27.598401 document_merge_service-6.2.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-24 09:43:27.598401 document_merge_service-6.2.2/document_merge_service/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-24 09:43:27.598401 document_merge_service-6.2.2/document_merge_service/api/__init__.py
+-rw-r--r--   0        0        0      405 2023-07-24 09:43:27.598401 document_merge_service-6.2.2/document_merge_service/api/apps.py
+-rw-r--r--   0        0        0     3159 2023-07-24 09:43:27.598401 document_merge_service-6.2.2/document_merge_service/api/authentication.py
+-rw-r--r--   0        0        0      504 2023-07-24 09:43:27.598401 document_merge_service-6.2.2/document_merge_service/api/data/__init__.py
+-rw-r--r--   0        0        0      559 2023-07-24 09:43:27.598401 document_merge_service-6.2.2/document_merge_service/api/data/black.png
+-rw-r--r--   0        0        0     9125 2023-07-24 09:43:27.598401 document_merge_service-6.2.2/document_merge_service/api/data/docx-mailmerge-syntax.docx
+-rw-r--r--   0        0        0    11489 2023-07-24 09:43:27.598401 document_merge_service-6.2.2/document_merge_service/api/data/docx-mailmerge.docx
+-rw-r--r--   0        0        0     5735 2023-07-24 09:43:27.598401 document_merge_service-6.2.2/document_merge_service/api/data/docx-template-filters.docx
+-rw-r--r--   0        0        0     6087 2023-07-24 09:43:27.598401 document_merge_service-6.2.2/document_merge_service/api/data/docx-template-loopcontrols.docx
+-rw-r--r--   0        0        0     5952 2023-07-24 09:43:27.598401 document_merge_service-6.2.2/document_merge_service/api/data/docx-template-placeholdercheck.docx
+-rw-r--r--   0        0        0     5091 2023-07-24 09:43:27.598401 document_merge_service-6.2.2/document_merge_service/api/data/docx-template-syntax.docx
+-rw-r--r--   0        0        0     5490 2023-07-24 09:43:27.598401 document_merge_service-6.2.2/document_merge_service/api/data/docx-template.docx
+-rw-r--r--   0        0        0  1127936 2023-07-24 09:43:27.602401 document_merge_service-6.2.2/document_merge_service/api/data/loadtest/1.doc
+-rw-r--r--   0        0        0   175922 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/data/loadtest/2.docx
+-rw-r--r--   0        0        0   163307 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/data/loadtest/3.docx
+-rw-r--r--   0        0        0   141498 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/data/loadtest/4.docx
+-rw-r--r--   0        0        0       22 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/data/test.txt
+-rw-r--r--   0        0        0        5 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/data/xlsx-not-valid.xlsx
+-rw-r--r--   0        0        0     6467 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/data/xlsx-structure.xlsx
+-rw-r--r--   0        0        0     6432 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/data/xlsx-syntax.xlsx
+-rw-r--r--   0        0        0     4750 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/data/xlsx-template.xlsx
+-rw-r--r--   0        0        0     9772 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/engines.py
+-rw-r--r--   0        0        0      389 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/factories.py
+-rw-r--r--   0        0        0     2841 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/filters.py
+-rw-r--r--   0        0        0     2546 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/jinja.py
+-rw-r--r--   0        0        0        0 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/management/commands/__init__.py
+-rw-r--r--   0        0        0     1628 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/management/commands/clean_dangling_files.py
+-rw-r--r--   0        0        0     1354 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/management/commands/upload_local_templates.py
+-rw-r--r--   0        0        0     1248 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/migrations/0001_initial.py
+-rw-r--r--   0        0        0      488 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/migrations/0002_template_group.py
+-rw-r--r--   0        0        0      374 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/migrations/0003_template_meta.py
+-rw-r--r--   0        0        0      145 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/migrations/0004_cleanup_files.py
+-rw-r--r--   0        0        0     1004 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/migrations/0005_xlsx_template_engine.py
+-rw-r--r--   0        0        0      932 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/migrations/0006_remove_template_group.py
+-rw-r--r--   0        0        0        0 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/migrations/__init__.py
+-rw-r--r--   0        0        0     1845 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/models.py
+-rw-r--r--   0        0        0      231 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/pagination.py
+-rw-r--r--   0        0        0      289 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/permissions.py
+-rw-r--r--   0        0        0     4651 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/serializers.py
+-rw-r--r--   0        0        0        0 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/tests/snapshots/__init__.py
+-rw-r--r--   0        0        0    29399 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/tests/snapshots/snap_test_template.py
+-rw-r--r--   0        0        0     2270 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/tests/test_authentication.py
+-rw-r--r--   0        0        0      942 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/tests/test_clean_dangling_files.py
+-rw-r--r--   0        0        0     1963 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/tests/test_excel.py
+-rw-r--r--   0        0        0     1372 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/tests/test_filters.py
+-rw-r--r--   0        0        0     1300 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/tests/test_jinja.py
+-rw-r--r--   0        0        0      749 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/tests/test_pagination.py
+-rw-r--r--   0        0        0    25634 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/tests/test_template.py
+-rw-r--r--   0        0        0     3425 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/tests/test_unoconv.py
+-rw-r--r--   0        0        0      597 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/tests/test_upload_local_templates.py
+-rw-r--r--   0        0        0     6947 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/unoconv.py
+-rw-r--r--   0        0        0      356 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/urls.py
+-rw-r--r--   0        0        0     3570 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/views.py
+-rw-r--r--   0        0        0     2909 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/conftest.py
+-rw-r--r--   0        0        0        0 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/extensions/__init__.py
+-rw-r--r--   0        0        0       52 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/extensions/permissions.py
+-rw-r--r--   0        0        0       52 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/extensions/visibilities.py
+-rw-r--r--   0        0        0      789 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/sentry.py
+-rw-r--r--   0        0        0     8818 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/settings.py
+-rw-r--r--   0        0        0        0 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/tests/__init__.py
+-rw-r--r--   0        0        0      434 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/tests/test_sentry.py
+-rw-r--r--   0        0        0      615 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/tests/test_settings.py
+-rw-r--r--   0        0        0      225 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/urls.py
+-rw-r--r--   0        0        0      412 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/wsgi.py
+-rw-r--r--   0        0        0     3571 2023-07-24 09:43:27.610401 document_merge_service-6.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4191 1970-01-01 00:00:00.000000 document_merge_service-6.2.2/PKG-INFO
```

### Comparing `document_merge_service-6.2.1/CHANGELOG.md` & `document_merge_service-6.2.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Changelog
 
+## 6.2.2 (24 July 2023)
+### Fix
+
+* **template:** Migrate group to meta property before removing ([`4480877`](https://github.com/adfinis/document-merge-service/commit/448087728f3103744b8245ff5400b63201352b19))
+
 ## 6.2.1 (19 July 2023)
 ### Fix
 
 * **dgap:** Add env variables to configure permissions and visibilities ([`67fc95a`](https://github.com/adfinis/document-merge-service/commit/67fc95a16f72e7afed37342972c6101c492d529a))
 * Storage generic file cleanup ([`0633fd2`](https://github.com/adfinis/document-merge-service/commit/0633fd20a7a11f00a8d7eb6aa903aa38520fe8b1))
 
 ## 6.2.0 (11 July 2023)
```

### Comparing `document_merge_service-6.2.1/LICENSE` & `document_merge_service-6.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.1/README.md` & `document_merge_service-6.2.2/README.md`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.1/document_merge_service/api/authentication.py` & `document_merge_service-6.2.2/document_merge_service/api/authentication.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.1/document_merge_service/api/data/black.png` & `document_merge_service-6.2.2/document_merge_service/api/data/black.png`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.1/document_merge_service/api/data/docx-mailmerge-syntax.docx` & `document_merge_service-6.2.2/document_merge_service/api/data/docx-mailmerge-syntax.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.1/document_merge_service/api/data/docx-mailmerge.docx` & `document_merge_service-6.2.2/document_merge_service/api/data/docx-mailmerge.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.1/document_merge_service/api/data/docx-template-filters.docx` & `document_merge_service-6.2.2/document_merge_service/api/data/docx-template-filters.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.1/document_merge_service/api/data/docx-template-loopcontrols.docx` & `document_merge_service-6.2.2/document_merge_service/api/data/docx-template-loopcontrols.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.1/document_merge_service/api/data/docx-template-placeholdercheck.docx` & `document_merge_service-6.2.2/document_merge_service/api/data/docx-template-placeholdercheck.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.1/document_merge_service/api/data/docx-template-syntax.docx` & `document_merge_service-6.2.2/document_merge_service/api/data/docx-template-syntax.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.1/document_merge_service/api/data/docx-template.docx` & `document_merge_service-6.2.2/document_merge_service/api/data/docx-template.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.1/document_merge_service/api/data/loadtest/1.doc` & `document_merge_service-6.2.2/document_merge_service/api/data/loadtest/1.doc`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.1/document_merge_service/api/data/loadtest/2.docx` & `document_merge_service-6.2.2/document_merge_service/api/data/loadtest/2.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.1/document_merge_service/api/data/loadtest/3.docx` & `document_merge_service-6.2.2/document_merge_service/api/data/loadtest/3.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.1/document_merge_service/api/data/loadtest/4.docx` & `document_merge_service-6.2.2/document_merge_service/api/data/loadtest/4.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.1/document_merge_service/api/data/xlsx-structure.xlsx` & `document_merge_service-6.2.2/document_merge_service/api/data/xlsx-structure.xlsx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.1/document_merge_service/api/data/xlsx-syntax.xlsx` & `document_merge_service-6.2.2/document_merge_service/api/data/xlsx-syntax.xlsx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.1/document_merge_service/api/data/xlsx-template.xlsx` & `document_merge_service-6.2.2/document_merge_service/api/data/xlsx-template.xlsx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.1/document_merge_service/api/engines.py` & `document_merge_service-6.2.2/document_merge_service/api/engines.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.1/document_merge_service/api/filters.py` & `document_merge_service-6.2.2/document_merge_service/api/filters.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.1/document_merge_service/api/jinja.py` & `document_merge_service-6.2.2/document_merge_service/api/jinja.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.1/document_merge_service/api/management/commands/clean_dangling_files.py` & `document_merge_service-6.2.2/document_merge_service/api/management/commands/clean_dangling_files.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.1/document_merge_service/api/management/commands/upload_local_templates.py` & `document_merge_service-6.2.2/document_merge_service/api/management/commands/upload_local_templates.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.1/document_merge_service/api/migrations/0001_initial.py` & `document_merge_service-6.2.2/document_merge_service/api/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.1/document_merge_service/api/migrations/0005_xlsx_template_engine.py` & `document_merge_service-6.2.2/document_merge_service/api/migrations/0005_xlsx_template_engine.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.1/document_merge_service/api/models.py` & `document_merge_service-6.2.2/document_merge_service/api/models.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.1/document_merge_service/api/serializers.py` & `document_merge_service-6.2.2/document_merge_service/api/serializers.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.1/document_merge_service/api/tests/snapshots/snap_test_template.py` & `document_merge_service-6.2.2/document_merge_service/api/tests/snapshots/snap_test_template.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.1/document_merge_service/api/tests/test_authentication.py` & `document_merge_service-6.2.2/document_merge_service/api/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.1/document_merge_service/api/tests/test_clean_dangling_files.py` & `document_merge_service-6.2.2/document_merge_service/api/tests/test_clean_dangling_files.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.1/document_merge_service/api/tests/test_excel.py` & `document_merge_service-6.2.2/document_merge_service/api/tests/test_excel.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.1/document_merge_service/api/tests/test_filters.py` & `document_merge_service-6.2.2/document_merge_service/api/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.1/document_merge_service/api/tests/test_jinja.py` & `document_merge_service-6.2.2/document_merge_service/api/tests/test_jinja.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.1/document_merge_service/api/tests/test_pagination.py` & `document_merge_service-6.2.2/document_merge_service/api/tests/test_pagination.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.1/document_merge_service/api/tests/test_template.py` & `document_merge_service-6.2.2/document_merge_service/api/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.1/document_merge_service/api/tests/test_unoconv.py` & `document_merge_service-6.2.2/document_merge_service/api/tests/test_unoconv.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.1/document_merge_service/api/tests/test_upload_local_templates.py` & `document_merge_service-6.2.2/document_merge_service/api/tests/test_upload_local_templates.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.1/document_merge_service/api/unoconv.py` & `document_merge_service-6.2.2/document_merge_service/api/unoconv.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.1/document_merge_service/api/views.py` & `document_merge_service-6.2.2/document_merge_service/api/views.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.1/document_merge_service/conftest.py` & `document_merge_service-6.2.2/document_merge_service/conftest.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.1/document_merge_service/sentry.py` & `document_merge_service-6.2.2/document_merge_service/sentry.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.1/document_merge_service/settings.py` & `document_merge_service-6.2.2/document_merge_service/settings.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.1/document_merge_service/tests/test_settings.py` & `document_merge_service-6.2.2/document_merge_service/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.1/pyproject.toml` & `document_merge_service-6.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "document-merge-service"
-version = "6.2.1"
+version = "6.2.2"
 description = "Merge Document Template Service"
 license = "GPL-3.0-or-later"
 authors = ["Adfinis AG <info@adfinis.com>"]
 homepage = "https://github.com/adfinis/document-merge-service"
 repository = "https://github.com/adfinis/document-merge-service"
 documentation = "https://github.com/adfinis/document-merge-service/blob/main/README.md"
 readme = "README.md"
@@ -63,18 +63,18 @@
 pytest-env = "0.8.2"
 pytest-factoryboy = "2.5.1"
 pytest-mock = "3.11.1"
 pytest-randomly = "3.13.0"
 python-semantic-release = "7.34.6"
 requests-mock = "1.11.0"
 snapshottest = "0.6.0"
-types-python-dateutil = "2.8.19.13"
-types-requests = "2.31.0.1"
-types-setuptools = "68.0.0.2"
-types-toml = "0.10.8.6"
+types-python-dateutil = "2.8.19.14"
+types-requests = "2.31.0.2"
+types-setuptools = "68.0.0.3"
+types-toml = "0.10.8.7"
 
 [tool.poetry.extras]
 mysql = ["mysqlclient"]
 pgsql = ["psycopg2-binary"]
 databases = ["mysqlclient", "psycopg2-binary"]
 
 [build-system]
```

### Comparing `document_merge_service-6.2.1/PKG-INFO` & `document_merge_service-6.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: document-merge-service
-Version: 6.2.1
+Version: 6.2.2
 Summary: Merge Document Template Service
 Home-page: https://github.com/adfinis/document-merge-service
 License: GPL-3.0-or-later
 Author: Adfinis AG
 Author-email: info@adfinis.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
```

