# Comparing `tmp/spatialdata_io-0.0.6.tar.gz` & `tmp/spatialdata_io-0.0.7.tar.gz`

## Comparing `spatialdata_io-0.0.6.tar` & `spatialdata_io-0.0.7.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/.bumpversion.cfg
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/.codecov.yaml
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/.editorconfig
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/.flake8
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/.mypy.ini
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/.readthedocs.yaml
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/CHANGELOG.md
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/_version.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/.github/workflows/build.yaml
--rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/.github/workflows/test_and_deploy.yaml
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/docs/Makefile
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/docs/api.md
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/docs/changelog.md
--rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/docs/conf.py
--rw-r--r--   0        0        0     7807 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/docs/contributing.md
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/docs/index.md
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/docs/make.bat
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/docs/references.bib
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/docs/references.md
--rw-r--r--   0        0        0    16386 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/docs/template_usage.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/docs/_static/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/docs/_templates/.gitkeep
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/docs/_templates/autosummary/class.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/docs/extensions/.gitkeep
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/docs/extensions/typed_returns.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/src/spatialdata_io/__init__.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/src/spatialdata_io/_docs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/src/spatialdata_io/_constants/__init__.py
--rw-r--r--   0        0        0     5019 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/src/spatialdata_io/_constants/_constants.py
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/src/spatialdata_io/_constants/_enum.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/src/spatialdata_io/readers/__init__.py
--rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/src/spatialdata_io/readers/codex.py
--rw-r--r--   0        0        0    12550 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/src/spatialdata_io/readers/cosmx.py
--rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/src/spatialdata_io/readers/curio.py
--rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/src/spatialdata_io/readers/mcmicro.py
--rw-r--r--   0        0        0     7492 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/src/spatialdata_io/readers/merscope.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/src/spatialdata_io/readers/metaspace.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/src/spatialdata_io/readers/resolve.py
--rw-r--r--   0        0        0     4051 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/src/spatialdata_io/readers/steinbock.py
--rw-r--r--   0        0        0     8707 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/src/spatialdata_io/readers/visium.py
--rw-r--r--   0        0        0     8080 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/src/spatialdata_io/readers/xenium.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/src/spatialdata_io/readers/_utils/__init__.py
--rw-r--r--   0        0        0     5340 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/src/spatialdata_io/readers/_utils/_read_10x_h5.py
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/src/spatialdata_io/readers/_utils/_utils.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/tests/test_basic.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/.gitignore
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/LICENSE
--rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/README.md
--rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     5361 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/.bumpversion.cfg
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/.codecov.yaml
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/.editorconfig
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/.flake8
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/.mypy.ini
+-rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/.readthedocs.yaml
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/CHANGELOG.md
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/_version.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/.github/workflows/build.yaml
+-rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/.github/workflows/test_and_deploy.yaml
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/docs/Makefile
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/docs/api.md
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/docs/changelog.md
+-rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/docs/conf.py
+-rw-r--r--   0        0        0     7807 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/docs/contributing.md
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/docs/index.md
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/docs/make.bat
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/docs/references.bib
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/docs/references.md
+-rw-r--r--   0        0        0    16386 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/docs/template_usage.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/docs/_static/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/docs/_templates/.gitkeep
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/docs/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/docs/extensions/.gitkeep
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/docs/extensions/typed_returns.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/src/spatialdata_io/__init__.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/src/spatialdata_io/_docs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/src/spatialdata_io/_constants/__init__.py
+-rw-r--r--   0        0        0     5019 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/src/spatialdata_io/_constants/_constants.py
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/src/spatialdata_io/_constants/_enum.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/src/spatialdata_io/readers/__init__.py
+-rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/src/spatialdata_io/readers/codex.py
+-rw-r--r--   0        0        0    12550 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/src/spatialdata_io/readers/cosmx.py
+-rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/src/spatialdata_io/readers/curio.py
+-rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/src/spatialdata_io/readers/mcmicro.py
+-rw-r--r--   0        0        0     7513 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/src/spatialdata_io/readers/merscope.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/src/spatialdata_io/readers/metaspace.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/src/spatialdata_io/readers/resolve.py
+-rw-r--r--   0        0        0     4051 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/src/spatialdata_io/readers/steinbock.py
+-rw-r--r--   0        0        0     8854 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/src/spatialdata_io/readers/visium.py
+-rw-r--r--   0        0        0     8065 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/src/spatialdata_io/readers/xenium.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/src/spatialdata_io/readers/_utils/__init__.py
+-rw-r--r--   0        0        0     5340 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/src/spatialdata_io/readers/_utils/_read_10x_h5.py
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/src/spatialdata_io/readers/_utils/_utils.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/tests/test_basic.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/README.md
+-rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     5361 2020-02-02 00:00:00.000000 spatialdata_io-0.0.7/PKG-INFO
```

### Comparing `spatialdata_io-0.0.6/.flake8` & `spatialdata_io-0.0.7/.flake8`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.6/.mypy.ini` & `spatialdata_io-0.0.7/.mypy.ini`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.6/.pre-commit-config.yaml` & `spatialdata_io-0.0.7/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -3,31 +3,31 @@
     python: python3
 default_stages:
     - commit
     - push
 minimum_pre_commit_version: 2.16.0
 repos:
     - repo: https://github.com/psf/black
