# Comparing `tmp/django-sso-client-manager-0.0.5.tar.gz` & `tmp/django-sso-client-manager-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-sso-client-manager-0.0.5.tar", last modified: Mon Jul 24 07:54:27 2023, max compression
+gzip compressed data, was "django-sso-client-manager-0.0.6.tar", last modified: Mon Jul 24 08:09:54 2023, max compression
```

## Comparing `django-sso-client-manager-0.0.5.tar` & `django-sso-client-manager-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 yil       (1000) yil       (1000)        0 2023-07-24 07:54:27.188801 django-sso-client-manager-0.0.5/
--rw-rw-r--   0 yil       (1000) yil       (1000)     5125 2023-07-24 07:54:27.188801 django-sso-client-manager-0.0.5/PKG-INFO
-drwxrwxr-x   0 yil       (1000) yil       (1000)        0 2023-07-24 07:54:27.184801 django-sso-client-manager-0.0.5/django_sso_client_manager.egg-info/
--rw-rw-r--   0 yil       (1000) yil       (1000)     5125 2023-07-24 07:54:27.000000 django-sso-client-manager-0.0.5/django_sso_client_manager.egg-info/PKG-INFO
--rw-rw-r--   0 yil       (1000) yil       (1000)      399 2023-07-24 07:54:27.000000 django-sso-client-manager-0.0.5/django_sso_client_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 yil       (1000) yil       (1000)        1 2023-07-24 07:54:27.000000 django-sso-client-manager-0.0.5/django_sso_client_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 yil       (1000) yil       (1000)       37 2023-07-24 07:54:27.000000 django-sso-client-manager-0.0.5/django_sso_client_manager.egg-info/requires.txt
--rw-rw-r--   0 yil       (1000) yil       (1000)       19 2023-07-24 07:54:27.000000 django-sso-client-manager-0.0.5/django_sso_client_manager.egg-info/top_level.txt
--rw-rw-r--   0 yil       (1000) yil       (1000)       38 2023-07-24 07:54:27.188801 django-sso-client-manager-0.0.5/setup.cfg
--rw-rw-r--   0 yil       (1000) yil       (1000)     1659 2023-07-24 07:53:59.000000 django-sso-client-manager-0.0.5/setup.py
-drwxrwxr-x   0 yil       (1000) yil       (1000)        0 2023-07-24 07:54:27.188801 django-sso-client-manager-0.0.5/sso_client_manager/
--rw-rw-r--   0 yil       (1000) yil       (1000)        0 2023-06-13 14:37:55.000000 django-sso-client-manager-0.0.5/sso_client_manager/__init__.py
--rw-rw-r--   0 yil       (1000) yil       (1000)      171 2023-07-07 05:33:04.000000 django-sso-client-manager-0.0.5/sso_client_manager/apps.py
--rw-rw-r--   0 yil       (1000) yil       (1000)     2548 2023-07-24 05:12:23.000000 django-sso-client-manager-0.0.5/sso_client_manager/middlewares.py
--rw-rw-r--   0 yil       (1000) yil       (1000)      353 2023-07-20 11:16:06.000000 django-sso-client-manager-0.0.5/sso_client_manager/urls.py
--rw-rw-r--   0 yil       (1000) yil       (1000)     5490 2023-07-24 04:45:43.000000 django-sso-client-manager-0.0.5/sso_client_manager/views.py
+drwxrwxr-x   0 yil       (1000) yil       (1000)        0 2023-07-24 08:09:54.753338 django-sso-client-manager-0.0.6/
+-rw-rw-r--   0 yil       (1000) yil       (1000)     5247 2023-07-24 08:09:54.753338 django-sso-client-manager-0.0.6/PKG-INFO
+drwxrwxr-x   0 yil       (1000) yil       (1000)        0 2023-07-24 08:09:54.753338 django-sso-client-manager-0.0.6/django_sso_client_manager.egg-info/
+-rw-rw-r--   0 yil       (1000) yil       (1000)     5247 2023-07-24 08:09:54.000000 django-sso-client-manager-0.0.6/django_sso_client_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 yil       (1000) yil       (1000)      399 2023-07-24 08:09:54.000000 django-sso-client-manager-0.0.6/django_sso_client_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 yil       (1000) yil       (1000)        1 2023-07-24 08:09:54.000000 django-sso-client-manager-0.0.6/django_sso_client_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 yil       (1000) yil       (1000)       37 2023-07-24 08:09:54.000000 django-sso-client-manager-0.0.6/django_sso_client_manager.egg-info/requires.txt
+-rw-rw-r--   0 yil       (1000) yil       (1000)       19 2023-07-24 08:09:54.000000 django-sso-client-manager-0.0.6/django_sso_client_manager.egg-info/top_level.txt
+-rw-rw-r--   0 yil       (1000) yil       (1000)       38 2023-07-24 08:09:54.753338 django-sso-client-manager-0.0.6/setup.cfg
+-rw-rw-r--   0 yil       (1000) yil       (1000)     1657 2023-07-24 08:09:21.000000 django-sso-client-manager-0.0.6/setup.py
+drwxrwxr-x   0 yil       (1000) yil       (1000)        0 2023-07-24 08:09:54.753338 django-sso-client-manager-0.0.6/sso_client_manager/
+-rw-rw-r--   0 yil       (1000) yil       (1000)        0 2023-06-13 14:37:55.000000 django-sso-client-manager-0.0.6/sso_client_manager/__init__.py
+-rw-rw-r--   0 yil       (1000) yil       (1000)      171 2023-07-07 05:33:04.000000 django-sso-client-manager-0.0.6/sso_client_manager/apps.py
+-rw-rw-r--   0 yil       (1000) yil       (1000)     2548 2023-07-24 05:12:23.000000 django-sso-client-manager-0.0.6/sso_client_manager/middlewares.py
+-rw-rw-r--   0 yil       (1000) yil       (1000)      353 2023-07-20 11:16:06.000000 django-sso-client-manager-0.0.6/sso_client_manager/urls.py
+-rw-rw-r--   0 yil       (1000) yil       (1000)     5490 2023-07-24 04:45:43.000000 django-sso-client-manager-0.0.6/sso_client_manager/views.py
```

### Comparing `django-sso-client-manager-0.0.5/PKG-INFO` & `django-sso-client-manager-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: django-sso-client-manager
-Version: 0.0.5
+Version: 0.0.6
 Summary: django-sso-client-manager is a Django application designed to simplify the management of Single Sign-On (SSO) clients within a web application. It provides functionalities for handling login and logout processes and conveniently sets codes in cookies for seamless authentication and user session management. By integrating this app into a Django project, developers can streamline the implementation of SSO functionality and enhance the overall user experience.
 Home-page: https://github.com/rjnp2/django-sso-client-manager
 Author: rjnp2
 Author-email: rjnp2@outlook.com
 License: MIT License
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 django-sso-client-manager
 =========================
 
 django-sso-client-manager is a Django application designed to simplify the management of Single Sign-On (SSO) clients within a web application. It provides functionalities for handling login and logout processes and conveniently sets codes in cookies for seamless authentication and user session management. By integrating this app into a Django project, developers can streamline the implementation of SSO functionality and enhance the overall user experience.
