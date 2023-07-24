# Comparing `tmp/otree-vcee-payment-0.8.1.tar.gz` & `tmp/otree_vcee_payment-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Philipp\PycharmProjects\otree-vcee-payment\dist\tmpprtgmeiz\otree-vcee-payment-0.8.1.tar", last modified: Thu May  6 09:31:28 2021, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `otree-vcee-payment-0.8.1.tar` & `otree_vcee_payment-0.9.0.tar`

### file list

```diff
@@ -1,28 +1,38 @@
-drwxrwxrwx   0        0        0        0 2021-05-06 09:31:28.908341 otree-vcee-payment-0.8.1/
--rw-rw-rw-   0        0        0      120 2021-04-26 11:02:12.000000 otree-vcee-payment-0.8.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1689 2021-05-06 09:31:28.908341 otree-vcee-payment-0.8.1/PKG-INFO
--rw-rw-rw-   0        0        0      705 2021-05-06 09:28:30.000000 otree-vcee-payment-0.8.1/README.rst
-drwxrwxrwx   0        0        0        0 2021-05-06 09:31:28.893340 otree-vcee-payment-0.8.1/otree_vcee_payment.egg-info/
--rw-rw-rw-   0        0        0     1689 2021-05-06 09:31:28.000000 otree-vcee-payment-0.8.1/otree_vcee_payment.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      602 2021-05-06 09:31:28.000000 otree-vcee-payment-0.8.1/otree_vcee_payment.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-05-06 09:31:28.000000 otree-vcee-payment-0.8.1/otree_vcee_payment.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2021-05-06 09:31:28.000000 otree-vcee-payment-0.8.1/otree_vcee_payment.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2021-05-06 09:31:28.000000 otree-vcee-payment-0.8.1/otree_vcee_payment.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      753 2021-05-06 09:31:28.909339 otree-vcee-payment-0.8.1/setup.cfg
--rw-rw-rw-   0        0        0       39 2021-04-26 10:57:28.000000 otree-vcee-payment-0.8.1/setup.py
-drwxrwxrwx   0        0        0        0 2021-05-06 09:31:28.900339 otree-vcee-payment-0.8.1/vceepayment/
--rw-rw-rw-   0        0        0        0 2021-01-28 11:20:50.000000 otree-vcee-payment-0.8.1/vceepayment/__init__.py
-drwxrwxrwx   0        0        0        0 2021-05-06 09:31:28.902339 otree-vcee-payment-0.8.1/vceepayment/_builtin/
--rw-rw-rw-   0        0        0      448 2021-01-28 11:20:50.000000 otree-vcee-payment-0.8.1/vceepayment/_builtin/__init__.py
--rw-rw-rw-   0        0        0     2176 2021-01-28 11:20:50.000000 otree-vcee-payment-0.8.1/vceepayment/encryption.py
--rw-rw-rw-   0        0        0     1282 2021-05-06 09:27:47.000000 otree-vcee-payment-0.8.1/vceepayment/models.py
--rw-rw-rw-   0        0        0     3791 2021-05-06 09:27:47.000000 otree-vcee-payment-0.8.1/vceepayment/pages.py
-drwxrwxrwx   0        0        0        0 2021-05-06 09:31:28.864339 otree-vcee-payment-0.8.1/vceepayment/static/
-drwxrwxrwx   0        0        0        0 2021-05-06 09:31:28.903340 otree-vcee-payment-0.8.1/vceepayment/static/vceepayment/
--rw-rw-rw-   0        0        0   166949 2021-01-28 11:20:50.000000 otree-vcee-payment-0.8.1/vceepayment/static/vceepayment/vcee_logo.jpg
-drwxrwxrwx   0        0        0        0 2021-05-06 09:31:28.865340 otree-vcee-payment-0.8.1/vceepayment/templates/
-drwxrwxrwx   0        0        0        0 2021-05-06 09:31:28.907339 otree-vcee-payment-0.8.1/vceepayment/templates/vceepayment/
--rw-rw-rw-   0        0        0     1139 2021-01-28 11:20:50.000000 otree-vcee-payment-0.8.1/vceepayment/templates/vceepayment/ConfirmationPage.html
--rw-rw-rw-   0        0        0     4722 2021-04-18 16:00:34.000000 otree-vcee-payment-0.8.1/vceepayment/templates/vceepayment/PaymentInfos.html
--rw-rw-rw-   0        0        0      523 2021-05-06 09:27:47.000000 otree-vcee-payment-0.8.1/vceepayment/templates/vceepayment/admin_report.html
--rw-rw-rw-   0        0        0     2588 2021-01-28 11:20:50.000000 otree-vcee-payment-0.8.1/vceepayment/tests.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/.flake8
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/.isort.cfg
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/Procfile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/__init__.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/manage.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/requirements.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/runtime.txt
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/_static/global/empty.css
+-rw-r--r--   0        0        0   166949 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/_static/vceepayment/vcee_logo.jpg
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/_templates/global/Page.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/vceepayment/__init__.py
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/vceepayment/encryption.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/vceepayment/models.py
+-rw-r--r--   0        0        0     3791 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/vceepayment/pages.py
+-rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/vceepayment/tests.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/vceepayment/_builtin/__init__.py
+-rw-r--r--   0        0        0   166949 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/vceepayment/static/vceepayment/vcee_logo.jpg
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/vceepayment/templates/vceepayment/ConfirmationPage.html
+-rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/vceepayment/templates/vceepayment/PaymentInfos.html
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/vceepayment/templates/vceepayment/admin_report.html
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/venvmac/pyvenv.cfg
+-rw-r--r--   0        0        0     8834 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/venvmac/bin/Activate.ps1
+-rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/venvmac/bin/activate
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/venvmac/bin/activate.csh
+-rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/venvmac/bin/activate.fish
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/venvmac/bin/django-admin
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/venvmac/bin/django-admin.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/venvmac/bin/otree
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/venvmac/bin/pip
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/venvmac/bin/pip3
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/venvmac/bin/pip3.8
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/venvmac/bin/sqlformat
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/.gitignore
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/README.rst
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/PKG-INFO
```

