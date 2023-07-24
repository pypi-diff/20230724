# Comparing `tmp/paystack_cli-0.1.0.tar.gz` & `tmp/paystack_cli-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paystack_cli-0.1.0.tar", max compression
+gzip compressed data, was "paystack_cli-0.1.1.tar", max compression
```

## Comparing `paystack_cli-0.1.0.tar` & `paystack_cli-0.1.1.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0      643 2023-07-24 19:11:31.024271 paystack_cli-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-07-19 21:04:35.944414 paystack_cli-0.1.0/paystack_cli/__init__.py
--rw-r--r--   0        0        0     1104 2023-07-24 16:58:10.490171 paystack_cli-0.1.0/paystack_cli/apple_pay.py
--rw-r--r--   0        0        0     3072 2023-07-24 17:35:10.884307 paystack_cli-0.1.0/paystack_cli/bulk_charges.py
--rw-r--r--   0        0        0     3586 2023-07-24 17:35:10.894307 paystack_cli-0.1.0/paystack_cli/charge.py
--rw-r--r--   0        0        0     3729 2023-07-24 17:35:10.924306 paystack_cli-0.1.0/paystack_cli/customers.py
--rw-r--r--   0        0        0     3746 2023-07-24 17:35:10.917640 paystack_cli-0.1.0/paystack_cli/dedicated_virtual_accounts.py
--rw-r--r--   0        0        0     3713 2023-07-24 17:40:00.337132 paystack_cli-0.1.0/paystack_cli/disputes.py
--rw-r--r--   0        0        0      710 2023-07-24 17:42:15.102544 paystack_cli-0.1.0/paystack_cli/integration.py
--rw-r--r--   0        0        0     7133 2023-07-24 19:14:49.539796 paystack_cli-0.1.0/paystack_cli/main.py
--rw-r--r--   0        0        0     1090 2023-07-24 17:46:04.587581 paystack_cli-0.1.0/paystack_cli/miscellaneous.py
--rw-r--r--   0        0        0     2795 2023-07-24 17:51:59.045863 paystack_cli-0.1.0/paystack_cli/payment_pages.py
--rw-r--r--   0        0        0     4479 2023-07-24 17:57:32.464325 paystack_cli-0.1.0/paystack_cli/payments_requests.py
--rw-r--r--   0        0        0     2093 2023-07-24 18:00:45.079200 paystack_cli-0.1.0/paystack_cli/plans.py
--rw-r--r--   0        0        0     1920 2023-07-24 18:04:03.576117 paystack_cli-0.1.0/paystack_cli/products.py
--rw-r--r--   0        0        0     1564 2023-07-24 18:06:12.699501 paystack_cli-0.1.0/paystack_cli/refunds.py
--rw-r--r--   0        0        0     1231 2023-07-24 18:09:03.792597 paystack_cli-0.1.0/paystack_cli/settlements.py
--rw-r--r--   0        0        0     3306 2023-07-24 18:12:46.875562 paystack_cli-0.1.0/paystack_cli/subaccounts.py
--rw-r--r--   0        0        0     2384 2023-07-24 18:16:37.889155 paystack_cli-0.1.0/paystack_cli/subscriptions.py
--rw-r--r--   0        0        0     2945 2023-07-24 18:28:41.008662 paystack_cli-0.1.0/paystack_cli/terminals.py
--rw-r--r--   0        0        0     5845 2023-07-24 18:32:52.056579 paystack_cli-0.1.0/paystack_cli/transactions.py
--rw-r--r--   0        0        0     2892 2023-07-24 18:36:11.984984 paystack_cli-0.1.0/paystack_cli/transactions_splits.py
--rw-r--r--   0        0        0     3150 2023-07-24 18:40:01.466531 paystack_cli-0.1.0/paystack_cli/transfer_recipients.py
--rw-r--r--   0        0        0     2447 2023-07-24 18:43:01.438487 paystack_cli-0.1.0/paystack_cli/transfers.py
--rw-r--r--   0        0        0     1921 2023-07-24 18:48:20.326076 paystack_cli-0.1.0/paystack_cli/transfers_control.py
--rw-r--r--   0        0        0     3426 2023-07-23 09:12:38.123328 paystack_cli-0.1.0/paystack_cli/utils.py
--rw-r--r--   0        0        0     1552 2023-07-24 18:51:27.954669 paystack_cli-0.1.0/paystack_cli/verification.py
--rw-r--r--   0        0        0      819 2023-07-24 19:13:51.417687 paystack_cli-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1347 1970-01-01 00:00:00.000000 paystack_cli-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-24 20:00:11.419052 paystack_cli-0.1.1/LICENSE
+-rw-r--r--   0        0        0      805 2023-07-24 20:19:18.129756 paystack_cli-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-19 21:04:35.944414 paystack_cli-0.1.1/paystack_cli/__init__.py
+-rw-r--r--   0        0        0     1104 2023-07-24 16:58:10.490171 paystack_cli-0.1.1/paystack_cli/apple_pay.py
+-rw-r--r--   0        0        0     3072 2023-07-24 17:35:10.884307 paystack_cli-0.1.1/paystack_cli/bulk_charges.py
+-rw-r--r--   0        0        0     3586 2023-07-24 17:35:10.894307 paystack_cli-0.1.1/paystack_cli/charge.py
+-rw-r--r--   0        0        0     3729 2023-07-24 17:35:10.924306 paystack_cli-0.1.1/paystack_cli/customers.py
+-rw-r--r--   0        0        0     3746 2023-07-24 17:35:10.917640 paystack_cli-0.1.1/paystack_cli/dedicated_virtual_accounts.py
+-rw-r--r--   0        0        0     3713 2023-07-24 17:40:00.337132 paystack_cli-0.1.1/paystack_cli/disputes.py
+-rw-r--r--   0        0        0      710 2023-07-24 17:42:15.102544 paystack_cli-0.1.1/paystack_cli/integration.py
+-rw-r--r--   0        0        0     7133 2023-07-24 19:57:51.596479 paystack_cli-0.1.1/paystack_cli/main.py
+-rw-r--r--   0        0        0     1090 2023-07-24 17:46:04.587581 paystack_cli-0.1.1/paystack_cli/miscellaneous.py
+-rw-r--r--   0        0        0     2795 2023-07-24 17:51:59.045863 paystack_cli-0.1.1/paystack_cli/payment_pages.py
+-rw-r--r--   0        0        0     4479 2023-07-24 17:57:32.464325 paystack_cli-0.1.1/paystack_cli/payments_requests.py
+-rw-r--r--   0        0        0     2093 2023-07-24 18:00:45.079200 paystack_cli-0.1.1/paystack_cli/plans.py
+-rw-r--r--   0        0        0     1920 2023-07-24 18:04:03.576117 paystack_cli-0.1.1/paystack_cli/products.py
+-rw-r--r--   0        0        0     1564 2023-07-24 18:06:12.699501 paystack_cli-0.1.1/paystack_cli/refunds.py
+-rw-r--r--   0        0        0     1231 2023-07-24 18:09:03.792597 paystack_cli-0.1.1/paystack_cli/settlements.py
+-rw-r--r--   0        0        0     3306 2023-07-24 18:12:46.875562 paystack_cli-0.1.1/paystack_cli/subaccounts.py
+-rw-r--r--   0        0        0     2384 2023-07-24 18:16:37.889155 paystack_cli-0.1.1/paystack_cli/subscriptions.py
+-rw-r--r--   0        0        0     2945 2023-07-24 18:28:41.008662 paystack_cli-0.1.1/paystack_cli/terminals.py
+-rw-r--r--   0        0        0     5845 2023-07-24 18:32:52.056579 paystack_cli-0.1.1/paystack_cli/transactions.py
+-rw-r--r--   0        0        0     2892 2023-07-24 18:36:11.984984 paystack_cli-0.1.1/paystack_cli/transactions_splits.py
+-rw-r--r--   0        0        0     3150 2023-07-24 18:40:01.466531 paystack_cli-0.1.1/paystack_cli/transfer_recipients.py
+-rw-r--r--   0        0        0     2447 2023-07-24 18:43:01.438487 paystack_cli-0.1.1/paystack_cli/transfers.py
+-rw-r--r--   0        0        0     1921 2023-07-24 18:48:20.326076 paystack_cli-0.1.1/paystack_cli/transfers_control.py
+-rw-r--r--   0        0        0     3426 2023-07-23 09:12:38.123328 paystack_cli-0.1.1/paystack_cli/utils.py
+-rw-r--r--   0        0        0     1552 2023-07-24 18:51:27.954669 paystack_cli-0.1.1/paystack_cli/verification.py
+-rw-r--r--   0        0        0      819 2023-07-24 19:58:10.869694 paystack_cli-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1509 1970-01-01 00:00:00.000000 paystack_cli-0.1.1/PKG-INFO
```

### Comparing `paystack_cli-0.1.0/README.md` & `paystack_cli-0.1.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # paystack cli
 A command line app for interacting with [Paystack's](https://paystack.com/) API
 
 ![utility in use](./paystack-cli.png)
 
 ## Installation
-Binaries of paystack cli be found [here](). Alternatively, Paystack cli can be installed from pypi
+Binaries of paystack cli be found [here](https://github.com/gray-adeyi/kuda-cli/releases/tag/0.1.1). Alternatively, Paystack cli can be installed from pypi
 with pip as shown below.
 ```bash
 pip install paystack-cli
 ```
 
 ## First time configurations
 You're required to add your paystack auth_key on first use as shown below
 ```bash
 paystack config AUTH_KEY
 ```
 This sets up your paystack cli for use in development mode if the test secret key is used. This auth_key can be
-removed with `paystack reset`. Run `paystack --help` to see available commands
+removed with `paystack reset`. Run `paystack --help` to see available commands
+
+## Source code
+[https://github.com/gray-adeyi/paystack-cli](https://github.com/gray-adeyi/paystack-cli)
```

### Comparing `paystack_cli-0.1.0/paystack_cli/apple_pay.py` & `paystack_cli-0.1.1/paystack_cli/apple_pay.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.0/paystack_cli/bulk_charges.py` & `paystack_cli-0.1.1/paystack_cli/bulk_charges.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.0/paystack_cli/charge.py` & `paystack_cli-0.1.1/paystack_cli/charge.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.0/paystack_cli/customers.py` & `paystack_cli-0.1.1/paystack_cli/customers.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.0/paystack_cli/dedicated_virtual_accounts.py` & `paystack_cli-0.1.1/paystack_cli/dedicated_virtual_accounts.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.0/paystack_cli/disputes.py` & `paystack_cli-0.1.1/paystack_cli/disputes.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.0/paystack_cli/integration.py` & `paystack_cli-0.1.1/paystack_cli/integration.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.0/paystack_cli/main.py` & `paystack_cli-0.1.1/paystack_cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,15 +226,15 @@
     reset_settings()
     rprint("auth key cleared! :boom:")
 
 
 @app.command()
 def version():
     """See CLI version"""
-    rprint("Paystack CLI Version 0.1.0")
+    rprint("Paystack CLI Version 0.1.1")
 
 
 def run():
     app()
 
 
 if __name__ == "__main__":
```

### Comparing `paystack_cli-0.1.0/paystack_cli/miscellaneous.py` & `paystack_cli-0.1.1/paystack_cli/miscellaneous.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.0/paystack_cli/payment_pages.py` & `paystack_cli-0.1.1/paystack_cli/payment_pages.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.0/paystack_cli/payments_requests.py` & `paystack_cli-0.1.1/paystack_cli/payments_requests.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.0/paystack_cli/plans.py` & `paystack_cli-0.1.1/paystack_cli/plans.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.0/paystack_cli/products.py` & `paystack_cli-0.1.1/paystack_cli/products.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.0/paystack_cli/refunds.py` & `paystack_cli-0.1.1/paystack_cli/refunds.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.0/paystack_cli/settlements.py` & `paystack_cli-0.1.1/paystack_cli/settlements.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.0/paystack_cli/subaccounts.py` & `paystack_cli-0.1.1/paystack_cli/subaccounts.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.0/paystack_cli/subscriptions.py` & `paystack_cli-0.1.1/paystack_cli/subscriptions.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.0/paystack_cli/terminals.py` & `paystack_cli-0.1.1/paystack_cli/terminals.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.0/paystack_cli/transactions.py` & `paystack_cli-0.1.1/paystack_cli/transactions.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.0/paystack_cli/transactions_splits.py` & `paystack_cli-0.1.1/paystack_cli/transactions_splits.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.0/paystack_cli/transfer_recipients.py` & `paystack_cli-0.1.1/paystack_cli/transfer_recipients.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.0/paystack_cli/transfers.py` & `paystack_cli-0.1.1/paystack_cli/transfers.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.0/paystack_cli/transfers_control.py` & `paystack_cli-0.1.1/paystack_cli/transfers_control.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.0/paystack_cli/utils.py` & `paystack_cli-0.1.1/paystack_cli/utils.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.0/paystack_cli/verification.py` & `paystack_cli-0.1.1/paystack_cli/verification.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.0/pyproject.toml` & `paystack_cli-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "paystack-cli"
-version = "0.1.0"
+version = "0.1.1"
 description = "A command line app for interacting with Paystack's API"
 authors = ["Gbenga Adeyi <adeyigbenga005@gmail.com>"]
 readme = "README.md"
 packages = [{include = "paystack_cli"}]
 keywords = ["paystack-python", "pypaystack", "paystack", "paystackapi"]
 license = "MIT"
 classifiers = [
```

### Comparing `paystack_cli-0.1.0/PKG-INFO` & `paystack_cli-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paystack-cli
-Version: 0.1.0
+Version: 0.1.1
 Summary: A command line app for interacting with Paystack's API
 License: MIT
 Keywords: paystack-python,pypaystack,paystack,paystackapi
 Author: Gbenga Adeyi
 Author-email: adeyigbenga005@gmail.com
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
@@ -19,20 +19,23 @@
 
 # paystack cli
 A command line app for interacting with [Paystack's](https://paystack.com/) API
 
 ![utility in use](./paystack-cli.png)
 
 ## Installation
-Binaries of paystack cli be found [here](). Alternatively, Paystack cli can be installed from pypi
+Binaries of paystack cli be found [here](https://github.com/gray-adeyi/kuda-cli/releases/tag/0.1.1). Alternatively, Paystack cli can be installed from pypi
 with pip as shown below.
 ```bash
 pip install paystack-cli
 ```
 
 ## First time configurations
 You're required to add your paystack auth_key on first use as shown below
 ```bash
 paystack config AUTH_KEY
 ```
 This sets up your paystack cli for use in development mode if the test secret key is used. This auth_key can be
 removed with `paystack reset`. Run `paystack --help` to see available commands
+
+## Source code
+[https://github.com/gray-adeyi/paystack-cli](https://github.com/gray-adeyi/paystack-cli)
```

