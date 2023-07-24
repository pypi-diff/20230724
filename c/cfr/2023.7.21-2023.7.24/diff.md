# Comparing `tmp/cfr-2023.7.21.tar.gz` & `tmp/cfr-2023.7.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfr-2023.7.21.tar", last modified: Fri Jul 21 21:06:39 2023, max compression
+gzip compressed data, was "cfr-2023.7.24.tar", last modified: Mon Jul 24 21:36:05 2023, max compression
```

## Comparing `cfr-2023.7.21.tar` & `cfr-2023.7.24.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-07-21 21:06:39.942666 cfr-2023.7.21/
--rw-r--r--   0 fengzhu    (502) staff       (20)     1516 2022-04-27 05:34:15.000000 cfr-2023.7.21/LICENSE
--rw-r--r--   0 fengzhu    (502) staff       (20)     1988 2023-07-21 21:06:39.942480 cfr-2023.7.21/PKG-INFO
--rw-r--r--   0 fengzhu    (502) staff       (20)     1421 2023-06-28 18:00:43.000000 cfr-2023.7.21/README.md
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-07-21 21:06:39.933181 cfr-2023.7.21/bin/
--rw-r--r--   0 fengzhu    (502) staff       (20)     5134 2023-06-22 22:28:33.000000 cfr-2023.7.21/bin/cfr
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-07-21 21:06:39.938993 cfr-2023.7.21/cfr/
--rw-r--r--   0 fengzhu    (502) staff       (20)      732 2023-06-21 18:25:21.000000 cfr-2023.7.21/cfr/__init__.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    22467 2023-05-29 23:34:35.000000 cfr-2023.7.21/cfr/climate.py
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-07-21 21:06:39.942141 cfr-2023.7.21/cfr/da/
--rw-r--r--   0 fengzhu    (502) staff       (20)       22 2022-07-02 05:30:36.000000 cfr-2023.7.21/cfr/da/__init__.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    16319 2023-03-27 02:39:30.000000 cfr-2023.7.21/cfr/da/enkf.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    22484 2023-04-17 19:25:37.000000 cfr-2023.7.21/cfr/gcm.py
--rw-r--r--   0 fengzhu    (502) staff       (20)     7623 2022-05-05 04:13:16.000000 cfr-2023.7.21/cfr/ml.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    67751 2023-07-10 01:52:31.000000 cfr-2023.7.21/cfr/proxy.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    45058 2023-06-20 03:51:38.000000 cfr-2023.7.21/cfr/psm.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    57520 2023-06-29 20:52:53.000000 cfr-2023.7.21/cfr/reconjob.py
--rw-r--r--   0 fengzhu    (502) staff       (20)     4551 2023-06-26 04:44:01.000000 cfr-2023.7.21/cfr/reconres.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    19837 2023-07-21 20:46:49.000000 cfr-2023.7.21/cfr/ts.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    25261 2023-07-10 00:33:58.000000 cfr-2023.7.21/cfr/utils.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    60578 2023-07-21 20:57:56.000000 cfr-2023.7.21/cfr/visual.py
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-07-21 21:06:39.941239 cfr-2023.7.21/cfr.egg-info/
--rw-r--r--   0 fengzhu    (502) staff       (20)     1988 2023-07-21 21:06:39.000000 cfr-2023.7.21/cfr.egg-info/PKG-INFO
--rw-r--r--   0 fengzhu    (502) staff       (20)      373 2023-07-21 21:06:39.000000 cfr-2023.7.21/cfr.egg-info/SOURCES.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)        1 2023-07-21 21:06:39.000000 cfr-2023.7.21/cfr.egg-info/dependency_links.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)        1 2022-04-28 04:59:29.000000 cfr-2023.7.21/cfr.egg-info/not-zip-safe
--rw-r--r--   0 fengzhu    (502) staff       (20)      201 2023-07-21 21:06:39.000000 cfr-2023.7.21/cfr.egg-info/requires.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)        4 2023-07-21 21:06:39.000000 cfr-2023.7.21/cfr.egg-info/top_level.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)       38 2023-07-21 21:06:39.942724 cfr-2023.7.21/setup.cfg
--rw-r--r--   0 fengzhu    (502) staff       (20)     1404 2023-07-21 18:01:48.000000 cfr-2023.7.21/setup.py
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-07-24 21:36:05.425219 cfr-2023.7.24/
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1516 2022-04-27 05:34:15.000000 cfr-2023.7.24/LICENSE
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1988 2023-07-24 21:36:05.425047 cfr-2023.7.24/PKG-INFO
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1421 2023-06-28 18:00:43.000000 cfr-2023.7.24/README.md
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-07-24 21:36:05.415800 cfr-2023.7.24/bin/
+-rw-r--r--   0 fengzhu    (502) staff       (20)     5134 2023-06-22 22:28:33.000000 cfr-2023.7.24/bin/cfr
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-07-24 21:36:05.421528 cfr-2023.7.24/cfr/
+-rw-r--r--   0 fengzhu    (502) staff       (20)      732 2023-06-21 18:25:21.000000 cfr-2023.7.24/cfr/__init__.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    22944 2023-07-24 19:22:13.000000 cfr-2023.7.24/cfr/climate.py
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-07-24 21:36:05.424684 cfr-2023.7.24/cfr/da/
+-rw-r--r--   0 fengzhu    (502) staff       (20)       22 2022-07-02 05:30:36.000000 cfr-2023.7.24/cfr/da/__init__.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    16319 2023-03-27 02:39:30.000000 cfr-2023.7.24/cfr/da/enkf.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    22484 2023-04-17 19:25:37.000000 cfr-2023.7.24/cfr/gcm.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)     7623 2022-05-05 04:13:16.000000 cfr-2023.7.24/cfr/ml.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    67751 2023-07-10 01:52:31.000000 cfr-2023.7.24/cfr/proxy.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    45056 2023-07-24 19:22:13.000000 cfr-2023.7.24/cfr/psm.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    58401 2023-07-24 20:46:54.000000 cfr-2023.7.24/cfr/reconjob.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)     4551 2023-06-26 04:44:01.000000 cfr-2023.7.24/cfr/reconres.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    19837 2023-07-21 20:46:49.000000 cfr-2023.7.24/cfr/ts.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    25261 2023-07-10 00:33:58.000000 cfr-2023.7.24/cfr/utils.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    60578 2023-07-24 19:22:58.000000 cfr-2023.7.24/cfr/visual.py
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-07-24 21:36:05.423891 cfr-2023.7.24/cfr.egg-info/
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1988 2023-07-24 21:36:05.000000 cfr-2023.7.24/cfr.egg-info/PKG-INFO
+-rw-r--r--   0 fengzhu    (502) staff       (20)      373 2023-07-24 21:36:05.000000 cfr-2023.7.24/cfr.egg-info/SOURCES.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)        1 2023-07-24 21:36:05.000000 cfr-2023.7.24/cfr.egg-info/dependency_links.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)        1 2022-04-28 04:59:29.000000 cfr-2023.7.24/cfr.egg-info/not-zip-safe
+-rw-r--r--   0 fengzhu    (502) staff       (20)      201 2023-07-24 21:36:05.000000 cfr-2023.7.24/cfr.egg-info/requires.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)        4 2023-07-24 21:36:05.000000 cfr-2023.7.24/cfr.egg-info/top_level.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)       38 2023-07-24 21:36:05.425266 cfr-2023.7.24/setup.cfg
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1404 2023-07-24 20:40:08.000000 cfr-2023.7.24/setup.py
```

### Comparing `cfr-2023.7.21/LICENSE` & `cfr-2023.7.24/LICENSE`

 * *Files identical despite different names*

### Comparing `cfr-2023.7.21/PKG-INFO` & `cfr-2023.7.24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfr
-Version: 2023.7.21
+Version: 2023.7.24
 Summary: cfr: a Python package for Climate Field Reconstruction
 Home-page: https://github.com/fzhu2e/cfr
 Author: Feng Zhu, Julien Emile-Geay
 Author-email: fengzhu@ucar.edu, julieneg@usc.edu
 License: BSD 3-Clause
 Keywords: climate field reconstruction
 Classifier: Natural Language :: English
