# Comparing `tmp/thelogger-0.3.5-py3-none-any.whl.zip` & `tmp/thelogger-0.3.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 15606 bytes, number of entries: 13
+Zip file size: 15726 bytes, number of entries: 13
 -rw-rw-rw-  2.0 fat      514 b- defN 23-Jul-22 00:12 thelogger/__init__.py
 -rw-rw-rw-  2.0 fat     4234 b- defN 22-Feb-20 09:05 thelogger/__logger.py
 -rw-rw-rw-  2.0 fat      214 b- defN 23-Apr-27 17:46 thelogger/__ver.py
 -rw-rw-rw-  2.0 fat     1049 b- defN 23-Jun-17 05:10 thelogger/dirty_timer.py
--rw-rw-rw-  2.0 fat     4390 b- defN 23-Jul-22 00:09 thelogger/sys_meta.py
+-rw-rw-rw-  2.0 fat     4771 b- defN 23-Jul-24 20:08 thelogger/sys_meta.py
 -rw-rw-rw-  2.0 fat      140 b- defN 22-Feb-20 09:05 thelogger/notify/__init__.py
 -rw-rw-rw-  2.0 fat     3611 b- defN 22-Feb-20 09:49 thelogger/notify/decorator.py
 -rw-rw-rw-  2.0 fat     6990 b- defN 23-Feb-28 14:35 thelogger/notify/exec_func.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Jul-22 00:13 thelogger-0.3.5.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     6692 b- defN 23-Jul-22 00:13 thelogger-0.3.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-22 00:13 thelogger-0.3.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-Jul-22 00:13 thelogger-0.3.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1041 b- defN 23-Jul-22 00:13 thelogger-0.3.5.dist-info/RECORD
-13 files, 40535 bytes uncompressed, 13876 bytes compressed:  65.8%
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Jul-24 20:08 thelogger-0.3.6.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     6692 b- defN 23-Jul-24 20:08 thelogger-0.3.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-24 20:08 thelogger-0.3.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Jul-24 20:08 thelogger-0.3.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1041 b- defN 23-Jul-24 20:08 thelogger-0.3.6.dist-info/RECORD
+13 files, 40916 bytes uncompressed, 13996 bytes compressed:  65.8%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: thelogger/notify/decorator.py
 Comment: 
 
 Filename: thelogger/notify/exec_func.py
 Comment: 
 
-Filename: thelogger-0.3.5.dist-info/LICENSE
+Filename: thelogger-0.3.6.dist-info/LICENSE
 Comment: 
 
-Filename: thelogger-0.3.5.dist-info/METADATA
+Filename: thelogger-0.3.6.dist-info/METADATA
 Comment: 
 
-Filename: thelogger-0.3.5.dist-info/WHEEL
+Filename: thelogger-0.3.6.dist-info/WHEEL
 Comment: 
 
-Filename: thelogger-0.3.5.dist-info/top_level.txt
+Filename: thelogger-0.3.6.dist-info/top_level.txt
 Comment: 
 
-Filename: thelogger-0.3.5.dist-info/RECORD
+Filename: thelogger-0.3.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## thelogger/sys_meta.py

