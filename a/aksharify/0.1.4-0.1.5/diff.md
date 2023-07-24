# Comparing `tmp/aksharify-0.1.4.tar.gz` & `tmp/aksharify-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aksharify-0.1.4.tar", max compression
+gzip compressed data, was "aksharify-0.1.5.tar", max compression
```

## Comparing `aksharify-0.1.4.tar` & `aksharify-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1094 2023-07-22 05:33:48.477839 aksharify-0.1.4/LICENSE.md
--rw-r--r--   0        0        0      674 2023-07-22 07:25:07.132234 aksharify-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     5988 2023-07-22 03:57:31.621402 aksharify-0.1.4/README.md
--rw-r--r--   0        0        0       55 2023-07-21 04:56:00.214997 aksharify-0.1.4/src/aksharify/__init__.py
--rw-r--r--   0        0        0     3529 2023-07-22 07:23:50.694034 aksharify-0.1.4/src/aksharify/aksharify.py
--rw-r--r--   0        0        0     5274 2023-07-20 14:19:37.279133 aksharify-0.1.4/src/aksharify/distributions.py
--rw-r--r--   0        0        0     1556 2023-07-18 11:04:22.323563 aksharify-0.1.4/src/aksharify/image.py
--rw-r--r--   0        0        0     4711 2023-07-18 04:15:13.427078 aksharify-0.1.4/src/aksharify/outputs.py
--rw-r--r--   0        0        0     6660 1970-01-01 00:00:00.000000 aksharify-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1094 2023-07-22 05:33:48.477839 aksharify-0.1.5/LICENSE.md
+-rw-r--r--   0        0        0      674 2023-07-24 11:53:11.163367 aksharify-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     5988 2023-07-22 03:57:31.621402 aksharify-0.1.5/README.md
+-rw-r--r--   0        0        0       55 2023-07-21 04:56:00.214997 aksharify-0.1.5/src/aksharify/__init__.py
+-rw-r--r--   0        0        0     5546 2023-07-24 11:46:55.981672 aksharify-0.1.5/src/aksharify/aksharify.py
+-rw-r--r--   0        0        0     5274 2023-07-24 11:33:53.947835 aksharify-0.1.5/src/aksharify/distributions.py
+-rw-r--r--   0        0        0     1565 2023-07-23 09:44:07.082682 aksharify-0.1.5/src/aksharify/image.py
+-rw-r--r--   0        0        0     4946 2023-07-23 04:22:55.602321 aksharify-0.1.5/src/aksharify/outputs.py
+-rw-r--r--   0        0        0     6659 1970-01-01 00:00:00.000000 aksharify-0.1.5/PKG-INFO
```

### Comparing `aksharify-0.1.4/LICENSE.md` & `aksharify-0.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aksharify-0.1.4/pyproject.toml` & `aksharify-0.1.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "aksharify"
-version = "0.1.4"
+version = "0.1.5"
 description = "Ascii Art + Emoji Art python Package"
 authors = ["Prime Patel <primespatel@gmail.com>"]
 readme = "README.md"
 packages = [{include = "aksharify", from = "src"}]
 license = "MIT"
 homepage = "https://primepatel.github.io/aksharify/"
 repository = "https://github.com/primepatel/aksharify"
 keywords = ["Ascii Art","Emoji Art","Prime Patel","primepatel"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-pillow = "^9.3.0"
-scikit-image = "^0.21.0"
+pillow = "^8.4.0"
+scikit-image = "^0.19.3"
 matplotlib = "^3.7.1"
 cairosvg = "^2.7.0"
-ipython = "^8.14.0"
+ipython = "^7.34.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `aksharify-0.1.4/README.md` & `aksharify-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `aksharify-0.1.4/src/aksharify/distributions.py` & `aksharify-0.1.5/src/aksharify/distributions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import numpy as np
 import matplotlib.pyplot as plt
 
-SORTEDCHARS = """ `.-_',~:*;!"^/\+><r=?()|7LxtcYivTljsz[]1Jnufy{}oI#FC4VX2ehk3aZw5ASbdpqUP6%9G8mKO&0EDHg$MWRNQB@"""
-
+SORTEDCHARS = '@BQNRWM$gHDE0&OKm8G9%6PUqpdbSA5wZa3khe2XV4CF#Io}{yfunJ1][zsjlTviYctxL7|)(?=r<>+\\/^"!;*:~,\'_-.` '
 class Dist:
-    def __init__(self, chars, unique=True, order=False) -> None:
+    def __init__(self, chars, order=False, unique=False) -> None:
         if unique:
             self.chars = []
             for char in chars:
                 if char not in self.chars:
                     self.chars.append(char)
         else:
             self.chars = list(chars)
@@ -68,37 +67,37 @@
         plt.xlim(0, 1)
         plt.ylim(0, 1)
         plt.show()
         self.normal_to_hex()
 
 
 class Linear(Dist):
-    def __init__(self, chars, unique=True, order=False) -> None:
-        super().__init__(chars, unique, order)
+    def __init__(self, chars, order=False, unique=False) -> None:
+        super().__init__(chars, order, unique)
         num = 255/len(self.chars)
         self.list = [0]
         for i in range(len(self.chars)):
             j = int(num * (i + 1))
             self.list.append(j)
         self.list[-1] = 255
         self.list = np.array(self.list)
         self.generate_char_dict()
 
 class Exponential(Linear):
-    def __init__(self, chars, power, unique=True, order=False) -> None:
-        super().__init__(chars, unique, order)
+    def __init__(self, chars, power, order=False, unique=False) -> None:
+        super().__init__(chars, order, unique)
         self.hex_to_normal()
         self.list = self.list**power
         self.normal_to_hex()
         self.y = lambda x: x**power
         self.generate_char_dict()  
         
 class Normal(Linear):
-    def __init__(self, chars, mean, var, unique=True, order=False) -> None:
-        super().__init__(chars, unique, order)
+    def __init__(self, chars, mean, var, order=False, unique=False) -> None:
+        super().__init__(chars, order, unique)
         self.mean = mean
         self.var = var
         self.hex_to_normal()
         self.list[0], self.list[-1] = 0.0001, 0.9999
         self.list = self.normalizer(self.list)
         self.normal_to_hex()
         self.y = self.normalizer
```

### Comparing `aksharify-0.1.4/src/aksharify/image.py` & `aksharify-0.1.5/src/aksharify/image.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,37 +2,37 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import requests
 from io import BytesIO
 
 class Image:
 
-    def __init__(self, image=None, url=None) -> None:
+    def __init__(self, path=None, url=None) -> None:
         self.CH_CONSTANT = 1.78
-        if image and url:
+        if path and url:
             raise ValueError("Provide image or link to the Image")
-        elif image:
-            self.obj = ski.io.imread(image)
+        elif path:
+            self.obj = ski.io.imread(path)
         else:
             response = requests.get(url)
             image_data = response.content
             self.obj = ski.io.imread(BytesIO(image_data))
         self.image = self.obj
         self.bwimg = ski.color.rgb2gray(self.obj[:,:,:3])
         self.w, self.h = self.obj.shape[1], self.obj.shape[0]
         
-    def show(self, bw=False):
+    def show(self, grayscale=False):
         plt.axis('off')
-        if not bw:
+        if not grayscale:
             plt.imshow(self.image)
         else:
             plt.imshow(self.bwimg, cmap='gray')
         plt.show()
 
-    def set_dim(self, width:int=None, height:int=None):
+    def resize(self, width:int=None, height:int=None):
         if width != None and height == None:
             w, h = width, int((self.h/self.w * width)/self.CH_CONSTANT)
         elif width == None and height != None:
             w, h = int((self.w/self.h * height) * self.CH_CONSTANT), height
         else:
             w, h = width, height
         self.image = ski.transform.resize(self.obj, (h, w), anti_aliasing=True)
```

### Comparing `aksharify-0.1.4/src/aksharify/outputs.py` & `aksharify-0.1.5/src/aksharify/outputs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 LINK = "https://primepatel.github.io/aksharify/"
 SVG_HEADER = '<?xml version="1.0" standalone="no"?><svg width="{}" height="{}" version="1.1" xmlns="http://www.w3.org/2000/svg" style="font-family: {}; font-size:{};"><desc>Aksharify Art</desc><rect width="100%" height="100%" fill="{}"/>'
 HTML_HEADER = '<!DOCTYPE html><html lang="en"><head><meta charset="UTF-8"><meta name="viewport" content="width=device-width, initial-scale=1.0"><title>Aksharify Art</title></head><body><a href="https://primepatel.github.io/aksharify/" style="text-decoration: none">{}</a></body></html>'
 
+class TXT:
+    def __init__(self) -> None:
+        self.type = 'TXT'
+        self.title = None
 
 class HTML:
     
     def __init__(self):
+        self.type = 'HTML'
         self.title = "Aksharify Art"
         self.link = LINK # not added yet
         self.font_family = "monospace"
         self.font_size = 10
         self.bold = False
         self.file_name = "aksharify"
 
@@ -37,14 +42,15 @@
         html_content += "</p>"
         return HTML_HEADER.format(html_content)
 
 
 class SVG:
     
     def __init__(self):
+        self.type = 'SVG'
         self.font_family = "monospace"
         self.font_size = 10
         self.background_color = "#ffffff"
         self.link = LINK # not added yet
         self.bold = False
         self.fill_color = None
         self.file_name = "aksharify"
@@ -93,28 +99,31 @@
             file += "</svg>"
         return file
 
 
 class PNG(SVG):
     def __init__(self) -> None:
         super().__init__()
+        self.type = 'PNG'
         self.width = None
         self.height = None
         
     def generate_svg(self, matrix, image) -> None:
         return self.generate_art(matrix, image)
 
 
 class PDF(SVG):
     def __init__(self) -> None:
         super().__init__()
+        self.type = 'PDF'
         
     def generate_svg(self, matrix, image) -> None:
         return self.generate_art(matrix, image)
     
 
 class EPS(SVG):
     def __init__(self) -> None:
         super().__init__()
+        self.type = 'EPS'
         
     def generate_svg(self, matrix, image) -> None:
         return self.generate_art(matrix, image)
```

### Comparing `aksharify-0.1.4/PKG-INFO` & `aksharify-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: aksharify
-Version: 0.1.4
+Version: 0.1.5
 Summary: Ascii Art + Emoji Art python Package
 Home-page: https://primepatel.github.io/aksharify/
 License: MIT
 Keywords: Ascii Art,Emoji Art,Prime Patel,primepatel
 Author: Prime Patel
 Author-email: primespatel@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cairosvg (>=2.7.0,<3.0.0)
-Requires-Dist: ipython (>=8.14.0,<9.0.0)
+Requires-Dist: ipython (>=7.34.0,<8.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
-Requires-Dist: pillow (>=9.3.0,<10.0.0)
-Requires-Dist: scikit-image (>=0.21.0,<0.22.0)
+Requires-Dist: pillow (>=8.4.0,<9.0.0)
+Requires-Dist: scikit-image (>=0.19.3,<0.20.0)
 Project-URL: Repository, https://github.com/primepatel/aksharify
 Description-Content-Type: text/markdown
 
 <a name="readme-top"></a>
 
 # __Aksharify__
```

