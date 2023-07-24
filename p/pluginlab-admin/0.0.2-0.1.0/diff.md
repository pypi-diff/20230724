# Comparing `tmp/pluginlab_admin-0.0.2.tar.gz` & `tmp/pluginlab_admin-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pluginlab_admin-0.0.2.tar", last modified: Sun Jul 23 16:18:19 2023, max compression
+gzip compressed data, was "pluginlab_admin-0.1.0.tar", last modified: Mon Jul 24 21:03:53 2023, max compression
```

## Comparing `pluginlab_admin-0.0.2.tar` & `pluginlab_admin-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 aurelienbrabant   (501) staff       (20)        0 2023-07-23 16:18:19.831738 pluginlab_admin-0.0.2/
--rw-r--r--   0 aurelienbrabant   (501) staff       (20)       18 2023-07-23 16:14:55.000000 pluginlab_admin-0.0.2/MANIFEST.in
--rw-r--r--   0 aurelienbrabant   (501) staff       (20)      140 2023-07-23 16:18:19.831629 pluginlab_admin-0.0.2/PKG-INFO
--rw-r--r--   0 aurelienbrabant   (501) staff       (20)     4730 2023-07-23 16:02:59.000000 pluginlab_admin-0.0.2/README.md
-drwxr-xr-x   0 aurelienbrabant   (501) staff       (20)        0 2023-07-23 16:18:19.830893 pluginlab_admin-0.0.2/pluginlab_admin/
--rw-r--r--   0 aurelienbrabant   (501) staff       (20)       66 2023-07-23 15:50:42.000000 pluginlab_admin-0.0.2/pluginlab_admin/__init__.py
--rw-r--r--   0 aurelienbrabant   (501) staff       (20)      909 2023-07-23 14:10:44.000000 pluginlab_admin-0.0.2/pluginlab_admin/app.py
--rw-r--r--   0 aurelienbrabant   (501) staff       (20)     6337 2023-07-23 14:10:40.000000 pluginlab_admin-0.0.2/pluginlab_admin/auth.py
--rw-r--r--   0 aurelienbrabant   (501) staff       (20)      612 2023-07-23 01:01:56.000000 pluginlab_admin-0.0.2/pluginlab_admin/token_verifier.py
--rw-r--r--   0 aurelienbrabant   (501) staff       (20)      894 2023-07-23 13:09:00.000000 pluginlab_admin-0.0.2/pluginlab_admin/webhook.py
-drwxr-xr-x   0 aurelienbrabant   (501) staff       (20)        0 2023-07-23 16:18:19.831470 pluginlab_admin-0.0.2/pluginlab_admin.egg-info/
--rw-r--r--   0 aurelienbrabant   (501) staff       (20)      140 2023-07-23 16:18:19.000000 pluginlab_admin-0.0.2/pluginlab_admin.egg-info/PKG-INFO
--rw-r--r--   0 aurelienbrabant   (501) staff       (20)      360 2023-07-23 16:18:19.000000 pluginlab_admin-0.0.2/pluginlab_admin.egg-info/SOURCES.txt
--rw-r--r--   0 aurelienbrabant   (501) staff       (20)        1 2023-07-23 16:18:19.000000 pluginlab_admin-0.0.2/pluginlab_admin.egg-info/dependency_links.txt
--rw-r--r--   0 aurelienbrabant   (501) staff       (20)       52 2023-07-23 16:18:19.000000 pluginlab_admin-0.0.2/pluginlab_admin.egg-info/requires.txt
--rw-r--r--   0 aurelienbrabant   (501) staff       (20)       16 2023-07-23 16:18:19.000000 pluginlab_admin-0.0.2/pluginlab_admin.egg-info/top_level.txt
--rw-r--r--   0 aurelienbrabant   (501) staff       (20)       38 2023-07-23 16:18:19.831776 pluginlab_admin-0.0.2/setup.cfg
--rw-r--r--   0 aurelienbrabant   (501) staff       (20)      267 2023-07-23 16:18:11.000000 pluginlab_admin-0.0.2/setup.py
+drwxr-xr-x   0 aurelienbrabant   (501) staff       (20)        0 2023-07-24 21:03:53.163233 pluginlab_admin-0.1.0/
+-rw-r--r--   0 aurelienbrabant   (501) staff       (20)       18 2023-07-23 16:14:55.000000 pluginlab_admin-0.1.0/MANIFEST.in
+-rw-r--r--   0 aurelienbrabant   (501) staff       (20)      140 2023-07-24 21:03:53.163112 pluginlab_admin-0.1.0/PKG-INFO
+-rw-r--r--   0 aurelienbrabant   (501) staff       (20)     5522 2023-07-24 20:58:53.000000 pluginlab_admin-0.1.0/README.md
+drwxr-xr-x   0 aurelienbrabant   (501) staff       (20)        0 2023-07-24 21:03:53.162342 pluginlab_admin-0.1.0/pluginlab_admin/
+-rw-r--r--   0 aurelienbrabant   (501) staff       (20)       66 2023-07-23 15:50:42.000000 pluginlab_admin-0.1.0/pluginlab_admin/__init__.py
+-rw-r--r--   0 aurelienbrabant   (501) staff       (20)      909 2023-07-23 14:10:44.000000 pluginlab_admin-0.1.0/pluginlab_admin/app.py
+-rw-r--r--   0 aurelienbrabant   (501) staff       (20)     6337 2023-07-23 14:10:40.000000 pluginlab_admin-0.1.0/pluginlab_admin/auth.py
+-rw-r--r--   0 aurelienbrabant   (501) staff       (20)     1646 2023-07-24 20:49:47.000000 pluginlab_admin-0.1.0/pluginlab_admin/token_verifier.py
+-rw-r--r--   0 aurelienbrabant   (501) staff       (20)      894 2023-07-23 13:09:00.000000 pluginlab_admin-0.1.0/pluginlab_admin/webhook.py
+drwxr-xr-x   0 aurelienbrabant   (501) staff       (20)        0 2023-07-24 21:03:53.162945 pluginlab_admin-0.1.0/pluginlab_admin.egg-info/
+-rw-r--r--   0 aurelienbrabant   (501) staff       (20)      140 2023-07-24 21:03:53.000000 pluginlab_admin-0.1.0/pluginlab_admin.egg-info/PKG-INFO
+-rw-r--r--   0 aurelienbrabant   (501) staff       (20)      360 2023-07-24 21:03:53.000000 pluginlab_admin-0.1.0/pluginlab_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 aurelienbrabant   (501) staff       (20)        1 2023-07-24 21:03:53.000000 pluginlab_admin-0.1.0/pluginlab_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 aurelienbrabant   (501) staff       (20)       52 2023-07-24 21:03:53.000000 pluginlab_admin-0.1.0/pluginlab_admin.egg-info/requires.txt
+-rw-r--r--   0 aurelienbrabant   (501) staff       (20)       16 2023-07-24 21:03:53.000000 pluginlab_admin-0.1.0/pluginlab_admin.egg-info/top_level.txt
+-rw-r--r--   0 aurelienbrabant   (501) staff       (20)       38 2023-07-24 21:03:53.163280 pluginlab_admin-0.1.0/setup.cfg
+-rw-r--r--   0 aurelienbrabant   (501) staff       (20)      267 2023-07-24 21:03:22.000000 pluginlab_admin-0.1.0/setup.py
```

### Comparing `pluginlab_admin-0.0.2/README.md` & `pluginlab_admin-0.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -33,19 +33,51 @@
 auth = app.get_auth();
 
 # usually you'd get the token from the Authorization header of the HTTP request, formatted as `Bearer <token>`
 token = "eyJhbGc...dQssw5c"
 
 try:
     payload = auth.verify_token(token)
