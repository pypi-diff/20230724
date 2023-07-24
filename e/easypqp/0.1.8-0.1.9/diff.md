# Comparing `tmp/easypqp-0.1.8.tar.gz` & `tmp/easypqp-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/easypqp-0.1.8.tar", last modified: Sat Jul 18 12:40:11 2020, max compression
+gzip compressed data, was "dist/easypqp-0.1.9.tar", last modified: Mon Dec  7 11:57:41 2020, max compression
```

## Comparing `easypqp-0.1.8.tar` & `easypqp-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-18 12:40:11.300830 easypqp-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (116)     1526 2020-07-18 12:39:59.000000 easypqp-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     2579 2020-07-18 12:40:11.300830 easypqp-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1307 2020-07-18 12:39:59.000000 easypqp-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-18 12:40:11.300830 easypqp-0.1.8/easypqp/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-18 12:39:59.000000 easypqp-0.1.8/easypqp/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    27745 2020-07-18 12:39:59.000000 easypqp-0.1.8/easypqp/convert.py
--rw-r--r--   0 runner    (1001) docker     (116)    18900 2020-07-18 12:39:59.000000 easypqp-0.1.8/easypqp/library.py
--rw-r--r--   0 runner    (1001) docker     (116)     9851 2020-07-18 12:39:59.000000 easypqp-0.1.8/easypqp/main.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-18 12:40:11.300830 easypqp-0.1.8/easypqp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     2579 2020-07-18 12:40:11.000000 easypqp-0.1.8/easypqp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      298 2020-07-18 12:40:11.000000 easypqp-0.1.8/easypqp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-07-18 12:40:11.000000 easypqp-0.1.8/easypqp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       46 2020-07-18 12:40:11.000000 easypqp-0.1.8/easypqp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)      111 2020-07-18 12:40:11.000000 easypqp-0.1.8/easypqp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        8 2020-07-18 12:40:11.000000 easypqp-0.1.8/easypqp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      102 2020-07-18 12:40:11.300830 easypqp-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1761 2020-07-18 12:39:59.000000 easypqp-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 11:57:41.082623 easypqp-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (116)     1526 2020-12-07 11:57:24.000000 easypqp-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)     2579 2020-12-07 11:57:41.082623 easypqp-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1307 2020-12-07 11:57:24.000000 easypqp-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 11:57:41.082623 easypqp-0.1.9/easypqp/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-07 11:57:24.000000 easypqp-0.1.9/easypqp/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)    27494 2020-12-07 11:57:24.000000 easypqp-0.1.9/easypqp/convert.py
+-rw-r--r--   0 runner    (1001) docker     (116)    19035 2020-12-07 11:57:24.000000 easypqp-0.1.9/easypqp/library.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9851 2020-12-07 11:57:24.000000 easypqp-0.1.9/easypqp/main.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 11:57:41.082623 easypqp-0.1.9/easypqp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     2579 2020-12-07 11:57:40.000000 easypqp-0.1.9/easypqp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      298 2020-12-07 11:57:40.000000 easypqp-0.1.9/easypqp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-07 11:57:40.000000 easypqp-0.1.9/easypqp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       46 2020-12-07 11:57:40.000000 easypqp-0.1.9/easypqp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      111 2020-12-07 11:57:40.000000 easypqp-0.1.9/easypqp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        8 2020-12-07 11:57:40.000000 easypqp-0.1.9/easypqp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      102 2020-12-07 11:57:41.082623 easypqp-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1761 2020-12-07 11:57:24.000000 easypqp-0.1.9/setup.py
```

### Comparing `easypqp-0.1.8/LICENSE` & `easypqp-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `easypqp-0.1.8/PKG-INFO` & `easypqp-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easypqp
-Version: 0.1.8
+Version: 0.1.9
 Summary: EasyPQP: Simple library generation for OpenSWATH
 Home-page: https://github.com/grosenberger/easypqp
 Author: George Rosenberger
 Author-email: gr2578@cumc.columbia.edu
 License: UNKNOWN
 Description: EasyPQP: Simple library generation for OpenSWATH
         ================================================
```

### Comparing `easypqp-0.1.8/README.md` & `easypqp-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `easypqp-0.1.8/easypqp/convert.py` & `easypqp-0.1.9/easypqp/convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,17 +248,14 @@
         scores = {}
 
         parsed_peptides = []
 
         po.IdXMLFile().load(self.idxml_file, proteins, peptides)
 
         for p in peptides:
-            #search engine scores
-            scores["var_MS:1002252_Comet:XCorr"] = float(p.getHits()[0].getMetaValue('MS:1002252'))
-            scores["var_MS:1002253_Comet:DeltCn"] = float(p.getHits()[0].getMetaValue('MS:1002253'))
 
             #percolator probability
             scores["q_value"] = float(p.getHits()[0].getMetaValue('MS:1001491'))
             scores["pep"] = float(p.getHits()[0].getMetaValue('MS:1001491'))
 
             try:
                 parsed_peptides.append({**{'run_id': self.base_name,
@@ -539,15 +536,15 @@
 
 					# Losses
 					if enable_specific_losses or enable_unspecific_losses:
 						for lossfragment_ordinal in range(1,ion.size()):
 							if (ion.getResidue(lossfragment_ordinal).hasNeutralLoss()):
 								losses = ion.getResidue(lossfragment_ordinal).getLossFormulas()
 								for loss in losses:
-									loss_type = loss.toString().decode("utf-8")
+									loss_type = loss.toString()
 
 									if (enable_specific_losses and loss_type not in unspecific_losses) or (enable_unspecific_losses and loss_type in unspecific_losses):
 										fragments[fragment_type + str(fragment_ordinal) + "-" + loss_type + "^" + str(fragment_charge)] = mass - (loss.getMonoWeight() / fragment_charge)
 
 	return list(fragments.keys()), np.fromiter(fragments.values(), np.float, len(fragments))
 
 def conversion(pepxmlfile, spectralfile, unimodfile, exclude_range, max_delta_unimod, max_delta_ppm, fragment_types, fragment_charges, enable_specific_losses, enable_unspecific_losses):
```

### Comparing `easypqp-0.1.8/easypqp/library.py` & `easypqp-0.1.9/easypqp/library.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,14 +166,17 @@
 
     click.echo("Info: %s redundant PSMs identified (q-value < %s; PP threshold = %s)" % (psms.shape[0], psm_fdr_threshold, np.min(1-psms['pep'])))
 
   return psms
 
 def lowess_iso(x, y, lowess_frac):
   lwf = sm.nonparametric.lowess(y, x.ravel(), frac=lowess_frac)
+  while pd.isna(lwf[:, 1]).any():
+    lowess_frac *= 2
+    lwf = sm.nonparametric.lowess(y, x.ravel(), frac=lowess_frac)
   lwf_x = lwf[:, 0]
   ir = sklearn.isotonic.IsotonicRegression()  # make the regression strictly increasing
   lwf_y = ir.fit_transform(lwf_x, lwf[:, 1])
   mask = np.concatenate([[True], np.diff(lwf_y) != 0])  # remove non increasing points
   return interp1d(lwf_x[mask], lwf_y[mask], bounds_error=False, fill_value="extrapolate")
 
 
@@ -418,12 +421,12 @@
         global_pqp['PrecursorCharge'] = global_pqp['PrecursorCharge'].astype(int)
         replicate_pqp.append(global_pqp)
 
   # Aggregate consensus spectra
   pqp = pd.concat(replicate_pqp)
   if consensus:
     pqp_irt = pqp[['ModifiedPeptideSequence','PrecursorCharge','NormalizedRetentionTime','PrecursorIonMobility']].drop_duplicates().groupby(['ModifiedPeptideSequence','PrecursorCharge'])[['NormalizedRetentionTime','PrecursorIonMobility']].median().reset_index()
-    pqp_mass = pqp.groupby(['PrecursorMz','ProductMz','Annotation','ProteinId','GeneName','PeptideSequence','ModifiedPeptideSequence','PrecursorCharge'])['LibraryIntensity'].median().reset_index()
+    pqp_mass = pqp.groupby(['PrecursorMz','ProductMz','Annotation','ProteinId','GeneName','PeptideSequence','ModifiedPeptideSequence','PrecursorCharge'], dropna=False)['LibraryIntensity'].median().reset_index()
     pqp = pd.merge(pqp_mass,pqp_irt, on=['ModifiedPeptideSequence','PrecursorCharge'])
 
   # Write output TSV file
   pqp.to_csv(outfile, sep="\t", index=False)
```

### Comparing `easypqp-0.1.8/easypqp/main.py` & `easypqp-0.1.9/easypqp/main.py`

 * *Files identical despite different names*

### Comparing `easypqp-0.1.8/easypqp.egg-info/PKG-INFO` & `easypqp-0.1.9/easypqp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easypqp
-Version: 0.1.8
+Version: 0.1.9
 Summary: EasyPQP: Simple library generation for OpenSWATH
 Home-page: https://github.com/grosenberger/easypqp
 Author: George Rosenberger
 Author-email: gr2578@cumc.columbia.edu
 License: UNKNOWN
 Description: EasyPQP: Simple library generation for OpenSWATH
         ================================================
```

### Comparing `easypqp-0.1.8/setup.py` & `easypqp-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='easypqp',
-    version='0.1.8',
+    version='0.1.9',
     description='EasyPQP: Simple library generation for OpenSWATH',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/grosenberger/easypqp",
 	author="George Rosenberger",
 	author_email="gr2578@cumc.columbia.edu",
     classifiers=[
```

