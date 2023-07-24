# Comparing `tmp/allianceauth_oidc_provider-0.0.1a3.tar.gz` & `tmp/allianceauth_oidc_provider-0.0.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allianceauth_oidc_provider-0.0.1a3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "allianceauth_oidc_provider-0.0.1b1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `allianceauth_oidc_provider-0.0.1a3.tar` & `allianceauth_oidc_provider-0.0.1b1.tar`

### file list

```diff
@@ -1,35 +1,37 @@
--rw-r--r--   0        0        0      347 2023-07-20 04:37:14.551222 allianceauth_oidc_provider-0.0.1a3/.coveragerc
--rw-r--r--   0        0        0     1342 2023-07-20 04:37:14.551222 allianceauth_oidc_provider-0.0.1a3/.github/workflows/main.yml
--rw-r--r--   0        0        0      718 2023-07-20 04:37:14.551222 allianceauth_oidc_provider-0.0.1a3/.github/workflows/publish.yml
--rw-r--r--   0        0        0     2116 2023-07-20 04:37:14.551222 allianceauth_oidc_provider-0.0.1a3/.gitignore
--rw-r--r--   0        0        0      631 2023-07-20 04:37:14.551222 allianceauth_oidc_provider-0.0.1a3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      139 2023-07-20 04:37:14.551222 allianceauth_oidc_provider-0.0.1a3/.prettierignore
--rw-r--r--   0        0        0       88 2023-07-20 04:37:14.551222 allianceauth_oidc_provider-0.0.1a3/.prettierrc
--rw-r--r--   0        0        0     1077 2023-07-20 04:37:14.551222 allianceauth_oidc_provider-0.0.1a3/LICENSE
--rw-r--r--   0        0        0      630 2023-07-20 04:37:14.551222 allianceauth_oidc_provider-0.0.1a3/Makefile
--rw-r--r--   0        0        0     1136 2023-07-20 04:37:14.551222 allianceauth_oidc_provider-0.0.1a3/README.md
--rw-r--r--   0        0        0      122 2023-07-20 04:37:14.551222 allianceauth_oidc_provider-0.0.1a3/allianceauth_oidc/__init__.py
--rw-r--r--   0        0        0      647 2023-07-20 04:37:14.551222 allianceauth_oidc_provider-0.0.1a3/allianceauth_oidc/admin.py
--rw-r--r--   0        0        0      281 2023-07-20 04:37:14.551222 allianceauth_oidc_provider-0.0.1a3/allianceauth_oidc/apps.py
--rw-r--r--   0        0        0        0 2023-07-20 04:37:14.551222 allianceauth_oidc_provider-0.0.1a3/allianceauth_oidc/auth_hooks.py
--rw-r--r--   0        0        0      836 2023-07-20 04:37:14.551222 allianceauth_oidc_provider-0.0.1a3/allianceauth_oidc/auth_provider.py
--rw-r--r--   0        0        0     3037 2023-07-20 04:37:14.551222 allianceauth_oidc_provider-0.0.1a3/allianceauth_oidc/migrations/0001_initial.py
--rw-r--r--   0        0        0      613 2023-07-20 04:37:14.551222 allianceauth_oidc_provider-0.0.1a3/allianceauth_oidc/migrations/0002_alter_allianceauthapplication_options_and_more.py
--rw-r--r--   0        0        0        0 2023-07-20 04:37:14.551222 allianceauth_oidc_provider-0.0.1a3/allianceauth_oidc/migrations/__init__.py
--rw-r--r--   0        0        0      772 2023-07-20 04:37:14.551222 allianceauth_oidc_provider-0.0.1a3/allianceauth_oidc/models.py
--rw-r--r--   0        0        0      186 2023-07-20 04:37:14.551222 allianceauth_oidc_provider-0.0.1a3/allianceauth_oidc/signals.py
--rw-r--r--   0        0        0     1392 2023-07-20 04:37:14.551222 allianceauth_oidc_provider-0.0.1a3/allianceauth_oidc/templates/allianceauth_oidc/authorize.html
--rw-r--r--   0        0        0     1294 2023-07-20 04:37:14.551222 allianceauth_oidc_provider-0.0.1a3/allianceauth_oidc/templates/allianceauth_oidc/base.html
--rw-r--r--   0        0        0     2449 2023-07-20 04:37:14.551222 allianceauth_oidc_provider-0.0.1a3/allianceauth_oidc/templates/allianceauth_oidc/denied.html
--rw-r--r--   0        0        0     1268 2023-07-20 04:37:14.551222 allianceauth_oidc_provider-0.0.1a3/allianceauth_oidc/templates/allianceauth_oidc/logout_confirm.html
--rw-r--r--   0        0        0     1412 2023-07-20 04:37:14.551222 allianceauth_oidc_provider-0.0.1a3/allianceauth_oidc/urls.py
--rw-r--r--   0        0        0     4267 2023-07-20 04:37:14.551222 allianceauth_oidc_provider-0.0.1a3/allianceauth_oidc/views.py
--rw-r--r--   0        0        0     1333 2023-07-20 04:37:14.551222 allianceauth_oidc_provider-0.0.1a3/pyproject.toml
--rw-r--r--   0        0        0      862 2023-07-20 04:37:14.551222 allianceauth_oidc_provider-0.0.1a3/runtests.py
--rw-r--r--   0        0        0       67 2023-07-20 04:37:14.555223 allianceauth_oidc_provider-0.0.1a3/tests/__init__.py
--rw-r--r--   0        0        0      627 2023-07-20 04:37:14.555223 allianceauth_oidc_provider-0.0.1a3/tests/celery.py
--rw-r--r--   0        0        0     1493 2023-07-20 04:37:14.555223 allianceauth_oidc_provider-0.0.1a3/tests/test_settings.py
--rw-r--r--   0        0        0      360 2023-07-20 04:37:14.555223 allianceauth_oidc_provider-0.0.1a3/tests/urls.py
--rw-r--r--   0        0        0      103 2023-07-20 04:37:14.555223 allianceauth_oidc_provider-0.0.1a3/tests/views.py
--rw-r--r--   0        0        0      290 2023-07-20 04:37:14.555223 allianceauth_oidc_provider-0.0.1a3/tox.ini
--rw-r--r--   0        0        0     2159 1970-01-01 00:00:00.000000 allianceauth_oidc_provider-0.0.1a3/PKG-INFO
+-rw-r--r--   0        0        0      347 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/.coveragerc
+-rw-r--r--   0        0        0     1342 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/.github/workflows/main.yml
+-rw-r--r--   0        0        0      718 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     2116 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/.gitignore
+-rw-r--r--   0        0        0      631 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      139 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/.prettierignore
+-rw-r--r--   0        0        0       88 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/.prettierrc
+-rw-r--r--   0        0        0     1077 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/LICENSE
+-rw-r--r--   0        0        0      629 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/Makefile
+-rw-r--r--   0        0        0     3172 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/README.md
+-rw-r--r--   0        0        0      122 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/__init__.py
+-rw-r--r--   0        0        0      647 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/admin.py
+-rw-r--r--   0        0        0      281 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/apps.py
+-rw-r--r--   0        0        0        0 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/auth_hooks.py
+-rw-r--r--   0        0        0      836 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/auth_provider.py
+-rw-r--r--   0        0        0     3037 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/migrations/0001_initial.py
+-rw-r--r--   0        0        0      613 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/migrations/0002_alter_allianceauthapplication_options_and_more.py
+-rw-r--r--   0        0        0        0 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/migrations/__init__.py
+-rw-r--r--   0        0        0      772 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/models.py
+-rw-r--r--   0        0        0      186 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/signals.py
+-rw-r--r--   0        0        0     1392 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/templates/allianceauth_oidc/authorize.html
+-rw-r--r--   0        0        0     1294 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/templates/allianceauth_oidc/base.html
+-rw-r--r--   0        0        0     2449 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/templates/allianceauth_oidc/denied.html
+-rw-r--r--   0        0        0     1268 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/templates/allianceauth_oidc/logout_confirm.html
+-rw-r--r--   0        0        0     7133 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/tests/__init__.py
+-rw-r--r--   0        0        0    10339 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/tests/test_access.py
+-rw-r--r--   0        0        0     1412 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/urls.py
+-rw-r--r--   0        0        0     3830 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/views.py
+-rw-r--r--   0        0        0     1333 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/pyproject.toml
+-rw-r--r--   0        0        0      862 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/runtests.py
+-rw-r--r--   0        0        0       67 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/tests/__init__.py
+-rw-r--r--   0        0        0      627 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/tests/celery.py
+-rw-r--r--   0        0        0     6622 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/tests/test_settings.py
+-rw-r--r--   0        0        0      458 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/tests/urls.py
+-rw-r--r--   0        0        0      103 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/tests/views.py
+-rw-r--r--   0        0        0      290 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/tox.ini
+-rw-r--r--   0        0        0     4195 1970-01-01 00:00:00.000000 allianceauth_oidc_provider-0.0.1b1/PKG-INFO
```

