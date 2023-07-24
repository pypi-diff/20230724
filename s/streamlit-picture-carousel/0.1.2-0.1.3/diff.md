# Comparing `tmp/streamlit-picture-carousel-0.1.2.tar.gz` & `tmp/streamlit-picture-carousel-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-picture-carousel-0.1.2.tar", last modified: Mon Jul 24 18:34:13 2023, max compression
+gzip compressed data, was "streamlit-picture-carousel-0.1.3.tar", last modified: Mon Jul 24 18:56:58 2023, max compression
```

## Comparing `streamlit-picture-carousel-0.1.2.tar` & `streamlit-picture-carousel-0.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:34:13.632721 streamlit-picture-carousel-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-24 18:34:02.000000 streamlit-picture-carousel-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-24 18:34:02.000000 streamlit-picture-carousel-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-24 18:34:13.632721 streamlit-picture-carousel-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-24 18:34:02.000000 streamlit-picture-carousel-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 18:34:13.632721 streamlit-picture-carousel-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-24 18:34:02.000000 streamlit-picture-carousel-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:34:13.632721 streamlit-picture-carousel-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:34:13.632721 streamlit-picture-carousel-0.1.2/src/st_picture_carousel/
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-24 18:34:02.000000 streamlit-picture-carousel-0.1.2/src/st_picture_carousel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:34:13.632721 streamlit-picture-carousel-0.1.2/src/st_picture_carousel/frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:34:13.632721 streamlit-picture-carousel-0.1.2/src/st_picture_carousel/frontend/carousel/
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-24 18:34:02.000000 streamlit-picture-carousel-0.1.2/src/st_picture_carousel/frontend/carousel/carousel.css
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-24 18:34:02.000000 streamlit-picture-carousel-0.1.2/src/st_picture_carousel/frontend/carousel/carousel.html
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-24 18:34:02.000000 streamlit-picture-carousel-0.1.2/src/st_picture_carousel/frontend/carousel/carousel.js
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-24 18:34:02.000000 streamlit-picture-carousel-0.1.2/src/st_picture_carousel/frontend/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-24 18:34:02.000000 streamlit-picture-carousel-0.1.2/src/st_picture_carousel/frontend/main.js
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-24 18:34:02.000000 streamlit-picture-carousel-0.1.2/src/st_picture_carousel/frontend/streamlit-component-lib.js
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:34:02.000000 streamlit-picture-carousel-0.1.2/src/st_picture_carousel/frontend/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:34:13.632721 streamlit-picture-carousel-0.1.2/src/streamlit_picture_carousel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-24 18:34:13.000000 streamlit-picture-carousel-0.1.2/src/streamlit_picture_carousel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-24 18:34:13.000000 streamlit-picture-carousel-0.1.2/src/streamlit_picture_carousel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:34:13.000000 streamlit-picture-carousel-0.1.2/src/streamlit_picture_carousel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 18:34:13.000000 streamlit-picture-carousel-0.1.2/src/streamlit_picture_carousel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-24 18:34:13.000000 streamlit-picture-carousel-0.1.2/src/streamlit_picture_carousel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:56:58.821443 streamlit-picture-carousel-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-24 18:56:46.000000 streamlit-picture-carousel-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-24 18:56:46.000000 streamlit-picture-carousel-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-24 18:56:58.821443 streamlit-picture-carousel-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-24 18:56:46.000000 streamlit-picture-carousel-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 18:56:58.821443 streamlit-picture-carousel-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-24 18:56:46.000000 streamlit-picture-carousel-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:56:58.817443 streamlit-picture-carousel-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:56:58.817443 streamlit-picture-carousel-0.1.3/src/st_picture_carousel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-24 18:56:46.000000 streamlit-picture-carousel-0.1.3/src/st_picture_carousel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:56:58.817443 streamlit-picture-carousel-0.1.3/src/st_picture_carousel/frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:56:58.817443 streamlit-picture-carousel-0.1.3/src/st_picture_carousel/frontend/carousel/
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-24 18:56:46.000000 streamlit-picture-carousel-0.1.3/src/st_picture_carousel/frontend/carousel/carousel.css
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-24 18:56:46.000000 streamlit-picture-carousel-0.1.3/src/st_picture_carousel/frontend/carousel/carousel.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-24 18:56:46.000000 streamlit-picture-carousel-0.1.3/src/st_picture_carousel/frontend/carousel/carousel.js
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-24 18:56:46.000000 streamlit-picture-carousel-0.1.3/src/st_picture_carousel/frontend/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-24 18:56:46.000000 streamlit-picture-carousel-0.1.3/src/st_picture_carousel/frontend/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-24 18:56:46.000000 streamlit-picture-carousel-0.1.3/src/st_picture_carousel/frontend/streamlit-component-lib.js
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:56:46.000000 streamlit-picture-carousel-0.1.3/src/st_picture_carousel/frontend/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:56:58.821443 streamlit-picture-carousel-0.1.3/src/streamlit_picture_carousel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-24 18:56:58.000000 streamlit-picture-carousel-0.1.3/src/streamlit_picture_carousel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-24 18:56:58.000000 streamlit-picture-carousel-0.1.3/src/streamlit_picture_carousel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:56:58.000000 streamlit-picture-carousel-0.1.3/src/streamlit_picture_carousel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 18:56:58.000000 streamlit-picture-carousel-0.1.3/src/streamlit_picture_carousel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-24 18:56:58.000000 streamlit-picture-carousel-0.1.3/src/streamlit_picture_carousel.egg-info/top_level.txt
```

### Comparing `streamlit-picture-carousel-0.1.2/LICENSE` & `streamlit-picture-carousel-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-picture-carousel-0.1.2/PKG-INFO` & `streamlit-picture-carousel-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-picture-carousel
-Version: 0.1.2
+Version: 0.1.3
 Summary: Displays 3d carousel of pictures
 Author: Rafal Cegiela
 Author-email: rcegiela@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `streamlit-picture-carousel-0.1.2/setup.py` & `streamlit-picture-carousel-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="streamlit-picture-carousel",
-    version="0.1.2",
+    version="0.1.3",
     author="Rafal Cegiela",
     author_email="rcegiela@gmail.com",
     description="Displays 3d carousel of pictures",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     package_dir={"": "src"},
```

