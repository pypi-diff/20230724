# Comparing `tmp/yanimage-1.0.1.tar.gz` & `tmp/yanimage-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yanimage-1.0.1.tar", last modified: Mon Jul 24 15:11:25 2023, max compression
+gzip compressed data, was "dist\yanimage-1.0.2.tar", last modified: Mon Jul 24 15:46:55 2023, max compression
```

## Comparing `yanimage-1.0.1.tar` & `yanimage-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 15:11:25.201071 yanimage-1.0.1/
--rw-rw-rw-   0        0        0     1233 2023-07-24 15:11:25.202072 yanimage-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      694 2023-07-24 14:35:20.000000 yanimage-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-24 15:11:25.212283 yanimage-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      532 2023-07-24 15:11:19.000000 yanimage-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-24 15:11:25.170338 yanimage-1.0.1/yanimage/
--rw-rw-rw-   0        0        0      540 2023-07-24 14:33:15.000000 yanimage-1.0.1/yanimage/Download.py
--rw-rw-rw-   0        0        0     1979 2023-07-24 12:49:33.000000 yanimage-1.0.1/yanimage/Parser.py
--rw-rw-rw-   0        0        0       60 2023-07-24 15:08:30.000000 yanimage-1.0.1/yanimage/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 15:11:25.198038 yanimage-1.0.1/yanimage.egg-info/
--rw-rw-rw-   0        0        0     1233 2023-07-24 15:11:25.000000 yanimage-1.0.1/yanimage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-07-24 15:11:25.000000 yanimage-1.0.1/yanimage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 15:11:25.000000 yanimage-1.0.1/yanimage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-24 15:11:25.000000 yanimage-1.0.1/yanimage.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 15:46:55.178862 yanimage-1.0.2/
+-rw-rw-rw-   0        0        0     1233 2023-07-24 15:46:55.179865 yanimage-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      694 2023-07-24 14:35:20.000000 yanimage-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-24 15:46:55.185925 yanimage-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      532 2023-07-24 15:46:38.000000 yanimage-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 15:46:55.148185 yanimage-1.0.2/yanimage/
+-rw-rw-rw-   0        0        0      540 2023-07-24 14:33:15.000000 yanimage-1.0.2/yanimage/Download.py
+-rw-rw-rw-   0        0        0     1963 2023-07-24 15:46:27.000000 yanimage-1.0.2/yanimage/Parser.py
+-rw-rw-rw-   0        0        0       60 2023-07-24 15:17:50.000000 yanimage-1.0.2/yanimage/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 15:46:55.175829 yanimage-1.0.2/yanimage.egg-info/
+-rw-rw-rw-   0        0        0     1233 2023-07-24 15:46:54.000000 yanimage-1.0.2/yanimage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-07-24 15:46:55.000000 yanimage-1.0.2/yanimage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 15:46:54.000000 yanimage-1.0.2/yanimage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-24 15:46:54.000000 yanimage-1.0.2/yanimage.egg-info/top_level.txt
```

### Comparing `yanimage-1.0.1/PKG-INFO` & `yanimage-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yanimage
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python module for searching, getting links and downloading images from Yandex images
 Home-page: UNKNOWN
 Author: Elieren
 Author-email: kir102906@gmail.com
 License: UNKNOWN
 Description: # Yanimage
```

### Comparing `yanimage-1.0.1/README.md` & `yanimage-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `yanimage-1.0.1/setup.py` & `yanimage-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 """
 :author: Elieren
 """
 
-version = '1.0.1'
+version = '1.0.2'
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='yanimage',
     version=version,
```

### Comparing `yanimage-1.0.1/yanimage/Download.py` & `yanimage-1.0.2/yanimage/Download.py`

 * *Files identical despite different names*

### Comparing `yanimage-1.0.1/yanimage/Parser.py` & `yanimage-1.0.2/yanimage/Parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,16 +43,16 @@
         image_link = self.__image_link
         image_link2 = self.__image_link2
         for i in range(len(image_link)):
                 url_image = re.split('img_url=|&from', image_link[i])
 
                 normal_link = url_image[1].replace('%3A', ':').replace(r'%2F', '/').replace('%25','%').replace('%28', '(').replace('%29', ')')
 
-                is_image = 'image' in requests.get(normal_link).headers['content-type']
+                is_image = requests.get(normal_link).status_code
 
-                if is_image:
+                if is_image == 200:
                     self.__url.append(normal_link)
                 
                 else:
                     self.__url.append(image_link2[i])
 
         return self.__url
```

### Comparing `yanimage-1.0.1/yanimage.egg-info/PKG-INFO` & `yanimage-1.0.2/yanimage.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yanimage
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python module for searching, getting links and downloading images from Yandex images
 Home-page: UNKNOWN
 Author: Elieren
 Author-email: kir102906@gmail.com
 License: UNKNOWN
 Description: # Yanimage
```