```

### Comparing `cfr-2023.7.21/README.md` & `cfr-2023.7.24/README.md`

 * *Files identical despite different names*

### Comparing `cfr-2023.7.21/bin/cfr` & `cfr-2023.7.24/bin/cfr`

 * *Files identical despite different names*

### Comparing `cfr-2023.7.21/cfr/__init__.py` & `cfr-2023.7.24/cfr/__init__.py`

 * *Files identical despite different names*

### Comparing `cfr-2023.7.21/cfr/climate.py` & `cfr-2023.7.24/cfr/climate.py`

 * *Files 2% similar despite different names*

```diff
@@ -633,15 +633,25 @@
         elif name == 'nino1+2':
             return self.geo_mean(lat_min=-10, lat_max=10, lon_min=np.mod(-90, 360), lon_max=np.mod(-80, 360))
         elif name == 'nino3':
             return self.geo_mean(lat_min=-5, lat_max=5, lon_min=np.mod(-150, 360), lon_max=np.mod(-90, 360))
         elif name == 'nino4':
             return self.geo_mean(lat_min=-5, lat_max=5, lon_min=np.mod(160, 360), lon_max=np.mod(-150, 360))
         elif name == 'wpi':
+            # Western Pacific Index
             return self.geo_mean(lat_min=-10, lat_max=10, lon_min=np.mod(120, 360), lon_max=np.mod(150, 360))
         elif name == 'tpi':
