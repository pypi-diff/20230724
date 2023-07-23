# Comparing `tmp/image-go-nord-0.1.5.tar.gz` & `tmp/image-go-nord-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image-go-nord-0.1.5.tar", last modified: Mon Apr 26 08:56:48 2021, max compression
+gzip compressed data, was "image-go-nord-0.1.6.tar", last modified: Sun Jul 23 22:24:56 2023, max compression
```

## Comparing `image-go-nord-0.1.5.tar` & `image-go-nord-0.1.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-26 08:56:48.794652 image-go-nord-0.1.5/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-26 08:56:48.794652 image-go-nord-0.1.5/ImageGoNord/
--rwxr-xr-x   0 root         (0) root         (0)    13850 2021-04-26 08:56:31.000000 image-go-nord-0.1.5/ImageGoNord/GoNord.py
--rw-r--r--   0 root         (0) root         (0)      768 2021-04-26 08:56:31.000000 image-go-nord-0.1.5/ImageGoNord/GoNord_test.py
--rwxr-xr-x   0 root         (0) root         (0)       72 2021-04-26 08:56:31.000000 image-go-nord-0.1.5/ImageGoNord/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-26 08:56:48.794652 image-go-nord-0.1.5/ImageGoNord/palettes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-26 08:56:48.794652 image-go-nord-0.1.5/ImageGoNord/palettes/Nord/
--rw-r--r--   0 root         (0) root         (0)        0 2021-04-26 08:56:31.000000 image-go-nord-0.1.5/ImageGoNord/palettes/Nord/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-04-26 08:56:31.000000 image-go-nord-0.1.5/ImageGoNord/palettes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-26 08:56:48.794652 image-go-nord-0.1.5/ImageGoNord/utility/
--rwxr-xr-x   0 root         (0) root         (0)     1737 2021-04-26 08:56:31.000000 image-go-nord-0.1.5/ImageGoNord/utility/ConvertUtility.py
--rwxr-xr-x   0 root         (0) root         (0)        0 2021-04-26 08:56:31.000000 image-go-nord-0.1.5/ImageGoNord/utility/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2324 2021-04-26 08:56:31.000000 image-go-nord-0.1.5/ImageGoNord/utility/palette_loader.py
--rw-r--r--   0 root         (0) root         (0)      962 2021-04-26 08:56:31.000000 image-go-nord-0.1.5/ImageGoNord/utility/quantize.py
--rw-r--r--   0 root         (0) root         (0)     1073 2021-04-26 08:56:31.000000 image-go-nord-0.1.5/LICENSE
--rwxr-xr-x   0 root         (0) root         (0)       16 2021-04-26 08:56:31.000000 image-go-nord-0.1.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6448 2021-04-26 08:56:48.794652 image-go-nord-0.1.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4537 2021-04-26 08:56:31.000000 image-go-nord-0.1.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-26 08:56:48.794652 image-go-nord-0.1.5/image_go_nord.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6448 2021-04-26 08:56:48.000000 image-go-nord-0.1.5/image_go_nord.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      506 2021-04-26 08:56:48.000000 image-go-nord-0.1.5/image_go_nord.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-04-26 08:56:48.000000 image-go-nord-0.1.5/image_go_nord.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        7 2021-04-26 08:56:48.000000 image-go-nord-0.1.5/image_go_nord.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2021-04-26 08:56:48.000000 image-go-nord-0.1.5/image_go_nord.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-04-26 08:56:48.794652 image-go-nord-0.1.5/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1527 2021-04-26 08:56:31.000000 image-go-nord-0.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-23 22:24:56.881472 image-go-nord-0.1.6/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-23 22:24:56.881472 image-go-nord-0.1.6/ImageGoNord/
+-rwxr-xr-x   0 root         (0) root         (0)    20646 2023-07-23 22:24:35.000000 image-go-nord-0.1.6/ImageGoNord/GoNord.py
+-rw-r--r--   0 root         (0) root         (0)      768 2023-07-23 22:24:35.000000 image-go-nord-0.1.6/ImageGoNord/GoNord_test.py
+-rwxr-xr-x   0 root         (0) root         (0)       72 2023-07-23 22:24:35.000000 image-go-nord-0.1.6/ImageGoNord/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-23 22:24:56.881472 image-go-nord-0.1.6/ImageGoNord/palettes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-23 22:24:56.881472 image-go-nord-0.1.6/ImageGoNord/palettes/Nord/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-23 22:24:35.000000 image-go-nord-0.1.6/ImageGoNord/palettes/Nord/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-23 22:24:35.000000 image-go-nord-0.1.6/ImageGoNord/palettes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-23 22:24:56.881472 image-go-nord-0.1.6/ImageGoNord/utility/
+-rwxr-xr-x   0 root         (0) root         (0)     2330 2023-07-23 22:24:35.000000 image-go-nord-0.1.6/ImageGoNord/utility/ConvertUtility.py
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-07-23 22:24:35.000000 image-go-nord-0.1.6/ImageGoNord/utility/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3368 2023-07-23 22:24:35.000000 image-go-nord-0.1.6/ImageGoNord/utility/palette_loader.py
+-rw-r--r--   0 root         (0) root         (0)      962 2023-07-23 22:24:35.000000 image-go-nord-0.1.6/ImageGoNord/utility/quantize.py
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-07-23 22:24:35.000000 image-go-nord-0.1.6/LICENSE
+-rwxr-xr-x   0 root         (0) root         (0)       16 2023-07-23 22:24:35.000000 image-go-nord-0.1.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5904 2023-07-23 22:24:56.881472 image-go-nord-0.1.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4870 2023-07-23 22:24:35.000000 image-go-nord-0.1.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-23 22:24:56.881472 image-go-nord-0.1.6/image_go_nord.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5904 2023-07-23 22:24:56.000000 image-go-nord-0.1.6/image_go_nord.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      506 2023-07-23 22:24:56.000000 image-go-nord-0.1.6/image_go_nord.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-23 22:24:56.000000 image-go-nord-0.1.6/image_go_nord.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-23 22:24:56.000000 image-go-nord-0.1.6/image_go_nord.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-23 22:24:56.000000 image-go-nord-0.1.6/image_go_nord.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-23 22:24:56.881472 image-go-nord-0.1.6/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1553 2023-07-23 22:24:35.000000 image-go-nord-0.1.6/setup.py
```

### Comparing `image-go-nord-0.1.5/ImageGoNord/GoNord_test.py` & `image-go-nord-0.1.6/ImageGoNord/GoNord_test.py`

 * *Files identical despite different names*

### Comparing `image-go-nord-0.1.5/ImageGoNord/utility/ConvertUtility.py` & `image-go-nord-0.1.6/ImageGoNord/utility/ConvertUtility.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # -*- coding: utf-8 -*-
+import numpy as np
 
 class ConvertUtility:
   """
   An utility class used for converting image to the nord palette
 
   Methods
   -------
@@ -77,7 +78,31 @@
         a += x[3]
 
     avg_color = (int(r/size), int(g/size), int(b/size))
     if (a != 255):
       avg_color = avg_color + (int(a/size), )
 
     return avg_color
+  
+  def convert_palette(color_cube, image):
+    """Convert frame color palette
+
+    Parameters
+    ----------
+    color_cube: ndarray
+      Color map of RGB colorspace created from palette colors
+    image: ndarray
+      Current frame
+
+    Returns
+    -------
+    ndarray
+      color converted frame
+    """
+
+    shape = image.shape[0:2]
+    indices = image.reshape(-1,3)
+    # Pass image colors and retrieve corresponding palette color
+    new_image = color_cube[indices[:,0],indices[:,1],indices[:,2]]
+
+    return new_image.reshape(shape[0],shape[1],3).astype(np.uint8)
+
```

### Comparing `image-go-nord-0.1.5/ImageGoNord/utility/quantize.py` & `image-go-nord-0.1.6/ImageGoNord/utility/quantize.py`

 * *Files identical despite different names*

### Comparing `image-go-nord-0.1.5/LICENSE` & `image-go-nord-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `image-go-nord-0.1.5/PKG-INFO` & `image-go-nord-0.1.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,134 +1,147 @@
 Metadata-Version: 2.1
 Name: image-go-nord
-Version: 0.1.5
+Version: 0.1.6
 Summary: A tool for converting RGB image to Nordtheme palette
 Home-page: https://github.com/Schrodinger-Hat/ImageGoNord-pip
 Author: Schrodinger Hat
 Author-email: schrodinger.hat.show@gmail.com
 License: MIT
 Download-URL: https://github.com/Schrodinger-Hat/ImageGoNord-pip/releases
 Project-URL: Homepage, https://ign.schrodinger-hat.it
 Project-URL: Source, https://github.com/Schrodinger-Hat/ImageGoNord-pip
 Project-URL: Bug Reports, https://github.com/Schrodinger-Hat/ImageGoNord-pip/issues
-Description: # ImageGoNord - RGB image to Nordtheme palette
-        
-        ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/image-go-nord)
-        [![PyPI](https://img.shields.io/pypi/v/image-go-nord)](https://pypi.org/project/image-go-nord/)
-        [![license](https://img.shields.io/badge/license-MIT-green)](https://github.com/Schrodinger-Hat/ImageGoNord-pip/blob/master/LICENSE)
-        [![Join the community on Spectrum](https://withspectrum.github.io/badge/badge.svg)](https://spectrum.chat/image-go-nord)
-        
-        A tool that can convert your rgb images to nordtheme palette.
-        
-        This repository is a python package that can convert any sort of image into a [nordtheme](https://github.com/arcticicestudio/nord) palette image.
-        
-        You can find a demo on [the website](https://ign.schrodinger-hat.it) for testing out the package.
-        
-        We build also a little API hosted on Heroku to give to anyone the change to test it out by theirself. You can find the documentation on the website too.
-        
-        The main repository of this whole project is [ImageGoNord](https://github.com/Schrodinger-Hat/ImageGoNord).
-        
-        ### Documentation
-        
-        You can find the [documentation into this repository](https://github.com/Schrodinger-Hat/ImageGoNord-pip/tree/master/docs) and also on the website.
-        
-        <!--
-        @TODO
-        - Describe very briefly but clearly what the project does.
-        - State if it is out-of-the-box user-friendly, so it’s clear to the user.
-        - List its most useful/innovative/noteworthy features.
-        - State its goals/what problem(s) it solves.
-        - Note and briefly describe any key concepts (technical, philosophical, or both) important to the user’s understanding.
-        - Link to any supplementary blog posts or project main pages.
-        - Note its development status.
-        - If possible, include screenshots and demo videos.
-        -->
-        
-        ### Inspiration
-        
-        We are in love with Nordtheme, that is why we created this repository.
-        
-        [![Nord Color Palette Overview](https://raw.githubusercontent.com/arcticicestudio/nord-docs/develop/assets/images/nord/repository-color-palettes.svg?sanitize=true)](https://www.nordtheme.com/docs/colors-and-palettes)
-        
-        Our goal is to make a shortcut to convert anything into this theme, by starting from the images.
-        <br>An example could be an awesome wallpaper converted into the Nordtheme palette.
-        
-        We checked the commnunity and we did not find anything similar or any project that can accomplish this task. So, here we are.
-        
-        ### What you can do with this package
-        
-        You can convert any image into the nord palette (or others). Here are some examples:
-        
-        **Original**
-        
-        [![Original](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test.jpg)](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test.jpg)
-        
-        
-        **Processed with avg algorithm**
-        
-        [![Original](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-average.jpg)](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-average.jpg)
-        
-        
-        -----
-        
-        
-        **Original**
-        
-        [![Original](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-profile.jpg)](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-profile.jpg)
-        
-        
-        **Processed with avg algorithm**
-        
-        [![Original](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-profile-average.jpg)](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-profile-average.jpg)
-        
-        ### Core Technical Concepts
-        
-        We are using the PIL because it is the most simple library and it is very useful when you need to manipolate some images.
-        
-        Our goal is also to make this project open source and maintainable by the community. We would love to.
-        
-        *We believe in the open source community.*
-        
-        ### Getting Started
-        
-        Getting it from PIP
-        
-        ```
-        pip install image-go-nord
-        ```
-        
-        Then you can use [some example](https://github.com/Schrodinger-Hat/ImageGoNord-pip/tree/master/docs/example) to getting started properly!
-        
-        ### Contributing
-        - Follow the contributor guidelines
-        - Follow the code style / requirements
-        - Format for commit messages
-        
-        ### TODO
-        - Testing
-        - Improvements on image quality and supporting any image format
-        - Make contributing guidelines
-        
-        # Authors
-        
-        [TheJoin95](https://github.com/TheJoin95) & [Wabri](https://github.com/Wabri)
-        
-        **NOTE**: we are not (yet) affiliated with the Nordtheme or [Arcticicestudio](https://github.com/arcticicestudio).
-        
-        # Credits
-        
-        [Nordtheme](https://www.nordtheme.com/)
-        
-        ### License
-        
-        [MIT license](https://github.com/Schrodinger-Hat/ImageGoNord-pip/blob/master/LICENSE)
-        
 Keywords: nordtheme,pillow,image,conversion,rgb,color-scheme,color-palette
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# ImageGoNord - RGB image to Nordtheme palette
+
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/image-go-nord)
+[![PyPI](https://img.shields.io/pypi/v/image-go-nord)](https://pypi.org/project/image-go-nord/)
+[![license](https://img.shields.io/badge/license-MIT-green)](https://github.com/Schrodinger-Hat/ImageGoNord-pip/blob/master/LICENSE)
+[![Join the community on Spectrum](https://withspectrum.github.io/badge/badge.svg)](https://spectrum.chat/image-go-nord)
+
+A tool that can convert your rgb images to nordtheme palette.
+
+This repository is a python package that can convert any sort of image into a [nordtheme](https://github.com/arcticicestudio/nord) palette image.
+
+You can find a demo on [the website](https://ign.schrodinger-hat.it) for testing out the package.
+
+We build also a little API hosted on Heroku to give to anyone the change to test it out by theirself. You can find the documentation on the website too.
+
+The main repository of this whole project is [ImageGoNord](https://github.com/Schrodinger-Hat/ImageGoNord).
+
+### Documentation
+
+You can find the [documentation into this repository](https://github.com/Schrodinger-Hat/ImageGoNord-pip/tree/master/docs) and also on the website.
+
+<!--
+@TODO
+- Describe very briefly but clearly what the project does.
+- State if it is out-of-the-box user-friendly, so it’s clear to the user.
+- List its most useful/innovative/noteworthy features.
+- State its goals/what problem(s) it solves.
+- Note and briefly describe any key concepts (technical, philosophical, or both) important to the user’s understanding.
+- Link to any supplementary blog posts or project main pages.
+- Note its development status.
+- If possible, include screenshots and demo videos.
+-->
+
+### Inspiration
+
+We are in love with Nordtheme, that is why we created this repository.
+
+[![Nord Color Palette Overview](https://raw.githubusercontent.com/arcticicestudio/nord-docs/develop/assets/images/nord/repository-color-palettes.svg?sanitize=true)](https://www.nordtheme.com/docs/colors-and-palettes)
+
+Our goal is to make a shortcut to convert anything into this theme, by starting from the images.
+<br>An example could be an awesome wallpaper converted into the Nordtheme palette.
+
+We checked the commnunity and we did not find anything similar or any project that can accomplish this task. So, here we are.
+
+### What you can do with this package
+
+You can convert any image into the nord palette (or others). Here are some examples:
+
+**Original**
+
+[![Original](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test.jpg)](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test.jpg)
+
+
+**Processed with avg algorithm**
+
+[![Original](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-average.jpg)](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-average.jpg)
+
+
+-----
+
+**Original**
+
+[![Original](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-profile.jpg)](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-profile.jpg)
+
+
+**Processed with avg algorithm**
+
+[![Original](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-profile-average.jpg)](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-profile-average.jpg)
+
+-----
+
+You can also convert videos into the nord palette (or others). Here is an example:  
+**Original**  
+
+https://github.com/05Alston/ImageGoNord-pip/assets/89850018/76d4c4a6-9660-4a02-9f46-e5f3f6d0147a
+
+**Processed with algorithm**
+
+https://github.com/05Alston/ImageGoNord-pip/assets/89850018/13822280-c019-49b1-92f7-7c658b33a01d
+
+### Core Technical Concepts
+
+We are using the PIL because it is the most simple library and it is very useful when you need to manipulate some images.
+
+Our goal is also to make this project open source and maintainable by the community. We would love to.
+
+*We believe in the open source community.*
+
+### Getting Started
+
+Getting it from PIP
+
+```
+pip install image-go-nord
+```
+
+Then you can use [some example](https://github.com/Schrodinger-Hat/ImageGoNord-pip/tree/master/docs/example) to getting started properly!
+
+### Contributing
+- Follow the contributor guidelines
+- Follow the code style / requirements
+- Format for commit messages
+
+### TODO
+- Testing
+- Improvements on image quality and supporting any image format
+- Make contributing guidelines
+
+# Authors
+
+[TheJoin95](https://github.com/TheJoin95) & [Wabri](https://github.com/Wabri)
+
+**NOTE**: we are not (yet) affiliated with the Nordtheme or [Arcticicestudio](https://github.com/arcticicestudio).
+
+# Credits
+
+[Nordtheme](https://www.nordtheme.com/)
+
+### License
+
+[MIT license](https://github.com/Schrodinger-Hat/ImageGoNord-pip/blob/master/LICENSE)
+
+
```

### Comparing `image-go-nord-0.1.5/README.md` & `image-go-nord-0.1.6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -54,27 +54,37 @@
 **Processed with avg algorithm**
 
 [![Original](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-average.jpg)](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-average.jpg)
 
 
 -----
 
-
 **Original**
 
 [![Original](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-profile.jpg)](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-profile.jpg)
 
 
 **Processed with avg algorithm**
 
 [![Original](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-profile-average.jpg)](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-profile-average.jpg)
 
+-----
+
+You can also convert videos into the nord palette (or others). Here is an example:  
+**Original**  
+
+https://github.com/05Alston/ImageGoNord-pip/assets/89850018/76d4c4a6-9660-4a02-9f46-e5f3f6d0147a
+
+**Processed with algorithm**
+
+https://github.com/05Alston/ImageGoNord-pip/assets/89850018/13822280-c019-49b1-92f7-7c658b33a01d
+
 ### Core Technical Concepts
 
-We are using the PIL because it is the most simple library and it is very useful when you need to manipolate some images.
+We are using the PIL because it is the most simple library and it is very useful when you need to manipulate some images.
 
 Our goal is also to make this project open source and maintainable by the community. We would love to.
 
 *We believe in the open source community.*
 
 ### Getting Started
```

### Comparing `image-go-nord-0.1.5/image_go_nord.egg-info/PKG-INFO` & `image-go-nord-0.1.6/image_go_nord.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,134 +1,147 @@
 Metadata-Version: 2.1
 Name: image-go-nord
-Version: 0.1.5
+Version: 0.1.6
 Summary: A tool for converting RGB image to Nordtheme palette
 Home-page: https://github.com/Schrodinger-Hat/ImageGoNord-pip
 Author: Schrodinger Hat
 Author-email: schrodinger.hat.show@gmail.com
 License: MIT
 Download-URL: https://github.com/Schrodinger-Hat/ImageGoNord-pip/releases
 Project-URL: Homepage, https://ign.schrodinger-hat.it
 Project-URL: Source, https://github.com/Schrodinger-Hat/ImageGoNord-pip
 Project-URL: Bug Reports, https://github.com/Schrodinger-Hat/ImageGoNord-pip/issues
-Description: # ImageGoNord - RGB image to Nordtheme palette
-        
-        ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/image-go-nord)
-        [![PyPI](https://img.shields.io/pypi/v/image-go-nord)](https://pypi.org/project/image-go-nord/)
-        [![license](https://img.shields.io/badge/license-MIT-green)](https://github.com/Schrodinger-Hat/ImageGoNord-pip/blob/master/LICENSE)
-        [![Join the community on Spectrum](https://withspectrum.github.io/badge/badge.svg)](https://spectrum.chat/image-go-nord)
-        
-        A tool that can convert your rgb images to nordtheme palette.
-        
-        This repository is a python package that can convert any sort of image into a [nordtheme](https://github.com/arcticicestudio/nord) palette image.
-        
-        You can find a demo on [the website](https://ign.schrodinger-hat.it) for testing out the package.
-        
-        We build also a little API hosted on Heroku to give to anyone the change to test it out by theirself. You can find the documentation on the website too.
-        
-        The main repository of this whole project is [ImageGoNord](https://github.com/Schrodinger-Hat/ImageGoNord).
-        
-        ### Documentation
-        
-        You can find the [documentation into this repository](https://github.com/Schrodinger-Hat/ImageGoNord-pip/tree/master/docs) and also on the website.
-        
-        <!--
-        @TODO
-        - Describe very briefly but clearly what the project does.
-        - State if it is out-of-the-box user-friendly, so it’s clear to the user.
-        - List its most useful/innovative/noteworthy features.
-        - State its goals/what problem(s) it solves.
-        - Note and briefly describe any key concepts (technical, philosophical, or both) important to the user’s understanding.
-        - Link to any supplementary blog posts or project main pages.
-        - Note its development status.
-        - If possible, include screenshots and demo videos.
-        -->
-        
-        ### Inspiration
-        
-        We are in love with Nordtheme, that is why we created this repository.
-        
-        [![Nord Color Palette Overview](https://raw.githubusercontent.com/arcticicestudio/nord-docs/develop/assets/images/nord/repository-color-palettes.svg?sanitize=true)](https://www.nordtheme.com/docs/colors-and-palettes)
-        
-        Our goal is to make a shortcut to convert anything into this theme, by starting from the images.
-        <br>An example could be an awesome wallpaper converted into the Nordtheme palette.
-        
-        We checked the commnunity and we did not find anything similar or any project that can accomplish this task. So, here we are.
-        
-        ### What you can do with this package
-        
-        You can convert any image into the nord palette (or others). Here are some examples:
-        
-        **Original**
-        
-        [![Original](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test.jpg)](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test.jpg)
-        
-        
-        **Processed with avg algorithm**
-        
-        [![Original](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-average.jpg)](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-average.jpg)
-        
-        
-        -----
-        
-        
-        **Original**
-        
-        [![Original](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-profile.jpg)](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-profile.jpg)
-        
-        
-        **Processed with avg algorithm**
-        
-        [![Original](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-profile-average.jpg)](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-profile-average.jpg)
-        
-        ### Core Technical Concepts
-        
-        We are using the PIL because it is the most simple library and it is very useful when you need to manipolate some images.
-        
-        Our goal is also to make this project open source and maintainable by the community. We would love to.
-        
-        *We believe in the open source community.*
-        
-        ### Getting Started
-        
-        Getting it from PIP
-        
-        ```
-        pip install image-go-nord
-        ```
-        
-        Then you can use [some example](https://github.com/Schrodinger-Hat/ImageGoNord-pip/tree/master/docs/example) to getting started properly!
-        
-        ### Contributing
-        - Follow the contributor guidelines
-        - Follow the code style / requirements
-        - Format for commit messages
-        
-        ### TODO
-        - Testing
-        - Improvements on image quality and supporting any image format
-        - Make contributing guidelines
-        
-        # Authors
-        
-        [TheJoin95](https://github.com/TheJoin95) & [Wabri](https://github.com/Wabri)
-        
-        **NOTE**: we are not (yet) affiliated with the Nordtheme or [Arcticicestudio](https://github.com/arcticicestudio).
-        
-        # Credits
-        
-        [Nordtheme](https://www.nordtheme.com/)
-        
-        ### License
-        
-        [MIT license](https://github.com/Schrodinger-Hat/ImageGoNord-pip/blob/master/LICENSE)
-        
 Keywords: nordtheme,pillow,image,conversion,rgb,color-scheme,color-palette
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# ImageGoNord - RGB image to Nordtheme palette
+
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/image-go-nord)
+[![PyPI](https://img.shields.io/pypi/v/image-go-nord)](https://pypi.org/project/image-go-nord/)
+[![license](https://img.shields.io/badge/license-MIT-green)](https://github.com/Schrodinger-Hat/ImageGoNord-pip/blob/master/LICENSE)
+[![Join the community on Spectrum](https://withspectrum.github.io/badge/badge.svg)](https://spectrum.chat/image-go-nord)
+
+A tool that can convert your rgb images to nordtheme palette.
+
+This repository is a python package that can convert any sort of image into a [nordtheme](https://github.com/arcticicestudio/nord) palette image.
+
+You can find a demo on [the website](https://ign.schrodinger-hat.it) for testing out the package.
+
+We build also a little API hosted on Heroku to give to anyone the change to test it out by theirself. You can find the documentation on the website too.
+
+The main repository of this whole project is [ImageGoNord](https://github.com/Schrodinger-Hat/ImageGoNord).
+
+### Documentation
+
+You can find the [documentation into this repository](https://github.com/Schrodinger-Hat/ImageGoNord-pip/tree/master/docs) and also on the website.
+
+<!--
+@TODO
+- Describe very briefly but clearly what the project does.
+- State if it is out-of-the-box user-friendly, so it’s clear to the user.
+- List its most useful/innovative/noteworthy features.
+- State its goals/what problem(s) it solves.
+- Note and briefly describe any key concepts (technical, philosophical, or both) important to the user’s understanding.
+- Link to any supplementary blog posts or project main pages.
+- Note its development status.
+- If possible, include screenshots and demo videos.
+-->
+
+### Inspiration
+
+We are in love with Nordtheme, that is why we created this repository.
+
+[![Nord Color Palette Overview](https://raw.githubusercontent.com/arcticicestudio/nord-docs/develop/assets/images/nord/repository-color-palettes.svg?sanitize=true)](https://www.nordtheme.com/docs/colors-and-palettes)
+
+Our goal is to make a shortcut to convert anything into this theme, by starting from the images.
+<br>An example could be an awesome wallpaper converted into the Nordtheme palette.
+
+We checked the commnunity and we did not find anything similar or any project that can accomplish this task. So, here we are.
+
+### What you can do with this package
+
+You can convert any image into the nord palette (or others). Here are some examples:
+
+**Original**
+
+[![Original](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test.jpg)](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test.jpg)
+
+
+**Processed with avg algorithm**
+
+[![Original](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-average.jpg)](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-average.jpg)
+
+
+-----
+
+**Original**
+
+[![Original](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-profile.jpg)](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-profile.jpg)
+
+
+**Processed with avg algorithm**
+
+[![Original](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-profile-average.jpg)](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-profile-average.jpg)
+
+-----
+
+You can also convert videos into the nord palette (or others). Here is an example:  
+**Original**  
+
+https://github.com/05Alston/ImageGoNord-pip/assets/89850018/76d4c4a6-9660-4a02-9f46-e5f3f6d0147a
+
+**Processed with algorithm**
+
+https://github.com/05Alston/ImageGoNord-pip/assets/89850018/13822280-c019-49b1-92f7-7c658b33a01d
+
+### Core Technical Concepts
+
+We are using the PIL because it is the most simple library and it is very useful when you need to manipulate some images.
+
+Our goal is also to make this project open source and maintainable by the community. We would love to.
+
+*We believe in the open source community.*
+
+### Getting Started
+
+Getting it from PIP
+
+```
+pip install image-go-nord
+```
+
+Then you can use [some example](https://github.com/Schrodinger-Hat/ImageGoNord-pip/tree/master/docs/example) to getting started properly!
+
+### Contributing
+- Follow the contributor guidelines
+- Follow the code style / requirements
+- Format for commit messages
+
+### TODO
+- Testing
+- Improvements on image quality and supporting any image format
+- Make contributing guidelines
+
+# Authors
+
+[TheJoin95](https://github.com/TheJoin95) & [Wabri](https://github.com/Wabri)
+
+**NOTE**: we are not (yet) affiliated with the Nordtheme or [Arcticicestudio](https://github.com/arcticicestudio).
+
+# Credits
+
+[Nordtheme](https://www.nordtheme.com/)
+
+### License
+
+[MIT license](https://github.com/Schrodinger-Hat/ImageGoNord-pip/blob/master/LICENSE)
+
+
```

### Comparing `image-go-nord-0.1.5/setup.py` & `image-go-nord-0.1.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 ROOT = pathlib.Path('.')
 README = (ROOT / "README.md").read_text()
 
 setup(
     name="image-go-nord",
-    version="0.1.5",
+    version="0.1.6",
     description="A tool for converting RGB image to Nordtheme palette",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/Schrodinger-Hat/ImageGoNord-pip",
     download_url = 'https://github.com/Schrodinger-Hat/ImageGoNord-pip/releases',
     keywords = ['nordtheme', 'pillow', 'image', 'conversion', 'rgb', 'color-scheme', 'color-palette'], 
     author="Schrodinger Hat",
@@ -28,10 +28,10 @@
         "Homepage": "https://ign.schrodinger-hat.it",
         "Source": "https://github.com/Schrodinger-Hat/ImageGoNord-pip",
         "Bug Reports": "https://github.com/Schrodinger-Hat/ImageGoNord-pip/issues",
     },
     packages=find_packages(),
     package_data={'': ['*.txt', 'palettes/*.txt']},
     include_package_data=True,
-    install_requires=["Pillow"],
+    install_requires=["Pillow", "ffmpeg-python", "numpy"],
     python_requires=">=3.5"
 )
```

