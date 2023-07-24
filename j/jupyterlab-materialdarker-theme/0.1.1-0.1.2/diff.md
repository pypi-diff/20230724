# Comparing `tmp/jupyterlab_materialdarker_theme-0.1.1.tar.gz` & `tmp/jupyterlab_materialdarker_theme-0.1.2.tar.gz`

## Comparing `jupyterlab_materialdarker_theme-0.1.1.tar` & `jupyterlab_materialdarker_theme-0.1.2.tar`

### file list

```diff
@@ -1,32 +1,29 @@
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.1/.copier-answers.yml
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.1/.prettierignore
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.1/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.1/CHANGELOG.md
--rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.1/RELEASE.md
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.1/install.json
--rw-r--r--   0        0        0     6171 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.1/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.1/setup.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.1/tsconfig.json
--rw-r--r--   0        0        0   194552 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.1/yarn.lock
--rw-r--r--   0        0        0   289182 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.1/images/jupyterlab_materialdarker_1.png
--rw-r--r--   0        0        0   233733 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.1/images/jupyterlab_materialdarker_2.png
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.1/jupyterlab_materialdarker_theme/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.1/jupyterlab_materialdarker_theme/_version.py
--rw-r--r--   0        0        0    21984 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.1/jupyterlab_materialdarker_theme/labextension/build_log.json
--rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.1/jupyterlab_materialdarker_theme/labextension/package.json
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.1/jupyterlab_materialdarker_theme/labextension/static/lib_index_js.e3aae18ec788fc34efc4.js
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.1/jupyterlab_materialdarker_theme/labextension/static/lib_index_js.e3aae18ec788fc34efc4.js.map
--rw-r--r--   0        0        0    27189 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.1/jupyterlab_materialdarker_theme/labextension/static/remoteEntry.cf00ebd6a5cdf8aa52da.js
--rw-r--r--   0        0        0    26129 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.1/jupyterlab_materialdarker_theme/labextension/static/remoteEntry.cf00ebd6a5cdf8aa52da.js.map
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.1/jupyterlab_materialdarker_theme/labextension/static/style.js
--rw-r--r--   0        0        0    15198 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.1/jupyterlab_materialdarker_theme/labextension/themes/jupyterlab_materialdarker_theme/index.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.1/jupyterlab_materialdarker_theme/labextension/themes/jupyterlab_materialdarker_theme/index.js
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.1/src/index.ts
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.1/src/index.ts.bckp
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.1/style/index.css
--rw-r--r--   0        0        0    14722 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.1/style/variables.css
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.1/.gitignore
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.1/LICENSE
--rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.1/README.md
--rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5838 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.2/.copier-answers.yml
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.2/.prettierignore
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.2/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.2/CHANGELOG.md
+-rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.2/RELEASE.md
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.2/install.json
+-rw-r--r--   0        0        0     6171 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.2/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.2/setup.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.2/tsconfig.json
+-rw-r--r--   0        0        0   194552 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.2/yarn.lock
+-rw-r--r--   0        0        0   289182 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.2/images/jupyterlab_materialdarker_1.png
+-rw-r--r--   0        0        0   233733 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.2/images/jupyterlab_materialdarker_2.png
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.2/jupyterlab_materialdarker_theme/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.2/jupyterlab_materialdarker_theme/_version.py
+-rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.2/jupyterlab_materialdarker_theme/labextension/package.json
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.2/jupyterlab_materialdarker_theme/labextension/static/568.b887e22d4f97175b6aa3.js
+-rw-r--r--   0        0        0     6327 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.2/jupyterlab_materialdarker_theme/labextension/static/remoteEntry.ab024d1ef289c264df8c.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.2/jupyterlab_materialdarker_theme/labextension/static/style.js
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.2/jupyterlab_materialdarker_theme/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0    15198 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.2/jupyterlab_materialdarker_theme/labextension/themes/jupyterlab_materialdarker_theme/index.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.2/jupyterlab_materialdarker_theme/labextension/themes/jupyterlab_materialdarker_theme/index.js
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.2/src/index.ts
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.2/style/index.css
+-rw-r--r--   0        0        0    14722 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.2/style/variables.css
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.2/README.md
+-rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5838 2020-02-02 00:00:00.000000 jupyterlab_materialdarker_theme-0.1.2/PKG-INFO
```

