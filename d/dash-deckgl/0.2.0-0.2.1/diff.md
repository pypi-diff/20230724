# Comparing `tmp/dash_deckgl-0.2.0.tar.gz` & `tmp/dash_deckgl-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_deckgl-0.2.0.tar", last modified: Thu Jun 15 03:52:04 2023, max compression
+gzip compressed data, was "dash_deckgl-0.2.1.tar", last modified: Mon Jul 24 03:53:47 2023, max compression
```

## Comparing `dash_deckgl-0.2.0.tar` & `dash_deckgl-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-15 03:52:04.524285 dash_deckgl-0.2.0/
--rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-05-23 00:50:44.000000 dash_deckgl-0.2.0/LICENSE
--rw-rw-r--   0 dave      (1000) dave      (1000)      226 2023-05-25 20:46:42.000000 dash_deckgl-0.2.0/MANIFEST.in
--rw-rw-r--   0 dave      (1000) dave      (1000)      589 2023-06-15 03:52:04.524285 dash_deckgl-0.2.0/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)     3899 2023-05-25 19:30:16.000000 dash_deckgl-0.2.0/README.md
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-15 03:52:04.520285 dash_deckgl-0.2.0/dash_deckgl/
--rw-rw-r--   0 dave      (1000) dave      (1000)     2981 2023-06-15 03:43:04.000000 dash_deckgl-0.2.0/dash_deckgl/DashDeckgl.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2513 2023-05-25 20:45:04.000000 dash_deckgl-0.2.0/dash_deckgl/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)       66 2023-06-15 03:43:04.000000 dash_deckgl-0.2.0/dash_deckgl/_imports_.py
--rw-rw-r--   0 dave      (1000) dave      (1000)  1202621 2023-06-15 03:43:02.000000 dash_deckgl-0.2.0/dash_deckgl/dash_deckgl.min.js
--rw-rw-r--   0 dave      (1000) dave      (1000)    16774 2023-06-15 03:43:02.000000 dash_deckgl-0.2.0/dash_deckgl/deckgl.js
--rw-rw-r--   0 dave      (1000) dave      (1000)     2917 2023-06-15 03:43:04.000000 dash_deckgl-0.2.0/dash_deckgl/metadata.json
--rw-rw-r--   0 dave      (1000) dave      (1000)     2806 2023-06-15 03:43:03.000000 dash_deckgl-0.2.0/dash_deckgl/package-info.json
--rw-rw-r--   0 dave      (1000) dave      (1000)   800972 2023-05-25 20:45:12.000000 dash_deckgl-0.2.0/dash_deckgl/vendor.js
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-15 03:52:04.524285 dash_deckgl-0.2.0/dash_deckgl.egg-info/
--rw-rw-r--   0 dave      (1000) dave      (1000)      589 2023-06-15 03:52:04.000000 dash_deckgl-0.2.0/dash_deckgl.egg-info/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)      417 2023-06-15 03:52:04.000000 dash_deckgl-0.2.0/dash_deckgl.egg-info/SOURCES.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-06-15 03:52:04.000000 dash_deckgl-0.2.0/dash_deckgl.egg-info/dependency_links.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       12 2023-06-15 03:52:04.000000 dash_deckgl-0.2.0/dash_deckgl.egg-info/top_level.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)     2806 2023-06-15 03:51:39.000000 dash_deckgl-0.2.0/package.json
--rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-06-15 03:52:04.524285 dash_deckgl-0.2.0/setup.cfg
--rw-rw-r--   0 dave      (1000) dave      (1000)      653 2023-05-25 20:56:07.000000 dash_deckgl-0.2.0/setup.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-15 03:52:04.524285 dash_deckgl-0.2.0/tests/
--rw-rw-r--   0 dave      (1000) dave      (1000)      329 2023-05-25 21:17:05.000000 dash_deckgl-0.2.0/tests/test_usage.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-24 03:53:47.796070 dash_deckgl-0.2.1/
+-rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-05-23 00:50:44.000000 dash_deckgl-0.2.1/LICENSE
+-rw-rw-r--   0 dave      (1000) dave      (1000)      226 2023-05-25 20:46:42.000000 dash_deckgl-0.2.1/MANIFEST.in
+-rw-rw-r--   0 dave      (1000) dave      (1000)      589 2023-07-24 03:53:47.796070 dash_deckgl-0.2.1/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3899 2023-05-25 19:30:16.000000 dash_deckgl-0.2.1/README.md
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-24 03:53:47.792070 dash_deckgl-0.2.1/dash_deckgl/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2981 2023-07-24 03:38:41.000000 dash_deckgl-0.2.1/dash_deckgl/DashDeckgl.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2513 2023-05-25 20:45:04.000000 dash_deckgl-0.2.1/dash_deckgl/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)       66 2023-07-24 03:38:41.000000 dash_deckgl-0.2.1/dash_deckgl/_imports_.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)  1202621 2023-07-24 03:44:21.000000 dash_deckgl-0.2.1/dash_deckgl/dash_deckgl.min.js
+-rw-rw-r--   0 dave      (1000) dave      (1000)    16785 2023-07-24 03:44:21.000000 dash_deckgl-0.2.1/dash_deckgl/deckgl.js
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2917 2023-07-24 03:38:41.000000 dash_deckgl-0.2.1/dash_deckgl/metadata.json
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2806 2023-07-24 03:38:40.000000 dash_deckgl-0.2.1/dash_deckgl/package-info.json
+-rw-rw-r--   0 dave      (1000) dave      (1000)   800972 2023-05-25 20:45:12.000000 dash_deckgl-0.2.1/dash_deckgl/vendor.js
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-24 03:53:47.796070 dash_deckgl-0.2.1/dash_deckgl.egg-info/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      589 2023-07-24 03:53:47.000000 dash_deckgl-0.2.1/dash_deckgl.egg-info/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)      417 2023-07-24 03:53:47.000000 dash_deckgl-0.2.1/dash_deckgl.egg-info/SOURCES.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-07-24 03:53:47.000000 dash_deckgl-0.2.1/dash_deckgl.egg-info/dependency_links.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       12 2023-07-24 03:53:47.000000 dash_deckgl-0.2.1/dash_deckgl.egg-info/top_level.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2806 2023-07-24 03:34:20.000000 dash_deckgl-0.2.1/package.json
+-rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-07-24 03:53:47.796070 dash_deckgl-0.2.1/setup.cfg
+-rw-rw-r--   0 dave      (1000) dave      (1000)      653 2023-05-25 20:56:07.000000 dash_deckgl-0.2.1/setup.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-24 03:53:47.796070 dash_deckgl-0.2.1/tests/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      329 2023-05-25 21:17:05.000000 dash_deckgl-0.2.1/tests/test_usage.py
```

### Comparing `dash_deckgl-0.2.0/PKG-INFO` & `dash_deckgl-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: dash_deckgl
-Version: 0.2.0
+Version: 0.2.1
 Summary: Deck.gl component for Dash
 Author: Oceanum developers <developers@oceanum.science>
 License: MIT
 Classifier: Framework :: Dash
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Package: dashDeckgl
 Title: Deck.gl component for Dash
