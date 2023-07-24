# Comparing `tmp/streamlit-picture-carousel-0.1.0.tar.gz` & `tmp/streamlit-picture-carousel-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-picture-carousel-0.1.0.tar", last modified: Sat Jul 22 09:48:00 2023, max compression
+gzip compressed data, was "streamlit-picture-carousel-0.1.2.tar", last modified: Mon Jul 24 18:34:13 2023, max compression
```

## Comparing `streamlit-picture-carousel-0.1.0.tar` & `streamlit-picture-carousel-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:48:00.677175 streamlit-picture-carousel-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-22 09:47:50.000000 streamlit-picture-carousel-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-22 09:47:50.000000 streamlit-picture-carousel-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-22 09:48:00.673175 streamlit-picture-carousel-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-22 09:47:50.000000 streamlit-picture-carousel-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 09:48:00.677175 streamlit-picture-carousel-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-22 09:47:50.000000 streamlit-picture-carousel-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:48:00.673175 streamlit-picture-carousel-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:48:00.673175 streamlit-picture-carousel-0.1.0/src/st_picture_carousel/
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-22 09:47:50.000000 streamlit-picture-carousel-0.1.0/src/st_picture_carousel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:48:00.673175 streamlit-picture-carousel-0.1.0/src/st_picture_carousel/frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:48:00.673175 streamlit-picture-carousel-0.1.0/src/st_picture_carousel/frontend/carousel/
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-22 09:47:50.000000 streamlit-picture-carousel-0.1.0/src/st_picture_carousel/frontend/carousel/carousel.css
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-22 09:47:50.000000 streamlit-picture-carousel-0.1.0/src/st_picture_carousel/frontend/carousel/carousel.html
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-22 09:47:50.000000 streamlit-picture-carousel-0.1.0/src/st_picture_carousel/frontend/carousel/carousel.js
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-22 09:47:50.000000 streamlit-picture-carousel-0.1.0/src/st_picture_carousel/frontend/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-22 09:47:50.000000 streamlit-picture-carousel-0.1.0/src/st_picture_carousel/frontend/main.js
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-22 09:47:50.000000 streamlit-picture-carousel-0.1.0/src/st_picture_carousel/frontend/streamlit-component-lib.js
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 09:47:50.000000 streamlit-picture-carousel-0.1.0/src/st_picture_carousel/frontend/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:48:00.673175 streamlit-picture-carousel-0.1.0/src/streamlit_picture_carousel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-22 09:48:00.000000 streamlit-picture-carousel-0.1.0/src/streamlit_picture_carousel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-22 09:48:00.000000 streamlit-picture-carousel-0.1.0/src/streamlit_picture_carousel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 09:48:00.000000 streamlit-picture-carousel-0.1.0/src/streamlit_picture_carousel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-22 09:48:00.000000 streamlit-picture-carousel-0.1.0/src/streamlit_picture_carousel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-22 09:48:00.000000 streamlit-picture-carousel-0.1.0/src/streamlit_picture_carousel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:34:13.632721 streamlit-picture-carousel-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-24 18:34:02.000000 streamlit-picture-carousel-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-24 18:34:02.000000 streamlit-picture-carousel-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-24 18:34:13.632721 streamlit-picture-carousel-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-24 18:34:02.000000 streamlit-picture-carousel-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 18:34:13.632721 streamlit-picture-carousel-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-24 18:34:02.000000 streamlit-picture-carousel-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:34:13.632721 streamlit-picture-carousel-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:34:13.632721 streamlit-picture-carousel-0.1.2/src/st_picture_carousel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-24 18:34:02.000000 streamlit-picture-carousel-0.1.2/src/st_picture_carousel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:34:13.632721 streamlit-picture-carousel-0.1.2/src/st_picture_carousel/frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:34:13.632721 streamlit-picture-carousel-0.1.2/src/st_picture_carousel/frontend/carousel/
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-24 18:34:02.000000 streamlit-picture-carousel-0.1.2/src/st_picture_carousel/frontend/carousel/carousel.css
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-24 18:34:02.000000 streamlit-picture-carousel-0.1.2/src/st_picture_carousel/frontend/carousel/carousel.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-24 18:34:02.000000 streamlit-picture-carousel-0.1.2/src/st_picture_carousel/frontend/carousel/carousel.js
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-24 18:34:02.000000 streamlit-picture-carousel-0.1.2/src/st_picture_carousel/frontend/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-24 18:34:02.000000 streamlit-picture-carousel-0.1.2/src/st_picture_carousel/frontend/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-24 18:34:02.000000 streamlit-picture-carousel-0.1.2/src/st_picture_carousel/frontend/streamlit-component-lib.js
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:34:02.000000 streamlit-picture-carousel-0.1.2/src/st_picture_carousel/frontend/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:34:13.632721 streamlit-picture-carousel-0.1.2/src/streamlit_picture_carousel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-24 18:34:13.000000 streamlit-picture-carousel-0.1.2/src/streamlit_picture_carousel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-24 18:34:13.000000 streamlit-picture-carousel-0.1.2/src/streamlit_picture_carousel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:34:13.000000 streamlit-picture-carousel-0.1.2/src/streamlit_picture_carousel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 18:34:13.000000 streamlit-picture-carousel-0.1.2/src/streamlit_picture_carousel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-24 18:34:13.000000 streamlit-picture-carousel-0.1.2/src/streamlit_picture_carousel.egg-info/top_level.txt
```

### Comparing `streamlit-picture-carousel-0.1.0/LICENSE` & `streamlit-picture-carousel-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-picture-carousel-0.1.0/PKG-INFO` & `streamlit-picture-carousel-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-picture-carousel
-Version: 0.1.0
+Version: 0.1.2
 Summary: Displays 3d carousel of pictures
 Author: Rafal Cegiela
 Author-email: rcegiela@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `streamlit-picture-carousel-0.1.0/setup.py` & `streamlit-picture-carousel-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="streamlit-picture-carousel",
-    version="0.1.0",
+    version="0.1.2",
     author="Rafal Cegiela",
     author_email="rcegiela@gmail.com",
     description="Displays 3d carousel of pictures",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     package_dir={"": "src"},
```