### Comparing `otree-vcee-payment-0.8.1/README.rst` & `otree_vcee_payment-0.9.0/README.rst`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -33,8 +33,8 @@
 ^^^^^^^^^^^^^^^^^^^^
 
 default: False
 
 disable_waiting_for_others
 ^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-default: False
+default: False
```

### Comparing `otree-vcee-payment-0.8.1/vceepayment/encryption.py` & `otree_vcee_payment-0.9.0/vceepayment/encryption.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-import base64
-
-from cryptography.hazmat.backends import default_backend
-from cryptography.hazmat.primitives import hashes, serialization
-from cryptography.hazmat.primitives.asymmetric import padding, rsa
-
-# Generates a private/public key pair, using rsa with key size 4096
-# key_size of 4096 is such an overkill
-# But given that we are not encrypting much, it shouldn't matter
-# public_exponent: commonly used one,
-
-
-def generate_key_pair():
-    """ Create private/public key pair and saves them. """
-    private_key = rsa.generate_private_key(
-        public_exponent=65537, key_size=4096, backend=default_backend()
-    )
-    public_key = private_key.public_key()
-
-    # Saving the private key
-    serial_private = private_key.private_bytes(
-        encoding=serialization.Encoding.PEM,
-        format=serialization.PrivateFormat.PKCS8,
-        encryption_algorithm=serialization.NoEncryption(),
-    )
-
-    with open("../private_noshare.pem", "wb") as f:
-        f.write(serial_private)
-
-    # Saving the public key
-    serial_pub = public_key.public_bytes(
-        encoding=serialization.Encoding.PEM,
-        format=serialization.PublicFormat.SubjectPublicKeyInfo,
-    )
-    with open("../public_shared.pem", "wb") as f:
-        f.write(serial_pub)
-
-
-def read_public_key(filename="public_shared.pem"):
-    with open("public_shared.pem", "rb") as key_file:
-        public_key = serialization.load_pem_public_key(
-            key_file.read(), backend=default_backend()
-        )
-    return public_key
-
-
-def encrypt_payment_data(payment_data: dict):
-    """Encrypt the payment data.
-    dict of payment data -> dict of encrypted payment data"""
-    public_key = read_public_key()
-    for key in payment_data.keys():
-        entry = bytes(str(payment_data[key]), "utf-8")
-        encrypted_entry = public_key.encrypt(
-            entry,
-            padding.OAEP(
-                mgf=padding.MGF1(algorithm=hashes.SHA256()),
-                algorithm=hashes.SHA256(),
-                label=None,
-            ),
-        )
-        payment_data[key] = base64.standard_b64encode(encrypted_entry)
-    return payment_data
+import base64
+
+from cryptography.hazmat.backends import default_backend
+from cryptography.hazmat.primitives import hashes, serialization
+from cryptography.hazmat.primitives.asymmetric import padding, rsa
+
+# Generates a private/public key pair, using rsa with key size 4096
+# key_size of 4096 is such an overkill
+# But given that we are not encrypting much, it shouldn't matter
+# public_exponent: commonly used one,
+
+
+def generate_key_pair():
+    """ Create private/public key pair and saves them. """
+    private_key = rsa.generate_private_key(
+        public_exponent=65537, key_size=4096, backend=default_backend()
+    )
+    public_key = private_key.public_key()
+
+    # Saving the private key
+    serial_private = private_key.private_bytes(
+        encoding=serialization.Encoding.PEM,
+        format=serialization.PrivateFormat.PKCS8,
+        encryption_algorithm=serialization.NoEncryption(),
+    )
+
+    with open("../private_noshare.pem", "wb") as f:
+        f.write(serial_private)
+
+    # Saving the public key
+    serial_pub = public_key.public_bytes(
+        encoding=serialization.Encoding.PEM,
+        format=serialization.PublicFormat.SubjectPublicKeyInfo,
+    )
+    with open("../public_shared.pem", "wb") as f:
+        f.write(serial_pub)
+
+
+def read_public_key(filename="public_shared.pem"):
+    with open("public_shared.pem", "rb") as key_file:
+        public_key = serialization.load_pem_public_key(
+            key_file.read(), backend=default_backend()
+        )
+    return public_key
+
+
+def encrypt_payment_data(payment_data: dict):
+    """Encrypt the payment data.
+    dict of payment data -> dict of encrypted payment data"""
+    public_key = read_public_key()
+    for key in payment_data.keys():
+        entry = bytes(str(payment_data[key]), "utf-8")
+        encrypted_entry = public_key.encrypt(
+            entry,
+            padding.OAEP(
+                mgf=padding.MGF1(algorithm=hashes.SHA256()),
+                algorithm=hashes.SHA256(),
+                label=None,
+            ),
+        )
+        payment_data[key] = base64.standard_b64encode(encrypted_entry)
+    return payment_data
```

### Comparing `otree-vcee-payment-0.8.1/vceepayment/models.py` & `otree_vcee_payment-0.9.0/vceepayment/models.py`

 * *Files identical despite different names*

### Comparing `otree-vcee-payment-0.8.1/vceepayment/pages.py` & `otree_vcee_payment-0.9.0/vceepayment/pages.py`

 * *Files identical despite different names*

### Comparing `otree-vcee-payment-0.8.1/vceepayment/static/vceepayment/vcee_logo.jpg` & `otree_vcee_payment-0.9.0/_static/vceepayment/vcee_logo.jpg`

 * *Files identical despite different names*

### Comparing `otree-vcee-payment-0.8.1/vceepayment/templates/vceepayment/ConfirmationPage.html` & `otree_vcee_payment-0.9.0/vceepayment/templates/vceepayment/ConfirmationPage.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,34 @@
-{% extends "global/Page.html" %}
-{% load otree static %}
-
-{% block head_title %}
-    Thank you!
-{% endblock %}
-
-{% block content %}
-    <div class="container-fluid">
-        <div class="row mb-4">
-            <div class="col-md-8 header mr-auto">
-                <img src="{% static "vceepayment/vcee_logo.jpg" %}" class="img-fluid"/>
-            </div>
-        </div>
-        <div class="row">
-            <div class="col-12">
-                <p>
-                    Thank you for submitting your bank details.
-                    We will now process your payment.
-                </p>
-
-                <p>
-                    You should receive your payment within a week.
-                    If you have not received it after 14 days, please contact us at <a href="mailto:vcee@univie.ac.at?subject=Feedback Online Experiment">vcee@univie.ac.at</a> with your full name and the date and time of the experiment.
-                    Remember that we will delete your data after four weeks, so please contact us before that time.
-                </p>
-            </div>
-        </div>
-    </div>
-{% endblock %}
+{% extends "global/Page.html" %}
+{% load otree static %}
+
+{% block head_title %}
+    Thank you!
+{% endblock %}
+
+{% block content %}
+    <div class="container-fluid">
+        <div class="row mb-4">
+            <div class="col-md-8 header mr-auto">
+                <img src="{% static "vceepayment/vcee_logo.jpg" %}" class="img-fluid"/>
+            </div>
+        </div>
+        <div class="row mb-4">
+            <div class="col-12">
+                <p>
+                    Thank you for submitting your bank details.
+                    We will now process your payment.
+                </p>
+
+                <p>
+                    If you have not received your payment after 14 days, please contact us at
+                    <a href="mailto:vcee@univie.ac.at?subject=Feedback Online Experiment">vcee@univie.ac.at</a>
+                    with your full name and the date and time of the experiment.
+                </p>
+
+                <h4>Thank you again for your participation!</h4>
+
+                <h4>You can close this window and leave the experiment.</h4>
+            </div>
+        </div>
+    </div>
+{% endblock %}
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 {% extends "global/Page.html" %} {% load otree static %} {% block head_title %}
 Thank you! {% endblock %} {% block content %}
 cee_logo.jpg" %}" class="img-fluid"/>
 Thank you for submitting your bank details. We will now process your payment.
