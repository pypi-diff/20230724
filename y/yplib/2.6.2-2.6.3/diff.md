# Comparing `tmp/yplib-2.6.2.tar.gz` & `tmp/yplib-2.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-2.6.2.tar", last modified: Mon Jul 24 00:35:56 2023, max compression
+gzip compressed data, was "dist\yplib-2.6.3.tar", last modified: Mon Jul 24 00:40:39 2023, max compression
```

## Comparing `yplib-2.6.2.tar` & `yplib-2.6.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 00:35:56.858426 yplib-2.6.2/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.6.2/LICENSE
--rw-rw-rw-   0        0        0      352 2023-07-24 00:35:56.858426 yplib-2.6.2/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.6.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-24 00:35:56.858426 yplib-2.6.2/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-07-24 00:32:55.000000 yplib-2.6.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-24 00:35:56.852239 yplib-2.6.2/yplib/
--rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.6.2/yplib/__init__.py
--rw-rw-rw-   0        0        0    10012 2023-07-10 07:39:00.000000 yplib-2.6.2/yplib/chart.py
--rw-rw-rw-   0        0        0     8406 2023-07-13 00:33:38.000000 yplib-2.6.2/yplib/chart_html.py
--rw-rw-rw-   0        0        0     1534 2023-07-10 07:30:11.000000 yplib-2.6.2/yplib/db.py
--rw-rw-rw-   0        0        0     5292 2023-07-17 02:22:22.000000 yplib-2.6.2/yplib/file.py
--rw-rw-rw-   0        0        0     6117 2023-07-11 01:16:49.000000 yplib-2.6.2/yplib/http_util.py
--rw-rw-rw-   0        0        0    34094 2023-07-24 00:35:08.000000 yplib-2.6.2/yplib/index.py
--rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.6.2/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.6.2/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.6.2/yplib/markdown.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.6.2/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-07-24 00:35:56.857702 yplib-2.6.2/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-07-24 00:35:56.000000 yplib-2.6.2/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-07-24 00:35:56.000000 yplib-2.6.2/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 00:35:56.000000 yplib-2.6.2/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-24 00:35:56.000000 yplib-2.6.2/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 00:40:39.280934 yplib-2.6.3/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.6.3/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-07-24 00:40:39.280435 yplib-2.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.6.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-24 00:40:39.281228 yplib-2.6.3/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-07-24 00:40:18.000000 yplib-2.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 00:40:39.277541 yplib-2.6.3/yplib/
+-rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.6.3/yplib/__init__.py
+-rw-rw-rw-   0        0        0    10012 2023-07-10 07:39:00.000000 yplib-2.6.3/yplib/chart.py
+-rw-rw-rw-   0        0        0     8406 2023-07-13 00:33:38.000000 yplib-2.6.3/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     1534 2023-07-10 07:30:11.000000 yplib-2.6.3/yplib/db.py
+-rw-rw-rw-   0        0        0     5292 2023-07-17 02:22:22.000000 yplib-2.6.3/yplib/file.py
+-rw-rw-rw-   0        0        0     6117 2023-07-11 01:16:49.000000 yplib-2.6.3/yplib/http_util.py
+-rw-rw-rw-   0        0        0    34070 2023-07-24 00:40:02.000000 yplib-2.6.3/yplib/index.py
+-rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.6.3/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.6.3/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.6.3/yplib/markdown.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.6.3/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-07-24 00:40:39.279934 yplib-2.6.3/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-07-24 00:40:39.000000 yplib-2.6.3/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-07-24 00:40:39.000000 yplib-2.6.3/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 00:40:39.000000 yplib-2.6.3/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-24 00:40:39.000000 yplib-2.6.3/yplib.egg-info/top_level.txt
```

### Comparing `yplib-2.6.2/LICENSE` & `yplib-2.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-2.6.2/setup.py` & `yplib-2.6.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="2.6.2",
+  version="2.6.3",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-2.6.2/yplib/__init__.py` & `yplib-2.6.3/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-2.6.2/yplib/chart.py` & `yplib-2.6.3/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-2.6.2/yplib/chart_html.py` & `yplib-2.6.3/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.6.2/yplib/db.py` & `yplib-2.6.3/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-2.6.2/yplib/file.py` & `yplib-2.6.3/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-2.6.2/yplib/http_util.py` & `yplib-2.6.3/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-2.6.2/yplib/index.py` & `yplib-2.6.3/yplib/index.py`

 * *Files 0% similar despite different names*

```diff
@@ -794,15 +794,15 @@
                 column_date=column_date,
                 column_datetime=column_datetime)
     return str_join.join(d) if r_str else json.loads(str_join.join(d)) if r_json else d
 
 
 def to_excel(data_list, file_name=None, file_path='excel'):
     if file_name is None:
-        file_name = get_file_name('excel', '.xlsx')
+        file_name = 'excel'
         sheet_name = 'Sheet1'
     else:
         sheet_name = file_name
     file_name = str(file_name)
     while file_path.endswith('/'):
         file_path = file_path[0:-1]
     check_file(file_path)
```

### Comparing `yplib-2.6.2/yplib/mail.py` & `yplib-2.6.3/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-2.6.2/yplib/mail_html.py` & `yplib-2.6.3/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.6.2/yplib/markdown.py` & `yplib-2.6.3/yplib/markdown.py`

 * *Files identical despite different names*

