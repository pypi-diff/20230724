# Comparing `tmp/scce-0.1.1.tar.gz` & `tmp/scce-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scce-0.1.1.tar", max compression
+gzip compressed data, was "scce-0.1.2.tar", max compression
```

## Comparing `scce-0.1.1.tar` & `scce-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,22 @@
--rw-r--r--   0        0        0     1636 2023-06-06 03:23:54.530322 scce-0.1.1/README.md
--rw-r--r--   0        0        0      934 2023-06-06 03:23:54.540322 scce-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-28 14:35:48.560479 scce-0.1.1/scce/__init__.py
--rw-r--r--   0        0        0      311 2023-05-28 14:35:48.561479 scce-0.1.1/scce/analyse/__init__.py
--rw-r--r--   0        0        0     1215 2023-05-28 14:35:48.562479 scce-0.1.1/scce/analyse/attribution.py
--rw-r--r--   0        0        0     1291 2023-05-28 14:35:48.563479 scce-0.1.1/scce/data.py
--rw-r--r--   0        0        0     8065 2023-06-06 03:23:54.541322 scce-0.1.1/scce/integrate.py
--rw-r--r--   0        0        0     4832 2023-05-28 14:35:48.566479 scce-0.1.1/scce/model/__init__.py
--rw-r--r--   0        0        0     2984 2023-06-06 03:15:24.744507 scce-0.1.1/scce/model/dataset.py
--rw-r--r--   0        0        0      566 2023-05-28 14:35:48.568479 scce-0.1.1/scce/model/focalloss.py
--rw-r--r--   0        0        0     3695 2023-05-28 14:35:48.569479 scce-0.1.1/scce/model/net.py
--rw-r--r--   0        0        0     5918 2023-05-28 14:35:48.570479 scce-0.1.1/scce/model/train_model.py
--rw-r--r--   0        0        0     1705 2023-05-28 14:35:48.571479 scce-0.1.1/scce/model/util.py
--rwxr-xr-x   0        0        0      811 2023-05-28 14:35:48.572479 scce-0.1.1/scce/model/validate.py
--rw-r--r--   0        0        0       62 2023-05-28 14:35:48.574479 scce-0.1.1/scce/plot/__init__.py
--rw-r--r--   0        0        0     2382 2023-05-28 14:35:48.575479 scce-0.1.1/scce/plot/base.py
--rw-r--r--   0        0        0     1346 2023-05-28 14:35:48.576479 scce-0.1.1/scce/plot/view.py
--rw-r--r--   0        0        0     3889 2023-06-06 03:23:54.543322 scce-0.1.1/scce/preprocess.py
--rw-r--r--   0        0        0     1434 2023-05-28 14:35:48.578479 scce-0.1.1/scce/utils.py
--rw-r--r--   0        0        0     2722 1970-01-01 00:00:00.000000 scce-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-06 03:48:04.000000 scce-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1636 2023-06-09 06:51:35.000000 scce-0.1.2/README.md
+-rw-r--r--   0        0        0      934 2023-07-24 09:33:38.714647 scce-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-09 06:51:36.000000 scce-0.1.2/scce/__init__.py
+-rw-r--r--   0        0        0     1206 2023-07-24 09:02:17.285714 scce-0.1.2/scce/analyse/__init__.py
+-rw-r--r--   0        0        0     1215 2023-07-21 08:59:16.129822 scce-0.1.2/scce/analyse/attribution.py
+-rw-r--r--   0        0        0     2571 2023-07-23 14:36:06.977044 scce-0.1.2/scce/analyse/chromatin_remodeling.py
+-rw-r--r--   0        0        0     1291 2023-06-09 06:51:36.000000 scce-0.1.2/scce/data.py
+-rw-r--r--   0        0        0     8065 2023-06-09 06:51:36.000000 scce-0.1.2/scce/integrate.py
+-rw-r--r--   0        0        0     4832 2023-06-09 06:51:36.000000 scce-0.1.2/scce/model/__init__.py
+-rw-r--r--   0        0        0     2984 2023-06-09 06:51:36.000000 scce-0.1.2/scce/model/dataset.py
+-rw-r--r--   0        0        0      566 2023-06-09 06:51:36.000000 scce-0.1.2/scce/model/focalloss.py
+-rw-r--r--   0        0        0     3695 2023-06-09 06:51:36.000000 scce-0.1.2/scce/model/net.py
+-rw-r--r--   0        0        0     5918 2023-06-09 06:51:36.000000 scce-0.1.2/scce/model/train_model.py
+-rw-r--r--   0        0        0     1705 2023-06-09 06:51:36.000000 scce-0.1.2/scce/model/util.py
+-rwxr-xr-x   0        0        0      811 2023-06-09 06:51:36.000000 scce-0.1.2/scce/model/validate.py
+-rw-r--r--   0        0        0       62 2023-06-09 06:51:36.000000 scce-0.1.2/scce/plot/__init__.py
+-rw-r--r--   0        0        0     3064 2023-07-24 09:04:27.214709 scce-0.1.2/scce/plot/base.py
+-rw-r--r--   0        0        0     1346 2023-07-24 08:56:48.266725 scce-0.1.2/scce/plot/view.py
+-rw-r--r--   0        0        0     3889 2023-06-09 06:51:36.000000 scce-0.1.2/scce/preprocess.py
+-rw-r--r--   0        0        0     1434 2023-06-09 06:51:36.000000 scce-0.1.2/scce/utils.py
+-rw-r--r--   0        0        0     2722 1970-01-01 00:00:00.000000 scce-0.1.2/PKG-INFO
```

### Comparing `scce-0.1.1/README.md` & `scce-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `scce-0.1.1/pyproject.toml` & `scce-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scce"
-version = "0.1.1"
+version = "0.1.2"
 description = "a Single-cell method for predicting Chromatin Conformation based on gene Expression"
 license = "Apache License 2.0"
 authors = ["liminghong.dev <lmh0066@outlook.com>"]
 readme = "README.md"
 repository = "https://github.com/LMH0066/SEE"
 keywords = ["bioinformatics", "deep-learning", "single-cell"]
```