-You should receive your payment within a week. If you have not received it
-after 14 days, please contact us at vcee@univie.ac.at with your full name and
-the date and time of the experiment. Remember that we will delete your data
-after four weeks, so please contact us before that time.
+If you have not received your payment after 14 days, please contact us at
+vcee@univie.ac.at with your full name and the date and time of the experiment.
+*** Thank you again for your participation! ***
+*** You can close this window and leave the experiment. ***
 {% endblock %}
```

### Comparing `otree-vcee-payment-0.8.1/vceepayment/templates/vceepayment/PaymentInfos.html` & `otree_vcee_payment-0.9.0/vceepayment/templates/vceepayment/PaymentInfos.html`

 * *Files 4% similar despite different names*

```diff
@@ -44,36 +44,26 @@
                 <p>
                     To process your payment, we will share your bank details with the Accounting and Finance Service of the University of Vienna.
                     We will not share it with anyone else, including the experimenter.
                 </p>
 
                 <h4>Security</h4>
 
-                <p>We will automatically remove your payment information after four weeks.</p>
-
                 <p>
                     Due to security reasons, we will not be able to change your bank details after you have submitted them.
                     Thus, we ask you to make sure the information you enter is correct.
                     In particular, please write your name as it is written in your bank account and on the ORSEE platform you signed up with.
                 </p>
                     <div class="form-check m-4">
                         <input type="checkbox" class="form-check-input" id="accept_checkbox">
                         <label class="form-check-label" for="accept_checkbox">I have read and understood the information above.</label>
                     </div>
             </div>
         </div>
 
