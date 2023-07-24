# Comparing `tmp/django-lazy-srcset-1.0.0.tar.gz` & `tmp/django-lazy-srcset-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-lazy-srcset-1.0.0.tar", last modified: Tue Jul 11 16:16:16 2023, max compression
+gzip compressed data, was "django-lazy-srcset-1.0.1.tar", last modified: Mon Jul 24 11:29:03 2023, max compression
```

## Comparing `django-lazy-srcset-1.0.0.tar` & `django-lazy-srcset-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-11 16:16:16.816509 django-lazy-srcset-1.0.0/
--rw-r--r--   0 quantra    (501) staff       (20)     1076 2023-05-02 22:05:05.000000 django-lazy-srcset-1.0.0/LICENSE
--rw-r--r--   0 quantra    (501) staff       (20)       73 2023-06-29 00:05:50.000000 django-lazy-srcset-1.0.0/MANIFEST.in
--rw-r--r--   0 quantra    (501) staff       (20)     8616 2023-07-11 16:16:16.816647 django-lazy-srcset-1.0.0/PKG-INFO
--rw-r--r--   0 quantra    (501) staff       (20)     7072 2023-07-11 15:48:24.000000 django-lazy-srcset-1.0.0/README.rst
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-11 16:16:16.805156 django-lazy-srcset-1.0.0/django_lazy_srcset.egg-info/
--rw-r--r--   0 quantra    (501) staff       (20)     8616 2023-07-11 16:16:16.000000 django-lazy-srcset-1.0.0/django_lazy_srcset.egg-info/PKG-INFO
--rw-r--r--   0 quantra    (501) staff       (20)      576 2023-07-11 16:16:16.000000 django-lazy-srcset-1.0.0/django_lazy_srcset.egg-info/SOURCES.txt
--rw-r--r--   0 quantra    (501) staff       (20)       40 2023-07-11 16:16:16.000000 django-lazy-srcset-1.0.0/django_lazy_srcset.egg-info/dependency_links.txt
--rw-r--r--   0 quantra    (501) staff       (20)       35 2023-07-11 16:16:16.000000 django-lazy-srcset-1.0.0/django_lazy_srcset.egg-info/requires.txt
--rw-r--r--   0 quantra    (501) staff       (20)       20 2023-07-11 16:16:16.000000 django-lazy-srcset-1.0.0/django_lazy_srcset.egg-info/top_level.txt
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-11 16:16:16.807438 django-lazy-srcset-1.0.0/lazy_srcset/
--rw-r--r--   0 quantra    (501) staff       (20)        0 2023-06-26 14:12:57.000000 django-lazy-srcset-1.0.0/lazy_srcset/__init__.py
--rw-r--r--   0 quantra    (501) staff       (20)       96 2023-06-26 17:31:28.000000 django-lazy-srcset-1.0.0/lazy_srcset/apps.py
--rw-r--r--   0 quantra    (501) staff       (20)     1947 2023-07-10 23:00:44.000000 django-lazy-srcset-1.0.0/lazy_srcset/conf.py
--rw-r--r--   0 quantra    (501) staff       (20)      679 2023-06-26 19:06:25.000000 django-lazy-srcset-1.0.0/lazy_srcset/imagegenerators.py
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-11 16:16:16.808194 django-lazy-srcset-1.0.0/lazy_srcset/management/
--rw-r--r--   0 quantra    (501) staff       (20)        0 2023-06-27 22:41:58.000000 django-lazy-srcset-1.0.0/lazy_srcset/management/__init__.py
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-11 16:16:16.813844 django-lazy-srcset-1.0.0/lazy_srcset/management/commands/
--rw-r--r--   0 quantra    (501) staff       (20)        0 2023-06-27 22:41:50.000000 django-lazy-srcset-1.0.0/lazy_srcset/management/commands/__init__.py
--rw-r--r--   0 quantra    (501) staff       (20)     3299 2023-06-29 00:03:00.000000 django-lazy-srcset-1.0.0/lazy_srcset/management/commands/imagekit_cleanup.py
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-11 16:16:16.816315 django-lazy-srcset-1.0.0/lazy_srcset/templatetags/
--rw-r--r--   0 quantra    (501) staff       (20)        0 2023-06-26 14:12:57.000000 django-lazy-srcset-1.0.0/lazy_srcset/templatetags/__init__.py
--rw-r--r--   0 quantra    (501) staff       (20)    11435 2023-07-11 12:35:35.000000 django-lazy-srcset-1.0.0/lazy_srcset/templatetags/lazy_srcset.py
--rw-r--r--   0 quantra    (501) staff       (20)       89 2023-06-26 19:06:22.000000 django-lazy-srcset-1.0.0/pyproject.toml
--rw-r--r--   0 quantra    (501) staff       (20)     1979 2023-07-11 16:16:16.820050 django-lazy-srcset-1.0.0/setup.cfg
--rw-r--r--   0 quantra    (501) staff       (20)       38 2023-06-26 17:04:23.000000 django-lazy-srcset-1.0.0/setup.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-24 11:29:03.582717 django-lazy-srcset-1.0.1/
+-rw-r--r--   0 quantra    (501) staff       (20)     1076 2023-05-02 22:05:05.000000 django-lazy-srcset-1.0.1/LICENSE
+-rw-r--r--   0 quantra    (501) staff       (20)       73 2023-06-29 00:05:50.000000 django-lazy-srcset-1.0.1/MANIFEST.in
+-rw-r--r--   0 quantra    (501) staff       (20)     9915 2023-07-24 11:29:03.582822 django-lazy-srcset-1.0.1/PKG-INFO
+-rw-r--r--   0 quantra    (501) staff       (20)     8408 2023-07-24 11:21:20.000000 django-lazy-srcset-1.0.1/README.rst
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-24 11:29:03.574347 django-lazy-srcset-1.0.1/django_lazy_srcset.egg-info/
+-rw-r--r--   0 quantra    (501) staff       (20)     9915 2023-07-24 11:29:03.000000 django-lazy-srcset-1.0.1/django_lazy_srcset.egg-info/PKG-INFO
+-rw-r--r--   0 quantra    (501) staff       (20)      576 2023-07-24 11:29:03.000000 django-lazy-srcset-1.0.1/django_lazy_srcset.egg-info/SOURCES.txt
+-rw-r--r--   0 quantra    (501) staff       (20)       40 2023-07-24 11:29:03.000000 django-lazy-srcset-1.0.1/django_lazy_srcset.egg-info/dependency_links.txt
+-rw-r--r--   0 quantra    (501) staff       (20)       35 2023-07-24 11:29:03.000000 django-lazy-srcset-1.0.1/django_lazy_srcset.egg-info/requires.txt
+-rw-r--r--   0 quantra    (501) staff       (20)       20 2023-07-24 11:29:03.000000 django-lazy-srcset-1.0.1/django_lazy_srcset.egg-info/top_level.txt
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-24 11:29:03.577616 django-lazy-srcset-1.0.1/lazy_srcset/
+-rw-r--r--   0 quantra    (501) staff       (20)        0 2023-06-26 14:12:57.000000 django-lazy-srcset-1.0.1/lazy_srcset/__init__.py
+-rw-r--r--   0 quantra    (501) staff       (20)       96 2023-06-26 17:31:28.000000 django-lazy-srcset-1.0.1/lazy_srcset/apps.py
+-rw-r--r--   0 quantra    (501) staff       (20)     2227 2023-07-13 22:02:32.000000 django-lazy-srcset-1.0.1/lazy_srcset/conf.py
+-rw-r--r--   0 quantra    (501) staff       (20)      679 2023-06-26 19:06:25.000000 django-lazy-srcset-1.0.1/lazy_srcset/imagegenerators.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-24 11:29:03.580309 django-lazy-srcset-1.0.1/lazy_srcset/management/
+-rw-r--r--   0 quantra    (501) staff       (20)        0 2023-06-27 22:41:58.000000 django-lazy-srcset-1.0.1/lazy_srcset/management/__init__.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-24 11:29:03.581365 django-lazy-srcset-1.0.1/lazy_srcset/management/commands/
+-rw-r--r--   0 quantra    (501) staff       (20)        0 2023-06-27 22:41:50.000000 django-lazy-srcset-1.0.1/lazy_srcset/management/commands/__init__.py
+-rw-r--r--   0 quantra    (501) staff       (20)     3299 2023-06-29 00:03:00.000000 django-lazy-srcset-1.0.1/lazy_srcset/management/commands/imagekit_cleanup.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-24 11:29:03.582540 django-lazy-srcset-1.0.1/lazy_srcset/templatetags/
+-rw-r--r--   0 quantra    (501) staff       (20)        0 2023-06-26 14:12:57.000000 django-lazy-srcset-1.0.1/lazy_srcset/templatetags/__init__.py
+-rw-r--r--   0 quantra    (501) staff       (20)    12157 2023-07-12 20:39:22.000000 django-lazy-srcset-1.0.1/lazy_srcset/templatetags/lazy_srcset.py
+-rw-r--r--   0 quantra    (501) staff       (20)       89 2023-06-26 19:06:22.000000 django-lazy-srcset-1.0.1/pyproject.toml
+-rw-r--r--   0 quantra    (501) staff       (20)     1936 2023-07-24 11:29:03.586634 django-lazy-srcset-1.0.1/setup.cfg
+-rw-r--r--   0 quantra    (501) staff       (20)       38 2023-06-26 17:04:23.000000 django-lazy-srcset-1.0.1/setup.py
```

### Comparing `django-lazy-srcset-1.0.0/LICENSE` & `django-lazy-srcset-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-lazy-srcset-1.0.0/PKG-INFO` & `django-lazy-srcset-1.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-lazy-srcset
-Version: 1.0.0
+Version: 1.0.1
 Summary: Lazy srcset and responsive image generation for Django. Minimum effort required. No database required.
 Home-page: https://github.com/Quantra/django-lazy-srcset
 Author: Vince Coleman
 Author-email: vince@shystudios.co.uk
 License: MIT
 Project-URL: Source, https://github.com/Quantra/django-lazy-srcset
 Keywords: django,django-lazy-srcset,django lazy srcset,django srcset,django responsive images,django responsive