+    # from that point we know the information in the token hasn't been tampered with
+
+    # we could, for instance, check if the user has a given plan and take specific action based on that
+    premium_plan_id = 'KWsmKyJnHBF2Dz1mETDF';
+    plan_id = payload.user.plan_id;
+
+    if plan_id:
+        if plan_id == premium_plan_id: 
+            do_something_special()
+        else
+            do_other_stuff()
+
     print(payload.uid)
 except Exception as e:
     print(f"An error occurred while verifying the token: {e}")
 ```
 
+The verified token payload is represented by the following typings:
+
+```python
+class TokenPayloadUser:
+    id: str
+    email: str
+    name: Optional[str] = None
+    given_name: Optional[str] = None
+    plan_id: Optional[str] = None
+    price_id: Optional[str] = None
+
+class TokenPayload:
+    uid: str
+    iss: str
+    aud: str
+    iat: int
+    exp: int
+    user: TokenPayloadUser
+```
+
 ## Get a member by id or email
 
 ### By email
 
 
 ```python
 member = auth.get_member_by_email('johndoe@example.com')
```

### Comparing `pluginlab_admin-0.0.2/pluginlab_admin/app.py` & `pluginlab_admin-0.1.0/pluginlab_admin/app.py`

 * *Files identical despite different names*

### Comparing `pluginlab_admin-0.0.2/pluginlab_admin/auth.py` & `pluginlab_admin-0.1.0/pluginlab_admin/auth.py`

 * *Files identical despite different names*

### Comparing `pluginlab_admin-0.0.2/pluginlab_admin/webhook.py` & `pluginlab_admin-0.1.0/pluginlab_admin/webhook.py`

 * *Files identical despite different names*

