# Comparing `tmp/ckanext-usmetadata-0.3.1.tar.gz` & `tmp/ckanext-usmetadata-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-usmetadata-0.3.1.tar", last modified: Thu Jul  6 18:12:39 2023, max compression
+gzip compressed data, was "ckanext-usmetadata-0.3.2.tar", last modified: Mon Jul 24 17:08:03 2023, max compression
```

## Comparing `ckanext-usmetadata-0.3.1.tar` & `ckanext-usmetadata-0.3.2.tar`

### file list

```diff
@@ -1,70 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:12:39.280271 ckanext-usmetadata-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-06 18:12:39.280271 ckanext-usmetadata-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:12:39.276271 ckanext-usmetadata-0.3.1/ckanext/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:12:39.276271 ckanext-usmetadata-0.3.1/ckanext/usmetadata/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/ckanext/usmetadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27535 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/ckanext/usmetadata/blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/ckanext/usmetadata/db_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:12:39.276271 ckanext-usmetadata-0.3.1/ckanext/usmetadata/fanstatic/
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/ckanext/usmetadata/fanstatic/add_subagency.js
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/ckanext/usmetadata/fanstatic/dataset_edit_form.js
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/ckanext/usmetadata/fanstatic/dataset_url.js
--rw-r--r--   0 runner    (1001) docker     (123)    13046 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/ckanext/usmetadata/fanstatic/redactions.js
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/ckanext/usmetadata/fanstatic/resource_form.css
--rw-r--r--   0 runner    (1001) docker     (123)    10080 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/ckanext/usmetadata/fanstatic/resource_form.js
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/ckanext/usmetadata/fanstatic/webassets.yml
--rw-r--r--   0 runner    (1001) docker     (123)    17613 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/ckanext/usmetadata/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    75906 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/ckanext/usmetadata/media_types.json
--rw-r--r--   0 runner    (1001) docker     (123)    18184 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/ckanext/usmetadata/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:12:39.276271 ckanext-usmetadata-0.3.1/ckanext/usmetadata/public/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:12:39.272271 ckanext-usmetadata-0.3.1/ckanext/usmetadata/public/base/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:12:39.276271 ckanext-usmetadata-0.3.1/ckanext/usmetadata/public/base/images/
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/ckanext/usmetadata/public/base/images/inventory-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    18236 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/ckanext/usmetadata/public/redacted_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    71431 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/ckanext/usmetadata/public/redaction_clear.png
--rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/ckanext/usmetadata/resource_formats.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:12:39.276271 ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/footer.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:12:39.276271 ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/organization/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/organization/activity_stream.html
--rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/organization/bulk_process.html
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/organization/member_new.html
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/organization/read_base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:12:39.276271 ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/package/
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/package/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/package/read.html
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/package/read_base.html
--rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/package/resource_read.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:12:39.280271 ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/package/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/package/snippets/expanded_common_core_fields.html
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/package/snippets/info.html
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/package/snippets/metadata_info.html
--rw-r--r--   0 runner    (1001) docker     (123)     8483 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/package/snippets/package_basic_fields.html
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/package/snippets/package_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/package/snippets/package_metadata_fields.html
--rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/package/snippets/required_common_core_fields.html
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/package/snippets/required_if_applicable_common_core_fields.html
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/package/snippets/resource_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/package/snippets/resource_item.html
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/package/snippets/resources.html
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/package/snippets/stages.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:12:39.280271 ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/snippets/activity_item.html
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/snippets/license.html
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/snippets/organization.html
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/snippets/package_item.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:12:39.280271 ckanext-usmetadata-0.3.1/ckanext_usmetadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-06 18:12:39.000000 ckanext-usmetadata-0.3.1/ckanext_usmetadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-07-06 18:12:39.000000 ckanext-usmetadata-0.3.1/ckanext_usmetadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 18:12:39.000000 ckanext-usmetadata-0.3.1/ckanext_usmetadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-06 18:12:39.000000 ckanext-usmetadata-0.3.1/ckanext_usmetadata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-06 18:12:39.000000 ckanext-usmetadata-0.3.1/ckanext_usmetadata.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 18:12:39.000000 ckanext-usmetadata-0.3.1/ckanext_usmetadata.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 18:12:39.000000 ckanext-usmetadata-0.3.1/ckanext_usmetadata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-06 18:12:39.280271 ckanext-usmetadata-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-06 18:12:38.000000 ckanext-usmetadata-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:08:03.294243 ckanext-usmetadata-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-24 17:08:02.000000 ckanext-usmetadata-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-24 17:08:03.294243 ckanext-usmetadata-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-24 17:08:02.000000 ckanext-usmetadata-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:08:03.290243 ckanext-usmetadata-0.3.2/ckanext/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-24 17:08:02.000000 ckanext-usmetadata-0.3.2/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:08:03.290243 ckanext-usmetadata-0.3.2/ckanext/usmetadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-24 17:08:02.000000 ckanext-usmetadata-0.3.2/ckanext/usmetadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27535 2023-07-24 17:08:02.000000 ckanext-usmetadata-0.3.2/ckanext/usmetadata/blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-24 17:08:02.000000 ckanext-usmetadata-0.3.2/ckanext/usmetadata/db_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:08:03.290243 ckanext-usmetadata-0.3.2/ckanext/usmetadata/fanstatic/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-24 17:08:02.000000 ckanext-usmetadata-0.3.2/ckanext/usmetadata/fanstatic/add_subagency.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-07-24 17:08:02.000000 ckanext-usmetadata-0.3.2/ckanext/usmetadata/fanstatic/dataset_edit_form.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-24 17:08:02.000000 ckanext-usmetadata-0.3.2/ckanext/usmetadata/fanstatic/dataset_url.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13046 2023-07-24 17:08:02.000000 ckanext-usmetadata-0.3.2/ckanext/usmetadata/fanstatic/redactions.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-24 17:08:02.000000 ckanext-usmetadata-0.3.2/ckanext/usmetadata/fanstatic/resource_form.css
+-rw-r--r--   0 runner    (1001) docker     (123)    10080 2023-07-24 17:08:02.000000 ckanext-usmetadata-0.3.2/ckanext/usmetadata/fanstatic/resource_form.js
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-24 17:08:02.000000 ckanext-usmetadata-0.3.2/ckanext/usmetadata/fanstatic/webassets.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    17613 2023-07-24 17:08:02.000000 ckanext-usmetadata-0.3.2/ckanext/usmetadata/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75906 2023-07-24 17:08:02.000000 ckanext-usmetadata-0.3.2/ckanext/usmetadata/media_types.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18184 2023-07-24 17:08:02.000000 ckanext-usmetadata-0.3.2/ckanext/usmetadata/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:08:03.290243 ckanext-usmetadata-0.3.2/ckanext/usmetadata/public/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:08:03.282243 ckanext-usmetadata-0.3.2/ckanext/usmetadata/public/base/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:08:03.290243 ckanext-usmetadata-0.3.2/ckanext/usmetadata/public/base/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-07-24 17:08:02.000000 ckanext-usmetadata-0.3.2/ckanext/usmetadata/public/base/images/inventory-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18236 2023-07-24 17:08:02.000000 ckanext-usmetadata-0.3.2/ckanext/usmetadata/public/redacted_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    71431 2023-07-24 17:08:02.000000 ckanext-usmetadata-0.3.2/ckanext/usmetadata/public/redaction_clear.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-07-24 17:08:02.000000 ckanext-usmetadata-0.3.2/ckanext/usmetadata/resource_formats.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:08:03.290243 ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-24 17:08:02.000000 ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-24 17:08:02.000000 ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/footer.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:08:03.290243 ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/organization/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-24 17:08:02.000000 ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/organization/activity_stream.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-24 17:08:02.000000 ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/organization/member_new.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-24 17:08:02.000000 ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/organization/read_base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:08:03.290243 ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/package/
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-24 17:08:02.000000 ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/package/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-24 17:08:02.000000 ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/package/read.html
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-24 17:08:02.000000 ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/package/read_base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-07-24 17:08:02.000000 ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/package/resource_read.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:08:03.294243 ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/package/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-07-24 17:08:02.000000 ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/package/snippets/expanded_common_core_fields.html
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-24 17:08:02.000000 ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/package/snippets/info.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-24 17:08:02.000000 ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/package/snippets/metadata_info.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8483 2023-07-24 17:08:02.000000 ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/package/snippets/package_basic_fields.html
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-24 17:08:02.000000 ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/package/snippets/package_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-24 17:08:02.000000 ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/package/snippets/package_metadata_fields.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-07-24 17:08:02.000000 ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/package/snippets/required_common_core_fields.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-24 17:08:02.000000 ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/package/snippets/required_if_applicable_common_core_fields.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-07-24 17:08:02.000000 ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/package/snippets/resource_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-24 17:08:02.000000 ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/package/snippets/resource_item.html
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-24 17:08:02.000000 ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/package/snippets/resources.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-24 17:08:02.000000 ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/package/snippets/stages.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:08:03.294243 ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-24 17:08:02.000000 ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/snippets/activity_item.html
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-24 17:08:02.000000 ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/snippets/license.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-24 17:08:02.000000 ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/snippets/organization.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-07-24 17:08:02.000000 ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/snippets/package_item.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:08:03.294243 ckanext-usmetadata-0.3.2/ckanext_usmetadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-24 17:08:03.000000 ckanext-usmetadata-0.3.2/ckanext_usmetadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-07-24 17:08:03.000000 ckanext-usmetadata-0.3.2/ckanext_usmetadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 17:08:03.000000 ckanext-usmetadata-0.3.2/ckanext_usmetadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-24 17:08:03.000000 ckanext-usmetadata-0.3.2/ckanext_usmetadata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-24 17:08:03.000000 ckanext-usmetadata-0.3.2/ckanext_usmetadata.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 17:08:03.000000 ckanext-usmetadata-0.3.2/ckanext_usmetadata.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-24 17:08:03.000000 ckanext-usmetadata-0.3.2/ckanext_usmetadata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:08:02.000000 ckanext-usmetadata-0.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-24 17:08:03.294243 ckanext-usmetadata-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-24 17:08:02.000000 ckanext-usmetadata-0.3.2/setup.py
```

### Comparing `ckanext-usmetadata-0.3.1/PKG-INFO` & `ckanext-usmetadata-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-usmetadata
-Version: 0.3.1
+Version: 0.3.2
 Summary: US Metadata Plugin for CKAN
 Home-page: https://github.com/GSA/ckanext-usmetadata
 Author: Data.gov
 Author-email: datagovhelp@gsa.gov
 License: Public Domain
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ckanext-usmetadata-0.3.1/README.md` & `ckanext-usmetadata-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.3.1/ckanext/usmetadata/blueprint.py` & `ckanext-usmetadata-0.3.2/ckanext/usmetadata/blueprint.py`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.3.1/ckanext/usmetadata/db_utils.py` & `ckanext-usmetadata-0.3.2/ckanext/usmetadata/db_utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.3.1/ckanext/usmetadata/fanstatic/dataset_edit_form.js` & `ckanext-usmetadata-0.3.2/ckanext/usmetadata/fanstatic/dataset_edit_form.js`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.3.1/ckanext/usmetadata/fanstatic/dataset_url.js` & `ckanext-usmetadata-0.3.2/ckanext/usmetadata/fanstatic/dataset_url.js`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.3.1/ckanext/usmetadata/fanstatic/redactions.js` & `ckanext-usmetadata-0.3.2/ckanext/usmetadata/fanstatic/redactions.js`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.3.1/ckanext/usmetadata/fanstatic/resource_form.css` & `ckanext-usmetadata-0.3.2/ckanext/usmetadata/fanstatic/resource_form.css`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.3.1/ckanext/usmetadata/fanstatic/resource_form.js` & `ckanext-usmetadata-0.3.2/ckanext/usmetadata/fanstatic/resource_form.js`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.3.1/ckanext/usmetadata/helper.py` & `ckanext-usmetadata-0.3.2/ckanext/usmetadata/helper.py`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.3.1/ckanext/usmetadata/media_types.json` & `ckanext-usmetadata-0.3.2/ckanext/usmetadata/media_types.json`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.3.1/ckanext/usmetadata/plugin.py` & `ckanext-usmetadata-0.3.2/ckanext/usmetadata/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.3.1/ckanext/usmetadata/public/base/images/inventory-logo.png` & `ckanext-usmetadata-0.3.2/ckanext/usmetadata/public/base/images/inventory-logo.png`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.3.1/ckanext/usmetadata/public/redacted_icon.png` & `ckanext-usmetadata-0.3.2/ckanext/usmetadata/public/redacted_icon.png`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.3.1/ckanext/usmetadata/public/redaction_clear.png` & `ckanext-usmetadata-0.3.2/ckanext/usmetadata/public/redaction_clear.png`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.3.1/ckanext/usmetadata/resource_formats.json` & `ckanext-usmetadata-0.3.2/ckanext/usmetadata/resource_formats.json`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/footer.html` & `ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/footer.html`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/organization/member_new.html` & `ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/organization/member_new.html`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/organization/read_base.html` & `ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/organization/read_base.html`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/package/base.html` & `ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/package/base.html`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/package/read.html` & `ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/package/read.html`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/package/resource_read.html` & `ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/package/resource_read.html`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/package/snippets/expanded_common_core_fields.html` & `ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/package/snippets/expanded_common_core_fields.html`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/package/snippets/info.html` & `ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/package/snippets/info.html`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/package/snippets/metadata_info.html` & `ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/package/snippets/metadata_info.html`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/package/snippets/package_basic_fields.html` & `ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/package/snippets/package_basic_fields.html`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/package/snippets/package_metadata_fields.html` & `ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/package/snippets/package_metadata_fields.html`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/package/snippets/required_common_core_fields.html` & `ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/package/snippets/required_common_core_fields.html`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/package/snippets/required_if_applicable_common_core_fields.html` & `ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/package/snippets/required_if_applicable_common_core_fields.html`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/package/snippets/resource_form.html` & `ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/package/snippets/resource_form.html`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/package/snippets/resource_item.html` & `ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/package/snippets/resource_item.html`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/package/snippets/resources.html` & `ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/package/snippets/resources.html`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/package/snippets/stages.html` & `ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/package/snippets/stages.html`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/snippets/organization.html` & `ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/snippets/organization.html`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.3.1/ckanext/usmetadata/templates/snippets/package_item.html` & `ckanext-usmetadata-0.3.2/ckanext/usmetadata/templates/snippets/package_item.html`

 * *Files identical despite different names*

### Comparing `ckanext-usmetadata-0.3.1/ckanext_usmetadata.egg-info/PKG-INFO` & `ckanext-usmetadata-0.3.2/ckanext_usmetadata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-usmetadata
-Version: 0.3.1
+Version: 0.3.2
 Summary: US Metadata Plugin for CKAN
 Home-page: https://github.com/GSA/ckanext-usmetadata
 Author: Data.gov
 Author-email: datagovhelp@gsa.gov
 License: Public Domain
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ckanext-usmetadata-0.3.1/ckanext_usmetadata.egg-info/SOURCES.txt` & `ckanext-usmetadata-0.3.2/ckanext_usmetadata.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 ckanext/usmetadata/fanstatic/webassets.yml
 ckanext/usmetadata/public/redacted_icon.png
 ckanext/usmetadata/public/redaction_clear.png
 ckanext/usmetadata/public/base/images/inventory-logo.png
 ckanext/usmetadata/templates/base.html
 ckanext/usmetadata/templates/footer.html
 ckanext/usmetadata/templates/organization/activity_stream.html
-ckanext/usmetadata/templates/organization/bulk_process.html
 ckanext/usmetadata/templates/organization/member_new.html
 ckanext/usmetadata/templates/organization/read_base.html
 ckanext/usmetadata/templates/package/base.html
 ckanext/usmetadata/templates/package/read.html
 ckanext/usmetadata/templates/package/read_base.html
 ckanext/usmetadata/templates/package/resource_read.html
 ckanext/usmetadata/templates/package/snippets/expanded_common_core_fields.html
```

### Comparing `ckanext-usmetadata-0.3.1/setup.py` & `ckanext-usmetadata-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Get the long description from the relevant file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='ckanext-usmetadata',
-    version='0.3.1',
+    version='0.3.2',
     description='US Metadata Plugin for CKAN',
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
         'Programming Language :: Python :: 3'
     ],  # Get strings from http://pypi.python.org/pypi?%3Aaction=list_classifiers
     keywords='',
```