### Comparing `streamlit-picture-carousel-0.1.2/src/st_picture_carousel/__init__.py` & `streamlit-picture-carousel-0.1.3/src/st_picture_carousel/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 
     return component_value
 
 
 def main():
     st.subheader("Example [st.header]")
     img_list=os.listdir("static/portraits")
-    st_picture_carousel(n_pics=9,
-                        cell=('300px', '150px'),
-                        img_path=r"/static/portraits",
+    st_picture_carousel(cell=("250px", "200px"),
+                        img_path=r"/app/static/portraits",
                         img_list=img_list,
-                        img_size=('180px', '130px'))
+                        img_size=("180px", "180px")))
 
 if __name__ == "__main__":
     main()
```

### Comparing `streamlit-picture-carousel-0.1.2/src/st_picture_carousel/frontend/carousel/carousel.css` & `streamlit-picture-carousel-0.1.3/src/st_picture_carousel/frontend/carousel/carousel.css`

 * *Files identical despite different names*

### Comparing `streamlit-picture-carousel-0.1.2/src/st_picture_carousel/frontend/carousel/carousel.html` & `streamlit-picture-carousel-0.1.3/src/st_picture_carousel/frontend/carousel/carousel.html`

 * *Files identical despite different names*

### Comparing `streamlit-picture-carousel-0.1.2/src/st_picture_carousel/frontend/carousel/carousel.js` & `streamlit-picture-carousel-0.1.3/src/st_picture_carousel/frontend/carousel/carousel.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -5,16 +5,16 @@
 var urlParams = new URLSearchParams(window.location.search);
 var n_pics = urlParams.get('n_pics');
 var cell = urlParams.get('cell').split(',');
 var img_path = urlParams.get('img_path');
 var img_list = urlParams.get('img_list').split(',');
 var img_size = urlParams.get('img_size').split(',');
 
-const testpara = document.getElementById("test_para")
-testpara.innerHTML = location.href
+// const testpara = document.getElementById("test_para")
+// testpara.innerHTML = location.href
 
 if (img_path) {
     n_pics = img_list.length;
 }
 
 for (var i = 0; i < n_pics; i++) {
     var div = document.createElement("div");
```

### Comparing `streamlit-picture-carousel-0.1.2/src/st_picture_carousel/frontend/index.html` & `streamlit-picture-carousel-0.1.3/src/st_picture_carousel/frontend/index.html`

 * *Files identical despite different names*

### Comparing `streamlit-picture-carousel-0.1.2/src/st_picture_carousel/frontend/main.js` & `streamlit-picture-carousel-0.1.3/src/st_picture_carousel/frontend/main.js`

 * *Files identical despite different names*

### Comparing `streamlit-picture-carousel-0.1.2/src/st_picture_carousel/frontend/streamlit-component-lib.js` & `streamlit-picture-carousel-0.1.3/src/st_picture_carousel/frontend/streamlit-component-lib.js`

 * *Files identical despite different names*

### Comparing `streamlit-picture-carousel-0.1.2/src/streamlit_picture_carousel.egg-info/PKG-INFO` & `streamlit-picture-carousel-0.1.3/src/streamlit_picture_carousel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-picture-carousel
-Version: 0.1.2
+Version: 0.1.3
 Summary: Displays 3d carousel of pictures
 Author: Rafal Cegiela
 Author-email: rcegiela@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `streamlit-picture-carousel-0.1.2/src/streamlit_picture_carousel.egg-info/SOURCES.txt` & `streamlit-picture-carousel-0.1.3/src/streamlit_picture_carousel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

