# Comparing `tmp/g2nb-23.2.1.tar.gz` & `tmp/g2nb-23.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g2nb-23.2.1.tar", last modified: Mon Feb  6 21:57:23 2023, max compression
+gzip compressed data, was "g2nb-23.7.1.tar", last modified: Mon Jul 24 16:15:27 2023, max compression
```

## Comparing `g2nb-23.2.1.tar` & `g2nb-23.7.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 tmtabor    (501) staff       (20)        0 2023-02-06 21:57:23.278067 g2nb-23.2.1/
--rw-r--r--   0 tmtabor    (501) staff       (20)     1565 2022-04-13 16:47:04.000000 g2nb-23.2.1/LICENSE.txt
--rw-r--r--   0 tmtabor    (501) staff       (20)     2080 2023-02-06 21:57:23.278195 g2nb-23.2.1/PKG-INFO
--rw-r--r--   0 tmtabor    (501) staff       (20)     1301 2022-04-13 19:27:38.000000 g2nb-23.2.1/README.md
-drwxr-xr-x   0 tmtabor    (501) staff       (20)        0 2023-02-06 21:57:23.277861 g2nb-23.2.1/g2nb.egg-info/
--rw-r--r--   0 tmtabor    (501) staff       (20)     2080 2023-02-06 21:57:23.000000 g2nb-23.2.1/g2nb.egg-info/PKG-INFO
--rw-r--r--   0 tmtabor    (501) staff       (20)      221 2023-02-06 21:57:23.000000 g2nb-23.2.1/g2nb.egg-info/SOURCES.txt
--rw-r--r--   0 tmtabor    (501) staff       (20)        1 2023-02-06 21:57:23.000000 g2nb-23.2.1/g2nb.egg-info/dependency_links.txt
--rw-r--r--   0 tmtabor    (501) staff       (20)        1 2023-02-06 21:56:00.000000 g2nb-23.2.1/g2nb.egg-info/not-zip-safe
--rw-r--r--   0 tmtabor    (501) staff       (20)      108 2023-02-06 21:57:23.000000 g2nb-23.2.1/g2nb.egg-info/requires.txt
--rw-r--r--   0 tmtabor    (501) staff       (20)        1 2023-02-06 21:57:23.000000 g2nb-23.2.1/g2nb.egg-info/top_level.txt
--rw-r--r--   0 tmtabor    (501) staff       (20)      563 2023-02-06 21:48:56.000000 g2nb-23.2.1/pyproject.toml
--rw-r--r--   0 tmtabor    (501) staff       (20)      106 2023-02-06 21:57:23.278627 g2nb-23.2.1/setup.cfg
--rw-r--r--   0 tmtabor    (501) staff       (20)     2048 2023-02-06 21:49:25.000000 g2nb-23.2.1/setup.py
+drwxr-xr-x   0 tmtabor    (501) staff       (20)        0 2023-07-24 16:15:27.786139 g2nb-23.7.1/
+-rw-r--r--   0 tmtabor    (501) staff       (20)     1565 2022-04-13 16:47:04.000000 g2nb-23.7.1/LICENSE.txt
+-rw-r--r--   0 tmtabor    (501) staff       (20)     2080 2023-07-24 16:15:27.786241 g2nb-23.7.1/PKG-INFO
+-rw-r--r--   0 tmtabor    (501) staff       (20)     1301 2022-04-13 19:27:38.000000 g2nb-23.7.1/README.md
+drwxr-xr-x   0 tmtabor    (501) staff       (20)        0 2023-07-24 16:15:27.785928 g2nb-23.7.1/g2nb.egg-info/
+-rw-r--r--   0 tmtabor    (501) staff       (20)     2080 2023-07-24 16:15:27.000000 g2nb-23.7.1/g2nb.egg-info/PKG-INFO
+-rw-r--r--   0 tmtabor    (501) staff       (20)      221 2023-07-24 16:15:27.000000 g2nb-23.7.1/g2nb.egg-info/SOURCES.txt
+-rw-r--r--   0 tmtabor    (501) staff       (20)        1 2023-07-24 16:15:27.000000 g2nb-23.7.1/g2nb.egg-info/dependency_links.txt
+-rw-r--r--   0 tmtabor    (501) staff       (20)        1 2023-02-06 21:56:00.000000 g2nb-23.7.1/g2nb.egg-info/not-zip-safe
+-rw-r--r--   0 tmtabor    (501) staff       (20)      119 2023-07-24 16:15:27.000000 g2nb-23.7.1/g2nb.egg-info/requires.txt
+-rw-r--r--   0 tmtabor    (501) staff       (20)        1 2023-07-24 16:15:27.000000 g2nb-23.7.1/g2nb.egg-info/top_level.txt
+-rw-r--r--   0 tmtabor    (501) staff       (20)      563 2023-02-06 21:48:56.000000 g2nb-23.7.1/pyproject.toml
+-rw-r--r--   0 tmtabor    (501) staff       (20)      106 2023-07-24 16:15:27.786645 g2nb-23.7.1/setup.cfg
+-rw-r--r--   0 tmtabor    (501) staff       (20)     2070 2023-07-24 16:13:49.000000 g2nb-23.7.1/setup.py
```

### Comparing `g2nb-23.2.1/LICENSE.txt` & `g2nb-23.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `g2nb-23.2.1/PKG-INFO` & `g2nb-23.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g2nb
-Version: 23.2.1
+Version: 23.7.1
 Summary: Meta-package for installing all the g2nb tools
 Home-page: https://github.com/g2nb/g2nb
 Author: Thorin Tabor
 Author-email: tmtabor@cloud.ucsd.edu
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `g2nb-23.2.1/README.md` & `g2nb-23.7.1/README.md`

 * *Files identical despite different names*

### Comparing `g2nb-23.2.1/g2nb.egg-info/PKG-INFO` & `g2nb-23.7.1/g2nb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g2nb
-Version: 23.2.1
+Version: 23.7.1
 Summary: Meta-package for installing all the g2nb tools
 Home-page: https://github.com/g2nb/g2nb
 Author: Thorin Tabor
 Author-email: tmtabor@cloud.ucsd.edu
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `g2nb-23.2.1/pyproject.toml` & `g2nb-23.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `g2nb-23.2.1/setup.py` & `g2nb-23.7.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,20 +18,21 @@
     author_email=pkg_json["author"]["email"],
     description=pkg_json["description"],
     license=pkg_json["license"],
     long_description=(HERE / "README.md").read_text(),
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     install_requires=[
-        "jupyterlab~=3.4",
+        "jupyterlab~=3.6",
         "jupyter-packaging>=0.12.0",
         "nbtools",
         "genepattern-notebook",
         "igv-jupyter",
         "cywidget",
+        "galaxy-gin",
         "jupyter-wysiwyg"
     ],
     zip_safe=False,
     include_package_data=True,
     python_requires=">=3.6",
     platforms="Linux, Mac OS X, Windows",
     keywords=["Jupyter", "JupyterLab", "JupyterLab3"],
```