### Comparing `scce-0.1.1/scce/analyse/attribution.py` & `scce-0.1.2/scce/analyse/attribution.py`

 * *Files identical despite different names*

### Comparing `scce-0.1.1/scce/data.py` & `scce-0.1.2/scce/data.py`

 * *Files identical despite different names*

### Comparing `scce-0.1.1/scce/integrate.py` & `scce-0.1.2/scce/integrate.py`

 * *Files identical despite different names*

### Comparing `scce-0.1.1/scce/model/__init__.py` & `scce-0.1.2/scce/model/__init__.py`

 * *Files identical despite different names*

### Comparing `scce-0.1.1/scce/model/dataset.py` & `scce-0.1.2/scce/model/dataset.py`

 * *Files identical despite different names*

### Comparing `scce-0.1.1/scce/model/focalloss.py` & `scce-0.1.2/scce/model/focalloss.py`

 * *Files identical despite different names*

### Comparing `scce-0.1.1/scce/model/net.py` & `scce-0.1.2/scce/model/net.py`

 * *Files identical despite different names*

### Comparing `scce-0.1.1/scce/model/train_model.py` & `scce-0.1.2/scce/model/train_model.py`

 * *Files identical despite different names*

### Comparing `scce-0.1.1/scce/model/util.py` & `scce-0.1.2/scce/model/util.py`

 * *Files identical despite different names*

### Comparing `scce-0.1.1/scce/model/validate.py` & `scce-0.1.2/scce/model/validate.py`

 * *Files identical despite different names*

### Comparing `scce-0.1.1/scce/plot/base.py` & `scce-0.1.2/scce/plot/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -78,7 +78,33 @@
     if xticklabels:
         ax.set_xticklabels(labels=xticklabels)
 
     if output_path:
         plt.savefig(output_path, bbox_inches="tight")
     else:
         plt.show()
+
+
+def heatmap(x, y, value, levels, cbar_label, output_path: str = None):
+    set_plt(figsize=(10, 10))
+    sns.set_theme(style="whitegrid")
+    fig, ax = plt.subplots()
+
+    cs = ax.contourf(x, y, value, levels=levels, cmap=plt.cm.jet)
+    cbar = plt.colorbar(cs)
+    cbar.set_label(cbar_label, rotation=90, fontsize=15)
+
+    ax.xaxis.set_ticks_position("top")
+    ax.invert_yaxis()
+    ax.set_aspect("equal", adjustable="box")
+    plt.tick_params(
+        colors="black",
+        top=True,
+        bottom=False,
+        left=True,
+        labelsize=figure_size["small"],
+    )
+
+    if output_path:
+        plt.savefig(output_path, bbox_inches="tight")
+    else:
+        plt.show()
```

### Comparing `scce-0.1.1/scce/plot/view.py` & `scce-0.1.2/scce/plot/view.py`

 * *Files identical despite different names*

### Comparing `scce-0.1.1/scce/preprocess.py` & `scce-0.1.2/scce/preprocess.py`

 * *Files identical despite different names*

### Comparing `scce-0.1.1/scce/utils.py` & `scce-0.1.2/scce/utils.py`

 * *Files identical despite different names*

### Comparing `scce-0.1.1/PKG-INFO` & `scce-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scce
-Version: 0.1.1
+Version: 0.1.2
 Summary: a Single-cell method for predicting Chromatin Conformation based on gene Expression
 Home-page: https://github.com/LMH0066/SEE
 License: Apache-2.0
 Keywords: bioinformatics,deep-learning,single-cell
 Author: liminghong.dev
 Author-email: lmh0066@outlook.com
 Requires-Python: >=3.8,<4.0
```