-      rev: 23.3.0
+      rev: 23.7.0
       hooks:
           - id: black
     - repo: https://github.com/pre-commit/mirrors-prettier
-      rev: v3.0.0-alpha.9-for-vscode
+      rev: v3.0.0
       hooks:
           - id: prettier
     - repo: https://github.com/asottile/blacken-docs
-      rev: 1.14.0
+      rev: 1.15.0
       hooks:
           - id: blacken-docs
     - repo: https://github.com/PyCQA/isort
       rev: 5.12.0
       hooks:
           - id: isort
     - repo: https://github.com/pre-commit/mirrors-mypy
-      rev: v1.3.0
+      rev: v1.4.1
       hooks:
           - id: mypy
             additional_dependencies: [numpy]
             exclude: docs/
     - repo: https://github.com/asottile/yesqa
       rev: v1.5.0
       hooks:
@@ -46,15 +46,15 @@
           - id: check-ast
           - id: end-of-file-fixer
           - id: mixed-line-ending
             args: [--fix=lf]
           - id: trailing-whitespace
           - id: check-case-conflict
     - repo: https://github.com/PyCQA/autoflake
-      rev: v2.1.1
+      rev: v2.2.0
       hooks:
           - id: autoflake
             args:
                 - --in-place
                 - --remove-all-unused-imports
                 - --remove-unused-variable
                 - --ignore-init-module-imports
@@ -66,15 +66,15 @@
                 - flake8-tidy-imports
                 - flake8-docstrings
                 - flake8-rst-docstrings
                 - flake8-comprehensions
                 - flake8-bugbear
                 - flake8-blind-except
     - repo: https://github.com/asottile/pyupgrade
-      rev: v3.7.0
+      rev: v3.9.0
       hooks:
           - id: pyupgrade
             args: [--py3-plus, --py39-plus, --keep-runtime-typing]
     - repo: local
       hooks:
           - id: forbid-to-commit
             name: Don't commit rej files
```

### Comparing `spatialdata_io-0.0.6/.github/workflows/build.yaml` & `spatialdata_io-0.0.7/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.6/.github/workflows/test_and_deploy.yaml` & `spatialdata_io-0.0.7/.github/workflows/test_and_deploy.yaml`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.6/docs/Makefile` & `spatialdata_io-0.0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.6/docs/conf.py` & `spatialdata_io-0.0.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.6/docs/contributing.md` & `spatialdata_io-0.0.7/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.6/docs/make.bat` & `spatialdata_io-0.0.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.6/docs/references.bib` & `spatialdata_io-0.0.7/docs/references.bib`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.6/docs/template_usage.md` & `spatialdata_io-0.0.7/docs/template_usage.md`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.6/docs/_templates/autosummary/class.rst` & `spatialdata_io-0.0.7/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.6/docs/extensions/typed_returns.py` & `spatialdata_io-0.0.7/docs/extensions/typed_returns.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.6/src/spatialdata_io/__init__.py` & `spatialdata_io-0.0.7/src/spatialdata_io/__init__.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.6/src/spatialdata_io/_docs.py` & `spatialdata_io-0.0.7/src/spatialdata_io/_docs.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.6/src/spatialdata_io/_constants/_constants.py` & `spatialdata_io-0.0.7/src/spatialdata_io/_constants/_constants.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.6/src/spatialdata_io/_constants/_enum.py` & `spatialdata_io-0.0.7/src/spatialdata_io/_constants/_enum.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.6/src/spatialdata_io/readers/codex.py` & `spatialdata_io-0.0.7/src/spatialdata_io/readers/codex.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,18 +78,18 @@
         image = imread(path_files[0], **imread_kwargs)
         images = {
             "images": Image2DModel.parse(
                 image,
                 scale_factors=[2, 2],
             )
         }
-        sdata = SpatialData(images=images, shapes={region: shapes}, table=table)
+        sdata = SpatialData(images=images, shapes={str(region): shapes}, table=table)
     else:
         logger.warning("Cannot find .tif file. Will build spatialdata with shapes and table only.")
-        sdata = SpatialData(shapes={region: shapes}, table=table)
+        sdata = SpatialData(shapes={str(region): shapes}, table=table)
 
     return sdata
 
 
 def _codex_df_to_anndata(df: pd.DataFrame) -> ad.AnnData:
     """Convert a codex formatted .fcs dataframe or .csv file to anndata."""
     adata = ad.AnnData(df.filter(regex="cyc.*"))
```

