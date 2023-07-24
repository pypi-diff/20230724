# Comparing `tmp/django-sso-client-manager-0.0.3.tar.gz` & `tmp/django-sso-client-manager-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-sso-client-manager-0.0.3.tar", last modified: Wed Jul 19 06:10:47 2023, max compression
+gzip compressed data, was "django-sso-client-manager-0.0.5.tar", last modified: Mon Jul 24 07:54:27 2023, max compression
```

## Comparing `django-sso-client-manager-0.0.3.tar` & `django-sso-client-manager-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxr-x   0 yil       (1000) yil       (1000)        0 2023-07-19 06:10:47.186351 django-sso-client-manager-0.0.3/
--rw-rw-r--   0 yil       (1000) yil       (1000)     1500 2023-07-19 06:10:47.186351 django-sso-client-manager-0.0.3/PKG-INFO
-drwxrwxr-x   0 yil       (1000) yil       (1000)        0 2023-07-19 06:10:47.186351 django-sso-client-manager-0.0.3/django_sso_client_manager.egg-info/
--rw-rw-r--   0 yil       (1000) yil       (1000)     1500 2023-07-19 06:10:47.000000 django-sso-client-manager-0.0.3/django_sso_client_manager.egg-info/PKG-INFO
--rw-rw-r--   0 yil       (1000) yil       (1000)      427 2023-07-19 06:10:47.000000 django-sso-client-manager-0.0.3/django_sso_client_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 yil       (1000) yil       (1000)        1 2023-07-19 06:10:47.000000 django-sso-client-manager-0.0.3/django_sso_client_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 yil       (1000) yil       (1000)       58 2023-07-19 06:10:47.000000 django-sso-client-manager-0.0.3/django_sso_client_manager.egg-info/requires.txt
--rw-rw-r--   0 yil       (1000) yil       (1000)       19 2023-07-19 06:10:47.000000 django-sso-client-manager-0.0.3/django_sso_client_manager.egg-info/top_level.txt
--rw-rw-r--   0 yil       (1000) yil       (1000)       38 2023-07-19 06:10:47.186351 django-sso-client-manager-0.0.3/setup.cfg
--rw-rw-r--   0 yil       (1000) yil       (1000)     1321 2023-07-19 05:58:22.000000 django-sso-client-manager-0.0.3/setup.py
-drwxrwxr-x   0 yil       (1000) yil       (1000)        0 2023-07-19 06:10:47.186351 django-sso-client-manager-0.0.3/sso_client_manager/
--rw-rw-r--   0 yil       (1000) yil       (1000)        0 2023-06-13 14:37:55.000000 django-sso-client-manager-0.0.3/sso_client_manager/__init__.py
--rw-rw-r--   0 yil       (1000) yil       (1000)      171 2023-07-07 05:33:04.000000 django-sso-client-manager-0.0.3/sso_client_manager/apps.py
--rw-rw-r--   0 yil       (1000) yil       (1000)     2417 2023-07-18 11:30:58.000000 django-sso-client-manager-0.0.3/sso_client_manager/middlewares.py
--rw-rw-r--   0 yil       (1000) yil       (1000)      295 2023-07-07 06:07:39.000000 django-sso-client-manager-0.0.3/sso_client_manager/urls.py
--rw-rw-r--   0 yil       (1000) yil       (1000)      229 2023-07-07 05:35:01.000000 django-sso-client-manager-0.0.3/sso_client_manager/utils.py
--rw-rw-r--   0 yil       (1000) yil       (1000)     6129 2023-07-19 05:54:20.000000 django-sso-client-manager-0.0.3/sso_client_manager/views.py
+drwxrwxr-x   0 yil       (1000) yil       (1000)        0 2023-07-24 07:54:27.188801 django-sso-client-manager-0.0.5/
+-rw-rw-r--   0 yil       (1000) yil       (1000)     5125 2023-07-24 07:54:27.188801 django-sso-client-manager-0.0.5/PKG-INFO
+drwxrwxr-x   0 yil       (1000) yil       (1000)        0 2023-07-24 07:54:27.184801 django-sso-client-manager-0.0.5/django_sso_client_manager.egg-info/
+-rw-rw-r--   0 yil       (1000) yil       (1000)     5125 2023-07-24 07:54:27.000000 django-sso-client-manager-0.0.5/django_sso_client_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 yil       (1000) yil       (1000)      399 2023-07-24 07:54:27.000000 django-sso-client-manager-0.0.5/django_sso_client_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 yil       (1000) yil       (1000)        1 2023-07-24 07:54:27.000000 django-sso-client-manager-0.0.5/django_sso_client_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 yil       (1000) yil       (1000)       37 2023-07-24 07:54:27.000000 django-sso-client-manager-0.0.5/django_sso_client_manager.egg-info/requires.txt
+-rw-rw-r--   0 yil       (1000) yil       (1000)       19 2023-07-24 07:54:27.000000 django-sso-client-manager-0.0.5/django_sso_client_manager.egg-info/top_level.txt
+-rw-rw-r--   0 yil       (1000) yil       (1000)       38 2023-07-24 07:54:27.188801 django-sso-client-manager-0.0.5/setup.cfg
+-rw-rw-r--   0 yil       (1000) yil       (1000)     1659 2023-07-24 07:53:59.000000 django-sso-client-manager-0.0.5/setup.py
+drwxrwxr-x   0 yil       (1000) yil       (1000)        0 2023-07-24 07:54:27.188801 django-sso-client-manager-0.0.5/sso_client_manager/
+-rw-rw-r--   0 yil       (1000) yil       (1000)        0 2023-06-13 14:37:55.000000 django-sso-client-manager-0.0.5/sso_client_manager/__init__.py
+-rw-rw-r--   0 yil       (1000) yil       (1000)      171 2023-07-07 05:33:04.000000 django-sso-client-manager-0.0.5/sso_client_manager/apps.py
+-rw-rw-r--   0 yil       (1000) yil       (1000)     2548 2023-07-24 05:12:23.000000 django-sso-client-manager-0.0.5/sso_client_manager/middlewares.py
+-rw-rw-r--   0 yil       (1000) yil       (1000)      353 2023-07-20 11:16:06.000000 django-sso-client-manager-0.0.5/sso_client_manager/urls.py
+-rw-rw-r--   0 yil       (1000) yil       (1000)     5490 2023-07-24 04:45:43.000000 django-sso-client-manager-0.0.5/sso_client_manager/views.py
```

### Comparing `django-sso-client-manager-0.0.3/setup.py` & `django-sso-client-manager-0.0.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 README = open(os.path.join(os.path.dirname(__file__), 'readme.md')).read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='django-sso-client-manager',
-    version='0.0.3',
+    version='0.0.5',
     packages=['sso_client_manager'],
     include_package_data=True,
     license='MIT License',