@@ -79,14 +79,18 @@
 
     This variable holds the url of the SSO server.
 
 3. KEY:
 
     This variable represents a secret key or encryption key used for secure communication or token validation between your application and the SSO server.
 
+        APPLICATION_ID = env.str('APPLICATION_ID')
+        KEY = env.str('KEY')
+        SSO_SERVER = env.str('SSO_SERVER')
+
 By setting these variables in your Django settings, your application will be able to communicate with the SSO server, authenticate users, and manage the login/logout processes securely.
 
 Compatibility
 -------------
 The compatibility information you provided indicates that the django-sso-client-manager package is compatible with Python 3.10 and Django versions 4 and above.
 
 To ensure proper compatibility, always check the official documentation and release notes of the django-sso-client-manager package to confirm its support for specific Python and Django versions.
```

### Comparing `django-sso-client-manager-0.0.5/django_sso_client_manager.egg-info/PKG-INFO` & `django-sso-client-manager-0.0.6/django_sso_client_manager.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: django-sso-client-manager
-Version: 0.0.5
+Version: 0.0.6
 Summary: django-sso-client-manager is a Django application designed to simplify the management of Single Sign-On (SSO) clients within a web application. It provides functionalities for handling login and logout processes and conveniently sets codes in cookies for seamless authentication and user session management. By integrating this app into a Django project, developers can streamline the implementation of SSO functionality and enhance the overall user experience.
 Home-page: https://github.com/rjnp2/django-sso-client-manager
 Author: rjnp2
 Author-email: rjnp2@outlook.com
 License: MIT License
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 django-sso-client-manager
 =========================
 
 django-sso-client-manager is a Django application designed to simplify the management of Single Sign-On (SSO) clients within a web application. It provides functionalities for handling login and logout processes and conveniently sets codes in cookies for seamless authentication and user session management. By integrating this app into a Django project, developers can streamline the implementation of SSO functionality and enhance the overall user experience.
