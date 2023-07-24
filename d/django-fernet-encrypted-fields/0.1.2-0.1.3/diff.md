# Comparing `tmp/django-fernet-encrypted-fields-0.1.2.tar.gz` & `tmp/django-fernet-encrypted-fields-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-fernet-encrypted-fields-0.1.2.tar", last modified: Tue May 17 01:08:42 2022, max compression
+gzip compressed data, was "django-fernet-encrypted-fields-0.1.3.tar", last modified: Mon Jul 24 15:03:55 2023, max compression
```

## Comparing `django-fernet-encrypted-fields-0.1.2.tar` & `django-fernet-encrypted-fields-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 naohide_a   (501) staff       (20)        0 2022-05-17 01:08:42.381245 django-fernet-encrypted-fields-0.1.2/
--rw-r--r--   0 naohide_a   (501) staff       (20)     1080 2022-05-06 00:01:30.000000 django-fernet-encrypted-fields-0.1.2/LICENCE.txt
--rw-r--r--   0 naohide_a   (501) staff       (20)     2430 2022-05-17 01:08:42.381123 django-fernet-encrypted-fields-0.1.2/PKG-INFO
--rw-r--r--   0 naohide_a   (501) staff       (20)     2098 2022-05-06 00:01:30.000000 django-fernet-encrypted-fields-0.1.2/README.md
-drwxr-xr-x   0 naohide_a   (501) staff       (20)        0 2022-05-17 01:08:42.380394 django-fernet-encrypted-fields-0.1.2/django_fernet_encrypted_fields.egg-info/
--rw-r--r--   0 naohide_a   (501) staff       (20)     2430 2022-05-17 01:08:42.000000 django-fernet-encrypted-fields-0.1.2/django_fernet_encrypted_fields.egg-info/PKG-INFO
--rw-r--r--   0 naohide_a   (501) staff       (20)      355 2022-05-17 01:08:42.000000 django-fernet-encrypted-fields-0.1.2/django_fernet_encrypted_fields.egg-info/SOURCES.txt
--rw-r--r--   0 naohide_a   (501) staff       (20)        1 2022-05-17 01:08:42.000000 django-fernet-encrypted-fields-0.1.2/django_fernet_encrypted_fields.egg-info/dependency_links.txt
--rw-r--r--   0 naohide_a   (501) staff       (20)       33 2022-05-17 01:08:42.000000 django-fernet-encrypted-fields-0.1.2/django_fernet_encrypted_fields.egg-info/requires.txt
--rw-r--r--   0 naohide_a   (501) staff       (20)       17 2022-05-17 01:08:42.000000 django-fernet-encrypted-fields-0.1.2/django_fernet_encrypted_fields.egg-info/top_level.txt
-drwxr-xr-x   0 naohide_a   (501) staff       (20)        0 2022-05-17 01:08:42.380839 django-fernet-encrypted-fields-0.1.2/encrypted_fields/
--rw-r--r--   0 naohide_a   (501) staff       (20)       22 2022-05-06 00:30:49.000000 django-fernet-encrypted-fields-0.1.2/encrypted_fields/__init__.py
--rw-r--r--   0 naohide_a   (501) staff       (20)     4863 2022-05-06 23:19:01.000000 django-fernet-encrypted-fields-0.1.2/encrypted_fields/fields.py
--rw-r--r--   0 naohide_a   (501) staff       (20)       38 2022-05-17 01:08:42.381288 django-fernet-encrypted-fields-0.1.2/setup.cfg
--rw-r--r--   0 naohide_a   (501) staff       (20)      580 2022-05-06 00:31:07.000000 django-fernet-encrypted-fields-0.1.2/setup.py
+drwxr-xr-x   0 naohide    (501) staff       (20)        0 2023-07-24 15:03:55.566481 django-fernet-encrypted-fields-0.1.3/
+-rw-r--r--   0 naohide    (501) staff       (20)     1080 2023-07-24 14:56:18.000000 django-fernet-encrypted-fields-0.1.3/LICENCE.txt
+-rw-r--r--   0 naohide    (501) staff       (20)     2453 2023-07-24 15:03:55.566361 django-fernet-encrypted-fields-0.1.3/PKG-INFO
+-rw-r--r--   0 naohide    (501) staff       (20)     2121 2023-07-24 14:56:18.000000 django-fernet-encrypted-fields-0.1.3/README.md
+drwxr-xr-x   0 naohide    (501) staff       (20)        0 2023-07-24 15:03:55.565989 django-fernet-encrypted-fields-0.1.3/django_fernet_encrypted_fields.egg-info/
+-rw-r--r--   0 naohide    (501) staff       (20)     2453 2023-07-24 15:03:55.000000 django-fernet-encrypted-fields-0.1.3/django_fernet_encrypted_fields.egg-info/PKG-INFO
+-rw-r--r--   0 naohide    (501) staff       (20)      355 2023-07-24 15:03:55.000000 django-fernet-encrypted-fields-0.1.3/django_fernet_encrypted_fields.egg-info/SOURCES.txt
+-rw-r--r--   0 naohide    (501) staff       (20)        1 2023-07-24 15:03:55.000000 django-fernet-encrypted-fields-0.1.3/django_fernet_encrypted_fields.egg-info/dependency_links.txt
+-rw-r--r--   0 naohide    (501) staff       (20)       33 2023-07-24 15:03:55.000000 django-fernet-encrypted-fields-0.1.3/django_fernet_encrypted_fields.egg-info/requires.txt
+-rw-r--r--   0 naohide    (501) staff       (20)       17 2023-07-24 15:03:55.000000 django-fernet-encrypted-fields-0.1.3/django_fernet_encrypted_fields.egg-info/top_level.txt
+drwxr-xr-x   0 naohide    (501) staff       (20)        0 2023-07-24 15:03:55.566196 django-fernet-encrypted-fields-0.1.3/encrypted_fields/
+-rw-r--r--   0 naohide    (501) staff       (20)       22 2023-07-24 14:56:18.000000 django-fernet-encrypted-fields-0.1.3/encrypted_fields/__init__.py
+-rw-r--r--   0 naohide    (501) staff       (20)     6368 2023-07-24 14:56:18.000000 django-fernet-encrypted-fields-0.1.3/encrypted_fields/fields.py
+-rw-r--r--   0 naohide    (501) staff       (20)       38 2023-07-24 15:03:55.566519 django-fernet-encrypted-fields-0.1.3/setup.cfg
+-rw-r--r--   0 naohide    (501) staff       (20)      580 2023-07-24 14:57:56.000000 django-fernet-encrypted-fields-0.1.3/setup.py
```

### Comparing `django-fernet-encrypted-fields-0.1.2/LICENCE.txt` & `django-fernet-encrypted-fields-0.1.3/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `django-fernet-encrypted-fields-0.1.2/PKG-INFO` & `django-fernet-encrypted-fields-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-fernet-encrypted-fields
-Version: 0.1.2
+Version: 0.1.3
 Summary: This is inspired by django-encrypted-fields.
 Home-page: http://github.com/frgmt/django-fernet-encrypted-fields/
 Author: fragment.co.jp
 Author-email: info@fragment.co.jp
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
@@ -60,14 +60,15 @@
 - `EncryptedCharField`
 - `EncryptedTextField`
 - `EncryptedDateTimeField`
 - `EncryptedIntegerField`
 - `EncryptedFloatField`
 - `EncryptedEmailField`
 - `EncryptedBooleanField`
+- `EncryptedJSONField`
 
 ### Compatible Django Version
 
 |Compatible Django Version|Specifically tested|
 |---|---|
 |`2.2`|:heavy_check_mark:|
 |`3.0`|:heavy_check_mark:|
```