-    description='A Django app for the managing sso client that have login, logout and set code a in cookies.',
+    description='django-sso-client-manager is a Django application designed to simplify the management of Single Sign-On (SSO) clients within a web application. It provides functionalities for handling login and logout processes and conveniently sets codes in cookies for seamless authentication and user session management. By integrating this app into a Django project, developers can streamline the implementation of SSO functionality and enhance the overall user experience.',
     long_description=README,
     long_description_content_type="text/markdown",
     url='https://github.com/rjnp2/django-sso-client-manager',
     author='rjnp2',
     author_email='rjnp2@outlook.com',
     classifiers=[
         'Environment :: Web Environment',
@@ -27,14 +27,13 @@
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.10',
         'Topic :: Internet :: WWW/HTTP',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
     ],
     python_requires=">=3.10",
     install_requires=[
-        'cryptography>=41.0.1',
         'requests>=2.31.0',
     ],
     extras_require={
         "dev": ['twine>=4.0.2',]
     }
 )
```

### Comparing `django-sso-client-manager-0.0.3/sso_client_manager/views.py` & `django-sso-client-manager-0.0.5/sso_client_manager/views.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,173 +1,148 @@
-import json
-
+import requests
 from django.conf import settings
 from django.contrib.auth import get_user_model
 from django.core.signing import Signer
 from django.http import HttpResponseRedirect, JsonResponse
 from django.shortcuts import redirect
 from django.urls import reverse
 from django.utils import timezone
-from django.utils.dateparse import parse_datetime
 from django.views import View
 
