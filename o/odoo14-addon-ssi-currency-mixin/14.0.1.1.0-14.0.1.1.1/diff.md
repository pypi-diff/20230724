# Comparing `tmp/odoo14_addon_ssi_currency_mixin-14.0.1.1.0-py3-none-any.whl.zip` & `tmp/odoo14_addon_ssi_currency_mixin-14.0.1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 52801 bytes, number of entries: 10
--rw-rw-r--  2.0 unx     1160 b- defN 23-Mar-26 06:15 odoo/addons/ssi_currency_mixin/README.rst
--rw-rw-r--  2.0 unx      181 b- defN 23-Mar-26 06:15 odoo/addons/ssi_currency_mixin/__init__.py
--rw-rw-r--  2.0 unx      491 b- defN 23-Mar-26 06:15 odoo/addons/ssi_currency_mixin/__manifest__.py
--rw-rw-r--  2.0 unx      189 b- defN 23-Mar-26 06:15 odoo/addons/ssi_currency_mixin/models/__init__.py
--rw-rw-r--  2.0 unx     2003 b- defN 23-Mar-26 06:15 odoo/addons/ssi_currency_mixin/models/mixin_currency.py
--rw-rw-r--  2.0 unx    48333 b- defN 23-Mar-26 06:15 odoo/addons/ssi_currency_mixin/static/description/icon.png
--rw-rw-r--  2.0 unx     1764 b- defN 23-Jul-20 08:02 odoo14_addon_ssi_currency_mixin-14.0.1.1.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-20 08:02 odoo14_addon_ssi_currency_mixin-14.0.1.1.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx        5 b- defN 23-Jul-20 08:02 odoo14_addon_ssi_currency_mixin-14.0.1.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1044 b- defN 23-Jul-20 08:02 odoo14_addon_ssi_currency_mixin-14.0.1.1.0.dist-info/RECORD
-10 files, 55262 bytes uncompressed, 50949 bytes compressed:  7.8%
+Zip file size: 52795 bytes, number of entries: 10
+-rw-r--r--  2.0 unx     1160 b- defN 23-Jul-24 08:23 odoo/addons/ssi_currency_mixin/README.rst
+-rw-r--r--  2.0 unx      181 b- defN 23-Jul-24 08:23 odoo/addons/ssi_currency_mixin/__init__.py
+-rw-r--r--  2.0 unx      491 b- defN 23-Jul-24 08:23 odoo/addons/ssi_currency_mixin/__manifest__.py
+-rw-r--r--  2.0 unx      189 b- defN 23-Jul-24 08:23 odoo/addons/ssi_currency_mixin/models/__init__.py
+-rw-r--r--  2.0 unx     2003 b- defN 23-Jul-24 08:23 odoo/addons/ssi_currency_mixin/models/mixin_currency.py
+-rw-r--r--  2.0 unx    48333 b- defN 23-Jul-24 08:23 odoo/addons/ssi_currency_mixin/static/description/icon.png
+-rw-r--r--  2.0 unx     1755 b- defN 23-Jul-24 08:23 odoo14_addon_ssi_currency_mixin-14.0.1.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-24 08:23 odoo14_addon_ssi_currency_mixin-14.0.1.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Jul-24 08:23 odoo14_addon_ssi_currency_mixin-14.0.1.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1044 b- defN 23-Jul-24 08:23 odoo14_addon_ssi_currency_mixin-14.0.1.1.1.dist-info/RECORD
+10 files, 55253 bytes uncompressed, 50943 bytes compressed:  7.8%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: odoo/addons/ssi_currency_mixin/models/mixin_currency.py
 Comment: 
 
 Filename: odoo/addons/ssi_currency_mixin/static/description/icon.png
 Comment: 
 