### Comparing `jupyterlab_materialdarker_theme-0.1.1/.copier-answers.yml` & `jupyterlab_materialdarker_theme-0.1.2/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `jupyterlab_materialdarker_theme-0.1.1/RELEASE.md` & `jupyterlab_materialdarker_theme-0.1.2/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_materialdarker_theme-0.1.1/package.json` & `jupyterlab_materialdarker_theme-0.1.2/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9772727272727273%*

 * *Differences: {"'version'": "'0.1.2'"}*

```diff
@@ -172,9 +172,9 @@
             "color-function-notation": null,
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.1"
+    "version": "0.1.2"
 }
```

### Comparing `jupyterlab_materialdarker_theme-0.1.1/tsconfig.json` & `jupyterlab_materialdarker_theme-0.1.2/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_materialdarker_theme-0.1.1/yarn.lock` & `jupyterlab_materialdarker_theme-0.1.2/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_materialdarker_theme-0.1.1/images/jupyterlab_materialdarker_1.png` & `jupyterlab_materialdarker_theme-0.1.2/images/jupyterlab_materialdarker_1.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_materialdarker_theme-0.1.1/images/jupyterlab_materialdarker_2.png` & `jupyterlab_materialdarker_theme-0.1.2/images/jupyterlab_materialdarker_2.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_materialdarker_theme-0.1.1/jupyterlab_materialdarker_theme/__init__.py` & `jupyterlab_materialdarker_theme-0.1.2/jupyterlab_materialdarker_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_materialdarker_theme-0.1.1/jupyterlab_materialdarker_theme/labextension/package.json` & `jupyterlab_materialdarker_theme-0.1.2/jupyterlab_materialdarker_theme/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9765625%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.ab024d1ef289c264df8c.js'}}",*

 * * "'version'": "'0.1.2'"}*

```diff
@@ -97,15 +97,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/eduardotlc/jupyterlab_materialdarker_theme",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.cf00ebd6a5cdf8aa52da.js"
+            "load": "static/remoteEntry.ab024d1ef289c264df8c.js"
         },
         "extension": true,
         "outputDir": "jupyterlab_materialdarker_theme/labextension",
         "themePath": "style/index.css"
     },
     "keywords": [
         "jupyter",
@@ -176,9 +176,9 @@
             "color-function-notation": null,
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.1"
+    "version": "0.1.2"
 }
```

### Comparing `jupyterlab_materialdarker_theme-0.1.1/jupyterlab_materialdarker_theme/labextension/themes/jupyterlab_materialdarker_theme/index.css` & `jupyterlab_materialdarker_theme-0.1.2/jupyterlab_materialdarker_theme/labextension/themes/jupyterlab_materialdarker_theme/index.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_materialdarker_theme-0.1.1/src/index.ts` & `jupyterlab_materialdarker_theme-0.1.2/src/index.ts`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
   activate: (app: JupyterFrontEnd, manager: IThemeManager) => {
     console.log(
       'JupyterLab extension jupyterlab_materialdarker_theme is activated!'
     );
     const style = 'jupyterlab_materialdarker_theme/index.css';
 
     manager.register({
-      name: 'jupyterlab_materialdarker_theme',
+      name: 'Material Darker',
       isLight: false,
       load: () => manager.loadCSS(style),
       unload: () => Promise.resolve(undefined)
     });
   }
 };
```

### Comparing `jupyterlab_materialdarker_theme-0.1.1/style/variables.css` & `jupyterlab_materialdarker_theme-0.1.2/style/variables.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_materialdarker_theme-0.1.1/.gitignore` & `jupyterlab_materialdarker_theme-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_materialdarker_theme-0.1.1/LICENSE` & `jupyterlab_materialdarker_theme-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_materialdarker_theme-0.1.1/README.md` & `jupyterlab_materialdarker_theme-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_materialdarker_theme-0.1.1/pyproject.toml` & `jupyterlab_materialdarker_theme-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_materialdarker_theme-0.1.1/PKG-INFO` & `jupyterlab_materialdarker_theme-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_materialdarker_theme
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Material derker JupyterLab theme extension.
 Project-URL: Homepage, https://github.com/eduardotlc/jupyterlab_materialdarker_theme
 Project-URL: Bug Tracker, https://github.com/eduardotlc/jupyterlab_materialdarker_theme/issues
 Project-URL: Repository, https://github.com/eduardotlc/jupyterlab_materialdarker_theme.git
 Author-email: Eduardo Campos <eduardotcampos@usp.br>
 License: BSD 3-Clause License
```

