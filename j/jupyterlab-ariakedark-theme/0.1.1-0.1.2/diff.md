# Comparing `tmp/jupyterlab_ariakedark_theme-0.1.1.tar.gz` & `tmp/jupyterlab_ariakedark_theme-0.1.2.tar.gz`

## Comparing `jupyterlab_ariakedark_theme-0.1.1.tar` & `jupyterlab_ariakedark_theme-0.1.2.tar`

### file list

```diff
@@ -1,29 +1,33 @@
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/.copier-answers.yml
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/.prettierignore
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/CHANGELOG.md
--rw-r--r--   0        0        0     3936 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/RELEASE.md
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/install.json
--rw-r--r--   0        0        0     6154 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/setup.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/tsconfig.json
--rw-r--r--   0        0        0   194544 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/yarn.lock
--rw-r--r--   0        0        0   193370 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/images/jupyterlab_ariakedark_1.png
--rw-r--r--   0        0        0   362052 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/images/jupyterlab_ariakedark_2.png
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/jupyterlab_ariakedark_theme/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/jupyterlab_ariakedark_theme/_version.py
--rw-r--r--   0        0        0     5434 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/jupyterlab_ariakedark_theme/labextension/package.json
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/jupyterlab_ariakedark_theme/labextension/static/568.a4c8391e2673163e5dd0.js
--rw-r--r--   0        0        0     6304 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/jupyterlab_ariakedark_theme/labextension/static/remoteEntry.42430a68b18808d3cc76.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/jupyterlab_ariakedark_theme/labextension/static/style.js
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/jupyterlab_ariakedark_theme/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0    13835 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/jupyterlab_ariakedark_theme/labextension/themes/jupyterlab_ariakedark_theme/index.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/jupyterlab_ariakedark_theme/labextension/themes/jupyterlab_ariakedark_theme/index.js
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/src/index.ts
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/style/index.css
--rw-r--r--   0        0        0    13623 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/style/variables.css
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/.gitignore
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/LICENSE
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/README.md
--rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5815 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/.copier-answers.yml
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/.prettierignore
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/CHANGELOG.md
+-rw-r--r--   0        0        0     3936 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/RELEASE.md
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/TODO.md
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/install.json
+-rw-r--r--   0        0        0     6154 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/setup.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/tsconfig.json
+-rw-r--r--   0        0        0   194544 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/yarn.lock
+-rw-r--r--   0        0        0    20317 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/images/badge_pypi.svg
+-rw-r--r--   0        0        0   193370 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/images/jupyterlab_ariakedark_1.png
+-rw-r--r--   0        0        0   362052 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/images/jupyterlab_ariakedark_2.png
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/jupyterlab_ariakedark_theme/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/jupyterlab_ariakedark_theme/_version.py
+-rw-r--r--   0        0        0    21924 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/jupyterlab_ariakedark_theme/labextension/build_log.json
+-rw-r--r--   0        0        0     5434 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/jupyterlab_ariakedark_theme/labextension/package.json
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/jupyterlab_ariakedark_theme/labextension/static/lib_index_js.ec0f4e74d248cc0e4f58.js
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/jupyterlab_ariakedark_theme/labextension/static/lib_index_js.ec0f4e74d248cc0e4f58.js.map
+-rw-r--r--   0        0        0    27153 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/jupyterlab_ariakedark_theme/labextension/static/remoteEntry.84696dca1279b4b085e4.js
+-rw-r--r--   0        0        0    26033 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/jupyterlab_ariakedark_theme/labextension/static/remoteEntry.84696dca1279b4b085e4.js.map
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/jupyterlab_ariakedark_theme/labextension/static/style.js
+-rw-r--r--   0        0        0    13835 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/jupyterlab_ariakedark_theme/labextension/themes/jupyterlab_ariakedark_theme/index.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/jupyterlab_ariakedark_theme/labextension/themes/jupyterlab_ariakedark_theme/index.js
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/src/index.ts
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/style/index.css
+-rw-r--r--   0        0        0    13623 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/style/variables.css
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/README.md
+-rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/PKG-INFO
```