-Filename: odoo14_addon_ssi_currency_mixin-14.0.1.1.0.dist-info/METADATA
+Filename: odoo14_addon_ssi_currency_mixin-14.0.1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addon_ssi_currency_mixin-14.0.1.1.0.dist-info/WHEEL
+Filename: odoo14_addon_ssi_currency_mixin-14.0.1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addon_ssi_currency_mixin-14.0.1.1.0.dist-info/top_level.txt
+Filename: odoo14_addon_ssi_currency_mixin-14.0.1.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addon_ssi_currency_mixin-14.0.1.1.0.dist-info/RECORD
+Filename: odoo14_addon_ssi_currency_mixin-14.0.1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/ssi_currency_mixin/README.rst

```diff
@@ -1,10 +1,10 @@
-.. image:: https://img.shields.io/badge/licence-LGPL--3-blue.svg
-   :target: http://www.gnu.org/licenses/lgpl-3.0-standalone.html
-   :alt: License: LGPL-3
+.. image:: https://img.shields.io/badge/licence-AGPL--3-blue.svg
+   :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
+   :alt: License: AGPL-3
 
 ==============
 Currency Mixin
 ==============
 
 
 Installation
```

## odoo/addons/ssi_currency_mixin/__init__.py

```diff
@@ -1,7 +1,7 @@
 # Copyright 2023 OpenSynergy Indonesia
 # Copyright 2023 PT. Simetri Sinergi Indonesia
-# License LGPL-3.0 or later (http://www.gnu.org/licenses/lgpl).
+# License AGPL-3.0 or later (http://www.gnu.org/licenses/agpl).
 
 from . import (
     models,
 )
```

## odoo/addons/ssi_currency_mixin/__manifest__.py

```diff
@@ -1,17 +1,17 @@
 # Copyright 2023 OpenSynergy Indonesia
 # Copyright 2023 PT. Simetri Sinergi Indonesia
-# License LGPL-3.0 or later (http://www.gnu.org/licenses/lgpl).
+# License AGPL-3.0 or later (http://www.gnu.org/licenses/agpl).
 
 {
     "name": "Currency Mixin",
-    "version": "14.0.1.1.0",
+    "version": "14.0.1.1.1",
     "website": "https://simetri-sinergi.id",
     "author": "OpenSynergy Indonesia, PT. Simetri Sinergi Indonesia",
-    "license": "LGPL-3",
+    "license": "AGPL-3",
     "installable": True,
     "depends": [
         "ssi_company_currency_mixin",
         "currency_rate_inverted",
     ],
     "data": [],
 }
```

## odoo/addons/ssi_currency_mixin/models/__init__.py

```diff
@@ -1,7 +1,7 @@
 # Copyright 2022 OpenSynergy Indonesia
 # Copyright 2022 PT. Simetri Sinergi Indonesia
-# License LGPL-3.0 or later (http://www.gnu.org/licenses/lgpl).
+# License AGPL-3.0 or later (http://www.gnu.org/licenses/agpl).
 
 from . import (
     mixin_currency,
 )
```

## odoo/addons/ssi_currency_mixin/models/mixin_currency.py

```diff
@@ -1,10 +1,10 @@
 # Copyright 2022 OpenSynergy Indonesia
 # Copyright 2022 PT. Simetri Sinergi Indonesia
-# License LGPL-3.0 or later (http://www.gnu.org/licenses/lgpl).
+# License AGPL-3.0 or later (http://www.gnu.org/licenses/agpl).
 
 from odoo import api, fields, models
 
 
 class MixinCurrency(models.AbstractModel):
     _name = "mixin.currency"
     _description = "Currency Mixin"
```

## Comparing `odoo14_addon_ssi_currency_mixin-14.0.1.1.0.dist-info/METADATA` & `odoo14_addon_ssi_currency_mixin-14.0.1.1.1.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: odoo14-addon-ssi-currency-mixin
-Version: 14.0.1.1.0
+Version: 14.0.1.1.1
 Summary: Currency Mixin
 Home-page: https://simetri-sinergi.id
 Author: OpenSynergy Indonesia, PT. Simetri Sinergi Indonesia