### Comparing `streamlit-picture-carousel-0.1.0/src/st_picture_carousel/__init__.py` & `streamlit-picture-carousel-0.1.2/src/st_picture_carousel/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,49 @@
 from pathlib import Path
 from typing import Optional
 
 import streamlit as st
 import streamlit.components.v1 as components
+import os
 
 # Tell streamlit that there is a component called st_picture_carousel,
 # and that the code to display that component is in the "frontend" folder
 frontend_dir = (Path(__file__).parent / "frontend").absolute()
 _component_func = components.declare_component(
     "st_picture_carousel", path=str(frontend_dir)
 )
 
 # Create the python function that will be called
 def st_picture_carousel(
         n_pics: Optional[int] = 7,
+        cell: Optional[tuple[str, str]] = ('190px', '120px'),
+        img_path: Optional[str] = "",
+        img_list: Optional[list[str]]=[],
+        img_size: Optional[tuple[str, str]] = ('100px', '50px'),
         key: Optional[str] = None,
 ):
     """
     Add a descriptive docstring
     """
     component_value = _component_func(
         n_pics=n_pics,
+        cell=cell,
+        img_path=img_path,
+        img_list=img_list,
+        img_size=img_size,
         key=key,
     )
 
     return component_value
 
 
 def main():
     st.subheader("Example [st.header]")
-    value = st_picture_carousel(15)
-    value = st_picture_carousel(7)
+    img_list=os.listdir("static/portraits")
+    st_picture_carousel(n_pics=9,
+                        cell=('300px', '150px'),
+                        img_path=r"/static/portraits",
+                        img_list=img_list,
+                        img_size=('180px', '130px'))
 
 if __name__ == "__main__":
     main()
```

### Comparing `streamlit-picture-carousel-0.1.0/src/st_picture_carousel/frontend/carousel/carousel.css` & `streamlit-picture-carousel-0.1.2/src/st_picture_carousel/frontend/carousel/carousel.css`

 * *Files 8% similar despite different names*

```diff
@@ -58,13 +58,20 @@
 .carousel__cell:nth-child(5) { transform: rotateY(160deg) translateZ(500px); }
 .carousel__cell:nth-child(6) { transform: rotateY(200deg) translateZ(500px); }
 .carousel__cell:nth-child(7) { transform: rotateY(240deg) translateZ(500px); }
 .carousel__cell:nth-child(8) { transform: rotateY(280deg) translateZ(500px); }
 .carousel__cell:nth-child(9) { transform: rotateY(320deg) translateZ(500px); }
 */
 