### Comparing `allianceauth_oidc_provider-0.0.1a3/.github/workflows/main.yml` & `allianceauth_oidc_provider-0.0.1b1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `allianceauth_oidc_provider-0.0.1a3/.github/workflows/publish.yml` & `allianceauth_oidc_provider-0.0.1b1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `allianceauth_oidc_provider-0.0.1a3/.gitignore` & `allianceauth_oidc_provider-0.0.1b1/.gitignore`

 * *Files identical despite different names*

### Comparing `allianceauth_oidc_provider-0.0.1a3/.pre-commit-config.yaml` & `allianceauth_oidc_provider-0.0.1b1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `allianceauth_oidc_provider-0.0.1a3/LICENSE` & `allianceauth_oidc_provider-0.0.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `allianceauth_oidc_provider-0.0.1a3/Makefile` & `allianceauth_oidc_provider-0.0.1b1/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 help:
 	@echo "This project assumes that an active Python virtualenv is present."
 	@echo "The following make targets are available:"
 	@echo "  dev        install all deps for dev environment"
 	@echo "  clean      remove all old packages"
 	@echo "  test       run tests"
 	@echo "  deploy     Configure the PyPi config file in CI"
-	@echo "  package  Build the PyPi package"
+	@echo "  package	Build the PyPi package"
 
 clean:
 	rm -rf dist/*
 
 dev:
 	pip install --upgrade pip
 	pip install wheel -U
```

### Comparing `allianceauth_oidc_provider-0.0.1a3/allianceauth_oidc/admin.py` & `allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth_oidc_provider-0.0.1a3/allianceauth_oidc/auth_provider.py` & `allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/auth_provider.py`

 * *Files identical despite different names*

### Comparing `allianceauth_oidc_provider-0.0.1a3/allianceauth_oidc/migrations/0001_initial.py` & `allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth_oidc_provider-0.0.1a3/allianceauth_oidc/migrations/0002_alter_allianceauthapplication_options_and_more.py` & `allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/migrations/0002_alter_allianceauthapplication_options_and_more.py`

 * *Files identical despite different names*

### Comparing `allianceauth_oidc_provider-0.0.1a3/allianceauth_oidc/models.py` & `allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth_oidc_provider-0.0.1a3/allianceauth_oidc/templates/allianceauth_oidc/authorize.html` & `allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/templates/allianceauth_oidc/authorize.html`

 * *Files identical despite different names*

### Comparing `allianceauth_oidc_provider-0.0.1a3/allianceauth_oidc/templates/allianceauth_oidc/base.html` & `allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/templates/allianceauth_oidc/base.html`

 * *Files identical despite different names*

### Comparing `allianceauth_oidc_provider-0.0.1a3/allianceauth_oidc/templates/allianceauth_oidc/denied.html` & `allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/templates/allianceauth_oidc/denied.html`

 * *Files identical despite different names*

### Comparing `allianceauth_oidc_provider-0.0.1a3/allianceauth_oidc/templates/allianceauth_oidc/logout_confirm.html` & `allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/templates/allianceauth_oidc/logout_confirm.html`

 * *Files identical despite different names*

### Comparing `allianceauth_oidc_provider-0.0.1a3/allianceauth_oidc/urls.py` & `allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth_oidc_provider-0.0.1a3/allianceauth_oidc/views.py` & `allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,20 +27,21 @@
     if user.is_superuser:
         log.debug(f"{user} is SU allowing full access")
         return
     group_access = True
     state_access = True
     if app.states.count():
         log.debug(
-            f"OAUTH STATE User: {user.profile.state} APP: {print(app.states.all())}")
+            f"OAUTH STATE User: {user.profile.state} APP: {app.states.all()}")
         state_access = app.states.filter(name=user.profile.state).exists()
     if app.groups.count():
         log.debug(
-            f"OAUTH GROUP User: {user.groups.all()} APP: {print(app.groups.all())}")
-        group_access = app.groups.filter(name__in=user.groups.all()).exists()
+            f"OAUTH GROUP User: {user.groups.all()} APP: {app.groups.all()}")
+        group_access = app.groups.filter(
+            name__in=user.groups.all().values_list('name', flat=True)).exists()
 
     if not group_access or not state_access:
         log.warning(
             f"OAUTH {user} - {app} - Group: {group_access} State: {state_access}")
         raise PermissionDenied()
 
 
@@ -85,16 +86,7 @@
                     log.warning(
                         f"OAUTH - {request.user} - {resp.context_data['application']} - Access Denied")
                     return render(request, "allianceauth_oidc/denied.html", context={"reason": f"{resp.context_data['application']} Access Denied", "error_code": "( 403 - Application Permission Denied )"})
             return resp
         else:
             log.warning(f"OAUTH - {request.user} - global - Access Denied")
             return render(request, "allianceauth_oidc/denied.html", context={"reason": "External OAuth Denied", "error_code": "( 403 - OAuth Permission Denied )"})
-
-    def redirect(self, redirect_to, application):
-        if application is None:
-            # The application can be None in case of an error during app validation
-            # In such cases, fall back to default ALLOWED_REDIRECT_URI_SCHEMES
-            allowed_schemes = oauth2_settings.ALLOWED_REDIRECT_URI_SCHEMES
-        else:
-            allowed_schemes = application.get_allowed_schemes()
-        return OAuth2ResponseRedirect(redirect_to, allowed_schemes)
```

### Comparing `allianceauth_oidc_provider-0.0.1a3/pyproject.toml` & `allianceauth_oidc_provider-0.0.1b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `allianceauth_oidc_provider-0.0.1a3/runtests.py` & `allianceauth_oidc_provider-0.0.1b1/runtests.py`

 * *Files identical despite different names*

### Comparing `allianceauth_oidc_provider-0.0.1a3/tests/celery.py` & `allianceauth_oidc_provider-0.0.1b1/tests/celery.py`

 * *Files identical despite different names*