+            # Tri-Pole Index
             v1 = self.geo_mean(lat_min=25, lat_max=45, lon_min=np.mod(140, 360), lon_max=np.mod(-145, 360))
             v2 = self.geo_mean(lat_min=-10, lat_max=10, lon_min=np.mod(170, 360), lon_max=np.mod(-90, 360))
             v3 = self.geo_mean(lat_min=-50, lat_max=-15, lon_min=np.mod(150, 360), lon_max=np.mod(-160, 360))
             return v2 - (v1 + v3)/2
+        elif name == 'dmi':
+            # Indian Ocean Dipole Mode
+            dmiw = self.geo_mean(lat_min=-10, lat_max=10, lon_min=50, lon_max=70)
+            dmie = self.geo_mean(lat_min=-10, lat_max=0, lon_min=90, lon_max=110)
+            return dmiw - dmie
+        elif name == 'iobw':
+            # Indian Ocean Basin Wide
+            return self.geo_mean(lat_min=-20, lat_max=20, lon_min=40 ,lon_max=100)
         else:
             raise ValueError('Wrong index name.')
```

### Comparing `cfr-2023.7.21/cfr/da/enkf.py` & `cfr-2023.7.24/cfr/da/enkf.py`

 * *Files identical despite different names*

### Comparing `cfr-2023.7.21/cfr/gcm.py` & `cfr-2023.7.24/cfr/gcm.py`

 * *Files identical despite different names*

### Comparing `cfr-2023.7.21/cfr/ml.py` & `cfr-2023.7.24/cfr/ml.py`

 * *Files identical despite different names*

### Comparing `cfr-2023.7.21/cfr/proxy.py` & `cfr-2023.7.24/cfr/proxy.py`

 * *Files identical despite different names*

### Comparing `cfr-2023.7.21/cfr/psm.py` & `cfr-2023.7.24/cfr/psm.py`

 * *Files 0% similar despite different names*

```diff
@@ -219,15 +219,15 @@
             df_copy = df.copy()
             for sn2 in season_list2:
                 exog2_ann = exog2.annualize(months=sn2)
                 df_exog2 = pd.DataFrame({'time': exog2_ann.da.time.values, exog2_colname: exog2_ann.da.values})
                 df = df.merge(df_exog2.dropna(), how='inner', on='time')
                 df.set_index('time', drop=True, inplace=True)
                 df.sort_index(inplace=True)
-                df.astype(np.float)
+                df.astype(float)
                 if calib_period is not None:
                     mask = (df.index>=calib_period[0]) & (df.index<=calib_period[1])
                     df = clean_df(df, mask=mask)
 
                 formula_spell = f'proxy ~ {exog1_colname} + {exog2_colname}'
                 nobs = len(df)
                 if nobs < nobs_lb:
