# Comparing `tmp/django-vies-6.0.2.tar.gz` & `tmp/django-vies-6.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-vies-6.0.2.tar", last modified: Wed Jul 14 08:13:35 2021, max compression
+gzip compressed data, was "django-vies-6.0.3.tar", last modified: Mon Jul 24 11:03:30 2023, max compression
```

## Comparing `django-vies-6.0.2.tar` & `django-vies-6.0.3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 08:13:35.652088 django-vies-6.0.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1081 2021-07-14 08:13:27.000000 django-vies-6.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      112 2021-07-14 08:13:27.000000 django-vies-6.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5446 2021-07-14 08:13:35.652088 django-vies-6.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4331 2021-07-14 08:13:27.000000 django-vies-6.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 08:13:35.652088 django-vies-6.0.2/django_vies.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5446 2021-07-14 08:13:35.000000 django-vies-6.0.2/django_vies.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      836 2021-07-14 08:13:35.000000 django-vies-6.0.2/django_vies.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-14 08:13:35.000000 django-vies-6.0.2/django_vies.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       40 2021-07-14 08:13:35.000000 django-vies-6.0.2/django_vies.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2021-07-14 08:13:35.000000 django-vies-6.0.2/django_vies.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       87 2021-07-14 08:13:27.000000 django-vies-6.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1984 2021-07-14 08:13:35.652088 django-vies-6.0.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1470 2021-07-14 08:13:27.000000 django-vies-6.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 08:13:35.652088 django-vies-6.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      157 2021-07-14 08:13:27.000000 django-vies-6.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2905 2021-07-14 08:13:27.000000 django-vies-6.0.2/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     1861 2021-07-14 08:13:27.000000 django-vies-6.0.2/tests/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (121)     4124 2021-07-14 08:13:27.000000 django-vies-6.0.2/tests/test_widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 08:13:35.652088 django-vies-6.0.2/tests/testapp/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-14 08:13:27.000000 django-vies-6.0.2/tests/testapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      299 2021-07-14 08:13:27.000000 django-vies-6.0.2/tests/testapp/forms.py
--rw-r--r--   0 runner    (1001) docker     (121)      265 2021-07-14 08:13:27.000000 django-vies-6.0.2/tests/testapp/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      824 2021-07-14 08:13:27.000000 django-vies-6.0.2/tests/testapp/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)       41 2021-07-14 08:13:27.000000 django-vies-6.0.2/tests/testapp/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 08:13:35.652088 django-vies-6.0.2/vies/
--rw-r--r--   0 runner    (1001) docker     (121)      172 2021-07-14 08:13:27.000000 django-vies-6.0.2/vies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 08:13:35.652088 django-vies-6.0.2/vies/forms/
--rw-r--r--   0 runner    (1001) docker     (121)      110 2021-07-14 08:13:27.000000 django-vies-6.0.2/vies/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1107 2021-07-14 08:13:27.000000 django-vies-6.0.2/vies/forms/fields.py
--rw-r--r--   0 runner    (1001) docker     (121)     1917 2021-07-14 08:13:27.000000 django-vies-6.0.2/vies/forms/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 08:13:35.652088 django-vies-6.0.2/vies/locale/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 08:13:35.648088 django-vies-6.0.2/vies/locale/ES/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 08:13:35.652088 django-vies-6.0.2/vies/locale/ES/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1266 2021-07-14 08:13:27.000000 django-vies-6.0.2/vies/locale/ES/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 08:13:35.648088 django-vies-6.0.2/vies/locale/da/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 08:13:35.652088 django-vies-6.0.2/vies/locale/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      955 2021-07-14 08:13:27.000000 django-vies-6.0.2/vies/locale/da/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 08:13:35.648088 django-vies-6.0.2/vies/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 08:13:35.652088 django-vies-6.0.2/vies/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1129 2021-07-14 08:13:27.000000 django-vies-6.0.2/vies/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 08:13:35.648088 django-vies-6.0.2/vies/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 08:13:35.652088 django-vies-6.0.2/vies/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1160 2021-07-14 08:13:27.000000 django-vies-6.0.2/vies/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 08:13:35.652088 django-vies-6.0.2/vies/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 08:13:35.652088 django-vies-6.0.2/vies/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1394 2021-07-14 08:13:27.000000 django-vies-6.0.2/vies/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 08:13:35.652088 django-vies-6.0.2/vies/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 08:13:35.652088 django-vies-6.0.2/vies/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1298 2021-07-14 08:13:27.000000 django-vies-6.0.2/vies/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 08:13:35.652088 django-vies-6.0.2/vies/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 08:13:35.652088 django-vies-6.0.2/vies/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1261 2021-07-14 08:13:27.000000 django-vies-6.0.2/vies/locale/pl/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)      765 2021-07-14 08:13:27.000000 django-vies-6.0.2/vies/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     4767 2021-07-14 08:13:27.000000 django-vies-6.0.2/vies/types.py
--rw-r--r--   0 runner    (1001) docker     (121)      773 2021-07-14 08:13:27.000000 django-vies-6.0.2/vies/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:03:30.165291 django-vies-6.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-24 11:03:17.000000 django-vies-6.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 11:03:17.000000 django-vies-6.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-07-24 11:03:30.165291 django-vies-6.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-07-24 11:03:17.000000 django-vies-6.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:03:30.161291 django-vies-6.0.3/django_vies.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-07-24 11:03:30.000000 django-vies-6.0.3/django_vies.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-24 11:03:30.000000 django-vies-6.0.3/django_vies.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 11:03:30.000000 django-vies-6.0.3/django_vies.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-24 11:03:30.000000 django-vies-6.0.3/django_vies.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-24 11:03:30.000000 django-vies-6.0.3/django_vies.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-24 11:03:17.000000 django-vies-6.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-24 11:03:30.169291 django-vies-6.0.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1470 2023-07-24 11:03:17.000000 django-vies-6.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:03:30.161291 django-vies-6.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-24 11:03:17.000000 django-vies-6.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-24 11:03:17.000000 django-vies-6.0.3/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-07-24 11:03:17.000000 django-vies-6.0.3/tests/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-24 11:03:17.000000 django-vies-6.0.3/tests/test_widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:03:30.165291 django-vies-6.0.3/tests/testapp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 11:03:17.000000 django-vies-6.0.3/tests/testapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-24 11:03:17.000000 django-vies-6.0.3/tests/testapp/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-24 11:03:17.000000 django-vies-6.0.3/tests/testapp/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-24 11:03:17.000000 django-vies-6.0.3/tests/testapp/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-24 11:03:17.000000 django-vies-6.0.3/tests/testapp/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:03:30.165291 django-vies-6.0.3/vies/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-24 11:03:17.000000 django-vies-6.0.3/vies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:03:30.165291 django-vies-6.0.3/vies/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-24 11:03:17.000000 django-vies-6.0.3/vies/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-24 11:03:17.000000 django-vies-6.0.3/vies/forms/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-24 11:03:17.000000 django-vies-6.0.3/vies/forms/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:03:30.161291 django-vies-6.0.3/vies/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:03:30.157292 django-vies-6.0.3/vies/locale/ES/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:03:30.165291 django-vies-6.0.3/vies/locale/ES/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-24 11:03:17.000000 django-vies-6.0.3/vies/locale/ES/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:03:30.157292 django-vies-6.0.3/vies/locale/da/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:03:30.165291 django-vies-6.0.3/vies/locale/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-24 11:03:17.000000 django-vies-6.0.3/vies/locale/da/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:03:30.157292 django-vies-6.0.3/vies/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:03:30.165291 django-vies-6.0.3/vies/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-24 11:03:17.000000 django-vies-6.0.3/vies/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:03:30.157292 django-vies-6.0.3/vies/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:03:30.165291 django-vies-6.0.3/vies/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-24 11:03:17.000000 django-vies-6.0.3/vies/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:03:30.161291 django-vies-6.0.3/vies/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:03:30.165291 django-vies-6.0.3/vies/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-24 11:03:17.000000 django-vies-6.0.3/vies/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:03:30.161291 django-vies-6.0.3/vies/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:03:30.165291 django-vies-6.0.3/vies/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-24 11:03:17.000000 django-vies-6.0.3/vies/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:03:30.161291 django-vies-6.0.3/vies/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:03:30.165291 django-vies-6.0.3/vies/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-24 11:03:17.000000 django-vies-6.0.3/vies/locale/pl/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-24 11:03:17.000000 django-vies-6.0.3/vies/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-07-24 11:03:17.000000 django-vies-6.0.3/vies/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-24 11:03:17.000000 django-vies-6.0.3/vies/validators.py
```

### Comparing `django-vies-6.0.2/LICENSE` & `django-vies-6.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-vies-6.0.2/PKG-INFO` & `django-vies-6.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: django-vies
-Version: 6.0.2
+Version: 6.0.3
 Summary: Validate and store VAT Information Exchange System (VIES) data in Django.
 Home-page: https://github.com/codingjoe/django-vies
 Author: Johannes Hoppe
 Author-email: info@johanneshoppe.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Programming Language :: Python