@@ -26,15 +26,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
 Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 |package version|
 |license|
 |pypi status|
 |coverage|
 
@@ -51,14 +50,16 @@
 
 Lazy srcset and responsive image generation for Django. Minimum effort required. No database required.
 
 Django Lazy srcset will create the markup and generate the images you need to provide responsive images via the `srcset and sizes attributes for the img tag <https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Responsive_images#resolution_switching_different_sizes>`_.  All you need to do is install it, configure your breakpoints and use the ``{% srcset %}`` template tag.
 
 All of the hard work (image generation and cacheing) is done by django-imagekit, by default this means images are generated just in time - lazily. Please see the `django-imagekit docs <https://django-imagekit.readthedocs.io>`_ for more info and configuration options.
 
+Width and height attributes are generated to help avoid layout shifts. Make sure you set these in CSS so they are only used by the browser for aspect ratio.
+
 SVG images are supported, they will not be converted or resized but width and height attributes are still added as well as the ``role="img"`` attribute.
 
 You will also need Django and Pillow.
 
 Installation & Usage
 --------------------
 
@@ -93,15 +94,16 @@
     # The default generator to use when not specified in the config.
     LAZY_SRCSET_GENERATOR_ID = "lazy_srcset:srcset_image"
 
     LAZY_SRCSET = {
         "default": {
             # breakpoints is the only setting you must define
             "breakpoints": [1920, 1580, 1280, 1024, 640],
-            # If max_width is not provided the source image width is used, it's a good idea to set this
+            # If max_width is not provided the source image width is used.
+            # It's a good idea to set this.
             "max_width": 2560,
             # If quality is not provided PIL will choose a default
             "quality": 91,
             # If format is not provided the source image format is used
             "format": "WEBP",
             # The difference in width (px) required to generate a new image
             # This prevents images being created which are too similar in size
@@ -113,27 +115,46 @@
 
 Use the ``{% srcset %}`` template tag:
 
 .. code-block:: django
 
     {% load lazy_srcset %}
 
-    {# image is probably an ImageField #}
+    {# image is an ImageField. With no args or kwargs provided all sizes are assumed to be 100vw #}
     <img {% srcset image %} alt="Lovely and lazy" />
 
-    {# You can also provide relative image widths e.g. for a 4 - 3 - 2 - 1 col degradation: #}
+    {# You can provide a path to a static file instead of an ImageField. #}
+    <img {% srcset 'path/to/my/image.png' %} />
+
+    {# You can provide relative (vw) image widths e.g. for a 4 - 3 - 2 - 1 col degradation #}
+    {# These are used to calculate the width of the generated images for each breakpoint #}
     <img {% srcset image 25 33 50 %}  />
 
-    {# You can provide a path to a static file #}
-    <img {% srcset 'path/to/my/image.png' %} />
+    {# Kwargs can be used to define breakpoints and some settings #}
+    <img {% srcset image 1920=25 1580=33 1024=50 640=100 max_width=1920 %} />
+
+    {# Fixed width images can be defined with px units. These are always made regardless of threshold #}
+    <img {% srcset image '500px' '400px' '300px' %} />
 
 Whilst not required it is advisable to take a nap at this stage.
 
 For further documentation and examples of all the options please see the huge and obvious docstring in the source code for `lazy_srcset/templatetags/lazy_srcset.py <https://github.com/Quantra/django-lazy-srcset/blob/master/lazy_srcset/templatetags/lazy_srcset.py>`_.
 
+How it Works
+------------
+
+If the source image is wider than the ``max_width`` it is resized to ``max_width``. Otherwise it is converted as is. This image is then used in the srcset and src attributes.
+
+For each breakpoint we calculate the target width of the image required and iterate from biggest to smallest. Images are then generated if the required width is:
+
+* Smaller than the source width (no upscaling!).
+* Smaller than the previously generated image by more than ``threshold`` px unless the size was defined with px units.
+
+Once imagekit has generated an image it won't create it again and it will store this fact in the cache to further speed up subsequent renders.
+
 Advanced
 --------
 
 Due to the awesomeness of django-imagekit it's possible to configure django-lazy-srcset to use any image generator you have registered on a per config basis. Take a look at `lazy_srcset/conf.py <https://github.com/Quantra/django-lazy-srcset/blob/master/lazy_srcset/conf.py>`_ to see how to change the ``generator_id`` setting. For an example image generator look at `lazy_srcset/imagegenerators.py <https://github.com/Quantra/django-lazy-srcset/blob/master/lazy_srcset/imagegenerators.py>`_. This is completely optional but I thought I'd mention it as there are potential artistic uses here; for example you could use a generator to add filters to some images.
 
 Currently imagekit ``SourceGroup`` has not been implemented therefore the imagekit ``generateimages`` management command will not generate images for django-lazy-srcset. If you want to pre-generate images you can ``render_to_string()`` your templates in an appropriate save method or signal.  If you are using `django-content-blocks <https://github.com/Quantra/django-content-blocks>`_ this happens on publish anyway.
```

### Comparing `django-lazy-srcset-1.0.0/README.rst` & `django-lazy-srcset-1.0.1/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 
 Lazy srcset and responsive image generation for Django. Minimum effort required. No database required.
 
 Django Lazy srcset will create the markup and generate the images you need to provide responsive images via the `srcset and sizes attributes for the img tag <https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Responsive_images#resolution_switching_different_sizes>`_.  All you need to do is install it, configure your breakpoints and use the ``{% srcset %}`` template tag.
 
 All of the hard work (image generation and cacheing) is done by django-imagekit, by default this means images are generated just in time - lazily. Please see the `django-imagekit docs <https://django-imagekit.readthedocs.io>`_ for more info and configuration options.
 
+Width and height attributes are generated to help avoid layout shifts. Make sure you set these in CSS so they are only used by the browser for aspect ratio.
+
 SVG images are supported, they will not be converted or resized but width and height attributes are still added as well as the ``role="img"`` attribute.
 
 You will also need Django and Pillow.
 
 Installation & Usage
 --------------------
 
@@ -58,15 +60,16 @@
     # The default generator to use when not specified in the config.
     LAZY_SRCSET_GENERATOR_ID = "lazy_srcset:srcset_image"
 
     LAZY_SRCSET = {
         "default": {
             # breakpoints is the only setting you must define
             "breakpoints": [1920, 1580, 1280, 1024, 640],
-            # If max_width is not provided the source image width is used, it's a good idea to set this
+            # If max_width is not provided the source image width is used.
+            # It's a good idea to set this.
             "max_width": 2560,
             # If quality is not provided PIL will choose a default
             "quality": 91,
             # If format is not provided the source image format is used
             "format": "WEBP",
             # The difference in width (px) required to generate a new image
             # This prevents images being created which are too similar in size
@@ -78,27 +81,46 @@
 
 Use the ``{% srcset %}`` template tag:
 
 .. code-block:: django
 
     {% load lazy_srcset %}
 
-    {# image is probably an ImageField #}
+    {# image is an ImageField. With no args or kwargs provided all sizes are assumed to be 100vw #}
     <img {% srcset image %} alt="Lovely and lazy" />
 
-    {# You can also provide relative image widths e.g. for a 4 - 3 - 2 - 1 col degradation: #}
+    {# You can provide a path to a static file instead of an ImageField. #}
+    <img {% srcset 'path/to/my/image.png' %} />
+
+    {# You can provide relative (vw) image widths e.g. for a 4 - 3 - 2 - 1 col degradation #}
+    {# These are used to calculate the width of the generated images for each breakpoint #}
     <img {% srcset image 25 33 50 %}  />
 
-    {# You can provide a path to a static file #}
-    <img {% srcset 'path/to/my/image.png' %} />
+    {# Kwargs can be used to define breakpoints and some settings #}
+    <img {% srcset image 1920=25 1580=33 1024=50 640=100 max_width=1920 %} />
+
+    {# Fixed width images can be defined with px units. These are always made regardless of threshold #}
+    <img {% srcset image '500px' '400px' '300px' %} />
 
 Whilst not required it is advisable to take a nap at this stage.
 
 For further documentation and examples of all the options please see the huge and obvious docstring in the source code for `lazy_srcset/templatetags/lazy_srcset.py <https://github.com/Quantra/django-lazy-srcset/blob/master/lazy_srcset/templatetags/lazy_srcset.py>`_.
 
+How it Works
+------------
+
+If the source image is wider than the ``max_width`` it is resized to ``max_width``. Otherwise it is converted as is. This image is then used in the srcset and src attributes.
+
+For each breakpoint we calculate the target width of the image required and iterate from biggest to smallest. Images are then generated if the required width is:
+
+* Smaller than the source width (no upscaling!).
+* Smaller than the previously generated image by more than ``threshold`` px unless the size was defined with px units.
+
+Once imagekit has generated an image it won't create it again and it will store this fact in the cache to further speed up subsequent renders.
+
 Advanced
 --------
 
 Due to the awesomeness of django-imagekit it's possible to configure django-lazy-srcset to use any image generator you have registered on a per config basis. Take a look at `lazy_srcset/conf.py <https://github.com/Quantra/django-lazy-srcset/blob/master/lazy_srcset/conf.py>`_ to see how to change the ``generator_id`` setting. For an example image generator look at `lazy_srcset/imagegenerators.py <https://github.com/Quantra/django-lazy-srcset/blob/master/lazy_srcset/imagegenerators.py>`_. This is completely optional but I thought I'd mention it as there are potential artistic uses here; for example you could use a generator to add filters to some images.
 
 Currently imagekit ``SourceGroup`` has not been implemented therefore the imagekit ``generateimages`` management command will not generate images for django-lazy-srcset. If you want to pre-generate images you can ``render_to_string()`` your templates in an appropriate save method or signal.  If you are using `django-content-blocks <https://github.com/Quantra/django-content-blocks>`_ this happens on publish anyway.
```

### Comparing `django-lazy-srcset-1.0.0/django_lazy_srcset.egg-info/PKG-INFO` & `django-lazy-srcset-1.0.1/django_lazy_srcset.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-lazy-srcset
-Version: 1.0.0
+Version: 1.0.1
 Summary: Lazy srcset and responsive image generation for Django. Minimum effort required. No database required.
 Home-page: https://github.com/Quantra/django-lazy-srcset
 Author: Vince Coleman
 Author-email: vince@shystudios.co.uk
 License: MIT
 Project-URL: Source, https://github.com/Quantra/django-lazy-srcset
 Keywords: django,django-lazy-srcset,django lazy srcset,django srcset,django responsive images,django responsive
@@ -26,15 +26,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
 Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 |package version|
 |license|
 |pypi status|
 |coverage|
 
@@ -51,14 +50,16 @@
 
 Lazy srcset and responsive image generation for Django. Minimum effort required. No database required.
 
 Django Lazy srcset will create the markup and generate the images you need to provide responsive images via the `srcset and sizes attributes for the img tag <https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Responsive_images#resolution_switching_different_sizes>`_.  All you need to do is install it, configure your breakpoints and use the ``{% srcset %}`` template tag.
 
 All of the hard work (image generation and cacheing) is done by django-imagekit, by default this means images are generated just in time - lazily. Please see the `django-imagekit docs <https://django-imagekit.readthedocs.io>`_ for more info and configuration options.
 
+Width and height attributes are generated to help avoid layout shifts. Make sure you set these in CSS so they are only used by the browser for aspect ratio.
+
 SVG images are supported, they will not be converted or resized but width and height attributes are still added as well as the ``role="img"`` attribute.
 
 You will also need Django and Pillow.
 
 Installation & Usage
 --------------------
 
@@ -93,15 +94,16 @@
     # The default generator to use when not specified in the config.
     LAZY_SRCSET_GENERATOR_ID = "lazy_srcset:srcset_image"
 
     LAZY_SRCSET = {
         "default": {
             # breakpoints is the only setting you must define
             "breakpoints": [1920, 1580, 1280, 1024, 640],
-            # If max_width is not provided the source image width is used, it's a good idea to set this
+            # If max_width is not provided the source image width is used.
+            # It's a good idea to set this.
             "max_width": 2560,
             # If quality is not provided PIL will choose a default
             "quality": 91,
             # If format is not provided the source image format is used
             "format": "WEBP",
             # The difference in width (px) required to generate a new image
             # This prevents images being created which are too similar in size
@@ -113,27 +115,46 @@
 
 Use the ``{% srcset %}`` template tag:
 
 .. code-block:: django
 
     {% load lazy_srcset %}
 
-    {# image is probably an ImageField #}
+    {# image is an ImageField. With no args or kwargs provided all sizes are assumed to be 100vw #}
     <img {% srcset image %} alt="Lovely and lazy" />
 
-    {# You can also provide relative image widths e.g. for a 4 - 3 - 2 - 1 col degradation: #}
+    {# You can provide a path to a static file instead of an ImageField. #}
+    <img {% srcset 'path/to/my/image.png' %} />
+
+    {# You can provide relative (vw) image widths e.g. for a 4 - 3 - 2 - 1 col degradation #}
+    {# These are used to calculate the width of the generated images for each breakpoint #}
     <img {% srcset image 25 33 50 %}  />
 
-    {# You can provide a path to a static file #}
-    <img {% srcset 'path/to/my/image.png' %} />
+    {# Kwargs can be used to define breakpoints and some settings #}
+    <img {% srcset image 1920=25 1580=33 1024=50 640=100 max_width=1920 %} />
+
+    {# Fixed width images can be defined with px units. These are always made regardless of threshold #}
+    <img {% srcset image '500px' '400px' '300px' %} />
 
 Whilst not required it is advisable to take a nap at this stage.
 
 For further documentation and examples of all the options please see the huge and obvious docstring in the source code for `lazy_srcset/templatetags/lazy_srcset.py <https://github.com/Quantra/django-lazy-srcset/blob/master/lazy_srcset/templatetags/lazy_srcset.py>`_.
 
+How it Works
+------------
+
+If the source image is wider than the ``max_width`` it is resized to ``max_width``. Otherwise it is converted as is. This image is then used in the srcset and src attributes.
+
+For each breakpoint we calculate the target width of the image required and iterate from biggest to smallest. Images are then generated if the required width is:
+
+* Smaller than the source width (no upscaling!).
+* Smaller than the previously generated image by more than ``threshold`` px unless the size was defined with px units.
+
+Once imagekit has generated an image it won't create it again and it will store this fact in the cache to further speed up subsequent renders.
+
 Advanced
 --------
 
 Due to the awesomeness of django-imagekit it's possible to configure django-lazy-srcset to use any image generator you have registered on a per config basis. Take a look at `lazy_srcset/conf.py <https://github.com/Quantra/django-lazy-srcset/blob/master/lazy_srcset/conf.py>`_ to see how to change the ``generator_id`` setting. For an example image generator look at `lazy_srcset/imagegenerators.py <https://github.com/Quantra/django-lazy-srcset/blob/master/lazy_srcset/imagegenerators.py>`_. This is completely optional but I thought I'd mention it as there are potential artistic uses here; for example you could use a generator to add filters to some images.
 
 Currently imagekit ``SourceGroup`` has not been implemented therefore the imagekit ``generateimages`` management command will not generate images for django-lazy-srcset. If you want to pre-generate images you can ``render_to_string()`` your templates in an appropriate save method or signal.  If you are using `django-content-blocks <https://github.com/Quantra/django-content-blocks>`_ this happens on publish anyway.
```

### Comparing `django-lazy-srcset-1.0.0/django_lazy_srcset.egg-info/SOURCES.txt` & `django-lazy-srcset-1.0.1/django_lazy_srcset.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-lazy-srcset-1.0.0/lazy_srcset/conf.py` & `django-lazy-srcset-1.0.1/lazy_srcset/conf.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,25 +16,29 @@
 
     # The default generator to use when not specified in the config.
     LAZY_SRCSET_GENERATOR_ID = "lazy_srcset:srcset_image"
 
     # Configs
     LAZY_SRCSET = {
         "default": {
-            # breakpoints is the only setting you must define
+            # breakpoints is the only setting you must define in each config
+            # a sizes entry for each breakpoint will be generated
             "breakpoints": [1920, 1580, 1280, 1024, 640],
-            # If max_width is not provided the source image width is used, it's a good idea to set this
+            # max_width is the widest a generated image can be
+            # If max_width is not provided or the source image is smaller the source image width is used
             "max_width": 2560,
             # If quality is not provided PIL will choose a default
+            # You may want to tune this to your needs
             "quality": 91,
             # If format is not provided the source image format is used
             "format": "WEBP",
             # The difference in width (px) required to generate a new image
             # This prevents images being created which are too similar in size
             # If threshold is not provided LAZY_SRCSET_THRESHOLD is used
+            # Set to 0 to generate all images even if they are only 1 px smaller
             "threshold": LAZY_SRCSET_THRESHOLD,
             # If generator_id is not provided LAZY_SRCSET_GENERATOR_ID is used
             "generator_id": LAZY_SRCSET_GENERATOR_ID,
         }
     }
 
     def __getattribute__(self, item):
```

### Comparing `django-lazy-srcset-1.0.0/lazy_srcset/imagegenerators.py` & `django-lazy-srcset-1.0.1/lazy_srcset/imagegenerators.py`

 * *Files identical despite different names*

### Comparing `django-lazy-srcset-1.0.0/lazy_srcset/management/commands/imagekit_cleanup.py` & `django-lazy-srcset-1.0.1/lazy_srcset/management/commands/imagekit_cleanup.py`

 * *Files identical despite different names*

### Comparing `django-lazy-srcset-1.0.0/lazy_srcset/templatetags/lazy_srcset.py` & `django-lazy-srcset-1.0.1/lazy_srcset/templatetags/lazy_srcset.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,24 +26,14 @@
     for key, value in zip(keys, values):
         combined_dict[key] = value
     for key in keys[len(values):]:  # fmt: skip
         combined_dict[key] = default_value
     return combined_dict
 
 
-def get_from_kwargs_or_conf(key, kwargs, conf):
-    """
-    Pop the key from kwargs and return if possible. If not get the key from conf and return even if its None.
-    """
-    try:
-        return kwargs.pop(key)
-    except KeyError:
-        return conf.get(key)
-
-
 def get_svg_dimensions(svg_file):
     """
     Try and get width and height from the svg file or return none for them if not possible.
     """
     with svg_file.open() as f:
         tree = ElementTree.parse(f)
         root = tree.getroot()
@@ -52,15 +42,15 @@
         width, height = root.get("width"), root.get("height")
 
         # If width or height attributes are missing, get values from viewbox.
         if width is None or height is None:
             viewbox = root.get("viewBox")
             try:
                 _, _, width, height = viewbox.split(" ")
-            except (AttributeError, ValueError):
+            except (AttributeError, ValueError):  # pragma: no cover
                 pass
 
         # These could include units E.g. px or pt so strip them out.
         width = re.sub("\\D", "", width) if width is not None else None
         height = re.sub("\\D", "", height) if height is not None else None
 
     return width, height
@@ -68,66 +58,113 @@
 
 def sanitize_breakpoint(breakpoint):
     """
     Breakpoints must be integers.
     """
     try:
         return int(breakpoint)
-    except ValueError:
+    except ValueError:  # pragma: no cover
         raise TemplateSyntaxError(
             "Invalid breakpoint: %s\nBreakpoints must be integers." % breakpoint
         )
 
 
 def sanitize_size(size):
     """
     Sizes need to be either an integer or a string with px or vw units.
     """
     try:
         return int(size), "vw"
     except ValueError:
         pass
 
+    size = size.replace(" ", "")
     try:
         size, units = int(size[:-2]), size[-2:]
-    except (IndexError, ValueError):
+    except (IndexError, ValueError):  # pragma: no cover
         raise TemplateSyntaxError(
             "Invalid size: %s\nBreakpoints must be integers.\nSizes must specify vw or px units or be integers."
             % size
         )
 
     if units not in ["px", "vw"]:
-        raise TemplateSyntaxError("Invalid size: %s\nUnits must be px or vw." % size)
+        raise TemplateSyntaxError(
+            "Invalid size: %s\nUnits must be px or vw." % size
+        )  # pragma: no cover
 
     return size, units
 
 
-def svg_srcset(svg):
+def get_config(kwargs):
+    """
+    Pop from kwargs as needed and set up the config dict ready for this run.
+    After running this kwargs will only contain breakpoints if anything.
+    """
+    # Get the conf from the config kwarg or default and copy it so changes don't persist
+    try:
+        conf_key = kwargs.pop("config")
+    except KeyError:
+        conf_key = "default"
+    conf = settings.LAZY_SRCSET[conf_key].copy()
+
+    # Try to pop these from kwargs
+    for key in ["default_size", "max_width", "quality", "threshold"]:
+        try:
+            conf[key] = kwargs.pop(key)
+        except KeyError:
+            pass
+
+    # Set a default from settings
+    conf.setdefault("threshold", settings.LAZY_SRCSET_THRESHOLD)
+    conf.setdefault("generator_id", settings.LAZY_SRCSET_GENERATOR_ID)
+
+    return conf
+
+
+def svg_srcset(source_img):
     """
     Returns attrs string containing src and width and height if possible. Will also add role="img" attr.
     """
     # Try getting width and height from attrs.
     try:
-        width = svg.width
-        height = svg.height
-    except AttributeError:
+        width = source_img.width
+        height = source_img.height
+    except AttributeError:  # pragma: no cover
         width, height = None, None
 
     # If we don't have the width and height try getting it from the SVG file.
     if width is None or height is None:
-        width, height = get_svg_dimensions(svg)
+        width, height = get_svg_dimensions(source_img)
 
     # Return with width and height if we have them.
     if width is not None and height is not None:
-        return format_html(
-            'src="{}" width="{}" height="{}" role="img"', svg.url, width, height
+        html = format_html(
+            'src="{}" width="{}" height="{}" role="img"', source_img.url, width, height
         )
+    else:
+        # Return with src only if we don't have width and height
+        html = format_html('src="{}" role="img"', source_img.url)
+
+    source_img.close()
+    return html
+
 
-    # Return with src only if we don't have width and height
-    return format_html('src="{}" role="img"', svg.url)
+def noop(source_img):
+    """
+    The no-op returns src, width and height so images still work.
+    This is used when LAZY_SRCSET_ENABLED=False and whilst images are being generated.
+    """
+    html = format_html(
+        'src="{}" width="{}" height="{}"',
+        source_img.url,
+        source_img.width,
+        source_img.height,
+    )
+    source_img.close()
+    return html
 
 
 @register.simple_tag
 def srcset(*args, **kwargs):
     """
     The srcset template tag will create srcset, sizes, src, width and height attributes for an <img> tag.
 
@@ -183,136 +220,112 @@
     <!-- You can set the default size with units in the same way as the sizes args -->
     <img {% srcset image default_size='300px' %} />
 
     <!-- You can mix and match all of the above E.g. -->
     <img {% srcset image 25 33 50 config='custom_breakpoints' max_width=1920 image_quality=50 threshold=100 %} />
     <img {% srcset image 1920=25 1024=50 default_size=50 image_quality=50 %} />
     """
-    # INIT
     args = list(args)
 
     # If the image has an open method we should be good to go.  If not assume it's a string and get it from
     # staticfiles wrapped up in ImageFile. Set the url attribute, so we can use it later.
-    image = args.pop(0)
-    if not hasattr(image, "open"):
-        url = staticfiles_storage.url(image)
-        image = ImageFile(open(finders.find(image), "rb"))
-        image.url = url
+    source_img = args.pop(0)
+    if not hasattr(source_img, "open"):
+        url = staticfiles_storage.url(source_img)
+        source_img = ImageFile(open(finders.find(source_img), "rb"))
+        source_img.url = url
 
     # If the image is an SVG return now with src, width and height if possible. SVG is lazy king!
-    if Path(image.name).suffix.lower() == ".svg":
-        return svg_srcset(image)
+    if Path(source_img.name).suffix.lower() == ".svg":
+        return svg_srcset(source_img)
 
     # If LAZY_SRCSET_ENABLED = False return src, width and height
     if not settings.LAZY_SRCSET_ENABLED:
-        return format_html(
-            'src="{}" width="{}" height="{}"', image.url, image.width, image.height
-        )
-
-    # Get the conf from the config kwarg or default
-    try:
-        conf = settings.LAZY_SRCSET[kwargs.pop("config")]
-    except KeyError:
-        conf = settings.LAZY_SRCSET["default"]
-
-    # Get the default size from kwargs
-    try:
-        default_size = kwargs.pop("default_size")
-    except KeyError:
-        default_size = None
-
-    # Get the max_width from kwargs or conf.
-    max_width = get_from_kwargs_or_conf("max_width", kwargs, conf)
-
-    # Get the kwargs for the image generator
-    output_format = conf.get("format")
-    quality = get_from_kwargs_or_conf("quality", kwargs, conf)
-    generator_id = conf.get("generator_id", settings.LAZY_SRCSET_GENERATOR_ID)
-    threshold = int(
-        get_from_kwargs_or_conf("threshold", kwargs, conf)
-        or settings.LAZY_SRCSET_THRESHOLD
-    )
+        return noop(source_img)
 
-    # All kwargs except breakpoint kwargs must be popped by now!
+    # Prepare config, sizes_dict and widths_dict
+    conf = get_config(kwargs)
 
     # If we have kwargs we can set the sizes otherwise try and get them from args.
     sizes_dict = kwargs or lists_to_dict(conf["breakpoints"], args)
 
-    # The sizes in our dict are strings and might contain px|vw
-    # After this our dict will be like: {1920: (50, "vw")}
+    # The sizes in our dict are strings and might contain px|vw. After this our dict will be like: {1920: (50, "vw")}
     sizes_dict = {
         sanitize_breakpoint(k): sanitize_size(v) for k, v in sizes_dict.items()
     }
 
-    # Create the sizes for the sizes attr
-    sizes = [
-        format_html("(max-width: {}px) {}{}", size, *sizes_dict[size])
-        for size in sorted(sizes_dict.keys())
-    ]
-
-    # Add the default size
-    if default_size is not None:
-        default_size = sanitize_size(default_size)
-    else:
-        default_size = sizes_dict[max(sizes_dict.keys())]
-    sizes.append(format_html("{}{}", *default_size))
-
     # Set the maximum width image in our srcset.
-    if max_width is None or max_width > image.width:
+    if conf["max_width"] is None or conf["max_width"] > source_img.width:
         # Limit max_width to image.width or use image.width if max_width is None.
-        max_width = image.width
-
-    # widths_dict will be a dict with the image width as key and a boolean if the image must be created E.g.
-    # {960: True}
-    widths_dict = {max_width: True}
+        conf["max_width"] = source_img.width
 
-    # Make sure the image file is closed as soon as we can.
-    image.close()
+    # widths_dict is a dict with the image width as key and a boolean if the image must be created E.g. {960: True}
+    widths_dict = {conf["max_width"]: True}
 
-    # GO!
+    # Loop through the sizes_dict to create the widths_dict used for image generation.  Create sizes list for the attr
+    sizes = []
+    width, units = "100", "vw"
+    for breakpoint_width in sorted(sizes_dict.keys()):
+        width, units = sizes_dict[breakpoint_width]
+
+        # Add an entry to sizes
+        sizes.append(
+            format_html("(max-width: {}px) {}{}", breakpoint_width, width, units)
+        )
 
-    # Loop through the sizes_dict to create the widths_dict used for image generation.
-    for breakpoint_width, (width, units) in sizes_dict.items():
         if units == "px":
             # When px units are defined always generate an image with that width
             widths_dict[width] = True
             continue
 
         # Calculate the target width for this breakpoint with some quick maths.
         target_width = math.ceil(breakpoint_width * width / 100)
-        if target_width < max_width:
+        if target_width < conf["max_width"]:
             # Don't upscale images, that would require extra effort.
             widths_dict[target_width] = False
 
+    # Add the default size (sneaky use of the sorted loop above leaves us with the width and units we need)
+    if "default_size" in conf.keys():
+        width, units = sanitize_size(conf["default_size"])
+    sizes.append(format_html("{}{}", width, units))
+
     # Loop through the widths of images and generate what is needed
-    current_width = max_width
-    images = []
+    current_width = conf["max_width"]
+    output_imgs = []
     for width in reversed(sorted(widths_dict.keys())):
-        if not widths_dict[width] and (current_width - width) < threshold:
+        if not widths_dict[width] and (current_width - width) < conf["threshold"]:
             # Only generate required images and images outside our threshold
             continue
 
-        current_width = width
-
         # Generate the image via imagekit.
         generator = generator_registry.get(
-            generator_id,
+            conf["generator_id"],
             width=width,
-            source=image,
-            output_format=output_format,
-            quality=quality,
+            source=source_img,
+            output_format=conf.get("format"),
+            quality=conf["quality"],
         )
         generator_image = ImageCacheFile(generator)
-        images.append(generator_image)
+        output_imgs.append(generator_image)
+
+        current_width = width
 
     # Create the srcsets
-    srcsets = [format_html("{} {}w", image.url, image.width) for image in images]
+    try:
+        srcsets = [
+            format_html("{} {}w", image.url, image.width) for image in output_imgs
+        ]
+    except FileNotFoundError:  # pragma: no cover
+        # Images are being generated in another thread right now, but we can rely on source_img to actually exist
+        return noop(source_img)
+
+    source_img.close()
 
     # Stringify!
     return format_html(
         'src="{}" srcset="{}" sizes="{}" width="{}" height="{}"',
-        images[0].url,
+        output_imgs[0].url,
         ", ".join(srcsets),
         ", ".join(sizes),
-        images[0].width,
-        images[0].height,
+        output_imgs[0].width,
+        output_imgs[0].height,
     )
```

### Comparing `django-lazy-srcset-1.0.0/setup.cfg` & `django-lazy-srcset-1.0.1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 [metadata]
 name = django-lazy-srcset
-version = 1.0.0
+version = 1.0.1
 description = Lazy srcset and responsive image generation for Django. Minimum effort required. No database required.
 long_description = file:README.rst
-long_description_content_type = text/x-rst
 url = https://github.com/Quantra/django-lazy-srcset
 author = Vince Coleman
 author_email = vince@shystudios.co.uk
 license = MIT
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
```