-from .utils import decrypt_data
-
 User = get_user_model()
 signer = Signer()
 
 def profile(request):
     if not request.user.is_authenticated:
         return JsonResponse({
             'user_data':None
         }, status=401)
     
-    user = request.user
     return JsonResponse({
-        'user_data':{
-            'id': user.id,
-            'username': user.username,
-            'is_active': user.is_active,
-            'is_staff': user.is_staff,
-            'date_joined': user.date_joined,
-            'last_login': user.last_login,
-        }
+        'id': request.user.id,
+        'username': request.user.username,
+        'is_active': request.user.is_active,
+        'is_staff': request.user.is_staff,
+        'is_superuser': request.user.is_superuser,
+        'date_joined': request.user.date_joined,
+        'last_login': request.user.last_login,
     })
-    
+
+def login_checker(request):
+    next_url = request.GET.get('next') or request.build_absolute_uri('/')
+    url_path = request.build_absolute_uri(reverse('set-code'))
+    sso_url = settings.SSO_SERVER + 'login-checker/'
+    sso_url = f'{sso_url}?next={url_path}&frontend_url={next_url}&application_id={settings.APPLICATION_ID}'
+    response = redirect(sso_url)
+    response.delete_cookie('user_data')
+    response.delete_cookie('access_code')
+    response.delete_cookie('is_logged_in')
+    return response
+   
 def login(request):
-    show_login_page = request.GET.get('show_login_page', True)
     next_url = request.GET.get('next') or '/'
-    if request.user.is_authenticated:        
-        return JsonResponse({'message':'You have already login to this sytem.'})
-
-    signed_obj = signer.sign_object({
-        'date_time' : str(timezone.now()),
-        'secret_key' : request.build_absolute_uri('/'),   
-    })
-
     url_path = request.build_absolute_uri(reverse('set-code'))
-    
-    url = f'{settings.SSO_SERVER_LOGIN}?next={url_path}&frontend_url={next_url}&verify_code={signed_obj}&application_id={settings.APPLICATION_ID}&show_login_page={show_login_page}'
-    return redirect(url)
+    sso_url = settings.SSO_SERVER + 'login/'
+    sso_url = f'{sso_url}?next={url_path}&frontend_url={next_url}&application_id={settings.APPLICATION_ID}'
+    response = redirect(sso_url)
+    response.delete_cookie('user_data')
+    response.delete_cookie('access_code')
+    response.delete_cookie('is_logged_in')
+    return response
 
 def logout(request):
     if not request.user.is_authenticated:
         return JsonResponse({'message':'You have not login to this sytem.'})
 
     next_url = request.GET.get('next') or request.build_absolute_uri('/')
-    url = f'{settings.SSO_SERVER_LOGOUT}?next={next_url}'
-    response = redirect(url)
-    response.delete_cookie('my_code')
-    response.delete_cookie('code')
+    sso_url = settings.SSO_SERVER + 'logout/'
+    sso_url = f'{sso_url}?next={next_url}'
+    response = redirect(sso_url)
+    response.delete_cookie('user_data')
+    response.delete_cookie('access_code')
+    response.delete_cookie('is_logged_in')
     return response
 
 class SetCodeView(View):
     def create_or_update_user(self, user_data):
         try:
-            user = User.objects.get(username=user_data['username'])
+            username=user_data['username']
+        except Exception as e:
+            raise ValueError(
+                f"Error due to {e}"
+            )
+        
+        try:
+            user = User.objects.get(username=username)
             user.last_login = user_data.get('last_login', timezone.now())
             user.save()
         except:
             user = User.objects.create(
                 username=user_data.get('username'),
                 is_staff = user_data.get('is_staff', False),
                 is_active = user_data.get('is_active', False),
                 is_superuser = user_data.get('is_superuser', False),
-                date_joined = user_data.get('created_at', timezone.now()),
+                date_joined = user_data.get('date_joined', timezone.now()),
                 last_login = user_data.get('last_login', timezone.now()),
             )
 
         if hasattr(user, 'sso_id') and user_data.get('id'):
             user.sso_id = user_data.get('id')
             user.save()
 
         return user
 
     def get(self, request):