@@ -105,46 +104,52 @@
 
 e.g. using celery
 
 .. code:: python
 
     from celery import shared_task
     from vies.models import VATINField
+    from vies.types import VATIN
+    from django.core.exceptions import ValidationError
 
 
     class Company(models.Model):
         name = models.CharField(max_length=100)
         vat = VATINField()
         vat_is_valid = models.BooleanField(default=False)
 
         def __init__(self, *args, **kwargs):
-            self.__vat = self.vat
             super(Company, self).__init__(*args, **kwargs)
+            self.__vat = self.vat
 
         def save(self, *args, **kwargs):
             if self.__vat != self.vat:
-                validate_vat_field.delay(self)
+                validate_vat_field.delay(self.pk)
             super(Company, self).save(*args, **kwargs)
             self.__vat = self.vat
 
         def refresh_from_db(self, *args, **kwargs)
             super(Company, self).refresh_from_db(*args, **kwargs)
             self.__vat = self.vat
 
+
     @shared_task
-    def validate_vat_field(company):
+    def validate_vat_field(company_id):
+        company = Company.objects.get(pk=company_id)
+        vat = VATIN.from_str(company.vat)
         try:
-            company.vat.validate()
+            vat.validate()
         except ValidationError:
             company.vat_is_valid = False
         else:
             company.vat_is_valid = True
         finally:
             company.save(update_fields=['vat_is_valid'])
 