### Comparing `django-fernet-encrypted-fields-0.1.2/README.md` & `django-fernet-encrypted-fields-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 - `EncryptedCharField`
 - `EncryptedTextField`
 - `EncryptedDateTimeField`
 - `EncryptedIntegerField`
 - `EncryptedFloatField`
 - `EncryptedEmailField`
 - `EncryptedBooleanField`
+- `EncryptedJSONField`
 
 ### Compatible Django Version
 
 |Compatible Django Version|Specifically tested|
 |---|---|
 |`2.2`|:heavy_check_mark:|
 |`3.0`|:heavy_check_mark:|
```

### Comparing `django-fernet-encrypted-fields-0.1.2/django_fernet_encrypted_fields.egg-info/PKG-INFO` & `django-fernet-encrypted-fields-0.1.3/django_fernet_encrypted_fields.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-fernet-encrypted-fields
-Version: 0.1.2
+Version: 0.1.3
 Summary: This is inspired by django-encrypted-fields.
 Home-page: http://github.com/frgmt/django-fernet-encrypted-fields/
 Author: fragment.co.jp
 Author-email: info@fragment.co.jp
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
@@ -60,14 +60,15 @@
 - `EncryptedCharField`
 - `EncryptedTextField`
 - `EncryptedDateTimeField`
 - `EncryptedIntegerField`
 - `EncryptedFloatField`
 - `EncryptedEmailField`
 - `EncryptedBooleanField`
+- `EncryptedJSONField`
 
 ### Compatible Django Version
 
 |Compatible Django Version|Specifically tested|
 |---|---|
 |`2.2`|:heavy_check_mark:|
 |`3.0`|:heavy_check_mark:|
```

### Comparing `django-fernet-encrypted-fields-0.1.2/setup.py` & `django-fernet-encrypted-fields-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,13 +7,13 @@
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="http://github.com/frgmt/django-fernet-encrypted-fields/",
     license="MIT",
     author="fragment.co.jp",
     author_email="info@fragment.co.jp",
     packages=["encrypted_fields"],
-    version="0.1.2",
+    version="0.1.3",
     install_requires=[
         "Django>=2.2",
         "cryptography>=35.0.0",
     ],
 )
```