```diff
@@ -57,34 +57,44 @@
         cpu_used = str(cpu_used) + '%',
         memory_used = str(memory_used)  + '%',
         datetime = dttm
         )
     return usage
 
 def try_version(x):
+    # some pkgs have diff dist names so this doesnt always work
+    # std libs don't have versions
     try:
         ver = version(x)
     except:
-        ver = '?'# std libs don't have versions
+        ver = None
     return ver
 
 def get_imported_pkg_vers():
-    # excludes std libs
-    package_names = set()
+    nms = []
+    vers = []
     for module_name, module in sys.modules.items():
         if (module and hasattr(module, '__package__') and module.__package__
-        and module_name[0] != '_'):
-            package_names.add(module.__package__)
-    imp_mod = pd.Series(list(package_names), name = 'pkgs')
-    imp_mod = imp_mod.str.split('.').str[0]
-    imp_mod = imp_mod.drop_duplicates()
-    imp_mod = pd.DataFrame(imp_mod)
-    imp_mod['version'] = imp_mod.pkgs.apply(lambda x: try_version(x))
-    imp_mod = imp_mod.loc[imp_mod.version != '?'].sort_values('pkgs')\
-        .reset_index(drop=True)
+        and module_name[0] != '_' and '.' not in module_name):
+            try:
+                # some pkgs dont have __version__ attr
+                ver = getattr(module, '__version__')
+            except:
+                ver = None 
+            nms.append(module.__package__)
+            vers.append(ver)
+    imp_mod = pd.DataFrame(dict(nm=nms, ver=vers)).drop_duplicates()
+    missing_ver = imp_mod.loc[imp_mod.ver.isnull()]
+    ver_from_meta = missing_ver.nm.apply(lambda x: try_version(x))
+    imp_mod.ver = imp_mod.ver.fillna(ver_from_meta)
+    imp_mod.ver = imp_mod.ver.str.strip()
+    imp_mod = imp_mod.loc[imp_mod.ver.notnull()].drop_duplicates()\
+        .sort_values('nm').reset_index(drop=True)
+    imp_mod.columns = ['pkgs', 'version']
+            
     return imp_mod
 
 def get_env_info(pkgs = None):
     py_ver = ".".join(str(component) for component in sys.version_info[:3])
     pkgs = [pkgs] if type(pkgs) == str else pkgs
     imported_pkgs = get_imported_pkg_vers()
     if pkgs:
```

## Comparing `thelogger-0.3.5.dist-info/LICENSE` & `thelogger-0.3.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `thelogger-0.3.5.dist-info/METADATA` & `thelogger-0.3.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thelogger
-Version: 0.3.5
+Version: 0.3.6
 Summary: Easy logging, timing and email notifications of code execution.
 Home-page: https://github.com/tom1919/TheLogger
 Author: Tom1919
 Author-email: py.notify1@gmail.com
 License: Apache 2.0
 Keywords: log,logging,logger,email,timimg,notification
 Platform: UNKNOWN
```

## Comparing `thelogger-0.3.5.dist-info/RECORD` & `thelogger-0.3.6.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 thelogger/__init__.py,sha256=_I66PepW9Wf-esyHGfSXp_FdzdrI1i7RweTEWBMLMgo,514
 thelogger/__logger.py,sha256=JTyQbecMYpi1n7zKoVe9sohS6tTy87Bx2UnCDHb4-N4,4234
 thelogger/__ver.py,sha256=v27jnS60TKa54IbFVzSTknhDiKMS4J3KCuFTOffZqRU,214
 thelogger/dirty_timer.py,sha256=NxlxGSQ09Q3BRRKYlIRgFahGFgvAn78a9xb-xrNKkXc,1049
-thelogger/sys_meta.py,sha256=_sjOQqeeIPDBX6YhX_LkYsOy060BMCCOxPt2qcC4Y80,4390
+thelogger/sys_meta.py,sha256=mlFpnSDHrvrmQiCZ8jPMF23k8OSYFrKgKcO9h9koDmM,4771
 thelogger/notify/__init__.py,sha256=X0cVRenLKIbnOoapwPN9KJvtwXaHycKVb-ZTZ8tmuWQ,140
 thelogger/notify/decorator.py,sha256=kiiVpcCayMsdtGtiOtswHaa_v8OzSQjXnKnoSvrt0Uk,3611
 thelogger/notify/exec_func.py,sha256=uN4mbHtdmG4-djWnEzomVeFfbOJ6jHqlNmydolX5QwU,6990
-thelogger-0.3.5.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-thelogger-0.3.5.dist-info/METADATA,sha256=pX7isIrFv2qonNpVBNI7vrSVUbtT0ZHBi2pqSPkquSQ,6692
-thelogger-0.3.5.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-thelogger-0.3.5.dist-info/top_level.txt,sha256=6qGJ7TaRPKJuypP1ToyTCDT03pcvwWZ-vqDreYaUfjQ,10
-thelogger-0.3.5.dist-info/RECORD,,
+thelogger-0.3.6.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+thelogger-0.3.6.dist-info/METADATA,sha256=B0ozM77g7CqvdQzkpVsq8qW_azh_x1kwcfYe_mZnGDs,6692
+thelogger-0.3.6.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+thelogger-0.3.6.dist-info/top_level.txt,sha256=6qGJ7TaRPKJuypP1ToyTCDT03pcvwWZ-vqDreYaUfjQ,10
+thelogger-0.3.6.dist-info/RECORD,,
```