+You can also use ``celery.current_app.send_task('validate_vat_field', kwargs={"company_id": self.pk})`` to call asynchronous task to avoid **circular import errors**.
 
 Translations
 ------------
 
 Feel free to contribute translations, it's simple!
 
 .. code:: shell
@@ -173,9 +178,7 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-
-
```

### Comparing `django-vies-6.0.2/README.rst` & `django-vies-6.0.3/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -77,46 +77,52 @@
 
 e.g. using celery
 
 .. code:: python
 
     from celery import shared_task
     from vies.models import VATINField
+    from vies.types import VATIN
+    from django.core.exceptions import ValidationError
 
 
     class Company(models.Model):
         name = models.CharField(max_length=100)
         vat = VATINField()
         vat_is_valid = models.BooleanField(default=False)
 
         def __init__(self, *args, **kwargs):
-            self.__vat = self.vat
             super(Company, self).__init__(*args, **kwargs)
+            self.__vat = self.vat
 
         def save(self, *args, **kwargs):
             if self.__vat != self.vat:
-                validate_vat_field.delay(self)
+                validate_vat_field.delay(self.pk)
             super(Company, self).save(*args, **kwargs)
             self.__vat = self.vat
 
         def refresh_from_db(self, *args, **kwargs)
             super(Company, self).refresh_from_db(*args, **kwargs)
             self.__vat = self.vat
 
+
     @shared_task
-    def validate_vat_field(company):
+    def validate_vat_field(company_id):
+        company = Company.objects.get(pk=company_id)
+        vat = VATIN.from_str(company.vat)
         try:
-            company.vat.validate()
+            vat.validate()
         except ValidationError:
             company.vat_is_valid = False
         else:
             company.vat_is_valid = True
         finally:
             company.save(update_fields=['vat_is_valid'])
 
+You can also use ``celery.current_app.send_task('validate_vat_field', kwargs={"company_id": self.pk})`` to call asynchronous task to avoid **circular import errors**.
 
 Translations
 ------------
 
 Feel free to contribute translations, it's simple!
 
 .. code:: shell
```

### Comparing `django-vies-6.0.2/django_vies.egg-info/PKG-INFO` & `django-vies-6.0.3/django_vies.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: django-vies
-Version: 6.0.2
+Version: 6.0.3
 Summary: Validate and store VAT Information Exchange System (VIES) data in Django.
 Home-page: https://github.com/codingjoe/django-vies
 Author: Johannes Hoppe
 Author-email: info@johanneshoppe.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Programming Language :: Python
@@ -105,46 +104,52 @@
 
 e.g. using celery
 
 .. code:: python
 
     from celery import shared_task
     from vies.models import VATINField
+    from vies.types import VATIN
+    from django.core.exceptions import ValidationError
 
 
     class Company(models.Model):
         name = models.CharField(max_length=100)
         vat = VATINField()
         vat_is_valid = models.BooleanField(default=False)
 
         def __init__(self, *args, **kwargs):
-            self.__vat = self.vat
             super(Company, self).__init__(*args, **kwargs)
+            self.__vat = self.vat
 
         def save(self, *args, **kwargs):
             if self.__vat != self.vat:
-                validate_vat_field.delay(self)
+                validate_vat_field.delay(self.pk)
             super(Company, self).save(*args, **kwargs)
             self.__vat = self.vat
 
         def refresh_from_db(self, *args, **kwargs)
             super(Company, self).refresh_from_db(*args, **kwargs)
             self.__vat = self.vat
 
+
     @shared_task
-    def validate_vat_field(company):
+    def validate_vat_field(company_id):
+        company = Company.objects.get(pk=company_id)
+        vat = VATIN.from_str(company.vat)
         try:
-            company.vat.validate()
+            vat.validate()
         except ValidationError:
             company.vat_is_valid = False
         else:
             company.vat_is_valid = True
         finally:
             company.save(update_fields=['vat_is_valid'])
 
+You can also use ``celery.current_app.send_task('validate_vat_field', kwargs={"company_id": self.pk})`` to call asynchronous task to avoid **circular import errors**.
 
 Translations
 ------------
 
 Feel free to contribute translations, it's simple!
 
 .. code:: shell
@@ -173,9 +178,7 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-
-
```

### Comparing `django-vies-6.0.2/django_vies.egg-info/SOURCES.txt` & `django-vies-6.0.3/django_vies.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-vies-6.0.2/setup.cfg` & `django-vies-6.0.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 [aliases]
 test = pytest
 
 [tool:pytest]
 norecursedirs = venv env .eggs
 addopts = 
 	--cov=vies
-django_settings_module = tests.testapp.settings
+DJANGO_SETTINGS_MODULE = tests.testapp.settings
 
 [coverage:run]
 source = .
 omit = 
 	*/migrations/*
 	*/tests/*
 	*/test_*.py
```

### Comparing `django-vies-6.0.2/setup.py` & `django-vies-6.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `django-vies-6.0.2/tests/test_types.py` & `django-vies-6.0.3/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `django-vies-6.0.2/tests/test_validators.py` & `django-vies-6.0.3/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `django-vies-6.0.2/tests/test_widgets.py` & `django-vies-6.0.3/tests/test_widgets.py`

 * *Files identical despite different names*

### Comparing `django-vies-6.0.2/tests/testapp/settings.py` & `django-vies-6.0.3/tests/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `django-vies-6.0.2/vies/forms/fields.py` & `django-vies-6.0.3/vies/forms/fields.py`

 * *Files identical despite different names*

### Comparing `django-vies-6.0.2/vies/forms/widgets.py` & `django-vies-6.0.3/vies/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `django-vies-6.0.2/vies/locale/ES/LC_MESSAGES/django.po` & `django-vies-6.0.3/vies/locale/ES/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-vies-6.0.2/vies/locale/da/LC_MESSAGES/django.po` & `django-vies-6.0.3/vies/locale/da/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-vies-6.0.2/vies/locale/de/LC_MESSAGES/django.po` & `django-vies-6.0.3/vies/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-vies-6.0.2/vies/locale/fr/LC_MESSAGES/django.po` & `django-vies-6.0.3/vies/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-vies-6.0.2/vies/locale/it/LC_MESSAGES/django.po` & `django-vies-6.0.3/vies/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-vies-6.0.2/vies/locale/nl/LC_MESSAGES/django.po` & `django-vies-6.0.3/vies/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-vies-6.0.2/vies/locale/pl/LC_MESSAGES/django.po` & `django-vies-6.0.3/vies/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-vies-6.0.2/vies/models.py` & `django-vies-6.0.3/vies/models.py`

 * *Files identical despite different names*

### Comparing `django-vies-6.0.2/vies/types.py` & `django-vies-6.0.3/vies/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 def fr_format(v):
     return "%s %s" % (v[:4], v[4:])
 
 
 VIES_OPTIONS = {
     "AT": ("Austria", re.compile(r"^ATU\d{8}$")),
-    "BE": ("Belgium", re.compile(r"^BE0?\d{9}$")),
+    "BE": ("Belgium", re.compile(r"^BE(0|1)\d{9}$")),
     "BG": ("Bulgaria", re.compile(r"^BG\d{9,10}$")),
     "HR": ("Croatia", re.compile(r"^HR\d{11}$")),
     "CY": ("Cyprus", re.compile(r"^CY\d{8}[A-Z]$")),
     "CZ": ("Czech Republic", re.compile(r"^CZ\d{8,10}$")),
     "DE": ("Germany", re.compile(r"^DE\d{9}$")),
     "DK": ("Denmark", re.compile(r"^DK\d{8}$"), dk_format),
     "EE": ("Estonia", re.compile(r"^EE\d{9}$")),
```

### Comparing `django-vies-6.0.2/vies/validators.py` & `django-vies-6.0.3/vies/validators.py`

 * *Files identical despite different names*