### Comparing `jupyterlab_ariakedark_theme-0.1.1/RELEASE.md` & `jupyterlab_ariakedark_theme-0.1.2/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_ariakedark_theme-0.1.1/package.json` & `jupyterlab_ariakedark_theme-0.1.2/package.json`

 * *Files 1% similar despite different names*

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

### Comparing `jupyterlab_ariakedark_theme-0.1.1/tsconfig.json` & `jupyterlab_ariakedark_theme-0.1.2/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_ariakedark_theme-0.1.1/yarn.lock` & `jupyterlab_ariakedark_theme-0.1.2/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_ariakedark_theme-0.1.1/images/jupyterlab_ariakedark_1.png` & `jupyterlab_ariakedark_theme-0.1.2/images/jupyterlab_ariakedark_1.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ariakedark_theme-0.1.1/images/jupyterlab_ariakedark_2.png` & `jupyterlab_ariakedark_theme-0.1.2/images/jupyterlab_ariakedark_2.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ariakedark_theme-0.1.1/jupyterlab_ariakedark_theme/__init__.py` & `jupyterlab_ariakedark_theme-0.1.2/jupyterlab_ariakedark_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_ariakedark_theme-0.1.1/jupyterlab_ariakedark_theme/labextension/package.json` & `jupyterlab_ariakedark_theme-0.1.2/jupyterlab_ariakedark_theme/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992897727272727%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.84696dca1279b4b085e4.js'}}"}*

```diff
@@ -97,15 +97,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/eduardotlc/jupyterlab_ariakedark_theme",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.42430a68b18808d3cc76.js"
+            "load": "static/remoteEntry.84696dca1279b4b085e4.js"
         },
         "extension": true,
         "outputDir": "jupyterlab_ariakedark_theme/labextension",
         "themePath": "style/index.css"
     },
     "keywords": [
         "jupyter",
```

### Comparing `jupyterlab_ariakedark_theme-0.1.1/jupyterlab_ariakedark_theme/labextension/themes/jupyterlab_ariakedark_theme/index.css` & `jupyterlab_ariakedark_theme-0.1.2/jupyterlab_ariakedark_theme/labextension/themes/jupyterlab_ariakedark_theme/index.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_ariakedark_theme-0.1.1/src/index.ts` & `jupyterlab_ariakedark_theme-0.1.2/src/index.ts`

 * *Files 13% similar despite different names*

```diff
@@ -16,15 +16,15 @@
   activate: (app: JupyterFrontEnd, manager: IThemeManager) => {
     console.log(
       'JupyterLab extension jupyterlab_ariakedark_theme is activated!'
     );
     const style = 'jupyterlab_ariakedark_theme/index.css';
 
     manager.register({
-      name: 'jupyterlab_ariakedark_theme',
+      name: 'Ariake Dark',
       isLight: false,
       load: () => manager.loadCSS(style),
       unload: () => Promise.resolve(undefined)
     });
   }
 };
```

### Comparing `jupyterlab_ariakedark_theme-0.1.1/style/variables.css` & `jupyterlab_ariakedark_theme-0.1.2/style/variables.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_ariakedark_theme-0.1.1/.gitignore` & `jupyterlab_ariakedark_theme-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_ariakedark_theme-0.1.1/LICENSE` & `jupyterlab_ariakedark_theme-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_ariakedark_theme-0.1.1/README.md` & `jupyterlab_ariakedark_theme-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-# jupyterlab_ariakedark_theme
+# Jupyterlab Ariake Dark Theme
+
+---
 
 **An ariake dark palette based JupyterLab theme extension.**
 
 |       build       |         PyPi          |
 | :---------------: | :-------------------: |
 | [![ci-badge]][ci] | [![pypi-badge]][pypi] |
 
 [ci-badge]: https://github.com/eduardotlc/jupyterlab_ariakedark_theme/workflows/Build/badge.svg
 [ci]: https://github.com/eduardotlc/jupyterlab_ariakedark_theme/actions/workflows/build.yml
-[pypi-badge]: https://badge.fury.io/py/jupyterlab-ariakedark-theme.svg
+[pypi-badge]: ./images/badge_pypi.svg
 [pypi]: https://badge.fury.io/py/jupyterlab-ariakedark-theme
 
