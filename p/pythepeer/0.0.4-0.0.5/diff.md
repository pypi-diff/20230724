# Comparing `tmp/pythepeer-0.0.4.tar.gz` & `tmp/pythepeer-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/e-wave/Desktop/junkies/ogthepeer/dist/tmp2uhc_lxv/pythepeer-0.0.4.tar", last modified: Wed Jul 20 23:45:12 2022, max compression
+gzip compressed data, was "pythepeer-0.0.5.tar", last modified: Sun Jul 23 22:56:04 2023, max compression
```

## Comparing `pythepeer-0.0.4.tar` & `pythepeer-0.0.5.tar`

### file list

```diff
@@ -1,39 +1,19 @@
-drwxrwxr-x   0 e-wave    (1000) e-wave    (1000)        0 2022-07-20 23:45:12.000000 pythepeer-0.0.4/
-drwxrwxr-x   0 e-wave    (1000) e-wave    (1000)        0 2022-07-20 23:45:12.000000 pythepeer-0.0.4/.github/
-drwxrwxr-x   0 e-wave    (1000) e-wave    (1000)        0 2022-07-20 23:45:12.000000 pythepeer-0.0.4/.github/workflows/
--rw-rw-r--   0 e-wave    (1000) e-wave    (1000)     1147 2022-07-20 23:22:19.000000 pythepeer-0.0.4/.github/workflows/pytests.yml
--rw-rw-r--   0 e-wave    (1000) e-wave    (1000)     1852 2022-07-20 23:44:31.000000 pythepeer-0.0.4/.gitignore
--rw-rw-r--   0 e-wave    (1000) e-wave    (1000)      883 2022-05-18 21:14:03.000000 pythepeer-0.0.4/.pre-commit-config.yaml
--rw-rw-r--   0 e-wave    (1000) e-wave    (1000)       38 2022-05-06 22:34:48.000000 pythepeer-0.0.4/MANIFEST.in
--rw-rw-r--   0 e-wave    (1000) e-wave    (1000)    16217 2022-07-20 23:45:12.000000 pythepeer-0.0.4/PKG-INFO
--rw-rw-r--   0 e-wave    (1000) e-wave    (1000)    15300 2022-07-20 23:15:43.000000 pythepeer-0.0.4/README.md
--rw-rw-r--   0 e-wave    (1000) e-wave    (1000)       93 2022-05-26 22:26:40.000000 pythepeer-0.0.4/pyproject.toml
-drwxrwxr-x   0 e-wave    (1000) e-wave    (1000)        0 2022-07-20 23:45:12.000000 pythepeer-0.0.4/pythepeer.egg-info/
--rw-rw-r--   0 e-wave    (1000) e-wave    (1000)    16217 2022-07-20 23:45:12.000000 pythepeer-0.0.4/pythepeer.egg-info/PKG-INFO
--rw-rw-r--   0 e-wave    (1000) e-wave    (1000)      917 2022-07-20 23:45:12.000000 pythepeer-0.0.4/pythepeer.egg-info/SOURCES.txt
--rw-rw-r--   0 e-wave    (1000) e-wave    (1000)        1 2022-07-20 23:45:12.000000 pythepeer-0.0.4/pythepeer.egg-info/dependency_links.txt
--rw-rw-r--   0 e-wave    (1000) e-wave    (1000)        1 2022-05-18 21:19:30.000000 pythepeer-0.0.4/pythepeer.egg-info/not-zip-safe
--rw-rw-r--   0 e-wave    (1000) e-wave    (1000)        6 2022-07-20 23:45:12.000000 pythepeer-0.0.4/pythepeer.egg-info/requires.txt
--rw-rw-r--   0 e-wave    (1000) e-wave    (1000)        8 2022-07-20 23:45:12.000000 pythepeer-0.0.4/pythepeer.egg-info/top_level.txt
--rw-rw-r--   0 e-wave    (1000) e-wave    (1000)       21 2022-05-06 22:05:20.000000 pythepeer-0.0.4/requirements.txt
--rw-rw-r--   0 e-wave    (1000) e-wave    (1000)       38 2022-07-20 23:45:12.000000 pythepeer-0.0.4/setup.cfg
--rw-rw-r--   0 e-wave    (1000) e-wave    (1000)     1608 2022-07-20 23:22:48.000000 pythepeer-0.0.4/setup.py
-drwxrwxr-x   0 e-wave    (1000) e-wave    (1000)        0 2022-07-20 23:45:12.000000 pythepeer-0.0.4/thepeer/
--rw-rw-r--   0 e-wave    (1000) e-wave    (1000)       97 2022-07-20 23:15:43.000000 pythepeer-0.0.4/thepeer/__init__.py
--rw-rw-r--   0 e-wave    (1000) e-wave    (1000)     9286 2022-07-20 23:15:43.000000 pythepeer-0.0.4/thepeer/main.py
-drwxrwxr-x   0 e-wave    (1000) e-wave    (1000)        0 2022-07-20 23:45:12.000000 pythepeer-0.0.4/thepeer/utils/
--rw-rw-r--   0 e-wave    (1000) e-wave    (1000)        0 2022-05-06 20:45:11.000000 pythepeer-0.0.4/thepeer/utils/__init__.py
--rw-rw-r--   0 e-wave    (1000) e-wave    (1000)       36 2022-04-24 14:50:34.000000 pythepeer-0.0.4/thepeer/utils/constants.py
-drwxrwxr-x   0 e-wave    (1000) e-wave    (1000)        0 2022-07-20 23:45:12.000000 pythepeer-0.0.4/thepeer/utils/exceptions/
--rw-rw-r--   0 e-wave    (1000) e-wave    (1000)        0 2022-05-06 20:40:00.000000 pythepeer-0.0.4/thepeer/utils/exceptions/__init__.py
--rw-rw-r--   0 e-wave    (1000) e-wave    (1000)     1529 2022-05-01 10:52:53.000000 pythepeer-0.0.4/thepeer/utils/exceptions/handleErrors.py
-drwxrwxr-x   0 e-wave    (1000) e-wave    (1000)        0 2022-07-20 23:45:12.000000 pythepeer-0.0.4/thepeer/utils/exceptions/types/
--rw-rw-r--   0 e-wave    (1000) e-wave    (1000)        0 2022-05-06 20:40:15.000000 pythepeer-0.0.4/thepeer/utils/exceptions/types/__init__.py
--rw-rw-r--   0 e-wave    (1000) e-wave    (1000)      435 2022-04-24 14:50:34.000000 pythepeer-0.0.4/thepeer/utils/exceptions/types/base.py
--rw-rw-r--   0 e-wave    (1000) e-wave    (1000)      381 2022-04-24 15:13:46.000000 pythepeer-0.0.4/thepeer/utils/exceptions/types/forbidden.py
--rw-rw-r--   0 e-wave    (1000) e-wave    (1000)      418 2022-04-24 15:13:46.000000 pythepeer-0.0.4/thepeer/utils/exceptions/types/notacceptable.py
--rw-rw-r--   0 e-wave    (1000) e-wave    (1000)      382 2022-04-24 15:12:42.000000 pythepeer-0.0.4/thepeer/utils/exceptions/types/notfound.py
--rw-rw-r--   0 e-wave    (1000) e-wave    (1000)      425 2022-04-24 15:13:46.000000 pythepeer-0.0.4/thepeer/utils/exceptions/types/servererror.py
--rw-rw-r--   0 e-wave    (1000) e-wave    (1000)      471 2022-04-24 15:13:46.000000 pythepeer-0.0.4/thepeer/utils/exceptions/types/serviceunavailable.py
--rw-rw-r--   0 e-wave    (1000) e-wave    (1000)      390 2022-04-24 15:13:46.000000 pythepeer-0.0.4/thepeer/utils/exceptions/types/unauthorized.py
--rw-rw-r--   0 e-wave    (1000) e-wave    (1000)      690 2022-04-24 15:13:42.000000 pythepeer-0.0.4/thepeer/utils/exceptions/types/unprocessableentity.py
+drwxr-xr-x   0 e-wave     (502) staff       (20)        0 2023-07-23 22:56:04.790005 pythepeer-0.0.5/
+-rw-r--r--   0 e-wave     (502) staff       (20)       38 2023-07-22 21:36:52.000000 pythepeer-0.0.5/MANIFEST.in
+-rw-r--r--   0 e-wave     (502) staff       (20)    19125 2023-07-23 22:56:04.790400 pythepeer-0.0.5/PKG-INFO
+-rw-r--r--   0 e-wave     (502) staff       (20)    18157 2023-07-23 22:26:08.000000 pythepeer-0.0.5/README.md
+-rw-r--r--   0 e-wave     (502) staff       (20)       93 2023-07-22 21:36:52.000000 pythepeer-0.0.5/pyproject.toml
+drwxr-xr-x   0 e-wave     (502) staff       (20)        0 2023-07-23 22:56:04.787606 pythepeer-0.0.5/pythepeer.egg-info/
+-rw-r--r--   0 e-wave     (502) staff       (20)    19125 2023-07-23 22:56:04.000000 pythepeer-0.0.5/pythepeer.egg-info/PKG-INFO
+-rw-r--r--   0 e-wave     (502) staff       (20)      309 2023-07-23 22:56:04.000000 pythepeer-0.0.5/pythepeer.egg-info/SOURCES.txt
+-rw-r--r--   0 e-wave     (502) staff       (20)        1 2023-07-23 22:56:04.000000 pythepeer-0.0.5/pythepeer.egg-info/dependency_links.txt
+-rw-r--r--   0 e-wave     (502) staff       (20)        1 2023-07-23 22:56:04.000000 pythepeer-0.0.5/pythepeer.egg-info/not-zip-safe
+-rw-r--r--   0 e-wave     (502) staff       (20)        6 2023-07-23 22:56:04.000000 pythepeer-0.0.5/pythepeer.egg-info/requires.txt
+-rw-r--r--   0 e-wave     (502) staff       (20)        8 2023-07-23 22:56:04.000000 pythepeer-0.0.5/pythepeer.egg-info/top_level.txt
+-rw-r--r--   0 e-wave     (502) staff       (20)       38 2023-07-23 22:56:04.791341 pythepeer-0.0.5/setup.cfg
+-rw-r--r--   0 e-wave     (502) staff       (20)     1658 2023-07-23 22:40:35.000000 pythepeer-0.0.5/setup.py
+drwxr-xr-x   0 e-wave     (502) staff       (20)        0 2023-07-23 22:56:04.788112 pythepeer-0.0.5/tests/
+-rw-r--r--   0 e-wave     (502) staff       (20)     8493 2023-07-23 00:26:04.000000 pythepeer-0.0.5/tests/test_thepeer.py
+drwxr-xr-x   0 e-wave     (502) staff       (20)        0 2023-07-23 22:56:04.789483 pythepeer-0.0.5/thepeer/
+-rw-r--r--   0 e-wave     (502) staff       (20)       97 2023-07-22 21:36:52.000000 pythepeer-0.0.5/thepeer/__init__.py
+-rw-r--r--   0 e-wave     (502) staff       (20)    10727 2023-07-23 00:22:01.000000 pythepeer-0.0.5/thepeer/main.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pythepeer-0.0.4/PKG-INFO` & `pythepeer-0.0.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythepeer
-Version: 0.0.4
+Version: 0.0.5
 Summary: official python sdk for interacting with thepeer payment processing     infrastructure
 Home-page: https://github.com/thepeerstack/python-sdk
 Author: Osagie Iyayi
 Author-email: iyayiemmanuel1@gmail.com
 License: MIT
 Keywords: python,fintech,peer-to-peer
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 
 # Thepeer python-sdk
 
 ![example workflow](https://github.com/thepeerstack/python-sdk/actions/workflows/pytests.yml/badge.svg) ![PyPI - Downloads](https://img.shields.io/pypi/dm/pythepeer?style=flat-square) ![PyPI - License](https://img.shields.io/pypi/l/pythepeer) ![PyPI](https://img.shields.io/pypi/v/pythepeer) ![Codecov](https://img.shields.io/codecov/c/gh/E-wave112/py-thepeer?token=gYijsI9TCm)
 
@@ -34,30 +35,30 @@
 ```bash
 pip install pythepeer
 ```
 
 ## Usage
 Instantiate ```Thepeer``` class like so:
 ```python
-import thepeer
 from thepeer import Thepeer
 
-# create an instance of ThepeerInit class
+# create an instance of Thepeer class
 
 thepeer_instance = Thepeer("YOUR_API_KEY_HERE")
 
 ```
 
 ## Available methods exposed by the sdk
 
 **Note:**
  - For more info about the exposed methods, please refer to the general [documentation](https://docs.thepeer.co/)
  - Be sure to keep your API Credentials securely in [environment variables](https://www.twilio.com/blog/environment-variables-python)
+
 ### Indexing a user
-This describes how to index a user on your account (this is usually the first step before using other methods)
+This method describes how to index a user on your account (this is usually the first step before using other methods)
 
 ```python
 test = thepeer_instance.index_user("Osagie Iyayi", "iyayiemmanuel1@gmail.com", "iyayiemmanuel1@gmail.com")
 ```
 
 #### Parameters supported
 
@@ -108,15 +109,15 @@
 | Parameters           | Data type                 | Required | Description                                                                                                                                                                                                                                         |
 |----------------------|---------------------------|----------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | ```page```            | ```integer```               |  ```false```    | ```the first page displaying all the indexed users. defaults to 1```
 |  ```per_page```      | ```integer```                  | ```false```     | ```The number of users to display per page. defaults to 15          ```                                                          |
 
 
 ### Update an indexed user
-This methods helps to update the details of an indexed user
+This method helps to update the details of an indexed user
 
 ```python
 test = thepeer_instance.update_user(reference,**data)
 ```
 #### Parameters supported
 
 | Parameters           | Data type                 | Required | Description                                                                                                                                                                                                                                         |
@@ -127,65 +128,109 @@
 ### Sample
 ```python
 test = thepeer_instance.update_user("3bbb0fbf-82fa-48a0-80eb-d2c0338fe7dd", identifier="dwave101@yahoo.com",
     name="Edmond Kirsch",
     email="dwave101@gmail.com")
 ```
 ### Remove an indexed user
-This methods helps to remove the details of an indexed user from a specific account
+This method helps to remove the details of an indexed user from a specific account
 
 ```python
 test = thepeer_instance.delete_user("3bbb0fbf-82fa-48a0-80eb-d2c0338fe7dd")
 ```
 
 #### Parameters supported
 
 | Parameters           | Data type                 | Required | Description                                                                                                                                                                                                                                         |
 |----------------------|---------------------------|----------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | ```reference```            | ```string```                  |  ```true```    | ```the unique reference returned when the user was indexed```
 
+
+
+
+ ### Get Businesses
+This method returns businesses based on the API they integrated.
+
+```python
+test = thepeer_instance.get_businesses("checkout")
+```
+
+#### Parameters supported
+
+
+| Parameters           | Data type                 | Required | Description                                                                                                                                                                                                                                         |
+|----------------------|---------------------------|----------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| ```channel```            | ```string```                  |  ```true```    | ```The specific API to return businesses of. supported values are send, checkout, and direct_charge```
+
+
+### Generate a Checkout
+This method allows you to generate a link for your customer to make a one-time payment with
+```python
+test = thepeer_instance.generate_checkout({
+    "amount": 1000000,
+    "currency": "NGN",
+    "redirect_url": "https://esportfolio.netlify.app",
+    "email": "jevede6918@muzitp.com",
+    "meta":{
+        "name": "Eddie Kirsch",
+        "identifier": "eddiekirsch",
+    }
+})
+```
+
+#### Parameters required
+
+| Parameters           | Data type                 | Required | Description                                                                                                                                                                                                                                         |
+|----------------------|---------------------------|----------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| ```redirect_url```        | ```string```                   | ```false```     | ```The url Thepeer should redirect to after the customer completes payment.```
+| ```amount```            | ```integer```               |  ```true```    | ```The amount you are debiting the customer. This should be in kobo. The minimum value is 10000```
+| ```email```        | ```string```                   | ```true```     | ```The customer’s email address```                                                                     |
+| ```currency```               | ```string```                    | ```true```    | ```The currency the transaction should be carried out in. The supported value is NGN.```
+| ```meta```               | ```dictionary```                    | ```false```    | ```An object containing additional attributes you will like to have in your transaction response.```
+
+
 ### Get user links
 
-This method gets all payment links associated to an indexed user
+This method returns all linked accounts of a user, the user’s account details, as well as the business the account is on.
 ```python
 test = thepeer_instance.get_user_links("3bbb0fbf-82fa-48a0-80eb-d2c0338fe7dd")
 ```
 #### Parameters required
 
 | Parameters           | Data type                 | Required | Description                                                                                                                                                                                                                                         |
 |----------------------|---------------------------|----------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | ```reference```            | ```string```                  |  ```true```    | ```the unique reference returned when the user was indexed```
 
 
-### Get single link
+### Get single link (linked account)
 
-This method gets the payment information located in a payment link
+This method returns a user's linked account's details.
 
 ```python
 test = thepeer_instance.get_single_link("da14a90c-61c2-4cf7-a837-e3112a2d0c3d")
 ```
 
 #### Parameters required
 
 | Parameters           | Data type                 | Required | Description                                                                                                                                                                                                                                         |
 |----------------------|---------------------------|----------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| ```link_id```           | ```string```                  |  ```true```    | ```the unique link_id containing the payment information```
+| ```link_id```           | ```string```                  |  ```true```    | ```The link’s identifier```
 
 
 ### Charge a link
 This method allows a business to charge a user via their linked account
 ```python
 test = thepeer_instance.charge_link(link_id, amount, remark, currency)
 ```
 
 #### Parameters required
 
 | Parameters           | Data type                 | Required | Description                                                                                                                                                                                                                                         |
 |----------------------|---------------------------|----------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| ```link_id```        | ```string```                   | ```true```     | ```the unique link_id containing the payment information```
+| ```link_id```        | ```string```                   | ```true```     | ```The link’s identifier```
 | ```amount```            | ```integer```               |  ```true```    | ```the amount of the whole transaction```
 | ```remark```        | ```string```                   | ```true```     | ```short detail about the transaction```                                                                     |
 | ```currency```               | ```string```                    | ```false```    | ```The denomination medium of paying (either one of NGN and USD). defaults to NGN```
 
 ### Authorize charge
 This method allows a business to authorize a direct charge request made by a user
 
@@ -195,15 +240,15 @@
 #### Parameters required
 
 | Parameters           | Data type                 | Required | Description                                                                                                                                                                                                                                         |
 |----------------------|---------------------------|----------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | ```charge_reference```            | ```string```          |  ```true```   | ```the reference associated to a pending charge request```
 |  ```event```     | ```string```                | ```true```     | ```the type of webhook event```                                              |
 
-**Pro Tip:** the various types of webhook events are available [here](https://docs.thepeer.co/authorization/process-authorization-requests#supported-events)
+**Pro Tip:** the various types of webhook events are available [here](https://docs.thepeer.co/webhooks/overview)
 
 
 ### Get transaction detail
 This method gets the details of a transaction
 ```python
 test = thepeer_instance.get_transaction_detail("eda58ee3-4f2c-4aa4-9da7-10a2b8ced453")
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pythepeer-0.0.4/README.md` & `pythepeer-0.0.5/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -12,30 +12,30 @@
 ```bash
 pip install pythepeer
 ```
 
 ## Usage
 Instantiate ```Thepeer``` class like so:
 ```python
-import thepeer
 from thepeer import Thepeer
 
-# create an instance of ThepeerInit class
+# create an instance of Thepeer class
 
 thepeer_instance = Thepeer("YOUR_API_KEY_HERE")
 
 ```
 
 ## Available methods exposed by the sdk
 
 **Note:**
  - For more info about the exposed methods, please refer to the general [documentation](https://docs.thepeer.co/)
  - Be sure to keep your API Credentials securely in [environment variables](https://www.twilio.com/blog/environment-variables-python)
+
 ### Indexing a user
-This describes how to index a user on your account (this is usually the first step before using other methods)
+This method describes how to index a user on your account (this is usually the first step before using other methods)
 
 ```python
 test = thepeer_instance.index_user("Osagie Iyayi", "iyayiemmanuel1@gmail.com", "iyayiemmanuel1@gmail.com")
 ```
 
 #### Parameters supported
 
@@ -86,15 +86,15 @@
 | Parameters           | Data type                 | Required | Description                                                                                                                                                                                                                                         |
 |----------------------|---------------------------|----------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | ```page```            | ```integer```               |  ```false```    | ```the first page displaying all the indexed users. defaults to 1```
 |  ```per_page```      | ```integer```                  | ```false```     | ```The number of users to display per page. defaults to 15          ```                                                          |
 
 
 ### Update an indexed user
-This methods helps to update the details of an indexed user
+This method helps to update the details of an indexed user
 
 ```python
 test = thepeer_instance.update_user(reference,**data)
 ```
 #### Parameters supported
 
 | Parameters           | Data type                 | Required | Description                                                                                                                                                                                                                                         |
@@ -105,65 +105,109 @@
 ### Sample
 ```python
 test = thepeer_instance.update_user("3bbb0fbf-82fa-48a0-80eb-d2c0338fe7dd", identifier="dwave101@yahoo.com",
     name="Edmond Kirsch",
     email="dwave101@gmail.com")
 ```
 ### Remove an indexed user
-This methods helps to remove the details of an indexed user from a specific account
+This method helps to remove the details of an indexed user from a specific account
 
 ```python
 test = thepeer_instance.delete_user("3bbb0fbf-82fa-48a0-80eb-d2c0338fe7dd")
 ```
 
 #### Parameters supported
 
 | Parameters           | Data type                 | Required | Description                                                                                                                                                                                                                                         |
 |----------------------|---------------------------|----------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | ```reference```            | ```string```                  |  ```true```    | ```the unique reference returned when the user was indexed```
 
+
+
+
+ ### Get Businesses
+This method returns businesses based on the API they integrated.
+
+```python
+test = thepeer_instance.get_businesses("checkout")
+```
+
+#### Parameters supported
+
+
+| Parameters           | Data type                 | Required | Description                                                                                                                                                                                                                                         |
+|----------------------|---------------------------|----------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| ```channel```            | ```string```                  |  ```true```    | ```The specific API to return businesses of. supported values are send, checkout, and direct_charge```
+
+
+### Generate a Checkout
+This method allows you to generate a link for your customer to make a one-time payment with
+```python
+test = thepeer_instance.generate_checkout({
+    "amount": 1000000,
+    "currency": "NGN",
+    "redirect_url": "https://esportfolio.netlify.app",
+    "email": "jevede6918@muzitp.com",
+    "meta":{
+        "name": "Eddie Kirsch",
+        "identifier": "eddiekirsch",
+    }
+})
+```
+
+#### Parameters required
+
+| Parameters           | Data type                 | Required | Description                                                                                                                                                                                                                                         |
+|----------------------|---------------------------|----------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| ```redirect_url```        | ```string```                   | ```false```     | ```The url Thepeer should redirect to after the customer completes payment.```
+| ```amount```            | ```integer```               |  ```true```    | ```The amount you are debiting the customer. This should be in kobo. The minimum value is 10000```
+| ```email```        | ```string```                   | ```true```     | ```The customer’s email address```                                                                     |
+| ```currency```               | ```string```                    | ```true```    | ```The currency the transaction should be carried out in. The supported value is NGN.```
+| ```meta```               | ```dictionary```                    | ```false```    | ```An object containing additional attributes you will like to have in your transaction response.```
+
+
 ### Get user links
 
-This method gets all payment links associated to an indexed user
+This method returns all linked accounts of a user, the user’s account details, as well as the business the account is on.
 ```python
 test = thepeer_instance.get_user_links("3bbb0fbf-82fa-48a0-80eb-d2c0338fe7dd")
 ```
 #### Parameters required
 
 | Parameters           | Data type                 | Required | Description                                                                                                                                                                                                                                         |
 |----------------------|---------------------------|----------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | ```reference```            | ```string```                  |  ```true```    | ```the unique reference returned when the user was indexed```
 
 
-### Get single link
+### Get single link (linked account)
 
-This method gets the payment information located in a payment link
+This method returns a user's linked account's details.
 
 ```python
 test = thepeer_instance.get_single_link("da14a90c-61c2-4cf7-a837-e3112a2d0c3d")
 ```
 
 #### Parameters required
 
 | Parameters           | Data type                 | Required | Description                                                                                                                                                                                                                                         |
 |----------------------|---------------------------|----------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| ```link_id```           | ```string```                  |  ```true```    | ```the unique link_id containing the payment information```
+| ```link_id```           | ```string```                  |  ```true```    | ```The link’s identifier```
 
 
 ### Charge a link
 This method allows a business to charge a user via their linked account
 ```python
 test = thepeer_instance.charge_link(link_id, amount, remark, currency)
 ```
 
 #### Parameters required
 
 | Parameters           | Data type                 | Required | Description                                                                                                                                                                                                                                         |
 |----------------------|---------------------------|----------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| ```link_id```        | ```string```                   | ```true```     | ```the unique link_id containing the payment information```
+| ```link_id```        | ```string```                   | ```true```     | ```The link’s identifier```
 | ```amount```            | ```integer```               |  ```true```    | ```the amount of the whole transaction```
 | ```remark```        | ```string```                   | ```true```     | ```short detail about the transaction```                                                                     |
 | ```currency```               | ```string```                    | ```false```    | ```The denomination medium of paying (either one of NGN and USD). defaults to NGN```
 
 ### Authorize charge
 This method allows a business to authorize a direct charge request made by a user
 
@@ -173,15 +217,15 @@
 #### Parameters required
 
 | Parameters           | Data type                 | Required | Description                                                                                                                                                                                                                                         |
 |----------------------|---------------------------|----------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | ```charge_reference```            | ```string```          |  ```true```   | ```the reference associated to a pending charge request```
 |  ```event```     | ```string```                | ```true```     | ```the type of webhook event```                                              |
 
-**Pro Tip:** the various types of webhook events are available [here](https://docs.thepeer.co/authorization/process-authorization-requests#supported-events)
+**Pro Tip:** the various types of webhook events are available [here](https://docs.thepeer.co/webhooks/overview)
 
 
 ### Get transaction detail
 This method gets the details of a transaction
 ```python
 test = thepeer_instance.get_transaction_detail("eda58ee3-4f2c-4aa4-9da7-10a2b8ced453")
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pythepeer-0.0.4/pythepeer.egg-info/PKG-INFO` & `pythepeer-0.0.5/pythepeer.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythepeer
-Version: 0.0.4
+Version: 0.0.5
 Summary: official python sdk for interacting with thepeer payment processing     infrastructure
 Home-page: https://github.com/thepeerstack/python-sdk
 Author: Osagie Iyayi
 Author-email: iyayiemmanuel1@gmail.com
 License: MIT
 Keywords: python,fintech,peer-to-peer
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 
 # Thepeer python-sdk
 
 ![example workflow](https://github.com/thepeerstack/python-sdk/actions/workflows/pytests.yml/badge.svg) ![PyPI - Downloads](https://img.shields.io/pypi/dm/pythepeer?style=flat-square) ![PyPI - License](https://img.shields.io/pypi/l/pythepeer) ![PyPI](https://img.shields.io/pypi/v/pythepeer) ![Codecov](https://img.shields.io/codecov/c/gh/E-wave112/py-thepeer?token=gYijsI9TCm)
 
@@ -34,30 +35,30 @@
 ```bash
 pip install pythepeer
 ```
 
 ## Usage
 Instantiate ```Thepeer``` class like so:
 ```python
-import thepeer
 from thepeer import Thepeer
 
-# create an instance of ThepeerInit class
+# create an instance of Thepeer class
 
 thepeer_instance = Thepeer("YOUR_API_KEY_HERE")
 
 ```
 
 ## Available methods exposed by the sdk
 
 **Note:**
  - For more info about the exposed methods, please refer to the general [documentation](https://docs.thepeer.co/)
  - Be sure to keep your API Credentials securely in [environment variables](https://www.twilio.com/blog/environment-variables-python)
+
 ### Indexing a user
-This describes how to index a user on your account (this is usually the first step before using other methods)
+This method describes how to index a user on your account (this is usually the first step before using other methods)
 
 ```python
 test = thepeer_instance.index_user("Osagie Iyayi", "iyayiemmanuel1@gmail.com", "iyayiemmanuel1@gmail.com")
 ```
 
 #### Parameters supported
 
@@ -108,15 +109,15 @@
 | Parameters           | Data type                 | Required | Description                                                                                                                                                                                                                                         |
 |----------------------|---------------------------|----------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | ```page```            | ```integer```               |  ```false```    | ```the first page displaying all the indexed users. defaults to 1```
 |  ```per_page```      | ```integer```                  | ```false```     | ```The number of users to display per page. defaults to 15          ```                                                          |
 
 
 ### Update an indexed user
-This methods helps to update the details of an indexed user
+This method helps to update the details of an indexed user
 
 ```python
 test = thepeer_instance.update_user(reference,**data)
 ```
 #### Parameters supported
 
 | Parameters           | Data type                 | Required | Description                                                                                                                                                                                                                                         |
@@ -127,65 +128,109 @@
 ### Sample
 ```python
 test = thepeer_instance.update_user("3bbb0fbf-82fa-48a0-80eb-d2c0338fe7dd", identifier="dwave101@yahoo.com",
     name="Edmond Kirsch",
     email="dwave101@gmail.com")
 ```
 ### Remove an indexed user
-This methods helps to remove the details of an indexed user from a specific account
+This method helps to remove the details of an indexed user from a specific account
 
 ```python
 test = thepeer_instance.delete_user("3bbb0fbf-82fa-48a0-80eb-d2c0338fe7dd")
 ```
 
 #### Parameters supported
 
 | Parameters           | Data type                 | Required | Description                                                                                                                                                                                                                                         |
 |----------------------|---------------------------|----------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | ```reference```            | ```string```                  |  ```true```    | ```the unique reference returned when the user was indexed```
 
+
+
+
+ ### Get Businesses
+This method returns businesses based on the API they integrated.
+
+```python
+test = thepeer_instance.get_businesses("checkout")
+```
+
+#### Parameters supported
+
+
+| Parameters           | Data type                 | Required | Description                                                                                                                                                                                                                                         |
+|----------------------|---------------------------|----------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| ```channel```            | ```string```                  |  ```true```    | ```The specific API to return businesses of. supported values are send, checkout, and direct_charge```
+
+
+### Generate a Checkout
+This method allows you to generate a link for your customer to make a one-time payment with
+```python
+test = thepeer_instance.generate_checkout({
+    "amount": 1000000,
+    "currency": "NGN",
+    "redirect_url": "https://esportfolio.netlify.app",
+    "email": "jevede6918@muzitp.com",
+    "meta":{
+        "name": "Eddie Kirsch",
+        "identifier": "eddiekirsch",
+    }
+})
+```
+
+#### Parameters required
+
+| Parameters           | Data type                 | Required | Description                                                                                                                                                                                                                                         |
+|----------------------|---------------------------|----------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| ```redirect_url```        | ```string```                   | ```false```     | ```The url Thepeer should redirect to after the customer completes payment.```
+| ```amount```            | ```integer```               |  ```true```    | ```The amount you are debiting the customer. This should be in kobo. The minimum value is 10000```
+| ```email```        | ```string```                   | ```true```     | ```The customer’s email address```                                                                     |
+| ```currency```               | ```string```                    | ```true```    | ```The currency the transaction should be carried out in. The supported value is NGN.```
+| ```meta```               | ```dictionary```                    | ```false```    | ```An object containing additional attributes you will like to have in your transaction response.```
+
+
 ### Get user links
 
-This method gets all payment links associated to an indexed user
+This method returns all linked accounts of a user, the user’s account details, as well as the business the account is on.
 ```python
 test = thepeer_instance.get_user_links("3bbb0fbf-82fa-48a0-80eb-d2c0338fe7dd")
 ```
 #### Parameters required
 
 | Parameters           | Data type                 | Required | Description                                                                                                                                                                                                                                         |
 |----------------------|---------------------------|----------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | ```reference```            | ```string```                  |  ```true```    | ```the unique reference returned when the user was indexed```
 
 
-### Get single link
+### Get single link (linked account)
 
-This method gets the payment information located in a payment link
+This method returns a user's linked account's details.
 
 ```python
 test = thepeer_instance.get_single_link("da14a90c-61c2-4cf7-a837-e3112a2d0c3d")
 ```
 
 #### Parameters required
 
 | Parameters           | Data type                 | Required | Description                                                                                                                                                                                                                                         |
 |----------------------|---------------------------|----------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| ```link_id```           | ```string```                  |  ```true```    | ```the unique link_id containing the payment information```
+| ```link_id```           | ```string```                  |  ```true```    | ```The link’s identifier```
 
 
 ### Charge a link
 This method allows a business to charge a user via their linked account
 ```python
 test = thepeer_instance.charge_link(link_id, amount, remark, currency)
 ```
 
 #### Parameters required
 
 | Parameters           | Data type                 | Required | Description                                                                                                                                                                                                                                         |
 |----------------------|---------------------------|----------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| ```link_id```        | ```string```                   | ```true```     | ```the unique link_id containing the payment information```
+| ```link_id```        | ```string```                   | ```true```     | ```The link’s identifier```
 | ```amount```            | ```integer```               |  ```true```    | ```the amount of the whole transaction```
 | ```remark```        | ```string```                   | ```true```     | ```short detail about the transaction```                                                                     |
 | ```currency```               | ```string```                    | ```false```    | ```The denomination medium of paying (either one of NGN and USD). defaults to NGN```
 
 ### Authorize charge
 This method allows a business to authorize a direct charge request made by a user
 
@@ -195,15 +240,15 @@
 #### Parameters required
 
 | Parameters           | Data type                 | Required | Description                                                                                                                                                                                                                                         |
 |----------------------|---------------------------|----------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | ```charge_reference```            | ```string```          |  ```true```   | ```the reference associated to a pending charge request```
 |  ```event```     | ```string```                | ```true```     | ```the type of webhook event```                                              |
 
-**Pro Tip:** the various types of webhook events are available [here](https://docs.thepeer.co/authorization/process-authorization-requests#supported-events)
+**Pro Tip:** the various types of webhook events are available [here](https://docs.thepeer.co/webhooks/overview)
 
 
 ### Get transaction detail
 This method gets the details of a transaction
 ```python
 test = thepeer_instance.get_transaction_detail("eda58ee3-4f2c-4aa4-9da7-10a2b8ced453")
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pythepeer-0.0.4/setup.py` & `pythepeer-0.0.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 
 setup(
     name="pythepeer",
-    version="0.0.4",
+    version="0.0.5",
     description="official python sdk for interacting with thepeer payment processing \
     infrastructure",
     author="Osagie Iyayi",
     packages=["thepeer"],
     author_email="iyayiemmanuel1@gmail.com",
     url="https://github.com/thepeerstack/python-sdk",
     license="MIT",
@@ -32,14 +32,15 @@
         "Programming Language :: Python :: 3",
         # Specify which python versions that you want to support
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Libraries",
     ],
     long_description=README,
     long_description_content_type="text/markdown",
     keywords=["python", "fintech", "peer-to-peer"],
     zip_safe=False,
 )
```

### Comparing `pythepeer-0.0.4/thepeer/main.py` & `pythepeer-0.0.5/thepeer/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,71 @@
 import hmac
 import hashlib
 import json  # type: ignore
-import os
-import sys
 
 import httpx  # noqa: E402
 from .utils.constants import BASE_URL  # noqa: E402
 from .utils.exceptions.handleErrors import SwitchErrorStates  # noqa: E402
+from typing import Union
 
 
 class Thepeer:
-    def __init__(self, secret):
+    def __init__(self, secret: str):
         # pass a default value for the url
         self.url = BASE_URL
         self.secret = secret
         # set default headers to be used in all requests
         self.headers = {"x-api-key": self.secret, "content-Type": "application/json"}
 
-    def validate_signature(self, data, signature):
+    def get_businesses(self, channel: str):
+        """This endpoint returns businesses based on the API they integrated.
+        Args:
+            channel (string): The specific API to return businesses of.
+            Supported values are `send`, `checkout`, and `direct_charge`.
+        """
+        try:
+            response = httpx.get(
+                f"{self.url}/businesses?channel={channel}", headers=dict(self.headers)
+            )
+            return response.json()
+        except Exception as e:
+            raise SwitchErrorStates(e).switch()
+
+    def generate_checkout(self, data: dict[str, Union[str, int]]):
+        """
+        This is a checkout endpoint that you can use to generate a link for your customer to make a
+        one-time payment with.
+        Args:
+            data (dict): The request payload which contains the `currency` (NGN),
+            `amount`, `email`, and optionally `redirect_url` and `meta` fields.
+        """
+        try:
+            parsed_data = json.dumps(data)
+            response = httpx.post(
+                f"{self.url}/checkout", data=parsed_data, headers=dict(self.headers)
+            )
+            return response.json()
+        except Exception as e:
+            raise SwitchErrorStates(e).switch()
+
+    def validate_signature(self, data, signature: str):
         """helper method to validate the signature of the data received
         from thepeer's servers, it's usually used for validating webhook events
         coming from thepeer's servers
         Args:
             data (dict|Any): the payload to which the signature is applied
             signature (string): the signature to be validated
 
         Returns:
             _type_: boolean if the signature is valid or not
         """
         SHA1 = hashlib.sha1
         return signature == hmac.new(self.secret.encode(), data.encode(), SHA1).hexdigest()
 
-    def index_user(self, name, identifier, email):
+    def index_user(self, name: str, identifier: str, email: str):
 
         """this method helps identify the user on thepeer's servers in order to facilitate
         more usage of the SDK
         it is usually the first method called by the user
 
         Args:
             name (string): the name of the registered user
@@ -46,22 +76,22 @@
             dict: the json response from the server containing the user's id and
             other related information
         """
         try:
 
             data = {"name": name, "identifier": identifier, "email": email}
             # convert the data to json
-            data = json.dumps(data)
-            response = httpx.post(f"{self.url}/users", data=data, headers=dict(self.headers))
+            parsed_data = json.dumps(data)
+            response = httpx.post(f"{self.url}/users", data=parsed_data, headers=dict(self.headers))
             return response.json()
 
         except Exception as e:
             raise SwitchErrorStates(e).switch()
 
-    def view_user(self, reference):
+    def view_user(self, reference: str):
         """this method helps view the user's information on thepeer's servers
         it is usually called after the user has indexed himself
 
         Args:
             reference (string): the reference of the indexed user
 
         Returns:
@@ -89,51 +119,52 @@
             response = httpx.get(
                 f"{self.url}/users?page={page}&perPage={per_page}", headers=dict(self.headers)
             )
             return response.json()
         except Exception as e:
             raise SwitchErrorStates(e).switch()
 
-    def update_user(self, reference, **data):
+    def update_user(self, reference: str, **data):
         """this method helps update the user's information on thepeer's servers
         it is usually called after the user has indexed himself
 
         Args:
             reference (string): the reference of the indexed user
             data (dict): the data to be updated which is a dictionary
             of at least one of the fields (name, identifier, identifier_type,email)
 
         Returns:
             dict: the json response from the server containing the user's id and
             other related information
         """
         try:
-            data = json.dumps(data)
+            parsed_data = json.dumps(data)
             response = httpx.put(
-                f"{self.url}/users/{reference}", data=data, headers=dict(self.headers)
+                f"{self.url}/users/{reference}", data=parsed_data, headers=dict(self.headers)
             )
             return response.json()
         except Exception as e:
             raise SwitchErrorStates(e).switch()
 
-    def delete_user(self, reference):
+    def delete_user(self, reference: str):
         """this method helps delete the indexed user info on thepeer's servers
         a user can always reindex himself
 
         Args:
             reference (string): the reference of the indexed user
         """
         try:
             response = httpx.delete(f"{self.url}/users/{reference}", headers=dict(self.headers))
             return response.json()
         except Exception as e:
             raise SwitchErrorStates(e).switch()
 
-    def get_user_links(self, reference):
-        """this method helps to get the user's payment links on thepeer's servers
+    def get_user_links(self, reference: str):
+        """This endpoint returns all linked accounts of a user, the user's account details,
+          as well as the business the account is on.
 
 
         Args:
             reference (string): the reference of the indexed user
 
         Returns:
             dict: the json response from the server containing the linked accounts
@@ -141,16 +172,16 @@
         """
         try:
             response = httpx.get(f"{self.url}/users/{reference}/links", headers=dict(self.headers))
             return response.json()
         except Exception as e:
             raise SwitchErrorStates(e).switch()
 
-    def get_single_link(self, link_id):
-        """this method returns a user's linked account details on thepeer's servers
+    def get_single_link(self, link_id: str):
+        """This endpoint returns a user's linked account's details.
 
 
         Args:
             link_id (string): the link ID
 
         Returns:
             dict: the json response from the server containing the payment link id and
@@ -158,15 +189,15 @@
         """
         try:
             response = httpx.get(f"{self.url}/link/{link_id}", headers=dict(self.headers))
             return response.json()
         except Exception as e:
             raise SwitchErrorStates(e).switch()
 
-    def charge_link(self, link_id, amount, remark, currency="NGN"):
+    def charge_link(self, link_id: str, amount: Union[str, int], remark: str, currency="NGN"):
         """allows a business to charge a user via their linked account
 
         Args:
             link_id (string):the link ID
             data (dict): the request payload which contains the amount and remark and optionally,
             a currency (which could be NGN or USD default being NGN)
 
@@ -179,15 +210,15 @@
             response = httpx.post(
                 f"{self.url}/link/{link_id}/charge", data=data, headers=dict(self.headers)
             )
             return response.json()
         except Exception as e:
             raise SwitchErrorStates(e).switch()
 
-    def authorize_charge(self, charge_reference, event):
+    def authorize_charge(self, charge_reference: str, event: str):
         """allows a business to authorize a direct charge request made by a user
 
         Args:
             charge_reference (string): reference generated from the direct charge webhook event
             event (string): a string which contains the kind of webhook event
 
         Returns:
@@ -201,15 +232,15 @@
                 headers=dict(self.headers),
             )
             return response.json()
 
         except Exception as e:
             raise SwitchErrorStates(e).switch()
 
-    def get_transaction_detail(self, transaction_id):
+    def get_transaction_detail(self, transaction_id: str):
         """Get the details about a transaction
         Args:
             transaction_id (string): the unique identifier of the transaction
 
         Returns:
             dict:containing the transaction object. more about a transaction object here
             https://docs.thepeer.co/transaction/transaction-object#anatomy-of-a-transaction-object
@@ -218,15 +249,15 @@
             response = httpx.get(
                 f"{self.url}/transactions/{transaction_id}", headers=dict(self.headers)
             )
             return response.json()
         except Exception as e:
             raise SwitchErrorStates(e).switch()
 
-    def refund_transaction(self, transaction_id, reason):
+    def refund_transaction(self, transaction_id: str, reason: str):
 
         """This method allows a business to refund a transaction back to the user
         who made the transaction for obvious reasons.
 
         Args:
             transaction_id (string): the unique identifier of the transaction
             reason (string): a string explaining the reason for the refund
```