-
-    <!--
-        <div class="bg-warning">
-            Test data: <br>
-            DE40100100100000012345 <br>
-            GENO DE M1 GLS
-        </div>
-    -->
             <div class="collapse" id="input-fields">
                 <div class="form-group row p-t-5">
                     <label for="FullName" class="col-sm-2 col-form-label">Full Name</label>
                     <div class="col-sm-10">
                         <input type="text" class="form-control" id="FullName" placeholder="Firstname Lastname" name="full_name" value="{{ saved.full_name }}">
                         <small id="FullName" class="form-text text-muted">This name needs to match the name you use on your bank account and on the ORSEE recruitment platform.</small>
                     </div>
```

### Comparing `otree-vcee-payment-0.8.1/vceepayment/templates/vceepayment/admin_report.html` & `otree_vcee_payment-0.9.0/vceepayment/templates/vceepayment/admin_report.html`

 * *Files identical despite different names*

### Comparing `otree-vcee-payment-0.8.1/vceepayment/tests.py` & `otree_vcee_payment-0.9.0/vceepayment/tests.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-from itertools import product
-
-from otree.api import Submission, SubmissionMustFail
-
-from . import pages
-from ._builtin import Bot
-
-correct_names = [
-    "Detlef Mueller",
-    "Detlef Müller",
-    "Detlef Hans Dieter Müller",
-    " Detlef Hans Dieter Müller  ",
-]
-
-
-incorrect_names = ["ichnureinennamenhaben", "Chloé IsNotAllowed", "陈玉"]
-
-# Combination iban + bic
-correct_iban_bic = [
-    ["DE40100100100000012345", ""],
-    ["DE75512108001245126199", ""],
-    ["de75512108001245126199", ""],
-    ["de 75 512 108 001 245  126199", ""],
-    ["DE75512108001245126199", "-"],
-    ["DE75512108001245126199", "nix"],
-    ["GR1601101250000000012300695", "ETHNGRAA"],
-    ["GB33BUKB20201555555555", "BUKBGB22"],
-    ["FR7630006000011234567890189", "AGRIFRPP"],
-    ["AT611904300234573201", "GIBAATWW"],
-    ["AT611904300234573201", ""],
-]
-
-incorrect_iban_bic = [
-    ["DE40100100100000012346", ""],
-    ["GR1601101250000000012300695", ""],
-    ["GB33BUKB20201555555555", ""],
-    ["FR7630006000011234567890189", ""],
-    ["AT6119043002345732012", "GIBAATWW"],
-    ["AT61190430023453201", "GIBAATWW"],
-]
-
-all_good_cases = product(correct_names, correct_iban_bic)
-all_bad_cases_1 = product(correct_names, incorrect_iban_bic)
-all_bad_cases_2 = product(incorrect_names, correct_iban_bic)
-all_very_bad_cases = product(incorrect_names, incorrect_iban_bic)
-
-
-all_good_cases_dict = [
-    {"full_name": entry[0], "iban": entry[1][0], "bic": entry[1][1], "is_correct": True}
-    for entry in all_good_cases
-]
-
-all_bad_cases_dict_1 = [
-    {
-        "full_name": entry[0],
-        "iban": entry[1][0],
-        "bic": entry[1][1],
-        "is_correct": False,
-    }
-    for entry in all_bad_cases_1
-]
-
-all_bad_cases_dict_2 = [
-    {
-        "full_name": entry[0],
-        "iban": entry[1][0],
-        "bic": entry[1][1],
-        "is_correct": False,
-    }
-    for entry in all_bad_cases_2
-]
-
-all_very_bad_cases_dict = [
-    {
-        "full_name": entry[0],
-        "iban": entry[1][0],
-        "bic": entry[1][1],
-        "is_correct": False,
-    }
-    for entry in all_very_bad_cases
-]
-
-all_cases = (
-    all_good_cases_dict
-    + all_bad_cases_dict_1
-    + all_bad_cases_dict_2
-    + all_very_bad_cases_dict
-)
-
-
-class PlayerBot(Bot):
-
-    cases = all_cases
-
-    def play_round(self):
-        if self.case["is_correct"]:
-            yield Submission(pages.PaymentInfos, self.case, check_html=False)
-        else:
-            yield SubmissionMustFail(pages.PaymentInfos, self.case, check_html=False)
+from itertools import product
+
+from otree.api import Submission, SubmissionMustFail
+
+from . import pages
+from ._builtin import Bot
+
+correct_names = [
+    "Detlef Mueller",
+    "Detlef Müller",
+    "Detlef Hans Dieter Müller",
+    " Detlef Hans Dieter Müller  ",
+]
+
+
+incorrect_names = ["ichnureinennamenhaben", "Chloé IsNotAllowed", "陈玉"]
+
+# Combination iban + bic
+correct_iban_bic = [
+    ["DE40100100100000012345", ""],
+    ["DE75512108001245126199", ""],
+    ["de75512108001245126199", ""],
+    ["de 75 512 108 001 245  126199", ""],
+    ["DE75512108001245126199", "-"],
+    ["DE75512108001245126199", "nix"],
+    ["GR1601101250000000012300695", "ETHNGRAA"],
+    ["GB33BUKB20201555555555", "BUKBGB22"],
+    ["FR7630006000011234567890189", "AGRIFRPP"],
+    ["AT611904300234573201", "GIBAATWW"],
+    ["AT611904300234573201", ""],
+]
+
+incorrect_iban_bic = [
+    ["DE40100100100000012346", ""],
+    ["GR1601101250000000012300695", ""],
+    ["GB33BUKB20201555555555", ""],
+    ["FR7630006000011234567890189", ""],
+    ["AT6119043002345732012", "GIBAATWW"],
+    ["AT61190430023453201", "GIBAATWW"],
+]
+
+all_good_cases = product(correct_names, correct_iban_bic)
+all_bad_cases_1 = product(correct_names, incorrect_iban_bic)
+all_bad_cases_2 = product(incorrect_names, correct_iban_bic)
+all_very_bad_cases = product(incorrect_names, incorrect_iban_bic)
+
+
+all_good_cases_dict = [
+    {"full_name": entry[0], "iban": entry[1][0], "bic": entry[1][1], "is_correct": True}
+    for entry in all_good_cases
+]
+
+all_bad_cases_dict_1 = [
+    {
+        "full_name": entry[0],
+        "iban": entry[1][0],
+        "bic": entry[1][1],
+        "is_correct": False,
+    }
+    for entry in all_bad_cases_1
+]
+
+all_bad_cases_dict_2 = [
+    {
+        "full_name": entry[0],
+        "iban": entry[1][0],
+        "bic": entry[1][1],
+        "is_correct": False,
+    }
+    for entry in all_bad_cases_2
+]
+
+all_very_bad_cases_dict = [
+    {
+        "full_name": entry[0],
+        "iban": entry[1][0],
+        "bic": entry[1][1],
+        "is_correct": False,
+    }
+    for entry in all_very_bad_cases
+]
+
+all_cases = (
+    all_good_cases_dict
+    + all_bad_cases_dict_1
+    + all_bad_cases_dict_2
+    + all_very_bad_cases_dict
+)
+
+
+class PlayerBot(Bot):
+
+    cases = all_cases
+
+    def play_round(self):
+        if self.case["is_correct"]:
+            yield Submission(pages.PaymentInfos, self.case, check_html=False)
+        else:
+            yield SubmissionMustFail(pages.PaymentInfos, self.case, check_html=False)
```