-License: LGPL-3
+License: AGPL-3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 14.0
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Requires-Python: >=3.6
 Requires-Dist: odoo14-addon-currency-rate-inverted
 Requires-Dist: odoo14-addon-ssi-company-currency-mixin
 Requires-Dist: odoo (<14.1dev,>=14.0a)
 
-.. image:: https://img.shields.io/badge/licence-LGPL--3-blue.svg
-   :target: http://www.gnu.org/licenses/lgpl-3.0-standalone.html
-   :alt: License: LGPL-3
+.. image:: https://img.shields.io/badge/licence-AGPL--3-blue.svg
+   :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
+   :alt: License: AGPL-3
 
 ==============
 Currency Mixin
 ==============
 
 
 Installation
```

## Comparing `odoo14_addon_ssi_currency_mixin-14.0.1.1.0.dist-info/RECORD` & `odoo14_addon_ssi_currency_mixin-14.0.1.1.1.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-odoo/addons/ssi_currency_mixin/README.rst,sha256=FFxoTZA3xiqv8VysstLxwz-c4eNBt07kHtqVfLii1S0,1160
-odoo/addons/ssi_currency_mixin/__init__.py,sha256=ZFas4kM9ysF28mx5Z5ufeUzTx2AT1NJxaf3-D8veqoU,181
-odoo/addons/ssi_currency_mixin/__manifest__.py,sha256=-i3LPRNfRz1uDNRuYu5ZiPcX8n44H-JfrKwZeW2QQ0E,491
-odoo/addons/ssi_currency_mixin/models/__init__.py,sha256=yQyjfQbprhkqT_t0qRJY3toyk_nrHrYXc8UaNI0n3Ls,189
-odoo/addons/ssi_currency_mixin/models/mixin_currency.py,sha256=mIQFTQCaehK4qpEY_9Czt26FbEfUTvgHC5Wy8Rm4OoE,2003
+odoo/addons/ssi_currency_mixin/README.rst,sha256=gym0sKQ-p42CsztYdu_2HeTf8lNPfNRQ6ojwRuhBPHo,1160
+odoo/addons/ssi_currency_mixin/__init__.py,sha256=M7twq1SJz2cc98CkgeiDiDg05QWWFb09lt5oh03-axA,181
+odoo/addons/ssi_currency_mixin/__manifest__.py,sha256=UH1taDGY3Bme-M9g8ZvOzptHgaJJZfNzTDooGu5-WRM,491
+odoo/addons/ssi_currency_mixin/models/__init__.py,sha256=waYtMl-o67ElLP2zQxwDJR-PMPF9_DnPueeGBWqkYPE,189
+odoo/addons/ssi_currency_mixin/models/mixin_currency.py,sha256=RSa-20LqhxcxCQEiRTQR2-bR7gcvuwnqwtKMQDJ2AFg,2003
 odoo/addons/ssi_currency_mixin/static/description/icon.png,sha256=lNGJOSg4cMRfwPTfFKVT6d5B2N1N83iVpEEN1blqu1I,48333
-odoo14_addon_ssi_currency_mixin-14.0.1.1.0.dist-info/METADATA,sha256=QUBIJ2IOKL6hJVDFrZrObIaXVpbJoNnvGV5Ig-Uqxys,1764
-odoo14_addon_ssi_currency_mixin-14.0.1.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-odoo14_addon_ssi_currency_mixin-14.0.1.1.0.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
-odoo14_addon_ssi_currency_mixin-14.0.1.1.0.dist-info/RECORD,,
+odoo14_addon_ssi_currency_mixin-14.0.1.1.1.dist-info/METADATA,sha256=vKftCBd5phviqQ0TiBJx-lXcxCRgC-eD1qXWFzwXP-o,1755
+odoo14_addon_ssi_currency_mixin-14.0.1.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+odoo14_addon_ssi_currency_mixin-14.0.1.1.1.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
+odoo14_addon_ssi_currency_mixin-14.0.1.1.1.dist-info/RECORD,,
```