@@ -79,14 +79,18 @@
 
     This variable holds the url of the SSO server.
 
 3. KEY:
 
     This variable represents a secret key or encryption key used for secure communication or token validation between your application and the SSO server.
 
+        APPLICATION_ID = env.str('APPLICATION_ID')
+        KEY = env.str('KEY')
+        SSO_SERVER = env.str('SSO_SERVER')
+
 By setting these variables in your Django settings, your application will be able to communicate with the SSO server, authenticate users, and manage the login/logout processes securely.
 
 Compatibility
 -------------
 The compatibility information you provided indicates that the django-sso-client-manager package is compatible with Python 3.10 and Django versions 4 and above.
 
 To ensure proper compatibility, always check the official documentation and release notes of the django-sso-client-manager package to confirm its support for specific Python and Django versions.
```

### Comparing `django-sso-client-manager-0.0.5/setup.py` & `django-sso-client-manager-0.0.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 README = open(os.path.join(os.path.dirname(__file__), 'readme.md')).read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='django-sso-client-manager',
-    version='0.0.5',
+    version='0.0.6',
     packages=['sso_client_manager'],
     include_package_data=True,
     license='MIT License',
     description='django-sso-client-manager is a Django application designed to simplify the management of Single Sign-On (SSO) clients within a web application. It provides functionalities for handling login and logout processes and conveniently sets codes in cookies for seamless authentication and user session management. By integrating this app into a Django project, developers can streamline the implementation of SSO functionality and enhance the overall user experience.',
     long_description=README,
     long_description_content_type="text/markdown",
     url='https://github.com/rjnp2/django-sso-client-manager',
@@ -21,19 +21,19 @@
     classifiers=[
         'Environment :: Web Environment',
         'Framework :: Django',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.8',
         'Topic :: Internet :: WWW/HTTP',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
     ],
-    python_requires=">=3.10",
+    python_requires=">=3.8",
     install_requires=[
-        'requests>=2.31.0',
+        'requests>=2.28.1',
     ],
     extras_require={
         "dev": ['twine>=4.0.2',]
     }
 )
```

### Comparing `django-sso-client-manager-0.0.5/sso_client_manager/middlewares.py` & `django-sso-client-manager-0.0.6/sso_client_manager/middlewares.py`

 * *Files identical despite different names*

### Comparing `django-sso-client-manager-0.0.5/sso_client_manager/views.py` & `django-sso-client-manager-0.0.6/sso_client_manager/views.py`

 * *Files identical despite different names*