-        if self.request.GET.get('show_login_page') == 'false':
+        access_code = request.GET.get('access_code')
+        if not access_code:
             frontend_url = request.GET.get('frontend_url') or '/'
             response = HttpResponseRedirect(frontend_url)
-            response.delete_cookie('code')
-            response.delete_cookie('my_code')
-            return response
-    
-        verify_code = request.GET.get('verify_code')
-        if not verify_code:
-            response = JsonResponse({
-                'verify_code':'This field is required.',
-            }, status=400)
-            response.delete_cookie('code')
-            response.delete_cookie('my_code')
+            response.delete_cookie('access_code')
+            response.delete_cookie('user_data')
+            response.delete_cookie('is_logged_in')
             return response
         
-        try:
-            obj = signer.unsign_object(verify_code)
-        except:
-            response = JsonResponse({
-                'message':'Problems while decrypt data.',
-            }, status=400)
-            response.delete_cookie('code')
-            response.delete_cookie('my_code')
-            return response
-        
-        try:
-            date_time = parse_datetime(obj['date_time'])
-        except:
-            response = JsonResponse({
-                'message':'Cannot parse time while decrypt data.',
-            }, status=400)
-            response.delete_cookie('code')
-            response.delete_cookie('my_code')
+        sso_url = settings.SSO_SERVER + 'api/v1/token-checker/'
+        headers = {
+            'Authorization': f'{settings.KEY}',
+            'Content-Type': 'application/json',  # Adjust the Content-Type if needed
+        }
+
+        response = requests.post(
+            url=sso_url,
+            json={
+                'access_code':access_code,
+                'application_id':settings.APPLICATION_ID
+            },
+            headers=headers
+        )
+
+        response_json = response.json()
+        if not response.ok:
+            frontend_url = request.GET.get('frontend_url') or '/'
+            response = HttpResponseRedirect(frontend_url)
+            response.delete_cookie('access_code')
+            response.delete_cookie('user_data')
+            response.delete_cookie('is_logged_in')
             return response
         
         try:
-            secret_key = obj['secret_key']
+            access_code = response_json.pop('access_code')
         except:
-            response = JsonResponse({
-                'message':'Cannot parse secret_key while decrypt data.',
-            }, status=400)
-            response.delete_cookie('code')
-            response.delete_cookie('my_code')
-            return response
-        
-        if secret_key != request.build_absolute_uri('/'):
-            response = JsonResponse({
-                'message':'Request is not origin from this site.',
-            }, status=400)
-            response.delete_cookie('code')
-            response.delete_cookie('my_code')
-            return response
-        
-        diff_time = (timezone.now() - date_time).total_seconds()
-        if diff_time > 60:
-            response = JsonResponse({
-                    'message':'Token is expiry or invalid.',
-                }, status=400)
-            response.delete_cookie('code')
-            response.delete_cookie('my_code')
-            return response
-        
-        code = request.GET.get('code')
-        if not code:
-            response = JsonResponse({
-                'code':'This field is required.',
-            }, status=400)
-            response.delete_cookie('code')
-            response.delete_cookie('my_code')
+            frontend_url = request.GET.get('frontend_url') or '/'
+            response = HttpResponseRedirect(frontend_url)
+            response.delete_cookie('access_code')
+            response.delete_cookie('user_data')
+            response.delete_cookie('is_logged_in')
             return response
-        
-        plain_code = decrypt_data(key=settings.KEY, ciphertext=code)
 
-        signed_obj = plain_code['signed_obj']
-        user_data = json.loads(plain_code['user_data'])
-        user = self.create_or_update_user(user_data)
-        
-        my_code = signer.sign_object({
-            'username' : user.username,
-            'code' : code,   
+        user = self.create_or_update_user(response_json)
+        user_data = signer.sign_object({
+            'username' : user.username
         }) 
-        
+
         frontend_url = request.GET.get('frontend_url') or '/'
         response = HttpResponseRedirect(frontend_url)
-        response.set_cookie('my_code', my_code, expires=30)
-        response.set_cookie('code', signed_obj)
+        response.set_cookie('user_data', user_data, expires=30, httponly=True)
+        response.set_cookie('access_code', access_code, httponly=True)
+        response.set_cookie('is_logged_in', 'true')
         return response
```