### Comparing `spatialdata_io-0.0.6/src/spatialdata_io/readers/cosmx.py` & `spatialdata_io-0.0.7/src/spatialdata_io/readers/cosmx.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.6/src/spatialdata_io/readers/curio.py` & `spatialdata_io-0.0.7/src/spatialdata_io/readers/curio.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.6/src/spatialdata_io/readers/mcmicro.py` & `spatialdata_io-0.0.7/src/spatialdata_io/readers/mcmicro.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.6/src/spatialdata_io/readers/merscope.py` & `spatialdata_io-0.0.7/src/spatialdata_io/readers/merscope.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,19 +148,18 @@
         images[f"{dataset_id}_z{z_layer}"] = parsed_im
 
     # Transcripts
     transcript_df = dd.read_csv(path / MerscopeKeys.TRANSCRIPTS_FILE)
     transcripts = PointsModel.parse(
         transcript_df,
         coordinates={"x": MerscopeKeys.GLOBAL_X, "y": MerscopeKeys.GLOBAL_Y},
-        transformations={"pixels": Identity()},
+        transformations={"pixels": microns_to_pixels},
     )
-    gene_categorical = dd.from_pandas(
-        transcripts["gene"].compute().astype("category"), npartitions=transcripts.npartitions
-    ).reset_index(drop=True)
+    categories = transcripts["gene"].compute().astype("category")
+    gene_categorical = dd.from_pandas(categories, npartitions=transcripts.npartitions).reset_index(drop=True)
     transcripts["gene"] = gene_categorical
 
     points = {f"{dataset_id}_transcripts": transcripts}
 
     # Polygons
     geo_df = geopandas.read_parquet(boundaries_path)
     geo_df = geo_df.rename_geometry("geometry")
```

### Comparing `spatialdata_io-0.0.6/src/spatialdata_io/readers/steinbock.py` & `spatialdata_io-0.0.7/src/spatialdata_io/readers/steinbock.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.6/src/spatialdata_io/readers/visium.py` & `spatialdata_io-0.0.7/src/spatialdata_io/readers/visium.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,17 @@
         else:
             raise ValueError(
                 f"Cannot determine the library_id. Expecting a file with format <library_id>_{VisiumKeys.COUNTS_FILE}. Has "
                 f"the files been renamed?"
             )
         counts_file = f"{library_id}_{VisiumKeys.COUNTS_FILE}"
     except IndexError as e:
-        logger.error(e)
+        logger.error(
+            f"{e}. \nError is due to the fact that the library id could not be found, this is the case when the `counts_file` is `.mtx`.",
+        )
         if dataset_id is None:
             raise ValueError("Cannot determine the `library_id`. Please provide `dataset_id`.")
         library_id = dataset_id
         if counts_file is None:
             raise ValueError("Cannot determine the library_id. Please provide `counts_file`.")
 
     if dataset_id is not None:
```

### Comparing `spatialdata_io-0.0.6/src/spatialdata_io/readers/xenium.py` & `spatialdata_io-0.0.7/src/spatialdata_io/readers/xenium.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,15 @@
 
 
 def _get_tables_and_circles(
     path: Path, cells_as_shapes: bool, specs: dict[str, Any]
 ) -> AnnData | tuple[AnnData, AnnData]:
     adata = _read_10x_h5(path / XeniumKeys.CELL_FEATURE_MATRIX_FILE)
     metadata = pd.read_parquet(path / XeniumKeys.CELL_METADATA_FILE)
-    np.testing.assert_array_equal(metadata.cell_id.str.decode("utf-8").values, adata.obs_names.values)
+    np.testing.assert_array_equal(metadata.cell_id.astype(str), adata.obs_names.values)
     circ = metadata[[XeniumKeys.CELL_X, XeniumKeys.CELL_Y]].to_numpy()
     adata.obsm["spatial"] = circ
     metadata.drop([XeniumKeys.CELL_X, XeniumKeys.CELL_Y], axis=1, inplace=True)
     adata.obs = metadata
     adata.obs["region"] = specs["region"]
     table = TableModel.parse(adata, region=specs["region"], region_key="region", instance_key=str(XeniumKeys.CELL_ID))
     if cells_as_shapes:
```

### Comparing `spatialdata_io-0.0.6/src/spatialdata_io/readers/_utils/_read_10x_h5.py` & `spatialdata_io-0.0.7/src/spatialdata_io/readers/_utils/_read_10x_h5.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.6/src/spatialdata_io/readers/_utils/_utils.py` & `spatialdata_io-0.0.7/src/spatialdata_io/readers/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.6/LICENSE` & `spatialdata_io-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.6/README.md` & `spatialdata_io-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.6/pyproject.toml` & `spatialdata_io-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.6/PKG-INFO` & `spatialdata_io-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatialdata-io
-Version: 0.0.6
+Version: 0.0.7
 Summary: SpatialData IO for common techs
 Project-URL: Documentation, https://spatialdata-io.readthedocs.io/
 Project-URL: Source, https://github.com/scverse/spatialdata-io
 Project-URL: Home-page, https://github.com/scverse/spatialdata-io
 Author: scverse
 Maintainer-email: scverse <scverse@scverse.scverse>
 License: BSD 3-Clause License
```

