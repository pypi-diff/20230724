# Comparing `tmp/kl_sdk-0.0.2.tar.gz` & `tmp/kl_sdk-0.0.3.tar.gz`

## Comparing `kl_sdk-0.0.2.tar` & `kl_sdk-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kl_sdk-0.0.2/src/kl_sdk/__init__.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 kl_sdk-0.0.2/src/kl_sdk/cryptoService.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 kl_sdk-0.0.2/src/kl_sdk/example.py
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 kl_sdk-0.0.2/src/kl_sdk/sendDataWithHmac.py
--rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 kl_sdk-0.0.2/src/kl_sdk/validatorService.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 kl_sdk-0.0.2/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 kl_sdk-0.0.2/LICENSE
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 kl_sdk-0.0.2/README.md
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 kl_sdk-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 kl_sdk-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kl_sdk-0.0.3/src/kl_sdk/__init__.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 kl_sdk-0.0.3/src/kl_sdk/cryptoService.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 kl_sdk-0.0.3/src/kl_sdk/example.py
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 kl_sdk-0.0.3/src/kl_sdk/sendDataWithHmac.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 kl_sdk-0.0.3/src/kl_sdk/sendReceipt.py
+-rw-r--r--   0        0        0     3025 2020-02-02 00:00:00.000000 kl_sdk-0.0.3/src/kl_sdk/validatorService.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 kl_sdk-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 kl_sdk-0.0.3/LICENSE
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 kl_sdk-0.0.3/README.md
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 kl_sdk-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 kl_sdk-0.0.3/PKG-INFO
```

### Comparing `kl_sdk-0.0.2/src/kl_sdk/validatorService.py` & `kl_sdk-0.0.3/src/kl_sdk/validatorService.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import List, Optional
-from pydantic import BaseModel, validator, ValidationError, conint, constr, root_validator
+from pydantic import BaseModel, validator, ValidationError, conint, constr, model_validator
 import re
 
 class TransactionPayment(BaseModel):
     reference_id: str
     amount: float
     customer_id: str
     transaction_date: str
@@ -26,66 +26,63 @@
         if not re.match(r'^\d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2}$', value):
             raise ValueError('Invalid date format. Expected format: YYYY-MM-DDTHH:mm:ss')
         return value
 
 class ReceiptPayload(BaseModel):
     reference_id: str
     amount: float
-    total_tax_amount: Optional[float]
     currency: str
     date: str
     covers: Optional[int]
     table: Optional[str]
     invoice: Optional[int]
-    total_discount: Optional[float]
+    total_discount: Optional[int] = None
     mode: Optional[int]
     partner_name: str
     merchant: Optional[dict]
     store: Optional[dict]
     taxes: Optional[List[dict]]
     items: Optional[List[dict]]
     payments: Optional[List[dict]]
-
+    total_tax_amount: int = None
+    @validator('date')
+    def validate_date(cls, value):
+        if not re.match(r'^\d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2}$', value):
+            raise ValueError('Invalid date format. Expected format: YYYY-MM-DDTHH:mm:ss')
+        return value
     @validator('amount')
     def amount_non_negative(cls, value):
         if value < 0:
             raise ValueError('Amount cannot be negative')
         return value
 
     @validator('currency')
     def validate_currency(cls, value):
         if value not in ['EUR', 'USD']:
             raise ValueError('Invalid currency. Expected currency: EUR or USD')
         return value
 
-    @validator('date')
-    def validate_date(cls, value):
-        if not re.match(r'^\d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2}$', value):
-            raise ValueError('Invalid date format. Expected format: YYYY-MM-DDTHH:mm:ss')
+    @validator('taxes', 'items', 'payments')
+    def validate_list_items(cls, value):
+        if value is not None and not isinstance(value, list):
+            raise ValueError('Expected a list')
         return value
 
-    @validator('siret')
+    @validator('siret',check_fields=False)
     def validate_siret(cls, value):
         if value and (len(value) != 14 or not value.isdigit()):
             raise ValueError('Invalid SIRET number. Expected 14 digits.')
         return value
 
-    @validator('taxes', 'items', 'payments')
-    def validate_list_items(cls, value):
-        if value is not None and not isinstance(value, list):
-            raise ValueError('Expected a list')
-        return value
-
-    @root_validator
-    def validate_tax_rate(cls, values):
-        taxes = values.get('taxes', [])
-        for tax in taxes:
+    @validator('taxes', pre=True)
+    def validate_tax_rate(cls, value):
+        for tax in value:
             if 'rate' in tax and tax['rate'] not in [550, 1000, 2000]:
                 raise ValueError('Invalid tax rate. Expected 550, 1000, or 2000')
-        return values
+        return value
 
 
 def validate_transaction_payload(payload):
     if not payload:
         raise ValueError('No payload to validate')
     TransactionPayment(**payload)
     return True
```

### Comparing `kl_sdk-0.0.2/.gitignore` & `kl_sdk-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `kl_sdk-0.0.2/LICENSE` & `kl_sdk-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kl_sdk-0.0.2/pyproject.toml` & `kl_sdk-0.0.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "kl_sdk"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name = "killbillsdev", email = "cto@killbills.co" }
 ]
 description = "KillBills e-receipt sdk"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -25,8 +25,9 @@
 Homepage = "https://github.com/killbillsdev/killbills-sdk-python"
 "Bug Tracker" = "https://github.com/killbillsdev/killbills-sdk-python/issues"
 
 [dependencies]
 python = ">=3.7"
 requests = ">=2.26.0"
 pydantic = ">=2.0.3"
+hmac = "20101005"
```

### Comparing `kl_sdk-0.0.2/PKG-INFO` & `kl_sdk-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kl_sdk
-Version: 0.0.2
+Version: 0.0.3
 Summary: KillBills e-receipt sdk
 Project-URL: Homepage, https://github.com/killbillsdev/killbills-sdk-python
 Project-URL: Bug Tracker, https://github.com/killbillsdev/killbills-sdk-python/issues
 Author-email: killbillsdev <cto@killbills.co>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