@@ -1121,8 +1121,8 @@
             ptype=self.pobj.ptype,
             value_name=self.pobj.value_name,
             value_unit=self.pobj.value_unit,
             time_name=self.pobj.time_name,
             time_unit=self.pobj.time_unit,
         )
 
-        return pp
+        return pp
```

### Comparing `cfr-2023.7.21/cfr/reconjob.py` & `cfr-2023.7.24/cfr/reconjob.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,15 +221,15 @@
         ''' Center the proxy timeseries against a reference time period.
 
         Args:
             ref_period (tuple or list): the reference time period in the form or (start_yr, end_yr)
             inplace (bool): if True, the annualized proxy database will replace the current `self.proxydb`.
             verbose (bool, optional): print verbose information. Defaults to False.
         '''
-        ref_period = self.io_cfg('proxydb_center_ref_period', ref_period, default=[1951, 1980], verbose=verbose)
+        ref_period = self.io_cfg('proxydb_center_ref_period', list(ref_period), default=[1951, 1980], verbose=verbose)
 
         centered_pdb = self.proxydb.center(ref_period)
         if inplace:
             self.proxydb = centered_pdb
         else:
             return centered_pdb
 
@@ -662,14 +662,17 @@
 
                 * 'nino3.4'
                 * 'nino1+2'
                 * 'nino3'
                 * 'nino4'
                 * 'tpi'
                 * 'wp'