-Version: 0.1.3
+Version: 0.2.1
 Description: Deck.gl component for Dash
 Depends: R (>= 3.0.2)
 Imports: 
 Suggests: 
 License: MIT + file LICENSE
 URL: https://github.com/oceanum-io/dash-deckgl
 BugReports: https://github.com/oceanum-io/dash-deckgl/issues
```

### Comparing `dash_deckgl-0.2.0/README.md` & `dash_deckgl-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `dash_deckgl-0.2.0/dash_deckgl/DashDeckgl.py` & `dash_deckgl-0.2.1/dash_deckgl/DashDeckgl.py`

 * *Files identical despite different names*

### Comparing `dash_deckgl-0.2.0/dash_deckgl/__init__.py` & `dash_deckgl-0.2.1/dash_deckgl/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_deckgl-0.2.0/dash_deckgl/dash_deckgl.min.js` & `dash_deckgl-0.2.1/dash_deckgl/dash_deckgl.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -50007,15 +50007,15 @@
         var l = jsonpScriptSrc;
         jsonpScriptSrc = function(t) {
             var e, n = (e = A(), /\/_dash-component-suites\//.test(e.src)),
                 i = l(t);
             if (!n) return i;
             var r = i.split("/"),
                 s = r.slice(-1)[0].split(".");
-            return s.splice(1, 0, "v0_1_3m1686800560"), r.splice(-1, 1, s.join(".")), r.join("/")
+            return s.splice(1, 0, "v0_2_1m1690170242"), r.splice(-1, 1, s.join(".")), r.join("/")
         }
     }(() => {
         var t = {
             179: 0
         };
         o.f.j = (e, n) => {
             var i = o.o(t, e) ? t[e] : void 0;
```

### Comparing `dash_deckgl-0.2.0/dash_deckgl/deckgl.js` & `dash_deckgl-0.2.1/dash_deckgl/deckgl.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -688,15 +688,15 @@
                 (0, o.useEffect)((function() {
                     ! function() {
                         var e, r;
                         e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : "https://api.tiles.mapbox.com/mapbox-gl-js/v1.13.2/mapbox-gl.css", (r = document.createElement("link")).type = "text/css", r.rel = "stylesheet", r.href = e, document.getElementsByTagName("head")[0].appendChild(r)
                     }()
                 }), []), (0, o.useEffect)((function() {
                     var e = C.convert(r);
-                    !x && e.initialViewState && k(e.initialViewState), S(D(D({}, L), e))
+                    console.log(e), e.initialViewState && k(e.initialViewState), S(D(D({}, L), e))
                 }), [r, C]), (0, o.useEffect)((function() {
                     var e = C.convert(g);
                     T(D(D({}, O), e))
                 }), [g, C]);
                 var W = (0, o.useCallback)((function(e) {
                     var r = e.viewState;
                     k(r)
```

### Comparing `dash_deckgl-0.2.0/dash_deckgl/metadata.json` & `dash_deckgl-0.2.1/dash_deckgl/metadata.json`

 * *Files identical despite different names*

### Comparing `dash_deckgl-0.2.0/dash_deckgl/package-info.json` & `dash_deckgl-0.2.1/dash_deckgl/package-info.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.2.1'"}*

```diff
@@ -66,9 +66,9 @@
         "build:backends": "dash-generate-components ./src/lib/components dash_deckgl -p package-info.json --r-prefix '' --jl-prefix '' --ignore \\.test\\.",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.1.3"
+    "version": "0.2.1"
 }
```

### Comparing `dash_deckgl-0.2.0/dash_deckgl/vendor.js` & `dash_deckgl-0.2.1/dash_deckgl/vendor.js`

 * *Files identical despite different names*

### Comparing `dash_deckgl-0.2.0/dash_deckgl.egg-info/PKG-INFO` & `dash_deckgl-0.2.1/dash_deckgl.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: dash-deckgl
-Version: 0.2.0
+Version: 0.2.1
 Summary: Deck.gl component for Dash
 Author: Oceanum developers <developers@oceanum.science>
 License: MIT
 Classifier: Framework :: Dash
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Package: dashDeckgl
 Title: Deck.gl component for Dash
-Version: 0.1.3
+Version: 0.2.1
 Description: Deck.gl component for Dash
 Depends: R (>= 3.0.2)
 Imports: 
 Suggests: 
 License: MIT + file LICENSE
 URL: https://github.com/oceanum-io/dash-deckgl
 BugReports: https://github.com/oceanum-io/dash-deckgl/issues
```

### Comparing `dash_deckgl-0.2.0/package.json` & `dash_deckgl-0.2.1/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.2.1'"}*

```diff
@@ -66,9 +66,9 @@
         "build:backends": "dash-generate-components ./src/lib/components dash_deckgl -p package-info.json --r-prefix '' --jl-prefix '' --ignore \\.test\\.",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.2.0"
+    "version": "0.2.1"
 }
```

### Comparing `dash_deckgl-0.2.0/setup.py` & `dash_deckgl-0.2.1/setup.py`

 * *Files identical despite different names*

