# Comparing `tmp/isyveri-0.1.2.tar.gz` & `tmp/isyveri-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isyveri-0.1.2.tar", last modified: Mon Jul 24 17:17:11 2023, max compression
+gzip compressed data, was "isyveri-0.1.3.tar", last modified: Mon Jul 24 17:34:56 2023, max compression
```

## Comparing `isyveri-0.1.2.tar` & `isyveri-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 17:17:11.531561 isyveri-0.1.2/
--rw-rw-rw-   0        0        0     1064 2023-07-23 21:22:22.000000 isyveri-0.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0     4469 2023-07-24 17:17:11.525584 isyveri-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     4086 2023-07-24 16:27:44.000000 isyveri-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-24 17:17:11.470720 isyveri-0.1.2/isyveri/
--rw-rw-rw-   0        0        0     3058 2023-07-24 13:39:38.000000 isyveri-0.1.2/isyveri/VeriCek.py
--rw-rw-rw-   0        0        0       29 2023-07-24 11:50:14.000000 isyveri-0.1.2/isyveri/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 17:17:11.509617 isyveri-0.1.2/isyveri.egg-info/
--rw-rw-rw-   0        0        0     4469 2023-07-24 17:17:11.000000 isyveri-0.1.2/isyveri.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-07-24 17:17:11.000000 isyveri-0.1.2/isyveri.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 17:17:11.000000 isyveri-0.1.2/isyveri.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-07-24 17:17:11.000000 isyveri-0.1.2/isyveri.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-24 17:17:11.000000 isyveri-0.1.2/isyveri.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-24 17:17:11.532555 isyveri-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      601 2023-07-24 17:12:39.000000 isyveri-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 17:34:56.350675 isyveri-0.1.3/
+-rw-rw-rw-   0        0        0     1064 2023-07-23 21:22:22.000000 isyveri-0.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     4618 2023-07-24 17:34:56.343695 isyveri-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4086 2023-07-24 16:27:44.000000 isyveri-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 17:34:56.286845 isyveri-0.1.3/isyveri/
+-rw-rw-rw-   0        0        0     3058 2023-07-24 13:39:38.000000 isyveri-0.1.3/isyveri/VeriCek.py
+-rw-rw-rw-   0        0        0       29 2023-07-24 11:50:14.000000 isyveri-0.1.3/isyveri/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 17:34:56.338706 isyveri-0.1.3/isyveri.egg-info/
+-rw-rw-rw-   0        0        0     4618 2023-07-24 17:34:55.000000 isyveri-0.1.3/isyveri.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-07-24 17:34:56.000000 isyveri-0.1.3/isyveri.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 17:34:55.000000 isyveri-0.1.3/isyveri.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-07-24 17:34:55.000000 isyveri-0.1.3/isyveri.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-24 17:34:55.000000 isyveri-0.1.3/isyveri.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 17:34:56.351672 isyveri-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      774 2023-07-24 17:34:42.000000 isyveri-0.1.3/setup.py
```

### Comparing `isyveri-0.1.2/LICENSE.txt` & `isyveri-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `isyveri-0.1.2/PKG-INFO` & `isyveri-0.1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: isyveri
-Version: 0.1.2
-Summary: İş Yatırım'ın web sitesinden veri çekme işlemlerini kolaylaştıran ve isteğe göre özelleştirilebilen bir kütüphane.
-Home-page: https://github.com/urazakgul/isyveri
-Author: Uraz Akgül
-Author-email: urazdev@gmail.com
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # isyveri v0.1.0
 
 ## Aciklama
 
 isyveri, Is Yatirim'in web sitesinden veri cekme islemlerini kolaylastirmak amaciyla gelistirilmis, istege gore ozellestirilebilir bir Python kutuphanesidir.
 
 ## Kurulum
@@ -161,8 +150,8 @@
 
 ### v0.1.0 - 24/07/2023
 
 * Ilk surum yayinlandi.
 
 ## Lisans
 
-Bu proje MIT Lisansi altinda lisanslanmistir - [LICENSE](LICENSE.txt) dosyasina bakin.
+Bu proje MIT Lisansi altinda lisanslanmistir - [LICENSE](LICENSE.txt) dosyasina bakin.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `isyveri-0.1.2/README.md` & `isyveri-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: isyveri
+Version: 0.1.3
+Summary: İş Yatırım'ın web sitesinden veri çekme işlemlerini kolaylaştıran ve isteğe göre özelleştirilebilen bir kütüphane.
+Home-page: https://github.com/urazakgul/isyveri
+Author: Uraz Akgül
+Author-email: urazdev@gmail.com
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # isyveri v0.1.0
 
 ## Aciklama
 
 isyveri, Is Yatirim'in web sitesinden veri cekme islemlerini kolaylastirmak amaciyla gelistirilmis, istege gore ozellestirilebilir bir Python kutuphanesidir.
 
 ## Kurulum
@@ -150,8 +164,8 @@
 
 ### v0.1.0 - 24/07/2023
 
 * Ilk surum yayinlandi.
 
 ## Lisans
 
-Bu proje MIT Lisansi altinda lisanslanmistir - [LICENSE](LICENSE.txt) dosyasina bakin.
+Bu proje MIT Lisansi altinda lisanslanmistir - [LICENSE](LICENSE.txt) dosyasina bakin.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `isyveri-0.1.2/isyveri/VeriCek.py` & `isyveri-0.1.3/isyveri/VeriCek.py`

 * *Files identical despite different names*

### Comparing `isyveri-0.1.2/isyveri.egg-info/PKG-INFO` & `isyveri-0.1.3/isyveri.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: isyveri
-Version: 0.1.2
+Version: 0.1.3
 Summary: İş Yatırım'ın web sitesinden veri çekme işlemlerini kolaylaştıran ve isteğe göre özelleştirilebilen bir kütüphane.
 Home-page: https://github.com/urazakgul/isyveri
 Author: Uraz Akgül
 Author-email: urazdev@gmail.com
 License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # isyveri v0.1.0
 
 ## Aciklama
```