+                * 'dmi'
+                * 'iobw'
+
             compress_params (dict): the paramters for compression when storing the reconstruction results to netCDF files.
             verbose (bool, optional): print verbose information. Defaults to False.
         '''
 
         compress_params = self.io_cfg(
             'compress_params', compress_params,
             default={'zlib': True},
@@ -713,20 +716,32 @@
                 if 'nino1+2' in output_indices:
                     ds['nino1+2'] = utils.geo_mean(da, lat_min=-10, lat_max=10, lon_min=np.mod(-90, 360), lon_max=np.mod(-80, 360))
                 if 'nino3' in output_indices:
                     ds['nino3'] = utils.geo_mean(da, lat_min=-5, lat_max=5, lon_min=np.mod(-150, 360), lon_max=np.mod(-90, 360))
                 if 'nino4' in output_indices:
                     ds['nino4'] = utils.geo_mean(da, lat_min=-5, lat_max=5, lon_min=np.mod(160, 360), lon_max=np.mod(-150, 360))
                 if 'wpi' in output_indices:
+                    # Western Pacific Index
                     ds['wpi'] = utils.geo_mean(da, lat_min=-10, lat_max=10, lon_min=np.mod(120, 360), lon_max=np.mod(150, 360))
                 if 'tpi' in output_indices:
+                    # Tri-Pole Index
                     v1 = utils.geo_mean(da, lat_min=25, lat_max=45, lon_min=np.mod(140, 360), lon_max=np.mod(-145, 360))
                     v2 = utils.geo_mean(da, lat_min=-10, lat_max=10, lon_min=np.mod(170, 360), lon_max=np.mod(-90, 360))
                     v3 = utils.geo_mean(da, lat_min=-50, lat_max=-15, lon_min=np.mod(150, 360), lon_max=np.mod(-160, 360))
                     ds['tpi'] = v2 - (v1 + v3)/2
+                if 'dmi' in output_indices:
+                    # Indian Ocean Dipole Mode
+                    dmiw = utils.geo_mean(da, lat_min=-10, lat_max=10, lon_min=50 ,lon_max=70)
+                    dmie = utils.geo_mean(da,lat_min=-10,lat_max=0,lon_min=90,lon_max=110)
+                    dmi = dmiw - dmie
+                    ds['dmi'] = dmi
+                if 'iobw' in output_indices:
+                    # Indian Ocean Basin Wide
+                    iobw =  utils.geo_mean(da, lat_min=-20, lat_max=20, lon_min=40 ,lon_max=100)
+                    ds['iobw'] = iobw
 
             if not output_full_ens: da = da.mean(dim='ens')
             ds[vn] = da
 
         encoding_dict = {}
         for k in self.recon_fields.keys():
             encoding_dict[k] = compress_params
@@ -1184,19 +1199,21 @@
                            lon_max=self.configs['obs_lon_max'], 
                            verbose=verbose)
 
 
         self.prep_graphem(
             recon_period=self.configs['recon_period'],  # period to reconstruct
             calib_period=self.configs['calib_period'],  # period for calibration
+            uniform_pdb=self.configs['uniform_pdb'],    # filter the proxydb to be more uniform
             verbose=verbose,
         )
 
         self.save_cfg(save_dirpath=self.configs['save_dirpath'], verbose=verbose)
 
         self.run_graphem(
             save_dirpath=self.configs['save_dirpath'],
             graph_method=self.configs['graph_method'],
             cutoff_radius=self.configs['cutoff_radius'],
-            output_indices=job.configs['output_indices'],
+            output_indices=self.configs['output_indices'],
+            sp_FF=self.configs['sp_FF'], sp_FP=self.configs['sp_FP'],
             verbose=verbose,
         )
```

### Comparing `cfr-2023.7.21/cfr/reconres.py` & `cfr-2023.7.24/cfr/reconres.py`

 * *Files identical despite different names*

### Comparing `cfr-2023.7.21/cfr/ts.py` & `cfr-2023.7.24/cfr/ts.py`

 * *Files identical despite different names*

### Comparing `cfr-2023.7.21/cfr/utils.py` & `cfr-2023.7.24/cfr/utils.py`

 * *Files identical despite different names*

### Comparing `cfr-2023.7.21/cfr/visual.py` & `cfr-2023.7.24/cfr/visual.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,17 +158,17 @@
         'peat.pollen': 'o',
     }
     markers_dict_plotly = {
         'coral.calc': 'cross',
         'coral.SrCa': 'x',
         'coral.d18O': 'circle',
         'coral.d18Osw': 'hexagon2',
-        'ice.melt': 'traingle-left',
+        'ice.melt': 'triangle-left',
         'ice.d18O': 'diamond-tall',
-        'ice.dD': 'traingle-right',
+        'ice.dD': 'triangle-right',
         'ice.d-excess': 'circle',
         'ice.isotope_diffusion': 'hexagon',
         'ice.hybrid': 'arrow-left',
         'tree.TRW': 'triangle-up',
         'tree.MXD': 'triangle-down',
         'tree.ENSO': 'triangle-up',
         'pollen.temp': 'circle',
@@ -181,17 +181,17 @@
         'bivalve.d18O': 'circle',
         'marine.TEX86': 'star',
         'marine.MgCa': 'triangle-down',
         'marine.d18O': 'circle',
         'marine.MAT': 'hexagon2',
         'marine.alkenone': 'hexagon',
         'marine.foram': 'arrow-left',
-        'marine.diatom': 'traingle-up',
+        'marine.diatom': 'triangle-up',
         'marine.dinocyst': 'triangle-right',
-        'marine.radiolaria': 'traingle-left',
+        'marine.radiolaria': 'triangle-left',
         'marine.GDGT': 'square',
         'lake.varve_thickness': 'hexagon2',
         'lake.varve_property': 'square',
         'lake.accumulation': 'triangle-down',
         'lake.chironomid': 'triangle-down',
         'lake.midge': 'triangle-right',
         'lake.TEX86': 'star',
```

### Comparing `cfr-2023.7.21/cfr.egg-info/PKG-INFO` & `cfr-2023.7.24/cfr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfr
-Version: 2023.7.21
+Version: 2023.7.24
 Summary: cfr: a Python package for Climate Field Reconstruction
 Home-page: https://github.com/fzhu2e/cfr
 Author: Feng Zhu, Julien Emile-Geay
 Author-email: fengzhu@ucar.edu, julieneg@usc.edu
 License: BSD 3-Clause
 Keywords: climate field reconstruction
 Classifier: Natural Language :: English
```

### Comparing `cfr-2023.7.21/setup.py` & `cfr-2023.7.24/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='cfr',  # required
-    version='2023.7.21',
+    version='2023.7.24',
     description='cfr: a Python package for Climate Field Reconstruction',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author='Feng Zhu, Julien Emile-Geay',
     author_email='fengzhu@ucar.edu, julieneg@usc.edu',
     url='https://github.com/fzhu2e/cfr',
     packages=find_packages(),
```