-.carousel-options {
-  text-align: center;
-  position: relative;
-  z-index: 2;
-  background: hsla(0, 0%, 100%, 0.8);
+
+.button {
+    .stButton;
+    transition-duration: 0.4s;
+    width: 100px;
+    background-color: grey;
+    border-radius: 8px;
+}
+
+.button:hover {
+    background-color: white;
+    color: black;
 }
```

### Comparing `streamlit-picture-carousel-0.1.0/src/st_picture_carousel/frontend/carousel/carousel.html` & `streamlit-picture-carousel-0.1.2/src/st_picture_carousel/frontend/carousel/carousel.html`

 * *Files 24% similar despite different names*

```diff
@@ -18,13 +18,16 @@
         <div class="carousel__cell">7</div>
         <div class="carousel__cell">8</div>
         <div class="carousel__cell">9</div>
         -->
       </div>
     </div>
     <p style="text-align: center;">
-      <button class="previous-button button">Previous</button>
-      <button class="next-button button">Next</button>
+      <button class="previous-button button stButton">Previous</button>
+      <button class="next-button button stButton">Next</button>
     </p>
+    <!--
+    <p id="test_para" style="color:green">Test</p>
     <script src="carousel.js"></script>
+    -->
   </body>
 </html>
```

### Comparing `streamlit-picture-carousel-0.1.0/src/st_picture_carousel/frontend/index.html` & `streamlit-picture-carousel-0.1.2/src/st_picture_carousel/frontend/index.html`

 * *Files 12% similar despite different names*

```diff
@@ -8,19 +8,14 @@
     <script src="./streamlit-component-lib.js"></script>
     <script src="./main.js"></script>
     <link rel="stylesheet" href="./style.css" />
   </head>
   <body>
     <div id="root">
       <!--
-      <label id="label" for="text_input">This is a label</label>
-      <div class="input">
-        <input type="text" name="text_input" id="input_box" />
-      </div>
-      <p style="color:orange">Testing 1,2,3...</p>
       <p id="number_para" style="color:green">Test</p>
       -->
       <iframe id="carousel_iframe" style="color:blue; border:0"
               src="./carousel/carousel.html?n_pics=7"
               title="In an iFrame"
               width="100%"
               height="400px">
```

### Comparing `streamlit-picture-carousel-0.1.0/src/st_picture_carousel/frontend/main.js` & `streamlit-picture-carousel-0.1.2/src/st_picture_carousel/frontend/main.js`

 * *Files 24% similar despite different names*

#### js-beautify {}

```diff
@@ -16,22 +16,30 @@
     // Only run the render code the first time the component is loaded.
     if (!window.rendered) {
         // You most likely want to get the data passed in like this
         // const {input1, input2, input3} = event.detail.args
 
         // Grab the label and default value that the user specified
         const {
-            n_pics
+            n_pics,
+            cell,
+            img_path,
+            img_list,
+            img_size
         } = event.detail.args;
 
-        // const para = document.getElementById("number_para")
-        // para.innerHTML = n_pics
+        //const numpara = document.getElementById("number_para")
+        //numpara.innerHTML = location.href
 
         const caiframe = document.getElementById("carousel_iframe")
-        caiframe.src = "./carousel/carousel.html?n_pics=" + n_pics
+        caiframe.src = ("./carousel/carousel.html?n_pics=" + n_pics +
+            "&cell=" + cell +
+            "&img_path=" + img_path +
+            "&img_list=" + img_list +
+            "&img_size=" + img_size)
 
         // You'll most likely want to pass some data back to Python like this
         // sendValue({output1: "foo", output2: "bar"})
         window.rendered = true
     }
 }
```

### Comparing `streamlit-picture-carousel-0.1.0/src/st_picture_carousel/frontend/streamlit-component-lib.js` & `streamlit-picture-carousel-0.1.2/src/st_picture_carousel/frontend/streamlit-component-lib.js`

 * *Files identical despite different names*

### Comparing `streamlit-picture-carousel-0.1.0/src/streamlit_picture_carousel.egg-info/PKG-INFO` & `streamlit-picture-carousel-0.1.2/src/streamlit_picture_carousel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-picture-carousel
-Version: 0.1.0
+Version: 0.1.2
 Summary: Displays 3d carousel of pictures
 Author: Rafal Cegiela
 Author-email: rcegiela@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `streamlit-picture-carousel-0.1.0/src/streamlit_picture_carousel.egg-info/SOURCES.txt` & `streamlit-picture-carousel-0.1.2/src/streamlit_picture_carousel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