-eduardotcampos@usp.br [2023]
+<eduardotcampos@usp.br> **[2023]**
 
 ## Appearance
 
 ![Example 1](./images/jupyterlab_ariakedark_1.png)
 
 ![Example 2](./images/jupyterlab_ariakedark_2.png)
 
@@ -27,49 +29,83 @@
 
 To install the extension, execute:
 
 ```bash
 pip install jupyterlab_ariakedark_theme
 ```
 
+To check the installation, execute:
+
+```bash
+jupyter labextension list
+```
+
 ## Uninstall
 
 To remove the extension, execute:
 
 ```bash
 pip uninstall jupyterlab_ariakedark_theme
 ```
 
 ## Contributing
 
+To make personal customizations to the theme, edit the [variables.css](./style/variables.css) file, and then run the development install steps listed bellow.
+
+Feel free to make [pending](./TODO.md) or other optimizations and pull requests, this theme is still under development and any contribution is very much appreciated.
+
 ### Development install
 
 Note: You will need NodeJS to build the extension package.
 
 The `jlpm` command is JupyterLab's pinned version of
 [yarn](https://yarnpkg.com/) that is installed with JupyterLab. You may use
 `yarn` or `npm` in lieu of `jlpm` below.
 
+- Clone the repo to your local environment:
+
+```bash
+git clone https://github.com/eduardotlc/jupyterlab_ariakedark_theme
+```
+
+- Change directory to the jupyterlab_ariakedark_theme directory:
+
+```bash
+cd jupyterlab_ariakedark_theme
+```
+
+- Install package in development mode:
+
+```bash
+pip install -ve "."
+```
+
+- Link your development version of the extension with JupyterLab:
+
 ```bash
-# Clone the repo to your local environment
-# Change directory to the jupyterlab_ariakedark_theme directory
-# Install package in development mode
-pip install -e "."
-# Link your development version of the extension with JupyterLab
 jupyter labextension develop . --overwrite
-# Rebuild extension Typescript source after making changes
+```
+
+- Rebuild extension Typescript source after making changes:
+
+```bash
 jlpm build
 ```
 
 You can watch the source directory and run JupyterLab at the same time in different terminals to watch for changes in the extension's source and automatically rebuild the extension.
 
+- Watch the source directory in one terminal, automatically rebuilding when needed:
+
 ```bash
-# Watch the source directory in one terminal, automatically rebuilding when needed
 jlpm watch
-# Run JupyterLab in another terminal
+```
+
+- Run JupyterLab in another terminal:
+
+```bash
 jupyter lab
 ```
 
 With the watch command running, every saved change will immediately be built locally and available in your running JupyterLab. Refresh JupyterLab to load the change in your browser (you may need to wait several seconds for the extension to be rebuilt).
 
 By default, the `jlpm build` command generates the source maps for this extension to make it easier to debug using the browser dev tools. To also generate source maps for the JupyterLab core extensions, you can run the following command:
 
@@ -82,11 +118,7 @@
 ```bash
 pip uninstall jupyterlab_ariakedark_theme
 ```
 
 In development mode, you will also need to remove the symlink created by `jupyter labextension develop`
 command. To find its location, you can run `jupyter labextension list` to figure out where the `labextensions`
 folder is located. Then you can remove the symlink named `jupyterlab_ariakedark_theme` within that folder.
-
-### Packaging the extension
-
-See [RELEASE](RELEASE.md)
```

### Comparing `jupyterlab_ariakedark_theme-0.1.1/pyproject.toml` & `jupyterlab_ariakedark_theme-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_ariakedark_theme-0.1.1/PKG-INFO` & `jupyterlab_ariakedark_theme-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_ariakedark_theme
-Version: 0.1.1
+Version: 0.1.2
 Summary: An ariake dark palette based JupyterLab theme extension.
 Project-URL: Homepage, https://github.com/eduardotlc/jupyterlab_ariakedark_theme
 Project-URL: Bug Tracker, https://github.com/eduardotlc/jupyterlab_ariakedark_theme/issues
 Project-URL: Repository, https://github.com/eduardotlc/jupyterlab_ariakedark_theme.git
 Author-email: Eduardo Campos <eduardotcampos@usp.br>
 License: BSD 3-Clause License
         
@@ -47,28 +47,30 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
-# jupyterlab_ariakedark_theme
+# Jupyterlab Ariake Dark Theme
+
+---
 
 **An ariake dark palette based JupyterLab theme extension.**
 
 |       build       |         PyPi          |
 | :---------------: | :-------------------: |
 | [![ci-badge]][ci] | [![pypi-badge]][pypi] |
 
 [ci-badge]: https://github.com/eduardotlc/jupyterlab_ariakedark_theme/workflows/Build/badge.svg
 [ci]: https://github.com/eduardotlc/jupyterlab_ariakedark_theme/actions/workflows/build.yml
-[pypi-badge]: https://badge.fury.io/py/jupyterlab-ariakedark-theme.svg
+[pypi-badge]: ./images/badge_pypi.svg
 [pypi]: https://badge.fury.io/py/jupyterlab-ariakedark-theme
 
-eduardotcampos@usp.br [2023]
+<eduardotcampos@usp.br> **[2023]**
 
 ## Appearance
 
 ![Example 1](./images/jupyterlab_ariakedark_1.png)
 
 ![Example 2](./images/jupyterlab_ariakedark_2.png)
 
@@ -80,49 +82,83 @@
 
 To install the extension, execute:
 
 ```bash
 pip install jupyterlab_ariakedark_theme
 ```
 
+To check the installation, execute:
+
+```bash
+jupyter labextension list
+```
+
 ## Uninstall
 
 To remove the extension, execute:
 
 ```bash
 pip uninstall jupyterlab_ariakedark_theme
 ```
 
 ## Contributing
 
+To make personal customizations to the theme, edit the [variables.css](./style/variables.css) file, and then run the development install steps listed bellow.
+
+Feel free to make [pending](./TODO.md) or other optimizations and pull requests, this theme is still under development and any contribution is very much appreciated.
+
 ### Development install
 
 Note: You will need NodeJS to build the extension package.
 
 The `jlpm` command is JupyterLab's pinned version of
 [yarn](https://yarnpkg.com/) that is installed with JupyterLab. You may use
 `yarn` or `npm` in lieu of `jlpm` below.
 
+- Clone the repo to your local environment:
+
+```bash
+git clone https://github.com/eduardotlc/jupyterlab_ariakedark_theme
+```
+
+- Change directory to the jupyterlab_ariakedark_theme directory:
+
+```bash
+cd jupyterlab_ariakedark_theme
+```
+
+- Install package in development mode:
+
+```bash
+pip install -ve "."
+```
+
+- Link your development version of the extension with JupyterLab:
+
 ```bash
-# Clone the repo to your local environment
-# Change directory to the jupyterlab_ariakedark_theme directory
-# Install package in development mode
-pip install -e "."
-# Link your development version of the extension with JupyterLab
 jupyter labextension develop . --overwrite
-# Rebuild extension Typescript source after making changes
+```
+
+- Rebuild extension Typescript source after making changes:
+
+```bash
 jlpm build
 ```
 
 You can watch the source directory and run JupyterLab at the same time in different terminals to watch for changes in the extension's source and automatically rebuild the extension.
 
+- Watch the source directory in one terminal, automatically rebuilding when needed:
+
 ```bash
-# Watch the source directory in one terminal, automatically rebuilding when needed
 jlpm watch
-# Run JupyterLab in another terminal
+```
+
+- Run JupyterLab in another terminal:
+
+```bash
 jupyter lab
 ```
 
 With the watch command running, every saved change will immediately be built locally and available in your running JupyterLab. Refresh JupyterLab to load the change in your browser (you may need to wait several seconds for the extension to be rebuilt).
 
 By default, the `jlpm build` command generates the source maps for this extension to make it easier to debug using the browser dev tools. To also generate source maps for the JupyterLab core extensions, you can run the following command:
 
@@ -135,11 +171,7 @@
 ```bash
 pip uninstall jupyterlab_ariakedark_theme
 ```
 
 In development mode, you will also need to remove the symlink created by `jupyter labextension develop`
 command. To find its location, you can run `jupyter labextension list` to figure out where the `labextensions`
 folder is located. Then you can remove the symlink named `jupyterlab_ariakedark_theme` within that folder.
-
-### Packaging the extension
-
-See [RELEASE](RELEASE.md)
```

