# Comparing `tmp/sd_meh-0.9.0.tar.gz` & `tmp/sd_meh-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sd_meh-0.9.0.tar", max compression
+gzip compressed data, was "sd_meh-0.9.2.tar", max compression
```

## Comparing `sd_meh-0.9.0.tar` & `sd_meh-0.9.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1062 2023-07-21 09:28:13.014860 sd_meh-0.9.0/LICENSE.txt
--rw-r--r--   0        0        0     1977 2023-07-21 09:28:13.014860 sd_meh-0.9.0/README.md
--rw-r--r--   0        0        0      390 2023-07-21 09:28:13.014860 sd_meh-0.9.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-07-21 09:28:13.014860 sd_meh-0.9.0/sd_meh/__init__.py
--rw-r--r--   0        0        0    13752 2023-07-21 09:28:13.014860 sd_meh-0.9.0/sd_meh/merge.py
--rw-r--r--   0        0        0     6626 2023-07-21 09:28:13.014860 sd_meh-0.9.0/sd_meh/merge_methods.py
--rw-r--r--   0        0        0     1606 2023-07-21 09:28:13.014860 sd_meh-0.9.0/sd_meh/model.py
--rw-r--r--   0        0        0    10306 2023-07-21 09:28:13.014860 sd_meh-0.9.0/sd_meh/presets.py
--rw-r--r--   0        0        0    83496 2023-07-21 09:28:13.014860 sd_meh-0.9.0/sd_meh/rebasin.py
--rw-r--r--   0        0        0     2501 1970-01-01 00:00:00.000000 sd_meh-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-24 08:25:59.731213 sd_meh-0.9.2/LICENSE.txt
+-rw-r--r--   0        0        0     1984 2023-07-24 08:25:59.731213 sd_meh-0.9.2/README.md
+-rw-r--r--   0        0        0      390 2023-07-24 08:25:59.731213 sd_meh-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-24 08:25:59.731213 sd_meh-0.9.2/sd_meh/__init__.py
+-rw-r--r--   0        0        0    13790 2023-07-24 08:25:59.731213 sd_meh-0.9.2/sd_meh/merge.py
+-rw-r--r--   0        0        0     6626 2023-07-24 08:25:59.731213 sd_meh-0.9.2/sd_meh/merge_methods.py
+-rw-r--r--   0        0        0     1606 2023-07-24 08:25:59.731213 sd_meh-0.9.2/sd_meh/model.py
+-rw-r--r--   0        0        0    10306 2023-07-24 08:25:59.731213 sd_meh-0.9.2/sd_meh/presets.py
+-rw-r--r--   0        0        0    83496 2023-07-24 08:25:59.731213 sd_meh-0.9.2/sd_meh/rebasin.py
+-rw-r--r--   0        0        0     2508 1970-01-01 00:00:00.000000 sd_meh-0.9.2/PKG-INFO
```

### Comparing `sd_meh-0.9.0/LICENSE.txt` & `sd_meh-0.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sd_meh-0.9.0/README.md` & `sd_meh-0.9.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 You can have a look at the provided `merge_models.py` cli for an example on how to use the function. Run `python3 merge_models.py --help` for a list of the available arguments.
 
 [Join](https://discord.gg/EZJuBfNVHh) our discord server for discussion and features/bugfix requests
 
 ## Changelog
 
-### 0.9.0
+### 0.9.1, 0.9.2
 - bugfixes
 - support for pix2pix and inpainting models
 
 ### 0.8.0
 - add `-bwpab, --block_weights_preset_alpha_b"` and `-pal, --presets_alpha_lambda` for presets interpolation (same for `beta`)
 - add `-ll, --logging_level`, default to `INFO`
```

### Comparing `sd_meh-0.9.0/sd_meh/merge.py` & `sd_meh-0.9.2/sd_meh/merge.py`

 * *Files 5% similar despite different names*

```diff
@@ -148,23 +148,20 @@
     if re_basin:
         merged = rebasin_merge(
             thetas,
             weights,
             bases,
             merge_mode,
             precision=precision,
-            weights_clip=False,
+            weights_clip=weights_clip,
             iterations=iterations,
             device=device,
             work_device=work_device,
             threads=threads,
         )
-        # clip only after the last re-basin iteration
-        if weights_clip:
-            merged = clip_weights(thetas, merged)
     else:
         merged = simple_merge(
             thetas,
             weights,
             bases,
             merge_mode,
             precision=precision,
@@ -294,15 +291,15 @@
         # normal block merge we already know and love
         thetas["model_a"] = simple_merge(
             thetas,
             new_weights,
             new_bases,
             merge_mode,
             precision,
-            weights_clip,
+            False,
             device,
             work_device,
             threads,
         )
 
         log_vram("simple merge done")
 
@@ -340,14 +337,19 @@
         ).tolist()[0]
         thetas["model_a"] = update_model_a(
             perm_spec, perm_2, thetas["model_a"], new_alpha
         )
 
         log_vram("model a updated")
 
+    if weights_clip:
+        clip_thetas = thetas.copy()
+        clip_thetas["model_a"] = model_a
+        thetas["model_a"] = clip_weights(thetas, thetas["model_a"])
+
     return thetas["model_a"]
 
 
 def simple_merge_key(progress, key, thetas, *args, **kwargs):
     with merge_key_context(key, thetas, *args, **kwargs) as result:
         if result is not None:
             thetas["model_a"].update({key: result.detach().clone()})
```

### Comparing `sd_meh-0.9.0/sd_meh/merge_methods.py` & `sd_meh-0.9.2/sd_meh/merge_methods.py`

 * *Files identical despite different names*

### Comparing `sd_meh-0.9.0/sd_meh/model.py` & `sd_meh-0.9.2/sd_meh/model.py`

 * *Files identical despite different names*

### Comparing `sd_meh-0.9.0/sd_meh/presets.py` & `sd_meh-0.9.2/sd_meh/presets.py`

 * *Files identical despite different names*

### Comparing `sd_meh-0.9.0/sd_meh/rebasin.py` & `sd_meh-0.9.2/sd_meh/rebasin.py`

 * *Files identical despite different names*

### Comparing `sd_meh-0.9.0/PKG-INFO` & `sd_meh-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sd-meh
-Version: 0.9.0
+Version: 0.9.2
 Summary: stable diffusion merging execution helper
 Home-page: https://github.com/s1dlx/meh
 License: MIT
 Author: s1dlx
 Author-email: s1dlx@proton.me
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -41,15 +41,15 @@
 
 You can have a look at the provided `merge_models.py` cli for an example on how to use the function. Run `python3 merge_models.py --help` for a list of the available arguments.
 
 [Join](https://discord.gg/EZJuBfNVHh) our discord server for discussion and features/bugfix requests
 
 ## Changelog
 
-### 0.9.0
+### 0.9.1, 0.9.2
 - bugfixes
 - support for pix2pix and inpainting models
 
 ### 0.8.0
 - add `-bwpab, --block_weights_preset_alpha_b"` and `-pal, --presets_alpha_lambda` for presets interpolation (same for `beta`)
 - add `-ll, --logging_level`, default to `INFO`
```

