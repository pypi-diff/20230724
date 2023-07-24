# Comparing `tmp/prodimopy-2.1.6.tar.gz` & `tmp/prodimopy-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodimopy-2.1.6.tar", last modified: Thu Apr 27 16:13:06 2023, max compression
+gzip compressed data, was "prodimopy-2.2.tar", last modified: Mon Jul 24 14:40:50 2023, max compression
```

## Comparing `prodimopy-2.1.6.tar` & `prodimopy-2.2.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxrwxr-x   0 rab      (11485) rab      (11485)        0 2023-04-27 16:13:06.973666 prodimopy-2.1.6/
--rw-rw-r--   0 rab      (11485) rab      (11485)      790 2023-01-11 15:23:54.000000 prodimopy-2.1.6/DESCRIPTION.md
--rw-rw-r--   0 rab      (11485) rab      (11485)     1069 2023-01-11 15:23:54.000000 prodimopy-2.1.6/LICENSE
--rw-rw-r--   0 rab      (11485) rab      (11485)       23 2023-03-16 13:01:01.000000 prodimopy-2.1.6/MANIFEST.in
--rw-rw-r--   0 rab      (11485) rab      (11485)     1392 2023-04-27 16:13:06.973666 prodimopy-2.1.6/PKG-INFO
--rw-rw-r--   0 rab      (11485) rab      (11485)     3002 2023-04-14 12:19:49.000000 prodimopy-2.1.6/README.md
-drwxrwxr-x   0 rab      (11485) rab      (11485)        0 2023-04-27 16:13:06.969666 prodimopy-2.1.6/prodimopy/
--rw-rw-r--   0 rab      (11485) rab      (11485)        0 2023-01-11 15:23:54.000000 prodimopy-2.1.6/prodimopy/__init__.py
-drwxrwxr-x   0 rab      (11485) rab      (11485)        0 2023-04-27 16:13:06.969666 prodimopy-2.1.6/prodimopy/chemistry/
--rw-rw-r--   0 rab      (11485) rab      (11485)        0 2023-01-11 15:23:54.000000 prodimopy-2.1.6/prodimopy/chemistry/__init__.py
--rw-rw-r--   0 rab      (11485) rab      (11485)    25757 2023-01-11 15:23:54.000000 prodimopy-2.1.6/prodimopy/chemistry/network.py
--rw-rw-r--   0 rab      (11485) rab      (11485)    30948 2023-04-27 10:53:09.000000 prodimopy-2.1.6/prodimopy/compare.py
--rw-rw-r--   0 rab      (11485) rab      (11485)    18647 2023-01-11 15:23:54.000000 prodimopy-2.1.6/prodimopy/extinction.py
--rw-rw-r--   0 rab      (11485) rab      (11485)     8251 2023-01-11 15:23:54.000000 prodimopy-2.1.6/prodimopy/grid.py
--rw-rw-r--   0 rab      (11485) rab      (11485)    36560 2023-01-11 15:23:54.000000 prodimopy-2.1.6/prodimopy/hitran.py
-drwxrwxr-x   0 rab      (11485) rab      (11485)        0 2023-04-27 16:13:06.973666 prodimopy-2.1.6/prodimopy/interface1D/
--rw-rw-r--   0 rab      (11485) rab      (11485)        0 2023-01-11 15:23:54.000000 prodimopy-2.1.6/prodimopy/interface1D/__init__.py
--rw-rw-r--   0 rab      (11485) rab      (11485)    19062 2023-01-11 15:23:54.000000 prodimopy-2.1.6/prodimopy/interface1D/infile.py
--rw-rw-r--   0 rab      (11485) rab      (11485)     8035 2023-01-11 15:23:54.000000 prodimopy-2.1.6/prodimopy/interface1D/twoppToProDiMo.py
-drwxrwxr-x   0 rab      (11485) rab      (11485)        0 2023-04-27 16:13:06.973666 prodimopy-2.1.6/prodimopy/interface2D/
--rw-rw-r--   0 rab      (11485) rab      (11485)        0 2023-01-11 15:23:54.000000 prodimopy-2.1.6/prodimopy/interface2D/__init__.py
--rw-rw-r--   0 rab      (11485) rab      (11485)     4385 2023-04-27 10:53:09.000000 prodimopy-2.1.6/prodimopy/interface2D/infile.py
--rw-rw-r--   0 rab      (11485) rab      (11485)    14741 2023-01-11 15:23:54.000000 prodimopy-2.1.6/prodimopy/movie.py
--rw-rw-r--   0 rab      (11485) rab      (11485)    91480 2023-04-27 13:48:22.000000 prodimopy-2.1.6/prodimopy/plot.py
--rw-rw-r--   0 rab      (11485) rab      (11485)    31715 2023-04-14 12:19:49.000000 prodimopy-2.1.6/prodimopy/plot_casasim.py
--rw-rw-r--   0 rab      (11485) rab      (11485)    11783 2023-01-11 15:23:54.000000 prodimopy-2.1.6/prodimopy/plot_mc.py
--rw-rw-r--   0 rab      (11485) rab      (11485)    53612 2023-04-14 12:19:49.000000 prodimopy-2.1.6/prodimopy/plot_models.py
--rw-rw-r--   0 rab      (11485) rab      (11485)    22534 2023-04-27 10:53:16.000000 prodimopy-2.1.6/prodimopy/plot_slab.py
--rw-rw-r--   0 rab      (11485) rab      (11485)   119635 2023-04-27 10:53:09.000000 prodimopy-2.1.6/prodimopy/read.py
--rw-rw-r--   0 rab      (11485) rab      (11485)    20456 2023-01-11 15:23:54.000000 prodimopy-2.1.6/prodimopy/read_casasim.py
--rw-rw-r--   0 rab      (11485) rab      (11485)     8556 2023-04-14 12:19:49.000000 prodimopy-2.1.6/prodimopy/read_mc.py
--rw-rw-r--   0 rab      (11485) rab      (11485)    88984 2023-04-27 16:00:15.000000 prodimopy-2.1.6/prodimopy/read_slab.py
--rwxrwxr-x   0 rab      (11485) rab      (11485)     2442 2023-01-11 15:23:54.000000 prodimopy-2.1.6/prodimopy/script_compare.py
--rwxrwxr-x   0 rab      (11485) rab      (11485)     2803 2023-01-11 15:23:54.000000 prodimopy-2.1.6/prodimopy/script_params.py
--rwxrwxr-x   0 rab      (11485) rab      (11485)     6430 2023-04-14 12:19:49.000000 prodimopy-2.1.6/prodimopy/script_plot.py
--rw-rw-r--   0 rab      (11485) rab      (11485)     6667 2023-01-11 15:23:54.000000 prodimopy-2.1.6/prodimopy/script_plot_models.py
--rw-rw-r--   0 rab      (11485) rab      (11485)     3331 2023-01-11 15:23:55.000000 prodimopy-2.1.6/prodimopy/utils.py
--rw-rw-r--   0 rab      (11485) rab      (11485)    22755 2023-01-11 15:23:55.000000 prodimopy-2.1.6/prodimopy/utils_casasim.py
-drwxrwxr-x   0 rab      (11485) rab      (11485)        0 2023-04-27 16:13:06.969666 prodimopy-2.1.6/prodimopy.egg-info/
--rw-rw-r--   0 rab      (11485) rab      (11485)     1392 2023-04-27 16:13:06.000000 prodimopy-2.1.6/prodimopy.egg-info/PKG-INFO
--rw-rw-r--   0 rab      (11485) rab      (11485)      981 2023-04-27 16:13:06.000000 prodimopy-2.1.6/prodimopy.egg-info/SOURCES.txt
--rw-rw-r--   0 rab      (11485) rab      (11485)        1 2023-04-27 16:13:06.000000 prodimopy-2.1.6/prodimopy.egg-info/dependency_links.txt
--rw-rw-r--   0 rab      (11485) rab      (11485)      181 2023-04-27 16:13:06.000000 prodimopy-2.1.6/prodimopy.egg-info/entry_points.txt
--rw-rw-r--   0 rab      (11485) rab      (11485)       86 2023-04-27 16:13:06.000000 prodimopy-2.1.6/prodimopy.egg-info/requires.txt
--rw-rw-r--   0 rab      (11485) rab      (11485)       10 2023-04-27 16:13:06.000000 prodimopy-2.1.6/prodimopy.egg-info/top_level.txt
--rw-rw-r--   0 rab      (11485) rab      (11485)       67 2023-04-27 16:13:06.973666 prodimopy-2.1.6/setup.cfg
--rw-rw-r--   0 rab      (11485) rab      (11485)     5519 2023-04-27 16:05:12.000000 prodimopy-2.1.6/setup.py
+drwxr-xr-x   0 work       (501) staff       (20)        0 2023-07-24 14:40:50.009188 prodimopy-2.2/
+-rw-r--r--   0 work       (501) staff       (20)      790 2023-03-30 07:05:59.000000 prodimopy-2.2/DESCRIPTION.md
+-rw-r--r--   0 work       (501) staff       (20)     1069 2023-03-30 07:05:59.000000 prodimopy-2.2/LICENSE
+-rw-r--r--   0 work       (501) staff       (20)       23 2023-04-28 23:48:28.000000 prodimopy-2.2/MANIFEST.in
+-rw-r--r--   0 work       (501) staff       (20)     1390 2023-07-24 14:40:50.009343 prodimopy-2.2/PKG-INFO
+-rw-r--r--   0 work       (501) staff       (20)     3002 2023-04-28 23:48:28.000000 prodimopy-2.2/README.md
+drwxr-xr-x   0 work       (501) staff       (20)        0 2023-07-24 14:40:50.000050 prodimopy-2.2/prodimopy/
+-rw-r--r--   0 work       (501) staff       (20)        0 2023-03-30 07:05:59.000000 prodimopy-2.2/prodimopy/__init__.py
+drwxr-xr-x   0 work       (501) staff       (20)        0 2023-07-24 14:40:50.003849 prodimopy-2.2/prodimopy/chemistry/
+-rw-r--r--   0 work       (501) staff       (20)        0 2023-03-30 07:05:59.000000 prodimopy-2.2/prodimopy/chemistry/__init__.py
+-rw-r--r--   0 work       (501) staff       (20)    25925 2023-05-27 16:54:54.000000 prodimopy-2.2/prodimopy/chemistry/network.py
+-rw-r--r--   0 work       (501) staff       (20)    31554 2023-07-13 12:33:52.000000 prodimopy-2.2/prodimopy/compare.py
+-rw-r--r--   0 work       (501) staff       (20)    18647 2023-03-30 07:05:59.000000 prodimopy-2.2/prodimopy/extinction.py
+-rw-r--r--   0 work       (501) staff       (20)     8251 2023-03-30 07:05:59.000000 prodimopy-2.2/prodimopy/grid.py
+-rw-r--r--   0 work       (501) staff       (20)    36560 2023-03-30 07:05:59.000000 prodimopy-2.2/prodimopy/hitran.py
+drwxr-xr-x   0 work       (501) staff       (20)        0 2023-07-24 14:40:50.007511 prodimopy-2.2/prodimopy/interface1D/
+-rw-r--r--   0 work       (501) staff       (20)        0 2023-03-30 07:05:59.000000 prodimopy-2.2/prodimopy/interface1D/__init__.py
+-rw-r--r--   0 work       (501) staff       (20)    19062 2023-03-30 07:05:59.000000 prodimopy-2.2/prodimopy/interface1D/infile.py
+-rw-r--r--   0 work       (501) staff       (20)     8035 2023-03-30 07:05:59.000000 prodimopy-2.2/prodimopy/interface1D/twoppToProDiMo.py
+drwxr-xr-x   0 work       (501) staff       (20)        0 2023-07-24 14:40:50.008376 prodimopy-2.2/prodimopy/interface2D/
+-rw-r--r--   0 work       (501) staff       (20)        0 2023-03-30 07:05:59.000000 prodimopy-2.2/prodimopy/interface2D/__init__.py
+-rw-r--r--   0 work       (501) staff       (20)    10986 2023-07-13 12:33:52.000000 prodimopy-2.2/prodimopy/interface2D/infile.py
+-rw-r--r--   0 work       (501) staff       (20)    14741 2023-03-30 07:05:59.000000 prodimopy-2.2/prodimopy/movie.py
+-rw-r--r--   0 work       (501) staff       (20)    93785 2023-07-13 12:33:52.000000 prodimopy-2.2/prodimopy/plot.py
+-rw-r--r--   0 work       (501) staff       (20)    31715 2023-04-28 23:48:28.000000 prodimopy-2.2/prodimopy/plot_casasim.py
+-rw-r--r--   0 work       (501) staff       (20)    11783 2023-03-30 07:05:59.000000 prodimopy-2.2/prodimopy/plot_mc.py
+-rw-r--r--   0 work       (501) staff       (20)    53940 2023-07-12 19:45:47.000000 prodimopy-2.2/prodimopy/plot_models.py
+-rw-r--r--   0 work       (501) staff       (20)    22534 2023-04-28 23:48:28.000000 prodimopy-2.2/prodimopy/plot_slab.py
+-rw-r--r--   0 work       (501) staff       (20)   124738 2023-07-13 12:33:52.000000 prodimopy-2.2/prodimopy/read.py
+-rw-r--r--   0 work       (501) staff       (20)    20456 2023-03-30 07:05:59.000000 prodimopy-2.2/prodimopy/read_casasim.py
+-rw-r--r--   0 work       (501) staff       (20)     8556 2023-04-28 23:48:28.000000 prodimopy-2.2/prodimopy/read_mc.py
+-rw-r--r--   0 work       (501) staff       (20)    89257 2023-07-24 14:30:32.000000 prodimopy-2.2/prodimopy/read_slab.py
+-rw-r--r--   0 work       (501) staff       (20)    18413 2023-07-24 14:30:32.000000 prodimopy-2.2/prodimopy/run_slab.py
+-rwxr-xr-x   0 work       (501) staff       (20)     2442 2023-03-30 07:05:59.000000 prodimopy-2.2/prodimopy/script_compare.py
+-rwxr-xr-x   0 work       (501) staff       (20)     2803 2023-03-30 07:05:59.000000 prodimopy-2.2/prodimopy/script_params.py
+-rwxr-xr-x   0 work       (501) staff       (20)     6430 2023-04-28 23:48:28.000000 prodimopy-2.2/prodimopy/script_plot.py
+-rw-r--r--   0 work       (501) staff       (20)     6667 2023-03-30 07:05:59.000000 prodimopy-2.2/prodimopy/script_plot_models.py
+-rw-r--r--   0 work       (501) staff       (20)     3331 2023-03-30 07:06:00.000000 prodimopy-2.2/prodimopy/utils.py
+-rw-r--r--   0 work       (501) staff       (20)    22755 2023-03-30 07:06:00.000000 prodimopy-2.2/prodimopy/utils_casasim.py
+drwxr-xr-x   0 work       (501) staff       (20)        0 2023-07-24 14:40:50.003100 prodimopy-2.2/prodimopy.egg-info/
+-rw-r--r--   0 work       (501) staff       (20)     1390 2023-07-24 14:40:49.000000 prodimopy-2.2/prodimopy.egg-info/PKG-INFO
+-rw-r--r--   0 work       (501) staff       (20)     1003 2023-07-24 14:40:49.000000 prodimopy-2.2/prodimopy.egg-info/SOURCES.txt
+-rw-r--r--   0 work       (501) staff       (20)        1 2023-07-24 14:40:49.000000 prodimopy-2.2/prodimopy.egg-info/dependency_links.txt
+-rw-r--r--   0 work       (501) staff       (20)      181 2023-07-24 14:40:49.000000 prodimopy-2.2/prodimopy.egg-info/entry_points.txt
+-rw-r--r--   0 work       (501) staff       (20)       86 2023-07-24 14:40:49.000000 prodimopy-2.2/prodimopy.egg-info/requires.txt
+-rw-r--r--   0 work       (501) staff       (20)       10 2023-07-24 14:40:49.000000 prodimopy-2.2/prodimopy.egg-info/top_level.txt
+-rw-r--r--   0 work       (501) staff       (20)       67 2023-07-24 14:40:50.010025 prodimopy-2.2/setup.cfg
+-rw-r--r--   0 work       (501) staff       (20)     5517 2023-07-24 11:30:15.000000 prodimopy-2.2/setup.py
```

### Comparing `prodimopy-2.1.6/DESCRIPTION.md` & `prodimopy-2.2/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `prodimopy-2.1.6/LICENSE` & `prodimopy-2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prodimopy-2.1.6/PKG-INFO` & `prodimopy-2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prodimopy
-Version: 2.1.6
+Version: 2.2
 Summary: Python tools for ProDiMo.
 Home-page: https://gitlab.astro.rug.nl/prodimo/prodimopy/
 Author: Christian Rab
 Author-email: rab@astro.rug.nl
 License: MIT License
 Keywords: astronomy astrophysics star-formation protoplanetary-disks
 Classifier: Development Status :: 4 - Beta
```

### Comparing `prodimopy-2.1.6/README.md` & `prodimopy-2.2/README.md`

 * *Files identical despite different names*

### Comparing `prodimopy-2.1.6/prodimopy/chemistry/network.py` & `prodimopy-2.2/prodimopy/chemistry/network.py`

 * *Files 0% similar despite different names*

```diff
@@ -550,72 +550,77 @@
     fr=open(filename)
     self.filename=filename
 
     lines=fr.readlines()
 
     # stupid workaround for old format
     oldformat=False
-    for line in lines:
+    try:
+      for line in lines:
 
-      if not oldformat:
-        fields=line.split()
-        # print(fields[-6])
-        try:
-          tidx=int(fields[-6])
-        except ValueError:
-          print("WARN: Try to read an older format ... let's hope it works!")
-          oldformat=True
-
-      if oldformat:
-      # now insert some spaces at the right places for the coefficients
-        line=line[:23]+" "+line[23:]
-        line=line[:53]+" "+line[53:]
-        line=line[:-43+8]+" "+line[-43+8:]
-        line=line[:-43+17]+" "+line[-43+17:]
-
-        fields=line.split()
-        tidx=int(fields[-6])
-
-      # new Reaction
-      if tidx==1:
-        reac=Reaction()
-        # new reactions, append it and fill it
-        self.reactions.append(reac)
-        reac.id=int(fields[0])
-        reac.idU=int(fields[1])
-        reac.type=fields[2]
+        if not oldformat:
+          fields=line.split()
+          try:
+            tidx=int(fields[-6])
+          except ValueError:
+            print("WARN: Try to read an older format ... let's hope it works!")
+            oldformat=True
 
         if oldformat:
-          reac.gasphase=True
+        # now insert some spaces at the right places for the coefficients
+          line=line[:23]+" "+line[23:]
+          line=line[:53]+" "+line[53:]
+          line=line[:-43+8]+" "+line[-43+8:]
+          line=line[:-43+17]+" "+line[-43+17:]
 
-          reacprod=fields[3:-6]
-        else:
-          reac.gasphase=fields[3].strip()=="T:"
-          reacprod=fields[4:-6]
+          fields=line.split()
+          tidx=int(fields[-6])
 
-        reac.coeffs[:]=[float(fields[-5]),float(fields[-4]),float(fields[-3])]
-        reac.temps[:]=[float(fields[-2]),float(fields[-1])]
+        # new Reaction
+        if tidx==1:
+          reac=Reaction()
+          # new reactions, append it and fill it
+          self.reactions.append(reac)
+          reac.id=int(fields[0])
+          reac.idU=int(fields[1])
+          reac.type=fields[2]
 
-        # print(reacprod)
-        nextisprod=False
-        for entry in reacprod:
-          if entry=="-->":
-            nextisprod=True
+          if oldformat:
+            reac.gasphase=True
 
-          elif entry=="+":
-            continue
+            reacprod=fields[3:-6]
           else:
-            if nextisprod:
-              reac.products.append(entry)
+            reac.gasphase=fields[3].strip()=="T:"
+            reacprod=fields[4:-6]
+
+          reac.coeffs[:]=[float(fields[-5]),float(fields[-4]),float(fields[-3])]
+          reac.temps[:]=[float(fields[-2]),float(fields[-1])]
+
+          # print(reacprod)
+          nextisprod=False
+          for entry in reacprod:
+            if entry=="-->":
+              nextisprod=True
+
+            elif entry=="+":
+              continue
             else:
-              reac.reactants.append(entry)
-      else:
-        reac=self.reactions[-1]
-        reac.coeffs=np.vstack((reac.coeffs,[float(fields[-5]),float(fields[-4]),float(fields[-3])]))
-        reac.temps=np.vstack((reac.temps,[float(fields[-2]),float(fields[-1])]))
+              if nextisprod:
+                reac.products.append(entry)
+              else:
+                reac.reactants.append(entry)
+        else:
+          reac=self.reactions[-1]
+          reac.coeffs=np.vstack((reac.coeffs,[float(fields[-5]),float(fields[-4]),float(fields[-3])]))
+          reac.temps=np.vstack((reac.temps,[float(fields[-2]),float(fields[-1])]))
+    except Exception as e:
+      print(line)
+      print(e)
+      fr.close()
+      raise e
 
       # print(reac)
     fr.close()
     print("Loaded ",len(self.reactions)," Reactions from ",self.filename)
 
   def _equalreaction(self,eq):
     '''
```

### Comparing `prodimopy-2.1.6/prodimopy/compare.py` & `prodimopy-2.2/prodimopy/compare.py`

 * *Files 2% similar despite different names*

```diff
@@ -669,14 +669,30 @@
 
   def compareRhog(self):
     '''
     checks the gas density
     '''
     return self.diffArray(self.m.rhog,self.mref.rhog)
 
+  def compareVelocity(self):
+    '''
+    checks the velocity structure.
+    If in one of the models velocity is None it is assumed it is an old model
+    and the comparison returns Tru
+    '''
+
+    if (self.m.velocity is None)^(self.mref.velocity is None):
+      print("WARN: Ignore velocity comparison as it does not exist in one of the models. ",end="")
+      return True,None,None
+
+    # if both are None it is also fine
+    if (self.m.velocity is None) and (self.mref.velocity is None): return True,None,None
+
+    return self.diffArray(self.m.velocity,self.mref.velocity,rtol=1.e-5)
+
   def compareRhod(self):
     '''
     checks the dust density
     '''
     return self.diffArray(self.m.rhod,self.mref.rhod)
 
   def compareD2g(self):
@@ -764,15 +780,15 @@
     '''
     Makes a fits file comparison with Mie.fits.gz
     '''
     return self.diffFitsFile("Mie.fits.gz",rtol=1.e-5)
 
   def compareFitsFileLineCubes(self):
     '''
-    Makes a fits file comparison with Mie.fits.gz
+    Makes a fits file comparison with for all line cubes (LINE_3D_)
     '''
     fcubes=glob.glob(self.m.directory+"/LINE_3D_???.fits")
 
     # FIXME: rtol is pretty high
     # FIXME: this deos not work if the other model actually has linecubes
     # e.g. it would say that it is okay
     if fcubes is not None:
```

### Comparing `prodimopy-2.1.6/prodimopy/extinction.py` & `prodimopy-2.2/prodimopy/extinction.py`

 * *Files identical despite different names*

### Comparing `prodimopy-2.1.6/prodimopy/grid.py` & `prodimopy-2.2/prodimopy/grid.py`

 * *Files identical despite different names*

### Comparing `prodimopy-2.1.6/prodimopy/hitran.py` & `prodimopy-2.2/prodimopy/hitran.py`

 * *Files identical despite different names*

### Comparing `prodimopy-2.1.6/prodimopy/interface1D/infile.py` & `prodimopy-2.2/prodimopy/interface1D/infile.py`

 * *Files identical despite different names*

### Comparing `prodimopy-2.1.6/prodimopy/interface1D/twoppToProDiMo.py` & `prodimopy-2.2/prodimopy/interface1D/twoppToProDiMo.py`

 * *Files identical despite different names*

### Comparing `prodimopy-2.1.6/prodimopy/movie.py` & `prodimopy-2.2/prodimopy/movie.py`

 * *Files identical despite different names*

### Comparing `prodimopy-2.1.6/prodimopy/plot.py` & `prodimopy-2.2/prodimopy/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import division
 from __future__ import print_function
 
+import collections
 import copy
 import math
 
 from matplotlib.ticker import MaxNLocator
 from scipy.interpolate import interp1d
 
 import astropy.units as u
@@ -1918,23 +1919,26 @@
     ax.set_ylabel(r"$\mathrm{\nu F_{\nu}\,[erg\,cm^{-2}\,s^{-1}]}$")
 
     self._dokwargs(ax,**kwargs)
 
     return self._closefig(fig)
 
   def plot_sed(self,model,plot_starSpec=True,sedObs=None,unit="erg",reddening=False,
-               ax=None,**kwargs):
+               incidx=0,ax=None,**kwargs):
     '''
     Plots the seds and the StarSpectrum
     '''
     print("PLOT: plot_sed ...")
     fig,ax=self._initfig(ax,**kwargs)
 
     xmin=0.1
     if model.sed==None: return
+    # to be sure we have the right inclination
+    model.sedinc(iinc=incidx)
+
     # only use every 5 element to speed up plotting
     x=model.sed.lam
     if unit=="W":
       y=model.sed.nuFnuW
     elif unit=="Jy":
       y=model.sed.fnuJy
     else:
@@ -2352,16 +2356,16 @@
                 verticalalignment='bottom',fontsize=lineLabelsFontsize,
                 transform=ax.transAxes,color=boxcolors[ibox],
                 bbox=dict(boxstyle='square,pad=0.1',fc='white',ec='none'))
         ibox+=1
 
     return self._closefig(fig)
 
-  def plot_lineprofile(self,model=None,wl=None,ident=None,lineObj=None,linetxt=None,lineObs=None,
-                       unit="Jy",normalized=False,convolved=False,style=None,ax=None,**kwargs):
+  def plot_lineprofile(self,model=None,wl=None,ident=None,lineObj=None,linetxt=None,lineObs=None,incidx=0,
+                       unit="Jy",normalized=False,convolved=False,style=None,color=None,ax=None,**kwargs):
     '''
     Plots the line profile for the given line (id wavelength and optionally the line ident)
 
     Parameters
     ----------
     model : :class:`~prodimopy.read.Data_ProDiMo`
       the model data. Only required if wl,ident and or lineObs are passed.
@@ -2379,61 +2383,107 @@
     linetxt : str
       A string the is used as the label for the line
 
     lineObs : array_like(ndim=1)
       list of :class:`prodimopy.read.DataLineObs` objects. Must be consistent with the list of
       lines from the line radiative transfer.
 
+    incidx : int or array_like(ndim=1)
+      which inclination (index) should be used for plotting (0 is the first one and default).
+      If it is a single value only the profile for that inclination index is plotted.
+
+      If it is an array of values all profiles for that chosen inclinations are plotted.
+      If `normalized=True` the profiles will be normalized to the first one, in that case.
+      If `incidx=[]` profiles for all inclinations will be plotted.
+
+      If lineObj is passed only one inclination (the one set in that obj) will be plotted.
+
+    unit : str
+      In what unit should the line flux be plotted. Current options
+      `unit="Jy"` (default) and `unit="ErgAng'
+
     normalized : boolean
-      if `True` normalize the profile to the peak flux of each line
+      if `True` normalize the profile to the peak flux
 
     convolved : boolean
       if `True` plot the convolved profile.
 
+    color : str
+      the color for the plotted profile.
+
     style : str
       if style is `step` the profile is plotted as a step function assuming
       the values are the mid point of the bin.
 
     '''
     print("PLOT: plot_line_profile ...")
     fig,ax=self._initfig(ax,**kwargs)
 
+    # first need a line object to properly init incidx.
+    # if lineObj is passed incidx is ignored
     if lineObj is None:
       line=model.getLine(wl,ident=ident)
       if line==None:
-        print("WARN: line "+str(ident)+" at "+str(line.wl)+" micron not found")
-    else:
-      line=lineObj
+          print("WARN: line "+str(ident)+" at "+str(line.wl)+" micron not found")
 
-    # text for the title
+      if not isinstance(incidx,(collections.abc.Sequence,np.ndarray)):
+        incidx=[incidx]
+      # just for convenience if it is an empty array take all the inclinations
+      elif len(incidx)==0:
+        # need the line for that
+        incidx=np.arange(len(line._inclinations))
+    else:
+      # make sure that in that case only one inclinations is done
+      incidx=[0]
+
+    # ignore the color attribute in that case.
+    # could also use and array of colors to enable to user to chose, but
+    # for now color is only used if a single profile is used.
+    if len(incidx)>1: color=None
+
+    # plot it for all selected inclinations
+    for i,iinc in enumerate(incidx):
+
+      if lineObj is None:
+        line=model.getLine(wl,ident=ident,incidx=iinc)
+        if line==None:
+          print("WARN: line "+str(ident)+" at "+str(line.wl)+" micron not found")
+      else:
+        line=lineObj
 
-    # FIXME: ist not up to date anymore with the unit treatment in lineprofile
-    x=line.profile.velo
+      incstr=r"$i="+"{:3.1f}".format(line.inclination)+r"^\degree$"
 
-    if convolved:
-      y=line.profile.flux_conv-line.profile.flux_conv[0]
-    else:
-      y=line.profile.flux-line.profile.flux[0]
+      # text for the title
 
-    if normalized:
-      y=y/np.max(y)
+      # FIXME: ist not up to date anymore with the unit treatment in lineprofile
+      x=line.profile.velo
 
-    if linetxt is None:
-      if ident is not None:
-        linetxt=ident
+      if convolved:
+        y=line.profile.flux_conv-line.profile.flux_conv[0]
       else:
-        linetxt=line.species
-      linetxt=linetxt+"@"+"{:.2f}".format(line.wl)+r" $\mathrm{\mu m}$"
+        y=line.profile.flux-line.profile.flux[0]
 
-    if style=="step":
-      ax.sep(x,y,marker=None,label=linetxt,where="mid")
-    else:
-      ax.plot(x,y,marker=None,label=linetxt)
+      if normalized:
+        if i==0:  # always normalize to the first inclination
+          norm=np.max(y)
+        y=y/norm
+
+      if linetxt is None:
+        if ident is not None:
+          linetxt=ident
+        else:
+          linetxt=line.species
+        linetxt=linetxt+"@"+"{:.2f}".format(line.wl)+r" $\mathrm{\mu m}$"
 
-    # plot the line profile if it exists
+      if style=="step":
+        ax.step(x,y,marker=None,label=incstr,where="mid",color=color)
+      else:
+        ax.plot(x,y,marker=None,label=incstr,color=color)
+
+    # plot the observed line profile if it exists
     if lineObs is not None:
       # FIXME: this is not very nice
       # make a warning if lineObs and line Data are not consistent
       # it could be that they are for one model
       lineIdx=model._getLineIdx(wl,ident=ident)
 
       line=lineObs[lineIdx]
@@ -2454,14 +2504,20 @@
       if line.profile.flux_unit=="ErgAng":
         ax.set_ylabel(r"$\mathrm{flux\,[erg s^{-1}cm^{-2}\AA^{-1}]}$")
       else:
         ax.set_ylabel(r"$\mathrm{flux\,[Jy]}$")
 
     ax.set_xlabel("velocity [km/s]")
 
+    ax.text(0.03,0.955,linetxt,fontsize=7.0,
+          horizontalalignment='left',
+          verticalalignment='top',
+          transform=ax.transAxes,color=self.pcolors["gray"],
+          bbox=dict(boxstyle='round',facecolor='white',edgecolor="0"))
+
     self._dokwargs(ax,**kwargs)
     self._legend(ax,**kwargs)
 
     return self._closefig(fig)
 
   def plot_lines(self,model,lineIdents,useLineEstimate=True,jansky=False,
                  showBoxes=True,lineObs=None,lineObsLabel="Obs.",peakFlux=False,
```

### Comparing `prodimopy-2.1.6/prodimopy/plot_casasim.py` & `prodimopy-2.2/prodimopy/plot_casasim.py`

 * *Files identical despite different names*

### Comparing `prodimopy-2.1.6/prodimopy/plot_mc.py` & `prodimopy-2.2/prodimopy/plot_mc.py`

 * *Files identical despite different names*

### Comparing `prodimopy-2.1.6/prodimopy/plot_models.py` & `prodimopy-2.2/prodimopy/plot_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from __future__ import division
 from __future__ import print_function
 
 from math import pi
-import prodimopy.extinction
-import prodimopy.plot
 
 from matplotlib import lines
 from matplotlib import patches
 
 import astropy.constants as const
 import astropy.units as u
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import matplotlib.ticker as plticker
 import numpy as np
+import prodimopy.extinction
+import prodimopy.plot
 
 
 # has to be this way because of circular imports
 class PlotModels(object):
 
   def __init__(self,pdf,
                colors=None,
@@ -1224,15 +1224,15 @@
 
     sedObsModels : boolean
       If True use the :class:`~prodimopy.read.DataContinuumObs` object from
       each model individually. So for each model the provided observations are plotted.
 
     unit : str
       In which unit the SED should be plotted.
-      Allowed values: `erg` [erg/s/cm^2], `W` [W/m^2], `Jy`.
+      Allowed values: `erg` [erg/s/cm^2], `W` [W/m^2], `Jy`, `mJy`.
 
     reddening : boolean
       If True also apply the reddening of the SED using the given A_V value from the
       provided observational data.
 
     '''
     print("PLOT: plot_sed ...")
@@ -1249,14 +1249,17 @@
       # only use every 5 element to speed up plotting
       x=model.sed.lam
 
       if unit=="W":
         y=model.sed.nuFnuW
       elif unit=="Jy":
         y=model.sed.fnuJy
+      elif unit=="mJy":
+        y=model.sed.fnuJy*1000.0
+        print("mJy")
       else:
         y=model.sed.nu*model.sed.fnuErg
 
       if reddening is True and model.sedObs is not None and model.sedObs.A_V is not None:
         # idx validity of extinction function
         ist=np.argmin(np.abs(x-0.0912))
         ien=np.argmin(np.abs(x-6.0))
@@ -1274,18 +1277,19 @@
 
         xStar=model.starSpec.lam[0::10]
         yStar=(model.starSpec.nu*model.starSpec.Inu)[0::10]
         yStar=yStar*(r**2.0*pi*dist**(-2.0))
 
         if unit=="W":
           yStar=(yStar*u.erg/(u.s*u.cm**2)).to(u.Watt/u.m**2).value
-        elif unit=="Jy":
+        elif unit=="Jy" or unit=="mJy":
           yStar=(model.starSpec.Inu)[0::10]
           yStar=yStar*(r**2.0*pi*dist**(-2.0))
           yStar=(yStar*u.erg/(u.s*u.cm**2*u.Hz)).to(u.Jy).value
+          if unit=="mJy": yStar=yStar*1000.0
 
         ax.plot(xStar,yStar,self.styles[iplot],color=colsed,linewidth=0.5*lwsed,zorder=-1,linestyle="--")
 
         if max(yStar)>ymax: ymax=max(yStar)
 
 #        ax.plot(xStar, yStar, self.styles[iplot], marker="*",ms=0.5,markeredgecolor=colsed,
 #                color=colsed,linewidth=0.5*lwsed)
@@ -1308,14 +1312,17 @@
 
           if unit=="W":
             ysedObs=plSedObs.nu*((plSedObs.fnuJy*u.Jy).si.value)
             ysedObsErr=plSedObs.nu*((sedObs.fnuJyErr*u.Jy).si.value)
           elif unit=="Jy":
             ysedObs=plSedObs.fnuJy
             ysedObsErr=plSedObs.fnuJyErr
+          elif unit=="mJy":
+            ysedObs=plSedObs.fnuJy*1000
+            ysedObsErr=plSedObs.fnuJyErr*1000
 
           ax.errorbar(xsedObs[okidx],ysedObs[okidx],
                       yerr=ysedObsErr[okidx],markeredgecolor="0.3",
                     linestyle="",fmt="o",color=sedcolor,ms=2,linewidth=1.0,
                     markeredgewidth=0.5,zorder=1000,ecolor='0.3')
           # nokidx=np.where(plSedObs.flag!="ok")
           # ax.plot(xsedObs[nokidx],ysedObs[nokidx],linestyle="",
@@ -1360,14 +1367,16 @@
     ax.semilogx()
     ax.semilogy()
     ax.set_xlabel(r"wavelength [$\mu$m]")
     if unit=="W":
       ax.set_ylabel(r"$\mathrm{\lambda F_{\lambda}\,[W\,m^{-2}]}$")
     elif unit=="Jy":
       ax.set_ylabel(r"$\mathrm{flux\,[Jy]}$")
+    elif unit=="mJy":
+      ax.set_ylabel(r"$\mathrm{flux\,[mJy]}$")
     else:
       ax.set_ylabel(r"$\mathrm{\nu F_{\nu}\,[erg\,cm^{-2}\,s^{-1}]}$")
 
     self._dokwargs(ax,**kwargs)
 
     self._legend(ax,**kwargs)
```

### Comparing `prodimopy-2.1.6/prodimopy/plot_slab.py` & `prodimopy-2.2/prodimopy/plot_slab.py`

 * *Files identical despite different names*

### Comparing `prodimopy-2.1.6/prodimopy/read.py` & `prodimopy-2.2/prodimopy/read.py`

 * *Files 4% similar despite different names*

```diff
@@ -213,14 +213,19 @@
     `UNIT:` |ergcm^-3|, `DIMS:` (nx,nz)
     """
     self.soundspeed=None
     """ array_like(float,ndim=2) :
     The isothermal sound speed.
     `UNIT:` |kms^-1|, `DIMS:` (nx,nz)
     """
+    self.velocity=None
+    """ array_like(float,ndim=2) :
+    The velocity field (vector) given as vx,vy,vz
+    `UNIT:` |kms^-1|, `DIMS:` (nx,nz,2)
+    """
     self.damean=None
     """ array_like(float,ndim=2) :
     The mean dust particle radius. Is defined as <a3>**(1/3)
     `UNIT:` micron, `DIMS:` (nx,nz)
     """
     self.da2mean=None
     """ array_like(float,ndim=2) :
@@ -231,15 +236,15 @@
     """ array_like(int,ndim=2) :
     The number of ice layers on the dust grains.
     `UNIT:` dimensionless, `DIMS:` (nx,nz)
     """
     self.Hx=None
     """ array_like(float,ndim=2) :
     The X-ray energy deposition rate per hydrogen nuclei
-    `UNIT:` erg <H>\ :sup:`-1`, `DIMS:` (nx,nz)
+    `UNIT:` erg <H>\\ :sup:`-1`, `DIMS:` (nx,nz)
     """
     self.zetaX=None
     """ array_like(float,ndim=2) :
     X-ray ionisation rate per hydrogen nuclei.
     `UNIT:` |s^-1|, `DIMS:` (nx,nz)
     """
     self.zetaCR=None  #
@@ -402,18 +407,19 @@
     """
     self.lines=None
     """ array_like(:class:`prodimopy.read.DataLine`) :
     Alle the spectral lines from line_flux.out (proper Linetransfer).
     Each spectral line in line_flux.out corresponds to
     one :class:`prodimopy.read.DataLine` object
     """
-    self.sed=None  # the spectral energy distribution (from proper ray tracing)
+    self._sed=None  # the spectral energy distribution (from proper ray tracing)
     """ :class:`prodimopy.read.DataSED` :
     The Spectral Energy Distribution for the model (SED) as calculated in the
-    radiative transfer with ray tracing.
+    radiative transfer with ray tracing. Can only be accessed via getter setter
+    to deal with inclinations
     see :class:`prodimopy.read.DataSED` for details.
     """
     self.contImages=None
     """ :class:`prodimopy.read.DataContinuumImages` :
     Reads the continuum images data (image.out) if available.
     The full images are only read if requested for a particular wavelength
     see :class:`prodimopy.read.DataContinuumImages` for details.
@@ -480,14 +486,45 @@
     self._sdg=None
     self._sdd=None
     self._vol=None
     self._cdnmol=None
     self._rcdnmol=None
     self._chemnet=None
 
+  def sedinc(self,iinc=0):
+    '''
+    Get the sed for a certain inclination
+    '''
+    # just for security
+
+    nincs=len(self._sed._inclinations)
+    if nincs==1:
+      self._sed._DataSED__incidx=0
+    elif iinc>=nincs:
+      self._sed._DataSED__incidx=nincs-1
+    else:
+      self._sed._DataSED__incidx=iinc
+    return self._sed
+
+  @property
+  def sed(self):
+    '''
+    not sure if this is the best solution, but need a getter it seems
+    return the current one with inclination
+    '''
+    # self._sed._DataSED__incidx=0
+    return self._sed
+
+  @sed.setter
+  def sed(self,value):
+    '''
+    Get the sed for a certain inclination
+    '''
+    self._sed=value
+
   @property
   def nmol(self):
     if self._nmol_cache is not None:
       self._nmol=np.array(self._nmol_cache,dtype=float)
       # remove the cache now
       self._nmol_cache=None
     return self._nmol
@@ -630,39 +667,53 @@
 
       if (abs(wls[idx]-wl)/wl)>0.01:
         print("WARN: No line found within 1% of the given wavelengeth:",wl)
         return None
       else:
         return idx
 
-  def getLine(self,wl,ident=None):
+  def getLine(self,wl,ident=None,incidx=0):
     '''
     Returns the spectral line closest to the given wavelentgh.
 
     Parameters
     ----------
+
     wl : float
       the wavelength which is used for the search. `UNIT:` micron.
+
     ident : string, optional
       A line identification string which should also be considered for the
       search. (default: `None`)
 
+    incidx : int
+      select the inclination for the line. (default: 0) . 0 means
+      the first one. If only one inclination exists always this one will be used
+      (i.e. the vaue of incidx is ignored).
+
+
     Returns
     -------
     :class:`prodimopy.read.DataLine`
       Returns `None` if no lines are included in the model.
 
     '''
 
     idx=self._getLineIdx(wl,ident=ident)
 
     if idx is None:
       return None
     else:
-      return self.lines[idx]
+      line=self.lines[idx]
+      if len(line._inclinations)==1:
+        line._DataLine__incidx=0
+      else:
+        # only here I want to really set it
+        line._DataLine__incidx=incidx
+      return line
 
   def gen_specFromLineEstimates(self,wlrange=[10,15],ident=None,specR=3000,
                                 unit="W",contOnly=False,noCont=False):
     '''
     Generates a "Spectrum" from the line estimates results of ProDiMo and
     convolves it to the given spectral resolution.
     If the SED was also calculated the line fluxes will be added to the continuum,
@@ -1585,43 +1636,78 @@
     """ string :
     The chemical species of the line. Identical to ident.
     """
     self.ident=""
     """ string :
     The identification of the line (i.e. as given in `LineTransferList.in`)
     """
-    self.flux=0.0
-    """ float:
-    The integrated line flux. UNIT: `W/m^2`
-    """
-    self.fcont=0.0
-    """ float:
-    The continuum flux at the line position. UNIT: Jy
-    """
-    self.profile=None
-    """ :class:`prodimopy.read.DataLineProfile` :
-    The line profile for this particular line.
-    """
     self.distance=None
     """ float :
     The distance use for the line calculations. UNIT: pc
     """
-    self.inclination=None
+    # self.flux
+    """ float :
+    The integrated line flux for the current inc. UNIT: `W/m^2`
+    """
+    # self.fcont
+    """ float :
+    The continuum flux at the line position for the current inc. UNIT: Jy
+    """
+    # self.profile
+    """ :class:`prodimopy.read.DataLineProfile` :
+    The line profile for this particular line and for the current inc.
+    """
+    # self.inclination
     """ float :
     The inclination use for the line calculations. UNIT: deg
     """
+    self._fluxs=list()
+    """ array_like(float,ndim=1) :
+    The integrated line flux. UNIT: `W/m^2`
+    """
+    self._fconts=list()
+    """ array_like(float,ndim=1) :
+    The continuum flux at the line position. UNIT: Jy
+    """
+    self._profiles=list()
+    """ array_like(:class:`prodimopy.read.DataLineProfile`,ndim=1): :
+    The line profile for this particular line for each inclination.
+    """
+    self._inclinations=list()
+    """ array_like(float,ndim=1) :
+    The list of inclinations to use for the line calculations. UNIT: deg
+    """
+    self.__incidx=0  # which inclination to use
+
+  @property
+  def flux(self):
+    return self._fluxs[self.__incidx]
+
+  @property
+  def fcont(self):
+    return self._fcont[self.__incidx]
+
+  @property
+  def profile(self):
+    return self._profiles[self.__incidx]
+
+  @property
+  def inclination(self):
+    return self._inclinations[self.__incidx]
 
   def __str__(self):
-    text=(self.species+"/"+
+    text=(self.ident+"/"+
           self.prodimoInf+"/"+
-          self.ident+"/"+
           str(self.wl)+"/"+
           str(self.frequency)+"/"+
-          str(self.flux)+"/"+
-          str(self.fcont))
+          str(self.distance)+"/"+"\n")
+
+    for i,inc in enumerate(self._inclinations):
+      text=text+str(inc)+"/"+str(self._fluxs[i])+"/"+str(self._fconts[i])+"\n"
+
     return text
 
   @property
   def flux_Jy(self):
     '''
     The flux of the line in  Jansky km |s^-1|.
     '''
@@ -1646,14 +1732,25 @@
   @property
   def luminosityWatt(self):
     '''
     Returns the line luminosity in Watt
     '''
     return (4.0*math.pi*(self.distance*u.pc).to(u.m)**2*self.flux*u.Watt/u.m**2).value
 
+  def convolve(self,R):
+    '''
+    Convolves all the profiles (for each inclination) for this lines.
+
+    simply calls :func:`~prodimopy.read.DataLineProfile.convovle`
+
+    '''
+
+    for i in range(len(self._inclinations)):
+      self._profiles[i].convolve(R)
+
 
 class DataLineObs(DataLine):
   '''
   Holds the observational data for one line.
   '''
 
   def __init__(self,flux,flux_err,fwhm,fwhm_err,flag):
@@ -2084,34 +2181,75 @@
 class DataSED(object):
   '''
   Holds the data for the Spectral Energy Distribution (SED).
 
   TODO: documentation for the fields.
   '''
 
-  def __init__(self,nlam,distance,inclination):
+  def __init__(self,nlam,distance):
     self.nlam=nlam
     self.distance=distance
-    self.inclination=inclination
+    self.lam=np.zeros(shape=(nlam))
+    self.nu=np.zeros(shape=(nlam))
+    # the analysis data
+    self.sedAna=None
 
+    # Quantitites that depend on inclination
+    # self.fnuErg=np.zeros(shape=(nlam))
+    # self.nuFnuW=np.zeros(shape=(nlam))
+    # self.fnuJy=np.zeros(shape=(nlam))
+    # self.inclination=inclination
     # the bolometric luminosity will be calculated by integrating over the whole
     # frequency range, considering also the distance)
     # units are Solar luminosities
-    self.Lbol=None
+    # self.Lbol=None
     # is also calculated in read_sed
-    self.Tbol=None
-    self.lam=np.zeros(shape=(nlam))
-    self.nu=np.zeros(shape=(nlam))
-    self.fnuErg=np.zeros(shape=(nlam))
-    self.nuFnuW=np.zeros(shape=(nlam))
-    self.fnuJy=np.zeros(shape=(nlam))
-    # self.nuFnu = np.zeros(shape=(nlam))
+    # self.Tbol=None
 
-    # the analysis data
-    self.sedAna=None
+    # the quantities that hold the data for all inclinations
+    self._fnuErgs=list()
+    self._nuFnuWs=list()
+    self._fnuJys=list()
+    self._inclinations=list()
+    self._Lbols=list()
+    self._Tbols=list()
+    self.__incidx=0  # which inclination to use
+
+  def __str__(self):
+    text=(str(self.nlam)+"/"+
+          str(self.inclination)+"/"+
+          str(self.distance)+"/"+"\n")
+
+    text=text+str(self._inclinations)
+
+    return text
+
+  @property
+  def fnuErg(self):
+    return self._fnuErgs[self.__incidx]
+
+  @property
+  def nuFnuW(self):
+    return self._nuFnuWs[self.__incidx]
+
+  @property
+  def fnuJy(self):
+    return self._fnuJys[self.__incidx]
+
+  @property
+  def inclination(self):
+    return self._inclinations[self.__incidx]
+
+  @property
+  def Lbol(self):
+    return self._Lbols[self.__incidx]
+
+  @property
+  def Tbol(self):
+    return self._Tbols[self.__incidx]
 
   def setLbolTbol(self):
     """
     Calculates the bolometric temperature and lumionsity for the given
     values of the SED.
 
     quite approximate at the moment.
@@ -2123,21 +2261,21 @@
       # calculate Tbol see Dunham 2008 Equation 6
     # check what is here the proper value
     # in particular Tbol is very sensitive to this value
     # Lbol does not seem to change much (e.g. if 0.1 is used instead)
     # for the moment exclude the shortest wavelength as these is most likely scattering
     mask=self.lam>0.2
 
-    self.Lbol=np.trapz(self.fnuErg[mask],x=self.nu[mask])*-1.0
-    self.Lbol=self.Lbol*4.0*math.pi*(((self.distance*u.pc).to(u.cm)).value)**2
-    self.Lbol=self.Lbol/(const.L_sun.cgs).value
+    self._Lbols[self.__incidx]=np.trapz(self.fnuErg[mask],x=self.nu[mask])*-1.0
+    self._Lbols[self.__incidx]=self.Lbol*4.0*math.pi*(((self.distance*u.pc).to(u.cm)).value)**2
+    self._Lbols[self.__incidx]=self.Lbol/(const.L_sun.cgs).value
 
     # print(np.trapz((sed.nu*sed.fnuErg),x=sed.nu))
     # print(np.trapz(sed.fnuErg,x=sed.nu))
-    self.Tbol=1.25e-11*np.trapz((self.nu[mask]*self.fnuErg[mask]),x=self.nu[mask])/np.trapz(self.fnuErg[mask],x=self.nu[mask])
+    self._Tbols[self.__incidx]=1.25e-11*np.trapz((self.nu[mask]*self.fnuErg[mask]),x=self.nu[mask])/np.trapz(self.fnuErg[mask],x=self.nu[mask])
 
 
 class DataSEDAna(object):
   '''
   Holds the analysis data for the Spectral Energy Distribution (SEDana.out).
   '''
 
@@ -2531,14 +2669,15 @@
   data.chi=np.zeros(shape=(data.nx,data.nz))
   data.chiRT=np.zeros(shape=(data.nx,data.nz))
   data.kappaRoss=np.zeros(shape=(data.nx,data.nz))
   data.zetaCR=np.zeros(shape=(data.nx,data.nz))
   data.zetaSTCR=np.zeros(shape=(data.nx,data.nz))
   data.da2mean=np.zeros(shape=(data.nx,data.nz))
   data.dNlayers=np.zeros(shape=(data.nx,data.nz))
+  data.velocity=np.zeros(shape=(data.nx,data.nz,3))
 
   data.heat_names=list()
   data.cool_names=list()
   data.rateH2form=np.zeros(shape=(data.nx,data.nz))
   data.rateH2diss=np.zeros(shape=(data.nx,data.nz,3))
 
   # init the caches, to avoid conversion to float if not necessary
@@ -2667,19 +2806,27 @@
       data.tauX1[ix,zidx]=fields[iAJJ+6]
       data.tauX5[ix,zidx]=fields[iAJJ+7]
       data.tauX10[ix,zidx]=fields[iAJJ+8]
       data.zetaX[ix,zidx]=fields[iAJJ+9]
       data.rateH2form[ix,zidx]=fields[iAJJ+10]
       data.rateH2diss[ix,zidx,:]=fields[iAJJ+11:iAJJ+11+3]
       data.zetaCR[ix,zidx]=fields[iAJJ+16]
-      if len(fields)>(iAJJ+17): data.zetaSTCR[ix,zidx]=fields[iAJJ+17]
-      if len(fields)>(iAJJ+18):
-        data.da2mean[ix,zidx]=fields[iAJJ+18]
-        data.dNlayers[ix,zidx]=fields[iAJJ+19]
-      # TODO: add a2mean and Nlayers for reading
+      if len(fields)>(iAJJ+17):
+        data.zetaSTCR[ix,zidx]=fields[iAJJ+17]
+        if len(fields)>(iAJJ+18):
+          data.da2mean[ix,zidx]=fields[iAJJ+18]
+          data.dNlayers[ix,zidx]=fields[iAJJ+19]
+          if len(fields)>(iAJJ+20):
+            data.velocity[ix,zidx,:]=fields[iAJJ+20:iAJJ+23]
+          else:
+            data.velocity=None  # for backward compatibilit, as it is a new field
+        else:
+          data.velocity=None  # for backward compatibilit, as it is a new field
+          data.da2mean=None
+          data.dNlayers=None
 
       i=i+1
 
   # endLoop=timer()
 
   # derived quantitites
   data.rhod=data.rhog*data.d2g
@@ -2976,15 +3123,15 @@
     rInfo=DataLineEstimateRInfo(ix-1,iz-1,Fcolumn,tauLine,tauDust,z15,z85,ztauD1,Ncol)
     lineEstimate.rInfo.append(rInfo)
 
   f.close()
 
 
 def  read_linefluxes(directory,filename="line_flux.out",tarfile=None):
-  """ Reads the line fluxes output.
+  """ Reads the line fluxes output. Can deal with multiple inclinations.
 
   Parameters
   ----------
   directory : str
     the model directory.
 
   filename : str
@@ -2998,69 +3145,90 @@
   f,dummy=_getfile(filename,directory,tarfile)
   if f is None: return None
 
   records=f.readlines()
   f.close()
 
   dist=float(records[0].split("=")[1])
-  incl=float(records[1].split("=")[1])
   nlines=int(records[2].split("=")[1])
   nvelo=int(records[3].split("=")[1])
 
-  # number of records in the file
-  nrecords=len(records)
-  # print dist,incl,nlines,nvelo,nrecords
-
   lines=list()
 
-  # loop over all lines
+  # determine if there are multiple inclinations
+  # likely very slow
+  ninc=sum('inclination[degree]' in s for s in records)
+  # this might be faster, but also a bit dirtz
+  # nrecords=len(records)
+  # nlinesinc=4+nlines*(5+nvelo)+2
+  # print(nrecords,nlinesinc,(nrecords+2)/nlinesinc)
+
   pos=5
-  for i in range(nlines):
-    # read the data for one line
-    line=DataLine()
-    rec=records[pos]
-    try:
-      line.species=(rec[10:20]).strip()
-      line.ident=line.species
-      line.prodimoInf=rec[21:36].strip()
-      line.wl=float(rec[43:54].strip())  # *u.um
-      line.frequency=float(rec[63:76].strip())  # *u.GHz
-    except:
-      # print("read_linefluxes: try new format")
-      line.species=(rec[10:20]).strip()
-      line.ident=line.species
-      line.prodimoInf=rec[21:47].strip()
-      line.wl=float(rec[48:64].strip())  # *u.um
-      line.frequency=float(rec[74:90].strip())  # *u.GHz
-
-    rec=records[pos+1]
-    line.flux=float(rec.split("=")[1].strip())  # *u.Watt/u.m**2
-
-    rec=records[pos+2]
-    line.fcont=float(rec.split("=")[1].strip())  # *u.Jansky
-
-    # simply store inclination and distance for each line
-    line.distance=dist
-    line.inclination=incl
-
-    # one line in the profile is for the continuum
-    line.profile=DataLineProfile(nvelo-1,restfrequency=line.frequency)
-
-    for j in range(nvelo-1):
-      # skip the header line and the first line (continuum)?
-      fields=records[pos+5+j].split()
-      line.profile.velo[j]=float(fields[0])  # *u.km/u.s
-      line.profile.flux[j]=float(fields[1])  # *u.Jansky
-      if (len(fields)>2):
-        line.profile.flux_conv[j]=float(fields[2])  # *u.Jansky
-      if (len(fields)>3):
-        line.profile.flux_dust[j]=float(fields[3])  # *u.Jansky
 
-    lines.append(line)
-    pos+=(nvelo+5)
+  # loop for all inclinations
+  for iinc in range(ninc):
+    # print("start",iinc,pos,records[pos])
+    incl=float(records[pos-4].split("=")[1])
+    # print(incl)
+    # print()
+    # loop over all lines
+    for i in range(nlines):
+      # read the data for one line this the same data for inclinations
+
+      if iinc==0:
+        line=DataLine()
+        rec=records[pos]
+        try:
+          line.species=(rec[10:20]).strip()
+          line.ident=line.species
+          line.prodimoInf=rec[21:36].strip()
+          line.wl=float(rec[43:54].strip())  # *u.um
+          line.frequency=float(rec[63:76].strip())  # *u.GHz
+        except:
+          # print("read_linefluxes: try new format")
+          line.species=(rec[10:20]).strip()
+          line.ident=line.species
+          line.prodimoInf=rec[21:41].strip()
+          line.wl=float(rec[48:64].strip())  # *u.um
+          line.frequency=float(rec[74:90].strip())  # *u.GHz
+        line.distance=dist
+      else:
+        # get the line the was already initialises
+        line=lines[i]
+
+      # thisis data the changes for each inclination
+      rec=records[pos+1]
+      line._fluxs.append(float(rec.split("=")[1].strip()))  # *u.Watt/u.m**2
+
+      rec=records[pos+2]
+      line._fconts.append(float(rec.split("=")[1].strip()))  # *u.Jansky
+
+      # simply store inclination and distance for each line
+
+      line._inclinations.append(incl)
+
+      # one line in the profile is for the continuum
+      profile=DataLineProfile(nvelo-1,restfrequency=line.frequency)
+
+      for j in range(nvelo-1):
+        # skip the header line and the first line (continuum)?
+        fields=records[pos+5+j].split()
+        profile.velo[j]=float(fields[0])  # *u.km/u.s
+        profile.flux[j]=float(fields[1])  # *u.Jansky
+        if (len(fields)>2):
+          profile.flux_conv[j]=float(fields[2])  # *u.Jansky
+        if (len(fields)>3):
+          profile.flux_dust[j]=float(fields[3])  # *u.Jansky
+      line._profiles.append(profile)
+
+      # don't add the object again
+      if iinc==0: lines.append(line)
+
+      pos+=(nvelo+5)
+    pos+=6
 
   return lines
 
 
 def read_lineObs(directory,nlines,filename="LINEobs.dat",tarfile=None):
   '''
   Reads the lineobs Data. the number of lines have to be known.
@@ -3284,15 +3452,15 @@
     fext=open(fn_ext,"r")
     fext.readline()
     contObs.E_BV=float(fext.readline())
     fext.readline()
     contObs.R_V=float(fext.readline())
     contObs.A_V=contObs.R_V*contObs.E_BV
 
-    fn_ext.close()
+    fext.close()
 
 #   # check if there is an image.in
 #   fn_images= directory+"/image.in"
 #   if os.path.exists(fn_images):
 #     if contObs is None:
 #       contObs=DataContinuumObs()
 #
@@ -3357,45 +3525,65 @@
 def read_sed(directory,filename="SED.out",filenameAna="SEDana.out",tarfile=None):
   '''
   Reads the ProDiMo SED output including the analysis data.
   '''
   f,dummy=_getfile(filename,directory,tarfile)
   if f is None: return None
 
-  elems=f.readline().split()
-  distance=float(elems[len(elems)-1])
-  # ignore the face-on SED
-  f.readline()
-  nlam=int(f.readline())
-  f.readline()
-  for i in range(nlam):
-    f.readline()
+  records=f.readlines()
+  f.close()
 
-  f.readline()
-  elems=f.readline().split()
-  inclination=float(elems[len(elems)-1])
-  nlam=int(f.readline())
-  f.readline()
-  sed=DataSED(nlam,distance,inclination)
-  for i in range(nlam):
-    elems=f.readline().split()
-    sed.lam[i]=float(elems[0])
-    sed.nu[i]=float(elems[1])
+  # determine if there are multiple inclinations
+  # likely very slow
+  # -1 becaus we ignore the analytic one
+  ninc=sum('inclination[degree]' in s for s in records)-1
 
-    # FIXME: Workaround to catch strange values from ProDiMo .. should be fixed
-    # in ProDiMo
-    try:
-      sed.fnuErg[i]=float(elems[2])
-      sed.nuFnuW[i]=float(elems[3])
-      sed.fnuJy[i]=float(elems[4])
-    except ValueError as err:
-      print("WARN: Could not read value from SED.out: ",err)
+  distance=float(records[0].split()[-1])
+  nlam=int(records[2])
 
-  sed.setLbolTbol()
-  f.close()
+  sed=DataSED(nlam,distance)
+
+  ridx=nlam+2+3
+
+  # need this already here
+  sed._Lbols=[None]*ninc
+  sed._Tbols=[None]*ninc
+
+  for iinc in range(ninc):
+    sed._inclinations.append(float(records[ridx].split()[-1]))
+    ridx+=3
+
+    fnuErg=np.zeros(shape=(nlam))
+    nuFnuW=np.zeros(shape=(nlam))
+    fnuJy=np.zeros(shape=(nlam))
+
+    for i in range(nlam):
+      elems=records[ridx].split()
+      if iinc==0:
+        sed.lam[i]=float(elems[0])
+        sed.nu[i]=float(elems[1])
+
+      # FIXME: Workaround to catch strange values from ProDiMo .. should be fixed
+      # in ProDiMo
+      try:
+        fnuErg[i]=float(elems[2])
+        nuFnuW[i]=float(elems[3])
+        fnuJy[i]=float(elems[4])
+      except ValueError as err:
+        print("WARN: Could not read value from SED.out: ",err)
+      ridx+=1
+
+    sed._fnuErgs.append(fnuErg)
+    sed._nuFnuWs.append(nuFnuW)
+    sed._fnuJys.append(fnuJy)
+
+    sed._DataSED__incidx=iinc
+    sed.setLbolTbol()
+    # next inc
+    ridx+=1
 
   # The analysis data, if it is not there not a big problem
   f,dummy=_getfile(filenameAna,directory,tarfile)
   if f is None:
     sed.sedAna=None
     return sed
```

### Comparing `prodimopy-2.1.6/prodimopy/read_casasim.py` & `prodimopy-2.2/prodimopy/read_casasim.py`

 * *Files identical despite different names*

### Comparing `prodimopy-2.1.6/prodimopy/read_mc.py` & `prodimopy-2.2/prodimopy/read_mc.py`

 * *Files identical despite different names*

### Comparing `prodimopy-2.1.6/prodimopy/read_slab.py` & `prodimopy-2.2/prodimopy/read_slab.py`

 * *Files 0% similar despite different names*

```diff
@@ -1784,3779 +1784,3796 @@
 00006f70: 7265 745f 6461 7461 0a0a 2020 2020 6465  ret_data..    de
 00006f80: 6620 636f 6e76 6f6c 7665 2873 656c 662c  f convolve(self,
 00006f90: 6672 6571 5f62 696e 733d 4e6f 6e65 2c52  freq_bins=None,R
 00006fa0: 3d31 2c6c 616d 6264 615f 303d 312c 6c61  =1,lambda_0=1,la
 00006fb0: 6d62 6461 5f6e 3d31 2c76 723d 3133 3030  mbda_n=1,vr=1300
 00006fc0: 2c4e 4c54 453d 4661 6c73 652c 636f 6e76  ,NLTE=False,conv
 00006fd0: 5f74 7970 653d 312c 7665 7262 6f73 653d  _type=1,verbose=
-00006fe0: 5472 7565 293a 0a20 2020 2020 2020 2066  True):.        f
-00006ff0: 6f72 2069 2c64 2069 6e20 656e 756d 6572  or i,d in enumer
-00007000: 6174 6528 7365 6c66 2e6d 6f64 656c 7329  ate(self.models)
-00007010: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00007020: 2076 6572 626f 7365 3a20 7072 696e 7428   verbose: print(
-00007030: 275c 6e27 2c69 2b31 2c27 3b20 4d6f 6465  '\n',i+1,'; Mode
-00007040: 6c20 6e75 6d62 6572 2027 2c73 656c 662e  l number ',self.
-00007050: 6d6f 6465 6c73 5b69 5d2e 6d6f 6465 6c5f  models[i].model_
-00007060: 6e75 6d62 6572 2c27 3b20 5370 6563 6965  number,'; Specie
-00007070: 7320 6e75 6d62 6572 2027 2c73 656c 662e  s number ',self.
-00007080: 6d6f 6465 6c73 5b69 5d2e 7370 6563 6965  models[i].specie
-00007090: 735f 6e75 6d62 6572 290a 2020 2020 2020  s_number).      
-000070a0: 2020 2020 2020 642e 636f 6e76 6f6c 7665        d.convolve
-000070b0: 2866 7265 715f 6269 6e73 3d66 7265 715f  (freq_bins=freq_
-000070c0: 6269 6e73 2c52 3d52 2c6c 616d 6264 615f  bins,R=R,lambda_
-000070d0: 303d 6c61 6d62 6461 5f30 2c6c 616d 6264  0=lambda_0,lambd
-000070e0: 615f 6e3d 6c61 6d62 6461 5f6e 2c76 723d  a_n=lambda_n,vr=
-000070f0: 7672 2c4e 4c54 453d 4e4c 5445 2c63 6f6e  vr,NLTE=NLTE,con
-00007100: 765f 7479 7065 3d63 6f6e 765f 7479 7065  v_type=conv_type
-00007110: 290a 0a20 2020 2064 6566 2063 6f6e 766f  )..    def convo
-00007120: 6c76 655f 6f76 6572 6c61 7028 7365 6c66  lve_overlap(self
-00007130: 2c52 3d31 2c6c 616d 6264 615f 303d 312c  ,R=1,lambda_0=1,
-00007140: 6c61 6d62 6461 5f6e 3d31 2c76 6572 626f  lambda_n=1,verbo
-00007150: 7365 3d54 7275 6529 3a0a 2020 2020 2020  se=True):.      
-00007160: 2020 666f 7220 692c 6420 696e 2065 6e75    for i,d in enu
-00007170: 6d65 7261 7465 2873 656c 662e 6d6f 6465  merate(self.mode
-00007180: 6c73 293a 0a20 2020 2020 2020 2020 2020  ls):.           
-00007190: 2069 6620 7665 7262 6f73 653a 2070 7269   if verbose: pri
-000071a0: 6e74 2827 5c6e 272c 692b 312c 273b 204d  nt('\n',i+1,'; M
-000071b0: 6f64 656c 206e 756d 6265 7220 272c 7365  odel number ',se
-000071c0: 6c66 2e6d 6f64 656c 735b 695d 2e6d 6f64  lf.models[i].mod
-000071d0: 656c 5f6e 756d 6265 7229 0a20 2020 2020  el_number).     
-000071e0: 2020 2020 2020 2064 2e63 6f6e 766f 6c76         d.convolv
-000071f0: 655f 6f76 6572 6c61 7028 523d 522c 6c61  e_overlap(R=R,la
-00007200: 6d62 6461 5f30 3d6c 616d 6264 615f 302c  mbda_0=lambda_0,
-00007210: 6c61 6d62 6461 5f6e 3d6c 616d 6264 615f  lambda_n=lambda_
-00007220: 6e29 0a0a 2020 2020 4070 726f 7065 7274  n)..    @propert
-00007230: 790a 2020 2020 6465 6620 6e6d 6f64 656c  y.    def nmodel
-00007240: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
-00007250: 2073 656c 662e 5f6e 6d6f 6465 6c73 3d6c   self._nmodels=l
-00007260: 656e 2873 656c 662e 6d6f 6465 6c73 290a  en(self.models).
-00007270: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00007280: 656c 662e 5f6e 6d6f 6465 6c73 0a0a 2020  elf._nmodels..  
-00007290: 2020 406e 6d6f 6465 6c73 2e73 6574 7465    @nmodels.sette
-000072a0: 720a 2020 2020 6465 6620 6e6d 6f64 656c  r.    def nmodel
-000072b0: 7328 7365 6c66 2c76 616c 7565 293a 0a20  s(self,value):. 
-000072c0: 2020 2020 2020 2073 656c 662e 5f6e 6d6f         self._nmo
-000072d0: 6465 6c73 3d76 616c 7565 0a0a 2020 2020  dels=value..    
-000072e0: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-000072f0: 6620 7370 6563 6965 735f 6e75 6d62 6572  f species_number
-00007300: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00007310: 6966 2073 656c 662e 6e6d 6f64 656c 733e  if self.nmodels>
-00007320: 313a 0a20 2020 2020 2020 2020 2020 2073  1:.            s
-00007330: 656c 662e 5f73 7065 6369 6573 5f6e 756d  elf._species_num
-00007340: 6265 723d 5b5d 0a20 2020 2020 2020 2020  ber=[].         
-00007350: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-00007360: 6528 7365 6c66 2e6e 6d6f 6465 6c73 293a  e(self.nmodels):
-00007370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007380: 2073 656c 662e 5f73 7065 6369 6573 5f6e   self._species_n
-00007390: 756d 6265 722e 6170 7065 6e64 2873 656c  umber.append(sel
-000073a0: 662e 6d6f 6465 6c73 5b69 5d2e 7370 6563  f.models[i].spec
-000073b0: 6965 735f 6e75 6d62 6572 290a 2020 2020  ies_number).    
-000073c0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-000073d0: 2020 2020 2020 7365 6c66 2e5f 7370 6563        self._spec
-000073e0: 6965 735f 6e75 6d62 6572 3d73 656c 662e  ies_number=self.
-000073f0: 6d6f 6465 6c73 5b30 5d2e 7370 6563 6965  models[0].specie
-00007400: 735f 6e75 6d62 6572 0a20 2020 2020 2020  s_number.       
-00007410: 2072 6574 7572 6e20 7365 6c66 2e5f 7370   return self._sp
-00007420: 6563 6965 735f 6e75 6d62 6572 0a0a 2020  ecies_number..  
-00007430: 2020 4073 7065 6369 6573 5f6e 756d 6265    @species_numbe
-00007440: 722e 7365 7474 6572 0a20 2020 2064 6566  r.setter.    def
-00007450: 2073 7065 6369 6573 5f6e 756d 6265 7228   species_number(
-00007460: 7365 6c66 2c76 616c 7565 293a 0a20 2020  self,value):.   
-00007470: 2020 2020 2073 656c 662e 5f73 7065 6369       self._speci
-00007480: 6573 5f6e 756d 6265 723d 7661 6c75 650a  es_number=value.
-00007490: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-000074a0: 2020 2064 6566 206d 6f64 656c 5f6e 756d     def model_num
-000074b0: 6265 7228 7365 6c66 293a 0a20 2020 2020  ber(self):.     
-000074c0: 2020 2069 6620 7365 6c66 2e6e 6d6f 6465     if self.nmode
-000074d0: 6c73 3e31 3a0a 2020 2020 2020 2020 2020  ls>1:.          
-000074e0: 2020 7365 6c66 2e5f 6d6f 6465 6c5f 6e75    self._model_nu
-000074f0: 6d62 6572 3d5b 5d0a 2020 2020 2020 2020  mber=[].        
-00007500: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-00007510: 6765 2873 656c 662e 6e6d 6f64 656c 7329  ge(self.nmodels)
-00007520: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00007530: 2020 7365 6c66 2e5f 6d6f 6465 6c5f 6e75    self._model_nu
-00007540: 6d62 6572 2e61 7070 656e 6428 7365 6c66  mber.append(self
-00007550: 2e6d 6f64 656c 735b 695d 2e6d 6f64 656c  .models[i].model
-00007560: 5f6e 756d 6265 7229 0a20 2020 2020 2020  _number).       
-00007570: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00007580: 2020 2073 656c 662e 5f6d 6f64 656c 5f6e     self._model_n
-00007590: 756d 6265 723d 7365 6c66 2e6d 6f64 656c  umber=self.model
-000075a0: 735b 305d 2e6d 6f64 656c 5f6e 756d 6265  s[0].model_numbe
-000075b0: 720a 2020 2020 2020 2020 7265 7475 726e  r.        return
-000075c0: 2073 656c 662e 5f6d 6f64 656c 5f6e 756d   self._model_num
-000075d0: 6265 720a 0a20 2020 2040 6d6f 6465 6c5f  ber..    @model_
-000075e0: 6e75 6d62 6572 2e73 6574 7465 720a 2020  number.setter.  
-000075f0: 2020 6465 6620 6d6f 6465 6c5f 6e75 6d62    def model_numb
-00007600: 6572 2873 656c 662c 7661 6c75 6529 3a0a  er(self,value):.
-00007610: 2020 2020 2020 2020 7365 6c66 2e5f 6d6f          self._mo
-00007620: 6465 6c5f 6e75 6d62 6572 3d76 616c 7565  del_number=value
-00007630: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-00007640: 2020 2020 6465 6620 4e48 2873 656c 6629      def NH(self)
-00007650: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
-00007660: 662e 6e6d 6f64 656c 733e 313a 0a20 2020  f.nmodels>1:.   
-00007670: 2020 2020 2020 2020 2073 656c 662e 5f4e           self._N
-00007680: 483d 5b5d 0a20 2020 2020 2020 2020 2020  H=[].           
-00007690: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-000076a0: 7365 6c66 2e6e 6d6f 6465 6c73 293a 0a20  self.nmodels):. 
-000076b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000076c0: 656c 662e 5f4e 482e 6170 7065 6e64 2873  elf._NH.append(s
-000076d0: 656c 662e 6d6f 6465 6c73 5b69 5d2e 4e48  elf.models[i].NH
-000076e0: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-000076f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00007700: 2e5f 4e48 3d73 656c 662e 6d6f 6465 6c73  ._NH=self.models
-00007710: 5b30 5d2e 4e48 0a20 2020 2020 2020 2072  [0].NH.        r
-00007720: 6574 7572 6e20 7365 6c66 2e5f 4e48 0a0a  eturn self._NH..
-00007730: 2020 2020 404e 482e 7365 7474 6572 0a20      @NH.setter. 
-00007740: 2020 2064 6566 204e 4828 7365 6c66 2c76     def NH(self,v
-00007750: 616c 7565 293a 0a20 2020 2020 2020 2073  alue):.        s
-00007760: 656c 662e 5f4e 483d 7661 6c75 650a 0a20  elf._NH=value.. 
-00007770: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-00007780: 2064 6566 206e 436f 6c6c 2873 656c 6629   def nColl(self)
-00007790: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
-000077a0: 662e 6e6d 6f64 656c 733e 313a 0a20 2020  f.nmodels>1:.   
-000077b0: 2020 2020 2020 2020 2073 656c 662e 5f6e           self._n
-000077c0: 436f 6c6c 3d5b 5d0a 2020 2020 2020 2020  Coll=[].        
-000077d0: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-000077e0: 6765 2873 656c 662e 6e6d 6f64 656c 7329  ge(self.nmodels)
-000077f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00007800: 2020 7365 6c66 2e5f 6e43 6f6c 6c2e 6170    self._nColl.ap
-00007810: 7065 6e64 2873 656c 662e 6d6f 6465 6c73  pend(self.models
-00007820: 5b69 5d2e 6e43 6f6c 6c29 0a20 2020 2020  [i].nColl).     
-00007830: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00007840: 2020 2020 2073 656c 662e 5f6e 436f 6c6c       self._nColl
-00007850: 3d73 656c 662e 6d6f 6465 6c73 5b30 5d2e  =self.models[0].
-00007860: 6e43 6f6c 6c0a 2020 2020 2020 2020 7265  nColl.        re
-00007870: 7475 726e 2073 656c 662e 5f6e 436f 6c6c  turn self._nColl
-00007880: 0a0a 2020 2020 406e 436f 6c6c 2e73 6574  ..    @nColl.set
-00007890: 7465 720a 2020 2020 6465 6620 6e43 6f6c  ter.    def nCol
-000078a0: 6c28 7365 6c66 2c76 616c 7565 293a 0a20  l(self,value):. 
-000078b0: 2020 2020 2020 2073 656c 662e 5f6e 436f         self._nCo
-000078c0: 6c6c 3d76 616c 7565 0a0a 2020 2020 4070  ll=value..    @p
-000078d0: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-000078e0: 6e65 2873 656c 6629 3a0a 2020 2020 2020  ne(self):.      
-000078f0: 2020 6966 2073 656c 662e 6e6d 6f64 656c    if self.nmodel
-00007900: 733e 313a 0a20 2020 2020 2020 2020 2020  s>1:.           
-00007910: 2073 656c 662e 5f6e 653d 5b5d 0a20 2020   self._ne=[].   
-00007920: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
-00007930: 6e20 7261 6e67 6528 7365 6c66 2e6e 6d6f  n range(self.nmo
-00007940: 6465 6c73 293a 0a20 2020 2020 2020 2020  dels):.         
-00007950: 2020 2020 2020 2073 656c 662e 5f6e 652e         self._ne.
-00007960: 6170 7065 6e64 2873 656c 662e 6d6f 6465  append(self.mode
-00007970: 6c73 5b69 5d2e 6e65 290a 2020 2020 2020  ls[i].ne).      
-00007980: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00007990: 2020 2020 7365 6c66 2e5f 6e65 3d73 656c      self._ne=sel
-000079a0: 662e 6d6f 6465 6c73 5b30 5d2e 6e65 0a20  f.models[0].ne. 
-000079b0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-000079c0: 6c66 2e5f 6e65 0a0a 2020 2020 406e 652e  lf._ne..    @ne.
-000079d0: 7365 7474 6572 0a20 2020 2064 6566 206e  setter.    def n
-000079e0: 6528 7365 6c66 2c76 616c 7565 293a 0a20  e(self,value):. 
-000079f0: 2020 2020 2020 2073 656c 662e 5f6e 653d         self._ne=
-00007a00: 7661 6c75 650a 0a20 2020 2040 7072 6f70  value..    @prop
-00007a10: 6572 7479 0a20 2020 2064 6566 206e 4865  erty.    def nHe
-00007a20: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00007a30: 6966 2073 656c 662e 6e6d 6f64 656c 733e  if self.nmodels>
-00007a40: 313a 0a20 2020 2020 2020 2020 2020 2073  1:.            s
-00007a50: 656c 662e 5f6e 4865 3d5b 5d0a 2020 2020  elf._nHe=[].    
-00007a60: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-00007a70: 2072 616e 6765 2873 656c 662e 6e6d 6f64   range(self.nmod
-00007a80: 656c 7329 3a0a 2020 2020 2020 2020 2020  els):.          
-00007a90: 2020 2020 2020 7365 6c66 2e5f 6e48 652e        self._nHe.
-00007aa0: 6170 7065 6e64 2873 656c 662e 6d6f 6465  append(self.mode
-00007ab0: 6c73 5b69 5d2e 6e48 6529 0a20 2020 2020  ls[i].nHe).     
-00007ac0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00007ad0: 2020 2020 2073 656c 662e 5f6e 4865 3d73       self._nHe=s
-00007ae0: 656c 662e 6d6f 6465 6c73 5b30 5d2e 6e48  elf.models[0].nH
-00007af0: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
-00007b00: 2073 656c 662e 5f6e 4865 0a0a 2020 2020   self._nHe..    
-00007b10: 406e 4865 2e73 6574 7465 720a 2020 2020  @nHe.setter.    
-00007b20: 6465 6620 6e48 6528 7365 6c66 2c76 616c  def nHe(self,val
-00007b30: 7565 293a 0a20 2020 2020 2020 2073 656c  ue):.        sel
-00007b40: 662e 5f6e 4865 3d76 616c 7565 0a0a 2020  f._nHe=value..  
-00007b50: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-00007b60: 6465 6620 6e48 4949 2873 656c 6629 3a0a  def nHII(self):.
-00007b70: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00007b80: 6e6d 6f64 656c 733e 313a 0a20 2020 2020  nmodels>1:.     
-00007b90: 2020 2020 2020 2073 656c 662e 5f6e 4849         self._nHI
-00007ba0: 493d 5b5d 0a20 2020 2020 2020 2020 2020  I=[].           
-00007bb0: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-00007bc0: 7365 6c66 2e6e 6d6f 6465 6c73 293a 0a20  self.nmodels):. 
-00007bd0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00007be0: 656c 662e 5f6e 4849 492e 6170 7065 6e64  elf._nHII.append
-00007bf0: 2873 656c 662e 6d6f 6465 6c73 5b69 5d2e  (self.models[i].
-00007c00: 6e48 4949 290a 2020 2020 2020 2020 656c  nHII).        el
-00007c10: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00007c20: 7365 6c66 2e5f 6e48 4949 3d73 656c 662e  self._nHII=self.
-00007c30: 6d6f 6465 6c73 5b30 5d2e 6e48 4949 0a20  models[0].nHII. 
-00007c40: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00007c50: 6c66 2e5f 6e48 4949 0a0a 2020 2020 406e  lf._nHII..    @n
-00007c60: 4849 492e 7365 7474 6572 0a20 2020 2064  HII.setter.    d
-00007c70: 6566 206e 4849 4928 7365 6c66 2c76 616c  ef nHII(self,val
-00007c80: 7565 293a 0a20 2020 2020 2020 2073 656c  ue):.        sel
-00007c90: 662e 5f6e 4849 493d 7661 6c75 650a 0a20  f._nHII=value.. 
-00007ca0: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-00007cb0: 2064 6566 206e 4849 2873 656c 6629 3a0a   def nHI(self):.
-00007cc0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00007cd0: 6e6d 6f64 656c 733e 313a 0a20 2020 2020  nmodels>1:.     
-00007ce0: 2020 2020 2020 2073 656c 662e 5f6e 4849         self._nHI
-00007cf0: 3d5b 5d0a 2020 2020 2020 2020 2020 2020  =[].            
-00007d00: 666f 7220 6920 696e 2072 616e 6765 2873  for i in range(s
-00007d10: 656c 662e 6e6d 6f64 656c 7329 3a0a 2020  elf.nmodels):.  
-00007d20: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00007d30: 6c66 2e5f 6e48 492e 6170 7065 6e64 2873  lf._nHI.append(s
-00007d40: 656c 662e 6d6f 6465 6c73 5b69 5d2e 6e48  elf.models[i].nH
-00007d50: 4929 0a20 2020 2020 2020 2065 6c73 653a  I).        else:
-00007d60: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00007d70: 662e 5f6e 4849 3d73 656c 662e 6d6f 6465  f._nHI=self.mode
-00007d80: 6c73 5b30 5d2e 6e48 490a 2020 2020 2020  ls[0].nHI.      
-00007d90: 2020 7265 7475 726e 2073 656c 662e 5f6e    return self._n
-00007da0: 4849 0a0a 2020 2020 406e 4849 2e73 6574  HI..    @nHI.set
-00007db0: 7465 720a 2020 2020 6465 6620 6e48 4928  ter.    def nHI(
-00007dc0: 7365 6c66 2c76 616c 7565 293a 0a20 2020  self,value):.   
-00007dd0: 2020 2020 2073 656c 662e 5f6e 4849 3d76       self._nHI=v
-00007de0: 616c 7565 0a0a 2020 2020 4070 726f 7065  alue..    @prope
-00007df0: 7274 790a 2020 2020 6465 6620 6e48 3228  rty.    def nH2(
-00007e00: 7365 6c66 293a 0a20 2020 2020 2020 2069  self):.        i
-00007e10: 6620 7365 6c66 2e6e 6d6f 6465 6c73 3e31  f self.nmodels>1
-00007e20: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00007e30: 6c66 2e5f 6e48 323d 5b5d 0a20 2020 2020  lf._nH2=[].     
-00007e40: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-00007e50: 7261 6e67 6528 7365 6c66 2e6e 6d6f 6465  range(self.nmode
-00007e60: 6c73 293a 0a20 2020 2020 2020 2020 2020  ls):.           
-00007e70: 2020 2020 2073 656c 662e 5f6e 4832 2e61       self._nH2.a
-00007e80: 7070 656e 6428 7365 6c66 2e6d 6f64 656c  ppend(self.model
-00007e90: 735b 695d 2e6e 4832 290a 2020 2020 2020  s[i].nH2).      
-00007ea0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00007eb0: 2020 2020 7365 6c66 2e5f 6e48 323d 7365      self._nH2=se
-00007ec0: 6c66 2e6d 6f64 656c 735b 305d 2e6e 4832  lf.models[0].nH2
-00007ed0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00007ee0: 7365 6c66 2e5f 6e48 320a 0a20 2020 2040  self._nH2..    @
-00007ef0: 6e48 322e 7365 7474 6572 0a20 2020 2064  nH2.setter.    d
-00007f00: 6566 206e 4832 2873 656c 662c 7661 6c75  ef nH2(self,valu
-00007f10: 6529 3a0a 2020 2020 2020 2020 7365 6c66  e):.        self
-00007f20: 2e5f 6e48 323d 7661 6c75 650a 0a20 2020  ._nH2=value..   
-00007f30: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-00007f40: 6566 2064 7573 745f 746f 5f67 6173 2873  ef dust_to_gas(s
-00007f50: 656c 6629 3a0a 2020 2020 2020 2020 6966  elf):.        if
-00007f60: 2073 656c 662e 6e6d 6f64 656c 733e 313a   self.nmodels>1:
-00007f70: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00007f80: 662e 5f64 7573 745f 746f 5f67 6173 3d5b  f._dust_to_gas=[
-00007f90: 5d0a 2020 2020 2020 2020 2020 2020 666f  ].            fo
-00007fa0: 7220 6920 696e 2072 616e 6765 2873 656c  r i in range(sel
-00007fb0: 662e 6e6d 6f64 656c 7329 3a0a 2020 2020  f.nmodels):.    
-00007fc0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00007fd0: 2e5f 6475 7374 5f74 6f5f 6761 732e 6170  ._dust_to_gas.ap
-00007fe0: 7065 6e64 2873 656c 662e 6d6f 6465 6c73  pend(self.models
-00007ff0: 5b69 5d2e 6475 7374 5f74 6f5f 6761 7329  [i].dust_to_gas)
-00008000: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00008010: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00008020: 5f64 7573 745f 746f 5f67 6173 3d73 656c  _dust_to_gas=sel
-00008030: 662e 6d6f 6465 6c73 5b30 5d2e 6475 7374  f.models[0].dust
-00008040: 5f74 6f5f 6761 730a 2020 2020 2020 2020  _to_gas.        
-00008050: 7265 7475 726e 2073 656c 662e 5f64 7573  return self._dus
-00008060: 745f 746f 5f67 6173 0a0a 2020 2020 4064  t_to_gas..    @d
-00008070: 7573 745f 746f 5f67 6173 2e73 6574 7465  ust_to_gas.sette
-00008080: 720a 2020 2020 6465 6620 6475 7374 5f74  r.    def dust_t
-00008090: 6f5f 6761 7328 7365 6c66 2c76 616c 7565  o_gas(self,value
-000080a0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-000080b0: 5f64 7573 745f 746f 5f67 6173 3d76 616c  _dust_to_gas=val
-000080c0: 7565 0a0a 2020 2020 4070 726f 7065 7274  ue..    @propert
-000080d0: 790a 2020 2020 6465 6620 7674 7572 6228  y.    def vturb(
-000080e0: 7365 6c66 293a 0a20 2020 2020 2020 2069  self):.        i
-000080f0: 6620 7365 6c66 2e6e 6d6f 6465 6c73 3e31  f self.nmodels>1
-00008100: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00008110: 6c66 2e5f 7674 7572 623d 5b5d 0a20 2020  lf._vturb=[].   
-00008120: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
-00008130: 6e20 7261 6e67 6528 7365 6c66 2e6e 6d6f  n range(self.nmo
-00008140: 6465 6c73 293a 0a20 2020 2020 2020 2020  dels):.         
-00008150: 2020 2020 2020 2073 656c 662e 5f76 7475         self._vtu
-00008160: 7262 2e61 7070 656e 6428 7365 6c66 2e6d  rb.append(self.m
-00008170: 6f64 656c 735b 695d 2e76 7475 7262 290a  odels[i].vturb).
-00008180: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00008190: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-000081a0: 7674 7572 623d 7365 6c66 2e6d 6f64 656c  vturb=self.model
-000081b0: 735b 305d 2e76 7475 7262 0a20 2020 2020  s[0].vturb.     
-000081c0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-000081d0: 7674 7572 620a 0a20 2020 2040 7674 7572  vturb..    @vtur
-000081e0: 622e 7365 7474 6572 0a20 2020 2064 6566  b.setter.    def
-000081f0: 2076 7475 7262 2873 656c 662c 7661 6c75   vturb(self,valu
-00008200: 6529 3a0a 2020 2020 2020 2020 7365 6c66  e):.        self
-00008210: 2e5f 7674 7572 623d 7661 6c75 650a 0a20  ._vturb=value.. 
-00008220: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-00008230: 2064 6566 2054 6728 7365 6c66 293a 0a20   def Tg(self):. 
-00008240: 2020 2020 2020 2069 6620 7365 6c66 2e6e         if self.n
-00008250: 6d6f 6465 6c73 3e31 3a0a 2020 2020 2020  models>1:.      
-00008260: 2020 2020 2020 7365 6c66 2e5f 5467 3d5b        self._Tg=[
-00008270: 5d0a 2020 2020 2020 2020 2020 2020 666f  ].            fo
-00008280: 7220 6920 696e 2072 616e 6765 2873 656c  r i in range(sel
-00008290: 662e 6e6d 6f64 656c 7329 3a0a 2020 2020  f.nmodels):.    
-000082a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000082b0: 2e5f 5467 2e61 7070 656e 6428 7365 6c66  ._Tg.append(self
-000082c0: 2e6d 6f64 656c 735b 695d 2e54 6729 0a20  .models[i].Tg). 
-000082d0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-000082e0: 2020 2020 2020 2020 2073 656c 662e 5f54           self._T
-000082f0: 673d 7365 6c66 2e6d 6f64 656c 735b 305d  g=self.models[0]
-00008300: 2e54 670a 2020 2020 2020 2020 7265 7475  .Tg.        retu
-00008310: 726e 2073 656c 662e 5f54 670a 0a20 2020  rn self._Tg..   
-00008320: 2040 5467 2e73 6574 7465 720a 2020 2020   @Tg.setter.    
-00008330: 6465 6620 5467 2873 656c 662c 7661 6c75  def Tg(self,valu
-00008340: 6529 3a0a 2020 2020 2020 2020 7365 6c66  e):.        self
-00008350: 2e5f 5467 3d76 616c 7565 0a0a 2020 2020  ._Tg=value..    
-00008360: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-00008370: 6620 5464 2873 656c 6629 3a0a 2020 2020  f Td(self):.    
-00008380: 2020 2020 6966 2073 656c 662e 6e6d 6f64      if self.nmod
-00008390: 656c 733e 313a 0a20 2020 2020 2020 2020  els>1:.         
-000083a0: 2020 2073 656c 662e 5f54 643d 5b5d 0a20     self._Td=[]. 
-000083b0: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-000083c0: 2069 6e20 7261 6e67 6528 7365 6c66 2e6e   in range(self.n
-000083d0: 6d6f 6465 6c73 293a 0a20 2020 2020 2020  models):.       
-000083e0: 2020 2020 2020 2020 2073 656c 662e 5f54           self._T
-000083f0: 642e 6170 7065 6e64 2873 656c 662e 6d6f  d.append(self.mo
-00008400: 6465 6c73 5b69 5d2e 5464 290a 2020 2020  dels[i].Td).    
-00008410: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00008420: 2020 2020 2020 7365 6c66 2e5f 5464 3d73        self._Td=s
-00008430: 656c 662e 6d6f 6465 6c73 5b30 5d2e 5464  elf.models[0].Td
-00008440: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00008450: 7365 6c66 2e5f 5464 0a0a 2020 2020 4054  self._Td..    @T
-00008460: 642e 7365 7474 6572 0a20 2020 2064 6566  d.setter.    def
-00008470: 2054 6428 7365 6c66 2c76 616c 7565 293a   Td(self,value):
-00008480: 0a20 2020 2020 2020 2073 656c 662e 5f54  .        self._T
-00008490: 643d 7661 6c75 650a 0a20 2020 2040 7072  d=value..    @pr
-000084a0: 6f70 6572 7479 0a20 2020 2064 6566 2073  operty.    def s
-000084b0: 7065 6369 6573 5f6e 616d 6528 7365 6c66  pecies_name(self
-000084c0: 293a 0a20 2020 2020 2020 2069 6620 7365  ):.        if se
-000084d0: 6c66 2e6e 6d6f 6465 6c73 3e31 3a0a 2020  lf.nmodels>1:.  
-000084e0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-000084f0: 7370 6563 6965 735f 6e61 6d65 3d5b 5d0a  species_name=[].
-00008500: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00008510: 6920 696e 2072 616e 6765 2873 656c 662e  i in range(self.
-00008520: 6e6d 6f64 656c 7329 3a0a 2020 2020 2020  nmodels):.      
-00008530: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00008540: 7370 6563 6965 735f 6e61 6d65 2e61 7070  species_name.app
-00008550: 656e 6428 7365 6c66 2e6d 6f64 656c 735b  end(self.models[
-00008560: 695d 2e73 7065 6369 6573 5f6e 616d 6529  i].species_name)
-00008570: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00008580: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00008590: 5f73 7065 6369 6573 5f6e 616d 653d 7365  _species_name=se
-000085a0: 6c66 2e6d 6f64 656c 735b 305d 2e73 7065  lf.models[0].spe
-000085b0: 6369 6573 5f6e 616d 650a 2020 2020 2020  cies_name.      
-000085c0: 2020 7265 7475 726e 2073 656c 662e 5f73    return self._s
-000085d0: 7065 6369 6573 5f6e 616d 650a 0a20 2020  pecies_name..   
-000085e0: 2040 7370 6563 6965 735f 6e61 6d65 2e73   @species_name.s
-000085f0: 6574 7465 720a 2020 2020 6465 6620 7370  etter.    def sp
-00008600: 6563 6965 735f 6e61 6d65 2873 656c 662c  ecies_name(self,
-00008610: 7661 6c75 6529 3a0a 2020 2020 2020 2020  value):.        
-00008620: 7365 6c66 2e5f 7370 6563 6965 735f 6e61  self._species_na
-00008630: 6d65 3d76 616c 7565 0a0a 2020 2020 4070  me=value..    @p
-00008640: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-00008650: 7370 6563 6965 735f 696e 6465 7828 7365  species_index(se
-00008660: 6c66 293a 0a20 2020 2020 2020 2069 6620  lf):.        if 
-00008670: 7365 6c66 2e6e 6d6f 6465 6c73 3e31 3a0a  self.nmodels>1:.
-00008680: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00008690: 2e5f 7370 6563 6965 735f 696e 6465 783d  ._species_index=
-000086a0: 5b5d 0a20 2020 2020 2020 2020 2020 2066  [].            f
-000086b0: 6f72 2069 2069 6e20 7261 6e67 6528 7365  or i in range(se
-000086c0: 6c66 2e6e 6d6f 6465 6c73 293a 0a20 2020  lf.nmodels):.   
-000086d0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000086e0: 662e 5f73 7065 6369 6573 5f69 6e64 6578  f._species_index
-000086f0: 2e61 7070 656e 6428 7365 6c66 2e6d 6f64  .append(self.mod
-00008700: 656c 735b 695d 2e73 7065 6369 6573 5f69  els[i].species_i
-00008710: 6e64 6578 290a 2020 2020 2020 2020 656c  ndex).        el
-00008720: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00008730: 7365 6c66 2e5f 7370 6563 6965 735f 696e  self._species_in
-00008740: 6465 783d 7365 6c66 2e6d 6f64 656c 735b  dex=self.models[
-00008750: 305d 2e73 7065 6369 6573 5f69 6e64 6578  0].species_index
-00008760: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00008770: 7365 6c66 2e5f 7370 6563 6965 735f 696e  self._species_in
-00008780: 6465 780a 0a20 2020 2040 7370 6563 6965  dex..    @specie
-00008790: 735f 696e 6465 782e 7365 7474 6572 0a20  s_index.setter. 
-000087a0: 2020 2064 6566 2073 7065 6369 6573 5f69     def species_i
-000087b0: 6e64 6578 2873 656c 662c 7661 6c75 6529  ndex(self,value)
-000087c0: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
-000087d0: 7370 6563 6965 735f 696e 6465 783d 7661  species_index=va
-000087e0: 6c75 650a 0a20 2020 2040 7072 6f70 6572  lue..    @proper
-000087f0: 7479 0a20 2020 2064 6566 2061 6275 6e64  ty.    def abund
-00008800: 616e 6365 2873 656c 6629 3a0a 2020 2020  ance(self):.    
-00008810: 2020 2020 6966 2073 656c 662e 6e6d 6f64      if self.nmod
-00008820: 656c 733e 313a 0a20 2020 2020 2020 2020  els>1:.         
-00008830: 2020 2073 656c 662e 5f61 6275 6e64 616e     self._abundan
-00008840: 6365 3d5b 5d0a 2020 2020 2020 2020 2020  ce=[].          
-00008850: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
-00008860: 2873 656c 662e 6e6d 6f64 656c 7329 3a0a  (self.nmodels):.
-00008870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008880: 7365 6c66 2e5f 6162 756e 6461 6e63 652e  self._abundance.
-00008890: 6170 7065 6e64 2873 656c 662e 6d6f 6465  append(self.mode
-000088a0: 6c73 5b69 5d2e 6162 756e 6461 6e63 6529  ls[i].abundance)
-000088b0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-000088c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000088d0: 5f61 6275 6e64 616e 6365 3d73 656c 662e  _abundance=self.
-000088e0: 6d6f 6465 6c73 5b30 5d2e 6162 756e 6461  models[0].abunda
-000088f0: 6e63 650a 2020 2020 2020 2020 7265 7475  nce.        retu
-00008900: 726e 2073 656c 662e 5f61 6275 6e64 616e  rn self._abundan
-00008910: 6365 0a0a 2020 2020 4061 6275 6e64 616e  ce..    @abundan
-00008920: 6365 2e73 6574 7465 720a 2020 2020 6465  ce.setter.    de
-00008930: 6620 6162 756e 6461 6e63 6528 7365 6c66  f abundance(self
-00008940: 2c76 616c 7565 293a 0a20 2020 2020 2020  ,value):.       
-00008950: 2073 656c 662e 5f61 6275 6e64 616e 6365   self._abundance
-00008960: 3d76 616c 7565 0a0a 2020 2020 4070 726f  =value..    @pro
-00008970: 7065 7274 790a 2020 2020 6465 6620 6476  perty.    def dv
-00008980: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00008990: 6966 2073 656c 662e 6e6d 6f64 656c 733e  if self.nmodels>
-000089a0: 313a 0a20 2020 2020 2020 2020 2020 2073  1:.            s
-000089b0: 656c 662e 5f64 763d 5b5d 0a20 2020 2020  elf._dv=[].     
-000089c0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-000089d0: 7261 6e67 6528 7365 6c66 2e6e 6d6f 6465  range(self.nmode
-000089e0: 6c73 293a 0a20 2020 2020 2020 2020 2020  ls):.           
-000089f0: 2020 2020 2073 656c 662e 5f64 762e 6170       self._dv.ap
-00008a00: 7065 6e64 2873 656c 662e 6d6f 6465 6c73  pend(self.models
-00008a10: 5b69 5d2e 6476 290a 2020 2020 2020 2020  [i].dv).        
-00008a20: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00008a30: 2020 7365 6c66 2e5f 6476 3d73 656c 662e    self._dv=self.
-00008a40: 6d6f 6465 6c73 5b30 5d2e 6476 0a20 2020  models[0].dv.   
-00008a50: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00008a60: 2e5f 6476 0a0a 2020 2020 4064 762e 7365  ._dv..    @dv.se
-00008a70: 7474 6572 0a20 2020 2064 6566 2064 7628  tter.    def dv(
-00008a80: 7365 6c66 2c76 616c 7565 293a 0a20 2020  self,value):.   
-00008a90: 2020 2020 2073 656c 662e 5f64 763d 7661       self._dv=va
-00008aa0: 6c75 650a 0a20 2020 2040 7072 6f70 6572  lue..    @proper
-00008ab0: 7479 0a20 2020 2064 6566 206e 6c65 7665  ty.    def nleve
-00008ac0: 6c73 2873 656c 6629 3a0a 2020 2020 2020  ls(self):.      
-00008ad0: 2020 6966 2073 656c 662e 6e6d 6f64 656c    if self.nmodel
-00008ae0: 733e 313a 0a20 2020 2020 2020 2020 2020  s>1:.           
-00008af0: 2073 656c 662e 5f6e 6c65 7665 6c73 3d5b   self._nlevels=[
-00008b00: 5d0a 2020 2020 2020 2020 2020 2020 666f  ].            fo
-00008b10: 7220 6920 696e 2072 616e 6765 2873 656c  r i in range(sel
-00008b20: 662e 6e6d 6f64 656c 7329 3a0a 2020 2020  f.nmodels):.    
-00008b30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00008b40: 2e5f 6e6c 6576 656c 732e 6170 7065 6e64  ._nlevels.append
-00008b50: 2873 656c 662e 6d6f 6465 6c73 5b69 5d2e  (self.models[i].
-00008b60: 6e6c 6576 656c 7329 0a20 2020 2020 2020  nlevels).       
-00008b70: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00008b80: 2020 2073 656c 662e 5f6e 6c65 7665 6c73     self._nlevels
-00008b90: 3d73 656c 662e 6d6f 6465 6c73 5b30 5d2e  =self.models[0].
-00008ba0: 6e6c 6576 656c 730a 2020 2020 2020 2020  nlevels.        
-00008bb0: 7265 7475 726e 2073 656c 662e 5f6e 6c65  return self._nle
-00008bc0: 7665 6c73 0a0a 2020 2020 406e 6c65 7665  vels..    @nleve
-00008bd0: 6c73 2e73 6574 7465 720a 2020 2020 6465  ls.setter.    de
-00008be0: 6620 6e6c 6576 656c 7328 7365 6c66 2c76  f nlevels(self,v
-00008bf0: 616c 7565 293a 0a20 2020 2020 2020 2073  alue):.        s
-00008c00: 656c 662e 5f6e 6c65 7665 6c73 3d76 616c  elf._nlevels=val
-00008c10: 7565 0a0a 2020 2020 4070 726f 7065 7274  ue..    @propert
-00008c20: 790a 2020 2020 6465 6620 6e6c 696e 6573  y.    def nlines
-00008c30: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00008c40: 6966 2073 656c 662e 6e6d 6f64 656c 733e  if self.nmodels>
-00008c50: 313a 0a20 2020 2020 2020 2020 2020 2073  1:.            s
-00008c60: 656c 662e 5f6e 6c69 6e65 733d 5b5d 0a20  elf._nlines=[]. 
-00008c70: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-00008c80: 2069 6e20 7261 6e67 6528 7365 6c66 2e6e   in range(self.n
-00008c90: 6d6f 6465 6c73 293a 0a20 2020 2020 2020  models):.       
-00008ca0: 2020 2020 2020 2020 2073 656c 662e 5f6e           self._n
-00008cb0: 6c69 6e65 732e 6170 7065 6e64 2873 656c  lines.append(sel
-00008cc0: 662e 6d6f 6465 6c73 5b69 5d2e 6e6c 696e  f.models[i].nlin
-00008cd0: 6573 290a 2020 2020 2020 2020 656c 7365  es).        else
-00008ce0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00008cf0: 6c66 2e5f 6e6c 696e 6573 3d73 656c 662e  lf._nlines=self.
-00008d00: 6d6f 6465 6c73 5b30 5d2e 6e6c 696e 6573  models[0].nlines
-00008d10: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00008d20: 7365 6c66 2e5f 6e6c 696e 6573 0a0a 2020  self._nlines..  
-00008d30: 2020 406e 6c69 6e65 732e 7365 7474 6572    @nlines.setter
-00008d40: 0a20 2020 2064 6566 206e 6c69 6e65 7328  .    def nlines(
-00008d50: 7365 6c66 2c76 616c 7565 293a 0a20 2020  self,value):.   
-00008d60: 2020 2020 2073 656c 662e 5f6e 6c69 6e65       self._nline
-00008d70: 733d 7661 6c75 650a 0a20 2020 2040 7072  s=value..    @pr
-00008d80: 6f70 6572 7479 0a20 2020 2064 6566 206c  operty.    def l
-00008d90: 696e 6564 6174 6128 7365 6c66 293a 0a20  inedata(self):. 
-00008da0: 2020 2020 2020 2069 6620 7365 6c66 2e6e         if self.n
-00008db0: 6d6f 6465 6c73 3e31 3a0a 2020 2020 2020  models>1:.      
-00008dc0: 2020 2020 2020 7365 6c66 2e5f 6c69 6e65        self._line
-00008dd0: 6461 7461 3d5b 5d0a 2020 2020 2020 2020  data=[].        
-00008de0: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-00008df0: 6765 2873 656c 662e 6e6d 6f64 656c 7329  ge(self.nmodels)
-00008e00: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00008e10: 2020 7365 6c66 2e5f 6c69 6e65 6461 7461    self._linedata
-00008e20: 2e61 7070 656e 6428 7365 6c66 2e6d 6f64  .append(self.mod
-00008e30: 656c 735b 695d 2e6c 696e 6564 6174 6129  els[i].linedata)
-00008e40: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00008e50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00008e60: 5f6c 696e 6564 6174 613d 7365 6c66 2e6d  _linedata=self.m
-00008e70: 6f64 656c 735b 305d 2e6c 696e 6564 6174  odels[0].linedat
-00008e80: 610a 2020 2020 2020 2020 7265 7475 726e  a.        return
-00008e90: 2073 656c 662e 5f6c 696e 6564 6174 610a   self._linedata.
-00008ea0: 0a20 2020 2040 6c69 6e65 6461 7461 2e73  .    @linedata.s
-00008eb0: 6574 7465 720a 2020 2020 6465 6620 6c69  etter.    def li
-00008ec0: 6e65 6461 7461 2873 656c 662c 7661 6c75  nedata(self,valu
-00008ed0: 6529 3a0a 2020 2020 2020 2020 7365 6c66  e):.        self
-00008ee0: 2e5f 6c69 6e65 6461 7461 3d76 616c 7565  ._linedata=value
-00008ef0: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-00008f00: 2020 2020 6465 6620 6c65 7665 6c64 6174      def leveldat
-00008f10: 6128 7365 6c66 293a 0a20 2020 2020 2020  a(self):.       
-00008f20: 2069 6620 7365 6c66 2e6e 6d6f 6465 6c73   if self.nmodels
-00008f30: 3e31 3a0a 2020 2020 2020 2020 2020 2020  >1:.            
-00008f40: 7365 6c66 2e5f 6c65 7665 6c64 6174 613d  self._leveldata=
-00008f50: 5b5d 0a20 2020 2020 2020 2020 2020 2066  [].            f
-00008f60: 6f72 2069 2069 6e20 7261 6e67 6528 7365  or i in range(se
-00008f70: 6c66 2e6e 6d6f 6465 6c73 293a 0a20 2020  lf.nmodels):.   
-00008f80: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00008f90: 662e 5f6c 6576 656c 6461 7461 2e61 7070  f._leveldata.app
-00008fa0: 656e 6428 7365 6c66 2e6d 6f64 656c 735b  end(self.models[
-00008fb0: 695d 2e6c 6576 656c 6461 7461 290a 2020  i].leveldata).  
-00008fc0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00008fd0: 2020 2020 2020 2020 7365 6c66 2e5f 6c65          self._le
-00008fe0: 7665 6c64 6174 613d 7365 6c66 2e6d 6f64  veldata=self.mod
-00008ff0: 656c 735b 305d 2e6c 6576 656c 6461 7461  els[0].leveldata
-00009000: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00009010: 7365 6c66 2e5f 6c65 7665 6c64 6174 610a  self._leveldata.
-00009020: 0a20 2020 2040 6c65 7665 6c64 6174 612e  .    @leveldata.
-00009030: 7365 7474 6572 0a20 2020 2064 6566 206c  setter.    def l
-00009040: 6576 656c 6461 7461 2873 656c 662c 7661  eveldata(self,va
-00009050: 6c75 6529 3a0a 2020 2020 2020 2020 7365  lue):.        se
-00009060: 6c66 2e5f 6c65 7665 6c64 6174 613d 7661  lf._leveldata=va
-00009070: 6c75 650a 0a20 2020 2040 7072 6f70 6572  lue..    @proper
-00009080: 7479 0a20 2020 2064 6566 2063 6f6e 7657  ty.    def convW
-00009090: 6176 656c 656e 6774 6828 7365 6c66 293a  avelength(self):
-000090a0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000090b0: 2e6e 6d6f 6465 6c73 3e31 3a0a 2020 2020  .nmodels>1:.    
-000090c0: 2020 2020 2020 2020 7365 6c66 2e5f 636f          self._co
-000090d0: 6e76 5761 7665 6c65 6e67 7468 3d5b 5d0a  nvWavelength=[].
-000090e0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000090f0: 6920 696e 2072 616e 6765 2873 656c 662e  i in range(self.
-00009100: 6e6d 6f64 656c 7329 3a0a 2020 2020 2020  nmodels):.      
-00009110: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00009120: 636f 6e76 5761 7665 6c65 6e67 7468 2e61  convWavelength.a
-00009130: 7070 656e 6428 7365 6c66 2e6d 6f64 656c  ppend(self.model
-00009140: 735b 695d 2e63 6f6e 7657 6176 656c 656e  s[i].convWavelen
-00009150: 6774 6829 0a20 2020 2020 2020 2065 6c73  gth).        els
-00009160: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00009170: 656c 662e 5f63 6f6e 7657 6176 656c 656e  elf._convWavelen
-00009180: 6774 683d 7365 6c66 2e6d 6f64 656c 735b  gth=self.models[
-00009190: 305d 2e63 6f6e 7657 6176 656c 656e 6774  0].convWavelengt
-000091a0: 680a 2020 2020 2020 2020 7265 7475 726e  h.        return
-000091b0: 2073 656c 662e 5f63 6f6e 7657 6176 656c   self._convWavel
-000091c0: 656e 6774 680a 0a20 2020 2040 636f 6e76  ength..    @conv
-000091d0: 5761 7665 6c65 6e67 7468 2e73 6574 7465  Wavelength.sette
-000091e0: 720a 2020 2020 6465 6620 636f 6e76 5761  r.    def convWa
-000091f0: 7665 6c65 6e67 7468 2873 656c 662c 7661  velength(self,va
-00009200: 6c75 6529 3a0a 2020 2020 2020 2020 7365  lue):.        se
-00009210: 6c66 2e5f 636f 6e76 5761 7665 6c65 6e67  lf._convWaveleng
-00009220: 7468 3d76 616c 7565 0a0a 2020 2020 4070  th=value..    @p
-00009230: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-00009240: 636f 6e76 4c54 4566 6c75 7828 7365 6c66  convLTEflux(self
-00009250: 293a 0a20 2020 2020 2020 2069 6620 7365  ):.        if se
-00009260: 6c66 2e6e 6d6f 6465 6c73 3e31 3a0a 2020  lf.nmodels>1:.  
-00009270: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00009280: 636f 6e76 4c54 4566 6c75 783d 5b5d 0a20  convLTEflux=[]. 
-00009290: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-000092a0: 2069 6e20 7261 6e67 6528 7365 6c66 2e6e   in range(self.n
-000092b0: 6d6f 6465 6c73 293a 0a20 2020 2020 2020  models):.       
-000092c0: 2020 2020 2020 2020 2073 656c 662e 5f63           self._c
-000092d0: 6f6e 764c 5445 666c 7578 2e61 7070 656e  onvLTEflux.appen
-000092e0: 6428 7365 6c66 2e6d 6f64 656c 735b 695d  d(self.models[i]
-000092f0: 2e63 6f6e 764c 5445 666c 7578 290a 2020  .convLTEflux).  
-00009300: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00009310: 2020 2020 2020 2020 7365 6c66 2e5f 636f          self._co
-00009320: 6e76 4c54 4566 6c75 783d 7365 6c66 2e6d  nvLTEflux=self.m
-00009330: 6f64 656c 735b 305d 2e63 6f6e 764c 5445  odels[0].convLTE
-00009340: 666c 7578 0a20 2020 2020 2020 2072 6574  flux.        ret
-00009350: 7572 6e20 7365 6c66 2e5f 636f 6e76 4c54  urn self._convLT
-00009360: 4566 6c75 780a 0a20 2020 2040 636f 6e76  Eflux..    @conv
-00009370: 4c54 4566 6c75 782e 7365 7474 6572 0a20  LTEflux.setter. 
-00009380: 2020 2064 6566 2063 6f6e 764c 5445 666c     def convLTEfl
-00009390: 7578 2873 656c 662c 7661 6c75 6529 3a0a  ux(self,value):.
-000093a0: 2020 2020 2020 2020 7365 6c66 2e5f 636f          self._co
-000093b0: 6e76 4c54 4566 6c75 783d 7661 6c75 650a  nvLTEflux=value.
-000093c0: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-000093d0: 2020 2064 6566 2063 6f6e 764e 4c54 4566     def convNLTEf
-000093e0: 6c75 7828 7365 6c66 293a 0a20 2020 2020  lux(self):.     
-000093f0: 2020 2069 6620 7365 6c66 2e6e 6d6f 6465     if self.nmode
-00009400: 6c73 3e31 3a0a 2020 2020 2020 2020 2020  ls>1:.          
-00009410: 2020 7365 6c66 2e5f 636f 6e76 4e4c 5445    self._convNLTE
-00009420: 666c 7578 3d5b 5d0a 2020 2020 2020 2020  flux=[].        
-00009430: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-00009440: 6765 2873 656c 662e 6e6d 6f64 656c 7329  ge(self.nmodels)
-00009450: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00009460: 2020 7365 6c66 2e5f 636f 6e76 4e4c 5445    self._convNLTE
-00009470: 666c 7578 2e61 7070 656e 6428 7365 6c66  flux.append(self
-00009480: 2e6d 6f64 656c 735b 695d 2e63 6f6e 764e  .models[i].convN
-00009490: 4c54 4566 6c75 7829 0a20 2020 2020 2020  LTEflux).       
-000094a0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-000094b0: 2020 2073 656c 662e 5f63 6f6e 764e 4c54     self._convNLT
-000094c0: 4566 6c75 783d 7365 6c66 2e6d 6f64 656c  Eflux=self.model
-000094d0: 735b 305d 2e63 6f6e 764e 4c54 4566 6c75  s[0].convNLTEflu
-000094e0: 780a 2020 2020 2020 2020 7265 7475 726e  x.        return
-000094f0: 2073 656c 662e 5f63 6f6e 764e 4c54 4566   self._convNLTEf
-00009500: 6c75 780a 0a20 2020 2040 636f 6e76 4e4c  lux..    @convNL
-00009510: 5445 666c 7578 2e73 6574 7465 720a 2020  TEflux.setter.  
-00009520: 2020 6465 6620 636f 6e76 4e4c 5445 666c    def convNLTEfl
-00009530: 7578 2873 656c 662c 7661 6c75 6529 3a0a  ux(self,value):.
-00009540: 2020 2020 2020 2020 7365 6c66 2e5f 636f          self._co
-00009550: 6e76 4e4c 5445 666c 7578 3d76 616c 7565  nvNLTEflux=value
-00009560: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-00009570: 2020 2020 6465 6620 636f 6e76 5479 7065      def convType
-00009580: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00009590: 6966 2073 656c 662e 6e6d 6f64 656c 733e  if self.nmodels>
-000095a0: 313a 0a20 2020 2020 2020 2020 2020 2073  1:.            s
-000095b0: 656c 662e 5f63 6f6e 7654 7970 653d 5b5d  elf._convType=[]
-000095c0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-000095d0: 2069 2069 6e20 7261 6e67 6528 7365 6c66   i in range(self
-000095e0: 2e6e 6d6f 6465 6c73 293a 0a20 2020 2020  .nmodels):.     
-000095f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00009600: 5f63 6f6e 7654 7970 652e 6170 7065 6e64  _convType.append
-00009610: 2873 656c 662e 6d6f 6465 6c73 5b69 5d2e  (self.models[i].
-00009620: 636f 6e76 5479 7065 290a 2020 2020 2020  convType).      
-00009630: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00009640: 2020 2020 7365 6c66 2e5f 636f 6e76 5479      self._convTy
-00009650: 7065 3d73 656c 662e 6d6f 6465 6c73 5b30  pe=self.models[0
-00009660: 5d2e 636f 6e76 5479 7065 0a20 2020 2020  ].convType.     
-00009670: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-00009680: 636f 6e76 5479 7065 0a0a 2020 2020 4063  convType..    @c
-00009690: 6f6e 7654 7970 652e 7365 7474 6572 0a20  onvType.setter. 
-000096a0: 2020 2064 6566 2063 6f6e 7654 7970 6528     def convType(
-000096b0: 7365 6c66 2c76 616c 7565 293a 0a20 2020  self,value):.   
-000096c0: 2020 2020 2073 656c 662e 5f63 6f6e 7654       self._convT
-000096d0: 7970 653d 7661 6c75 650a 0a20 2020 2040  ype=value..    @
-000096e0: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-000096f0: 2063 6f6e 7652 2873 656c 6629 3a0a 2020   convR(self):.  
-00009700: 2020 2020 2020 6966 2073 656c 662e 6e6d        if self.nm
-00009710: 6f64 656c 733e 313a 0a20 2020 2020 2020  odels>1:.       
-00009720: 2020 2020 2073 656c 662e 5f63 6f6e 7652       self._convR
-00009730: 3d5b 5d0a 2020 2020 2020 2020 2020 2020  =[].            
-00009740: 666f 7220 6920 696e 2072 616e 6765 2873  for i in range(s
-00009750: 656c 662e 6e6d 6f64 656c 7329 3a0a 2020  elf.nmodels):.  
-00009760: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00009770: 6c66 2e5f 636f 6e76 522e 6170 7065 6e64  lf._convR.append
-00009780: 2873 656c 662e 6d6f 6465 6c73 5b69 5d2e  (self.models[i].
-00009790: 636f 6e76 5229 0a20 2020 2020 2020 2065  convR).        e
-000097a0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-000097b0: 2073 656c 662e 5f63 6f6e 7652 3d73 656c   self._convR=sel
-000097c0: 662e 6d6f 6465 6c73 5b30 5d2e 636f 6e76  f.models[0].conv
-000097d0: 520a 2020 2020 2020 2020 7265 7475 726e  R.        return
-000097e0: 2073 656c 662e 5f63 6f6e 7652 0a0a 2020   self._convR..  
-000097f0: 2020 4063 6f6e 7652 2e73 6574 7465 720a    @convR.setter.
-00009800: 2020 2020 6465 6620 636f 6e76 5228 7365      def convR(se
-00009810: 6c66 2c76 616c 7565 293a 0a20 2020 2020  lf,value):.     
-00009820: 2020 2073 656c 662e 5f63 6f6e 7652 3d76     self._convR=v
-00009830: 616c 7565 0a0a 2020 2020 4070 726f 7065  alue..    @prope
-00009840: 7274 790a 2020 2020 6465 6620 636f 6e76  rty.    def conv
-00009850: 4f76 6572 6c61 7046 7265 7128 7365 6c66  OverlapFreq(self
-00009860: 293a 0a20 2020 2020 2020 2069 6620 7365  ):.        if se
-00009870: 6c66 2e6e 6d6f 6465 6c73 3e31 3a0a 2020  lf.nmodels>1:.  
-00009880: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00009890: 636f 6e76 4f76 6572 6c61 7046 7265 713d  convOverlapFreq=
-000098a0: 5b5d 0a20 2020 2020 2020 2020 2020 2066  [].            f
-000098b0: 6f72 2069 2069 6e20 7261 6e67 6528 7365  or i in range(se
-000098c0: 6c66 2e6e 6d6f 6465 6c73 293a 0a20 2020  lf.nmodels):.   
-000098d0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000098e0: 662e 5f63 6f6e 764f 7665 726c 6170 4672  f._convOverlapFr
-000098f0: 6571 2e61 7070 656e 6428 7365 6c66 2e6d  eq.append(self.m
-00009900: 6f64 656c 735b 695d 2e63 6f6e 764f 7665  odels[i].convOve
-00009910: 726c 6170 4672 6571 290a 2020 2020 2020  rlapFreq).      
-00009920: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00009930: 2020 2020 7365 6c66 2e5f 636f 6e76 4f76      self._convOv
-00009940: 6572 6c61 7046 7265 713d 7365 6c66 2e6d  erlapFreq=self.m
-00009950: 6f64 656c 735b 305d 2e63 6f6e 764f 7665  odels[0].convOve
-00009960: 726c 6170 4672 6571 0a20 2020 2020 2020  rlapFreq.       
-00009970: 2072 6574 7572 6e20 7365 6c66 2e5f 636f   return self._co
-00009980: 6e76 4f76 6572 6c61 7046 7265 710a 0a20  nvOverlapFreq.. 
-00009990: 2020 2040 636f 6e76 4f76 6572 6c61 7046     @convOverlapF
-000099a0: 7265 712e 7365 7474 6572 0a20 2020 2064  req.setter.    d
-000099b0: 6566 2063 6f6e 764f 7665 726c 6170 4672  ef convOverlapFr
-000099c0: 6571 2873 656c 662c 7661 6c75 6529 3a0a  eq(self,value):.
-000099d0: 2020 2020 2020 2020 7365 6c66 2e5f 636f          self._co
-000099e0: 6e76 4f76 6572 6c61 7046 7265 713d 7661  nvOverlapFreq=va
-000099f0: 6c75 650a 0a20 2020 2040 7072 6f70 6572  lue..    @proper
-00009a00: 7479 0a20 2020 2064 6566 2063 6f6e 764f  ty.    def convO
-00009a10: 7665 726c 6170 5761 7665 2873 656c 6629  verlapWave(self)
-00009a20: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
-00009a30: 662e 6e6d 6f64 656c 733e 313a 0a20 2020  f.nmodels>1:.   
-00009a40: 2020 2020 2020 2020 2073 656c 662e 5f63           self._c
-00009a50: 6f6e 764f 7665 726c 6170 5761 7665 3d5b  onvOverlapWave=[
-00009a60: 5d0a 2020 2020 2020 2020 2020 2020 666f  ].            fo
-00009a70: 7220 6920 696e 2072 616e 6765 2873 656c  r i in range(sel
-00009a80: 662e 6e6d 6f64 656c 7329 3a0a 2020 2020  f.nmodels):.    
-00009a90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00009aa0: 2e5f 636f 6e76 4f76 6572 6c61 7057 6176  ._convOverlapWav
-00009ab0: 652e 6170 7065 6e64 2873 656c 662e 6d6f  e.append(self.mo
-00009ac0: 6465 6c73 5b69 5d2e 636f 6e76 4f76 6572  dels[i].convOver
-00009ad0: 6c61 7057 6176 6529 0a20 2020 2020 2020  lapWave).       
-00009ae0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00009af0: 2020 2073 656c 662e 5f63 6f6e 764f 7665     self._convOve
-00009b00: 726c 6170 5761 7665 3d73 656c 662e 6d6f  rlapWave=self.mo
-00009b10: 6465 6c73 5b30 5d2e 636f 6e76 4f76 6572  dels[0].convOver
-00009b20: 6c61 7057 6176 650a 2020 2020 2020 2020  lapWave.        
-00009b30: 7265 7475 726e 2073 656c 662e 5f63 6f6e  return self._con
-00009b40: 764f 7665 726c 6170 5761 7665 0a0a 2020  vOverlapWave..  
-00009b50: 2020 4063 6f6e 764f 7665 726c 6170 5761    @convOverlapWa
-00009b60: 7665 2e73 6574 7465 720a 2020 2020 6465  ve.setter.    de
-00009b70: 6620 636f 6e76 4f76 6572 6c61 7057 6176  f convOverlapWav
-00009b80: 6528 7365 6c66 2c76 616c 7565 293a 0a20  e(self,value):. 
-00009b90: 2020 2020 2020 2073 656c 662e 5f63 6f6e         self._con
-00009ba0: 764f 7665 726c 6170 5761 7665 3d76 616c  vOverlapWave=val
-00009bb0: 7565 0a0a 2020 2020 4070 726f 7065 7274  ue..    @propert
-00009bc0: 790a 2020 2020 6465 6620 6f76 6572 6c61  y.    def overla
-00009bd0: 7046 7265 7128 7365 6c66 293a 0a20 2020  pFreq(self):.   
-00009be0: 2020 2020 2069 6620 7365 6c66 2e6e 6d6f       if self.nmo
-00009bf0: 6465 6c73 3e31 3a0a 2020 2020 2020 2020  dels>1:.        
-00009c00: 2020 2020 7365 6c66 2e5f 6f76 6572 6c61      self._overla
-00009c10: 7046 7265 713d 5b5d 0a20 2020 2020 2020  pFreq=[].       
-00009c20: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
-00009c30: 6e67 6528 7365 6c66 2e6e 6d6f 6465 6c73  nge(self.nmodels
-00009c40: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00009c50: 2020 2073 656c 662e 5f6f 7665 726c 6170     self._overlap
-00009c60: 4672 6571 2e61 7070 656e 6428 7365 6c66  Freq.append(self
-00009c70: 2e6d 6f64 656c 735b 695d 2e6f 7665 726c  .models[i].overl
-00009c80: 6170 4672 6571 290a 2020 2020 2020 2020  apFreq).        
-00009c90: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00009ca0: 2020 7365 6c66 2e5f 6f76 6572 6c61 7046    self._overlapF
-00009cb0: 7265 713d 7365 6c66 2e6d 6f64 656c 735b  req=self.models[
-00009cc0: 305d 2e6f 7665 726c 6170 4672 6571 0a20  0].overlapFreq. 
-00009cd0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00009ce0: 6c66 2e5f 6f76 6572 6c61 7046 7265 710a  lf._overlapFreq.
-00009cf0: 0a20 2020 2040 6f76 6572 6c61 7046 7265  .    @overlapFre
-00009d00: 712e 7365 7474 6572 0a20 2020 2064 6566  q.setter.    def
-00009d10: 206f 7665 726c 6170 4672 6571 2873 656c   overlapFreq(sel
-00009d20: 662c 7661 6c75 6529 3a0a 2020 2020 2020  f,value):.      
-00009d30: 2020 7365 6c66 2e5f 6f76 6572 6c61 7046    self._overlapF
-00009d40: 7265 713d 7661 6c75 650a 0a20 2020 2040  req=value..    @
-00009d50: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-00009d60: 2063 6f6e 764f 7665 726c 6170 4c54 4528   convOverlapLTE(
-00009d70: 7365 6c66 293a 0a20 2020 2020 2020 2069  self):.        i
-00009d80: 6620 7365 6c66 2e6e 6d6f 6465 6c73 3e31  f self.nmodels>1
-00009d90: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00009da0: 6c66 2e5f 636f 6e76 4f76 6572 6c61 704c  lf._convOverlapL
-00009db0: 5445 3d5b 5d0a 2020 2020 2020 2020 2020  TE=[].          
-00009dc0: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
-00009dd0: 2873 656c 662e 6e6d 6f64 656c 7329 3a0a  (self.nmodels):.
-00009de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009df0: 7365 6c66 2e5f 636f 6e76 4f76 6572 6c61  self._convOverla
-00009e00: 704c 5445 2e61 7070 656e 6428 7365 6c66  pLTE.append(self
-00009e10: 2e6d 6f64 656c 735b 695d 2e63 6f6e 764f  .models[i].convO
-00009e20: 7665 726c 6170 4c54 4529 0a20 2020 2020  verlapLTE).     
-00009e30: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00009e40: 2020 2020 2073 656c 662e 5f63 6f6e 764f       self._convO
-00009e50: 7665 726c 6170 4c54 453d 7365 6c66 2e6d  verlapLTE=self.m
-00009e60: 6f64 656c 735b 305d 2e63 6f6e 764f 7665  odels[0].convOve
-00009e70: 726c 6170 4c54 450a 2020 2020 2020 2020  rlapLTE.        
-00009e80: 7265 7475 726e 2073 656c 662e 5f63 6f6e  return self._con
-00009e90: 764f 7665 726c 6170 4c54 450a 0a20 2020  vOverlapLTE..   
-00009ea0: 2040 636f 6e76 4f76 6572 6c61 704c 5445   @convOverlapLTE
-00009eb0: 2e73 6574 7465 720a 2020 2020 6465 6620  .setter.    def 
-00009ec0: 636f 6e76 4f76 6572 6c61 704c 5445 2873  convOverlapLTE(s
-00009ed0: 656c 662c 7661 6c75 6529 3a0a 2020 2020  elf,value):.    
-00009ee0: 2020 2020 7365 6c66 2e5f 636f 6e76 4f76      self._convOv
-00009ef0: 6572 6c61 704c 5445 3d76 616c 7565 0a0a  erlapLTE=value..
-00009f00: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-00009f10: 2020 6465 6620 636f 6e76 4f76 6572 6c61    def convOverla
-00009f20: 704e 4c54 4528 7365 6c66 293a 0a20 2020  pNLTE(self):.   
-00009f30: 2020 2020 2069 6620 7365 6c66 2e6e 6d6f       if self.nmo
-00009f40: 6465 6c73 3e31 3a0a 2020 2020 2020 2020  dels>1:.        
-00009f50: 2020 2020 7365 6c66 2e5f 636f 6e76 4f76      self._convOv
-00009f60: 6572 6c61 704e 4c54 453d 5b5d 0a20 2020  erlapNLTE=[].   
-00009f70: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
-00009f80: 6e20 7261 6e67 6528 7365 6c66 2e6e 6d6f  n range(self.nmo
-00009f90: 6465 6c73 293a 0a20 2020 2020 2020 2020  dels):.         
-00009fa0: 2020 2020 2020 2073 656c 662e 5f63 6f6e         self._con
-00009fb0: 764f 7665 726c 6170 4e4c 5445 2e61 7070  vOverlapNLTE.app
-00009fc0: 656e 6428 7365 6c66 2e6d 6f64 656c 735b  end(self.models[
-00009fd0: 695d 2e63 6f6e 764f 7665 726c 6170 4e4c  i].convOverlapNL
-00009fe0: 5445 290a 2020 2020 2020 2020 656c 7365  TE).        else
-00009ff0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000a000: 6c66 2e5f 636f 6e76 4f76 6572 6c61 704e  lf._convOverlapN
-0000a010: 4c54 453d 7365 6c66 2e6d 6f64 656c 735b  LTE=self.models[
-0000a020: 305d 2e63 6f6e 764f 7665 726c 6170 4e4c  0].convOverlapNL
-0000a030: 5445 0a20 2020 2020 2020 2072 6574 7572  TE.        retur
-0000a040: 6e20 7365 6c66 2e5f 636f 6e76 4f76 6572  n self._convOver
-0000a050: 6c61 704e 4c54 450a 0a20 2020 2040 636f  lapNLTE..    @co
-0000a060: 6e76 4f76 6572 6c61 704e 4c54 452e 7365  nvOverlapNLTE.se
-0000a070: 7474 6572 0a20 2020 2064 6566 2063 6f6e  tter.    def con
-0000a080: 764f 7665 726c 6170 4e4c 5445 2873 656c  vOverlapNLTE(sel
-0000a090: 662c 7661 6c75 6529 3a0a 2020 2020 2020  f,value):.      
-0000a0a0: 2020 7365 6c66 2e5f 636f 6e76 4f76 6572    self._convOver
-0000a0b0: 6c61 704e 4c54 453d 7661 6c75 650a 0a20  lapNLTE=value.. 
-0000a0c0: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-0000a0d0: 2064 6566 206f 7665 726c 6170 4c54 4528   def overlapLTE(
-0000a0e0: 7365 6c66 293a 0a20 2020 2020 2020 2069  self):.        i
-0000a0f0: 6620 7365 6c66 2e6e 6d6f 6465 6c73 3e31  f self.nmodels>1
-0000a100: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000a110: 6c66 2e5f 6f76 6572 6c61 704c 5445 3d5b  lf._overlapLTE=[
-0000a120: 5d0a 2020 2020 2020 2020 2020 2020 666f  ].            fo
-0000a130: 7220 6920 696e 2072 616e 6765 2873 656c  r i in range(sel
-0000a140: 662e 6e6d 6f64 656c 7329 3a0a 2020 2020  f.nmodels):.    
-0000a150: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000a160: 2e5f 6f76 6572 6c61 704c 5445 2e61 7070  ._overlapLTE.app
-0000a170: 656e 6428 7365 6c66 2e6d 6f64 656c 735b  end(self.models[
-0000a180: 695d 2e6f 7665 726c 6170 4c54 4529 0a20  i].overlapLTE). 
-0000a190: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0000a1a0: 2020 2020 2020 2020 2073 656c 662e 5f6f           self._o
-0000a1b0: 7665 726c 6170 4c54 453d 7365 6c66 2e6d  verlapLTE=self.m
-0000a1c0: 6f64 656c 735b 305d 2e6f 7665 726c 6170  odels[0].overlap
-0000a1d0: 4c54 450a 2020 2020 2020 2020 7265 7475  LTE.        retu
-0000a1e0: 726e 2073 656c 662e 5f6f 7665 726c 6170  rn self._overlap
-0000a1f0: 4c54 450a 0a20 2020 2040 6f76 6572 6c61  LTE..    @overla
-0000a200: 704c 5445 2e73 6574 7465 720a 2020 2020  pLTE.setter.    
-0000a210: 6465 6620 6f76 6572 6c61 704c 5445 2873  def overlapLTE(s
-0000a220: 656c 662c 7661 6c75 6529 3a0a 2020 2020  elf,value):.    
-0000a230: 2020 2020 7365 6c66 2e5f 6f76 6572 6c61      self._overla
-0000a240: 704c 5445 3d76 616c 7565 0a0a 2020 2020  pLTE=value..    
-0000a250: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-0000a260: 6620 6f76 6572 6c61 704e 4c54 4528 7365  f overlapNLTE(se
-0000a270: 6c66 293a 0a20 2020 2020 2020 2069 6620  lf):.        if 
-0000a280: 7365 6c66 2e6e 6d6f 6465 6c73 3e31 3a0a  self.nmodels>1:.
-0000a290: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000a2a0: 2e5f 6f76 6572 6c61 704e 4c54 453d 5b5d  ._overlapNLTE=[]
-0000a2b0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-0000a2c0: 2069 2069 6e20 7261 6e67 6528 7365 6c66   i in range(self
-0000a2d0: 2e6e 6d6f 6465 6c73 293a 0a20 2020 2020  .nmodels):.     
-0000a2e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000a2f0: 5f6f 7665 726c 6170 4e4c 5445 2e61 7070  _overlapNLTE.app
-0000a300: 656e 6428 7365 6c66 2e6d 6f64 656c 735b  end(self.models[
-0000a310: 695d 2e6f 7665 726c 6170 4e4c 5445 290a  i].overlapNLTE).
-0000a320: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000a330: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0000a340: 6f76 6572 6c61 704e 4c54 453d 7365 6c66  overlapNLTE=self
-0000a350: 2e6d 6f64 656c 735b 305d 2e6f 7665 726c  .models[0].overl
-0000a360: 6170 4e4c 5445 0a20 2020 2020 2020 2072  apNLTE.        r
-0000a370: 6574 7572 6e20 7365 6c66 2e5f 6f76 6572  eturn self._over
-0000a380: 6c61 704e 4c54 450a 0a20 2020 2040 6f76  lapNLTE..    @ov
-0000a390: 6572 6c61 704e 4c54 452e 7365 7474 6572  erlapNLTE.setter
-0000a3a0: 0a20 2020 2064 6566 206f 7665 726c 6170  .    def overlap
-0000a3b0: 4e4c 5445 2873 656c 662c 7661 6c75 6529  NLTE(self,value)
-0000a3c0: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
-0000a3d0: 6f76 6572 6c61 704e 4c54 453d 7661 6c75  overlapNLTE=valu
-0000a3e0: 650a 0a20 2020 2040 7072 6f70 6572 7479  e..    @property
-0000a3f0: 0a20 2020 2064 6566 206f 7665 726c 6170  .    def overlap
-0000a400: 5461 754c 5445 2873 656c 6629 3a0a 2020  TauLTE(self):.  
-0000a410: 2020 2020 2020 6966 2073 656c 662e 6e6d        if self.nm
-0000a420: 6f64 656c 733e 313a 0a20 2020 2020 2020  odels>1:.       
-0000a430: 2020 2020 2073 656c 662e 5f6f 7665 726c       self._overl
-0000a440: 6170 5461 754c 5445 3d5b 5d0a 2020 2020  apTauLTE=[].    
-0000a450: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-0000a460: 2072 616e 6765 2873 656c 662e 6e6d 6f64   range(self.nmod
-0000a470: 656c 7329 3a0a 2020 2020 2020 2020 2020  els):.          
-0000a480: 2020 2020 2020 7365 6c66 2e5f 6f76 6572        self._over
-0000a490: 6c61 7054 6175 4c54 452e 6170 7065 6e64  lapTauLTE.append
-0000a4a0: 2873 656c 662e 6d6f 6465 6c73 5b69 5d2e  (self.models[i].
-0000a4b0: 6f76 6572 6c61 7054 6175 4c54 4529 0a20  overlapTauLTE). 
-0000a4c0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0000a4d0: 2020 2020 2020 2020 2073 656c 662e 5f6f           self._o
-0000a4e0: 7665 726c 6170 5461 754c 5445 3d73 656c  verlapTauLTE=sel
-0000a4f0: 662e 6d6f 6465 6c73 5b30 5d2e 6f76 6572  f.models[0].over
-0000a500: 6c61 7054 6175 4c54 450a 2020 2020 2020  lapTauLTE.      
-0000a510: 2020 7265 7475 726e 2073 656c 662e 5f6f    return self._o
-0000a520: 7665 726c 6170 5461 754c 5445 0a0a 2020  verlapTauLTE..  
-0000a530: 2020 406f 7665 726c 6170 5461 754c 5445    @overlapTauLTE
-0000a540: 2e73 6574 7465 720a 2020 2020 6465 6620  .setter.    def 
-0000a550: 6f76 6572 6c61 7054 6175 4c54 4528 7365  overlapTauLTE(se
-0000a560: 6c66 2c76 616c 7565 293a 0a20 2020 2020  lf,value):.     
-0000a570: 2020 2073 656c 662e 5f6f 7665 726c 6170     self._overlap
-0000a580: 5461 754c 5445 3d76 616c 7565 0a0a 2020  TauLTE=value..  
-0000a590: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-0000a5a0: 6465 6620 6f76 6572 6c61 7054 6175 4e4c  def overlapTauNL
-0000a5b0: 5445 2873 656c 6629 3a0a 2020 2020 2020  TE(self):.      
-0000a5c0: 2020 6966 2073 656c 662e 6e6d 6f64 656c    if self.nmodel
-0000a5d0: 733e 313a 0a20 2020 2020 2020 2020 2020  s>1:.           
-0000a5e0: 2073 656c 662e 5f6f 7665 726c 6170 5461   self._overlapTa
-0000a5f0: 754e 4c54 453d 5b5d 0a20 2020 2020 2020  uNLTE=[].       
-0000a600: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
-0000a610: 6e67 6528 7365 6c66 2e6e 6d6f 6465 6c73  nge(self.nmodels
-0000a620: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000a630: 2020 2073 656c 662e 5f6f 7665 726c 6170     self._overlap
-0000a640: 5461 754e 4c54 452e 6170 7065 6e64 2873  TauNLTE.append(s
-0000a650: 656c 662e 6d6f 6465 6c73 5b69 5d2e 6f76  elf.models[i].ov
-0000a660: 6572 6c61 7054 6175 4e4c 5445 290a 2020  erlapTauNLTE).  
-0000a670: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0000a680: 2020 2020 2020 2020 7365 6c66 2e5f 6f76          self._ov
-0000a690: 6572 6c61 7054 6175 4e4c 5445 3d73 656c  erlapTauNLTE=sel
-0000a6a0: 662e 6d6f 6465 6c73 5b30 5d2e 6f76 6572  f.models[0].over
-0000a6b0: 6c61 7054 6175 4e4c 5445 0a20 2020 2020  lapTauNLTE.     
-0000a6c0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-0000a6d0: 6f76 6572 6c61 7054 6175 4e4c 5445 0a0a  overlapTauNLTE..
-0000a6e0: 2020 2020 406f 7665 726c 6170 5461 754e      @overlapTauN
-0000a6f0: 4c54 452e 7365 7474 6572 0a20 2020 2064  LTE.setter.    d
-0000a700: 6566 206f 7665 726c 6170 5461 754e 4c54  ef overlapTauNLT
-0000a710: 4528 7365 6c66 2c76 616c 7565 293a 0a20  E(self,value):. 
-0000a720: 2020 2020 2020 2073 656c 662e 5f6f 7665         self._ove
-0000a730: 726c 6170 5461 754e 4c54 453d 7661 6c75  rlapTauNLTE=valu
-0000a740: 650a 0a20 2020 2040 7072 6f70 6572 7479  e..    @property
-0000a750: 0a20 2020 2064 6566 2063 6f6e 764f 7665  .    def convOve
-0000a760: 726c 6170 5228 7365 6c66 293a 0a20 2020  rlapR(self):.   
-0000a770: 2020 2020 2069 6620 7365 6c66 2e6e 6d6f       if self.nmo
-0000a780: 6465 6c73 3e31 3a0a 2020 2020 2020 2020  dels>1:.        
-0000a790: 2020 2020 7365 6c66 2e5f 636f 6e76 4f76      self._convOv
-0000a7a0: 6572 6c61 7052 3d5b 5d0a 2020 2020 2020  erlapR=[].      
-0000a7b0: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
-0000a7c0: 616e 6765 2873 656c 662e 6e6d 6f64 656c  ange(self.nmodel
-0000a7d0: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
-0000a7e0: 2020 2020 7365 6c66 2e5f 636f 6e76 4f76      self._convOv
-0000a7f0: 6572 6c61 7052 2e61 7070 656e 6428 7365  erlapR.append(se
-0000a800: 6c66 2e6d 6f64 656c 735b 695d 2e63 6f6e  lf.models[i].con
-0000a810: 764f 7665 726c 6170 5229 0a20 2020 2020  vOverlapR).     
-0000a820: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000a830: 2020 2020 2073 656c 662e 5f63 6f6e 764f       self._convO
-0000a840: 7665 726c 6170 523d 7365 6c66 2e6d 6f64  verlapR=self.mod
-0000a850: 656c 735b 305d 2e63 6f6e 764f 7665 726c  els[0].convOverl
-0000a860: 6170 520a 2020 2020 2020 2020 7265 7475  apR.        retu
-0000a870: 726e 2073 656c 662e 5f63 6f6e 764f 7665  rn self._convOve
-0000a880: 726c 6170 520a 0a20 2020 2040 636f 6e76  rlapR..    @conv
-0000a890: 4f76 6572 6c61 7052 2e73 6574 7465 720a  OverlapR.setter.
-0000a8a0: 2020 2020 6465 6620 636f 6e76 4f76 6572      def convOver
-0000a8b0: 6c61 7052 2873 656c 662c 7661 6c75 6529  lapR(self,value)
-0000a8c0: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
-0000a8d0: 636f 6e76 4f76 6572 6c61 7052 3d76 616c  convOverlapR=val
-0000a8e0: 7565 0a0a 2020 2020 4070 726f 7065 7274  ue..    @propert
-0000a8f0: 790a 2020 2020 6465 6620 6f76 6572 6c61  y.    def overla
-0000a900: 7052 2873 656c 6629 3a0a 2020 2020 2020  pR(self):.      
-0000a910: 2020 6966 2073 656c 662e 6e6d 6f64 656c    if self.nmodel
-0000a920: 733e 313a 0a20 2020 2020 2020 2020 2020  s>1:.           
-0000a930: 2073 656c 662e 5f6f 7665 726c 6170 523d   self._overlapR=
-0000a940: 5b5d 0a20 2020 2020 2020 2020 2020 2066  [].            f
-0000a950: 6f72 2069 2069 6e20 7261 6e67 6528 7365  or i in range(se
-0000a960: 6c66 2e6e 6d6f 6465 6c73 293a 0a20 2020  lf.nmodels):.   
-0000a970: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000a980: 662e 5f6f 7665 726c 6170 522e 6170 7065  f._overlapR.appe
-0000a990: 6e64 2873 656c 662e 6d6f 6465 6c73 5b69  nd(self.models[i
-0000a9a0: 5d2e 6f76 6572 6c61 7052 290a 2020 2020  ].overlapR).    
-0000a9b0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000a9c0: 2020 2020 2020 7365 6c66 2e5f 6f76 6572        self._over
-0000a9d0: 6c61 7052 3d73 656c 662e 6d6f 6465 6c73  lapR=self.models
-0000a9e0: 5b30 5d2e 6f76 6572 6c61 7052 0a20 2020  [0].overlapR.   
-0000a9f0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0000aa00: 2e5f 6f76 6572 6c61 7052 0a0a 2020 2020  ._overlapR..    
-0000aa10: 406f 7665 726c 6170 522e 7365 7474 6572  @overlapR.setter
-0000aa20: 0a20 2020 2064 6566 206f 7665 726c 6170  .    def overlap
-0000aa30: 5228 7365 6c66 2c76 616c 7565 293a 0a20  R(self,value):. 
-0000aa40: 2020 2020 2020 2073 656c 662e 5f6f 7665         self._ove
-0000aa50: 726c 6170 523d 7661 6c75 650a 0a0a 636c  rlapR=value...cl
-0000aa60: 6173 7320 736c 6162 3a0a 2020 2020 2222  ass slab:.    ""
-0000aa70: 220a 2020 2020 636c 6173 733a 3a20 736c  ".    class:: sl
-0000aa80: 6162 0a20 2020 2043 6c61 7373 2074 6f20  ab.    Class to 
-0000aa90: 686f 6c64 2074 6865 2064 6174 6120 6f66  hold the data of
-0000aaa0: 2069 6e64 6976 6964 7561 6c20 736c 6162   individual slab
-0000aab0: 206d 6f64 656c 730a 2020 2020 2222 220a   models.    """.
-0000aac0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-0000aad0: 5f28 7365 6c66 293a 0a20 2020 2020 2020  _(self):.       
-0000aae0: 2073 656c 662e 7370 6563 6965 735f 6e75   self.species_nu
-0000aaf0: 6d62 6572 3d4e 6f6e 650a 2020 2020 2020  mber=None.      
-0000ab00: 2020 7365 6c66 2e6d 6f64 656c 5f6e 756d    self.model_num
-0000ab10: 6265 723d 4e6f 6e65 0a20 2020 2020 2020  ber=None.       
-0000ab20: 2073 656c 662e 4e48 3d4e 6f6e 650a 2020   self.NH=None.  
-0000ab30: 2020 2020 2020 7365 6c66 2e6e 436f 6c6c        self.nColl
-0000ab40: 3d4e 6f6e 650a 2020 2020 2020 2020 7365  =None.        se
-0000ab50: 6c66 2e6e 653d 4e6f 6e65 0a20 2020 2020  lf.ne=None.     
-0000ab60: 2020 2073 656c 662e 6e48 653d 4e6f 6e65     self.nHe=None
-0000ab70: 0a20 2020 2020 2020 2073 656c 662e 6e48  .        self.nH
-0000ab80: 4949 3d4e 6f6e 650a 2020 2020 2020 2020  II=None.        
-0000ab90: 7365 6c66 2e6e 4849 3d4e 6f6e 650a 2020  self.nHI=None.  
-0000aba0: 2020 2020 2020 7365 6c66 2e6e 4832 3d4e        self.nH2=N
-0000abb0: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
-0000abc0: 2e64 7573 745f 746f 5f67 6173 3d4e 6f6e  .dust_to_gas=Non
-0000abd0: 650a 2020 2020 2020 2020 7365 6c66 2e76  e.        self.v
-0000abe0: 7475 7262 3d4e 6f6e 650a 2020 2020 2020  turb=None.      
-0000abf0: 2020 7365 6c66 2e54 673d 4e6f 6e65 0a20    self.Tg=None. 
-0000ac00: 2020 2020 2020 2073 656c 662e 5464 3d4e         self.Td=N
-0000ac10: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
-0000ac20: 2e73 7065 6369 6573 5f6e 616d 653d 4e6f  .species_name=No
-0000ac30: 6e65 0a20 2020 2020 2020 2073 656c 662e  ne.        self.
-0000ac40: 7370 6563 6965 735f 696e 6465 783d 4e6f  species_index=No
-0000ac50: 6e65 0a20 2020 2020 2020 2073 656c 662e  ne.        self.
-0000ac60: 6162 756e 6461 6e63 653d 4e6f 6e65 0a20  abundance=None. 
-0000ac70: 2020 2020 2020 2073 656c 662e 6476 3d4e         self.dv=N
-0000ac80: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
-0000ac90: 2e6e 6c65 7665 6c73 3d4e 6f6e 650a 2020  .nlevels=None.  
-0000aca0: 2020 2020 2020 7365 6c66 2e6e 6c69 6e65        self.nline
-0000acb0: 733d 4e6f 6e65 0a20 2020 2020 2020 2073  s=None.        s
-0000acc0: 656c 662e 6c69 6e65 6461 7461 3d4e 6f6e  elf.linedata=Non
-0000acd0: 650a 2020 2020 2020 2020 7365 6c66 2e6c  e.        self.l
-0000ace0: 6576 656c 6461 7461 3d4e 6f6e 650a 2020  eveldata=None.  
-0000acf0: 2020 2020 2020 7365 6c66 2e63 6f6e 7657        self.convW
-0000ad00: 6176 656c 656e 6774 683d 4e6f 6e65 0a20  avelength=None. 
-0000ad10: 2020 2020 2020 2073 656c 662e 636f 6e76         self.conv
-0000ad20: 4c54 4566 6c75 783d 4e6f 6e65 0a20 2020  LTEflux=None.   
-0000ad30: 2020 2020 2073 656c 662e 636f 6e76 4e4c       self.convNL
-0000ad40: 5445 666c 7578 3d4e 6f6e 650a 2020 2020  TEflux=None.    
-0000ad50: 2020 2020 7365 6c66 2e63 6f6e 7654 7970      self.convTyp
-0000ad60: 653d 4e6f 6e65 0a20 2020 2020 2020 2073  e=None.        s
-0000ad70: 656c 662e 636f 6e76 523d 4e6f 6e65 0a20  elf.convR=None. 
-0000ad80: 2020 2020 2020 2073 656c 662e 6f76 6572         self.over
-0000ad90: 6c61 704c 5445 3d4e 6f6e 650a 2020 2020  lapLTE=None.    
-0000ada0: 2020 2020 7365 6c66 2e6f 7665 726c 6170      self.overlap
-0000adb0: 4e4c 5445 3d4e 6f6e 650a 2020 2020 2020  NLTE=None.      
-0000adc0: 2020 7365 6c66 2e6f 7665 726c 6170 5461    self.overlapTa
-0000add0: 754c 5445 3d4e 6f6e 650a 2020 2020 2020  uLTE=None.      
-0000ade0: 2020 7365 6c66 2e6f 7665 726c 6170 5461    self.overlapTa
-0000adf0: 754e 4c54 453d 4e6f 6e65 0a20 2020 2020  uNLTE=None.     
-0000ae00: 2020 2073 656c 662e 6f76 6572 6c61 7046     self.overlapF
-0000ae10: 7265 713d 4e6f 6e65 0a20 2020 2020 2020  req=None.       
-0000ae20: 2073 656c 662e 636f 6e76 4f76 6572 6c61   self.convOverla
-0000ae30: 704c 5445 3d4e 6f6e 650a 2020 2020 2020  pLTE=None.      
-0000ae40: 2020 7365 6c66 2e63 6f6e 764f 7665 726c    self.convOverl
-0000ae50: 6170 4e4c 5445 3d4e 6f6e 650a 2020 2020  apNLTE=None.    
-0000ae60: 2020 2020 7365 6c66 2e63 6f6e 764f 7665      self.convOve
-0000ae70: 726c 6170 4672 6571 3d4e 6f6e 650a 2020  rlapFreq=None.  
-0000ae80: 2020 2020 2020 7365 6c66 2e63 6f6e 764f        self.convO
-0000ae90: 7665 726c 6170 5761 7665 3d4e 6f6e 650a  verlapWave=None.
-0000aea0: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-0000aeb0: 764f 7665 726c 6170 523d 3165 350a 2020  vOverlapR=1e5.  
-0000aec0: 2020 2020 2020 7365 6c66 2e6f 7665 726c        self.overl
-0000aed0: 6170 523d 3165 350a 0a20 2020 2064 6566  apR=1e5..    def
-0000aee0: 205f 5f73 7472 5f5f 2873 656c 6629 3a0a   __str__(self):.
-0000aef0: 2020 2020 2020 2020 6f75 7470 7574 3d22          output="
-0000af00: 496e 666f 204d 6f64 656c 3a20 5c6e 220a  Info Model: \n".
-0000af10: 2020 2020 2020 2020 6f75 7470 7574 2b3d          output+=
-0000af20: 2773 7065 6369 6573 5f6e 756d 6265 723d  'species_number=
-0000af30: 2027 0a20 2020 2020 2020 206f 7574 7075   '.        outpu
-0000af40: 742b 3d73 7472 2873 656c 662e 7370 6563  t+=str(self.spec
-0000af50: 6965 735f 6e75 6d62 6572 292b 275c 6e5c  ies_number)+'\n\
-0000af60: 6e27 0a20 2020 2020 2020 206f 7574 7075  n'.        outpu
-0000af70: 742b 3d27 6d6f 6465 6c5f 6e75 6d62 6572  t+='model_number
-0000af80: 2020 3d20 270a 2020 2020 2020 2020 6f75    = '.        ou
-0000af90: 7470 7574 2b3d 7374 7228 7365 6c66 2e6d  tput+=str(self.m
-0000afa0: 6f64 656c 5f6e 756d 6265 7229 2b27 5c6e  odel_number)+'\n
-0000afb0: 5c6e 270a 2020 2020 2020 2020 6f75 7470  \n'.        outp
-0000afc0: 7574 2b3d 274e 4820 2020 2020 2020 2020  ut+='NH         
-0000afd0: 2020 203d 2027 0a20 2020 2020 2020 206f     = '.        o
-0000afe0: 7574 7075 742b 3d73 7472 2873 656c 662e  utput+=str(self.
-0000aff0: 4e48 292b 275c 6e5c 6e27 0a20 2020 2020  NH)+'\n\n'.     
-0000b000: 2020 206f 7574 7075 742b 3d27 6e43 6f6c     output+='nCol
-0000b010: 6c20 2020 2020 2020 2020 3d20 270a 2020  l         = '.  
-0000b020: 2020 2020 2020 6f75 7470 7574 2b3d 7374        output+=st
-0000b030: 7228 7365 6c66 2e6e 436f 6c6c 292b 275c  r(self.nColl)+'\
-0000b040: 6e5c 6e27 0a20 2020 2020 2020 206f 7574  n\n'.        out
-0000b050: 7075 742b 3d27 6e65 2020 2020 2020 2020  put+='ne        
-0000b060: 2020 2020 3d20 270a 2020 2020 2020 2020      = '.        
-0000b070: 6f75 7470 7574 2b3d 7374 7228 7365 6c66  output+=str(self
-0000b080: 2e6e 6529 2b27 5c6e 5c6e 270a 2020 2020  .ne)+'\n\n'.    
-0000b090: 2020 2020 6f75 7470 7574 2b3d 276e 4865      output+='nHe
-0000b0a0: 2020 2020 2020 2020 2020 203d 2027 0a20             = '. 
-0000b0b0: 2020 2020 2020 206f 7574 7075 742b 3d73         output+=s
-0000b0c0: 7472 2873 656c 662e 6e48 6529 2b27 5c6e  tr(self.nHe)+'\n
-0000b0d0: 5c6e 270a 2020 2020 2020 2020 6f75 7470  \n'.        outp
-0000b0e0: 7574 2b3d 276e 4849 4920 2020 2020 2020  ut+='nHII       
-0000b0f0: 2020 203d 2027 0a20 2020 2020 2020 206f     = '.        o
-0000b100: 7574 7075 742b 3d73 7472 2873 656c 662e  utput+=str(self.
-0000b110: 6e48 4949 292b 275c 6e5c 6e27 0a20 2020  nHII)+'\n\n'.   
-0000b120: 2020 2020 206f 7574 7075 742b 3d27 6e48       output+='nH
-0000b130: 4920 2020 2020 2020 2020 2020 3d20 270a  I           = '.
-0000b140: 2020 2020 2020 2020 6f75 7470 7574 2b3d          output+=
-0000b150: 7374 7228 7365 6c66 2e6e 4849 292b 275c  str(self.nHI)+'\
-0000b160: 6e5c 6e27 0a20 2020 2020 2020 206f 7574  n\n'.        out
-0000b170: 7075 742b 3d27 6e48 3220 2020 2020 2020  put+='nH2       
-0000b180: 2020 2020 3d20 270a 2020 2020 2020 2020      = '.        
-0000b190: 6f75 7470 7574 2b3d 7374 7228 7365 6c66  output+=str(self
-0000b1a0: 2e6e 4832 292b 275c 6e5c 6e27 0a20 2020  .nH2)+'\n\n'.   
-0000b1b0: 2020 2020 206f 7574 7075 742b 3d27 6475       output+='du
-0000b1c0: 7374 5f74 6f5f 6761 7320 2020 3d20 270a  st_to_gas   = '.
-0000b1d0: 2020 2020 2020 2020 6f75 7470 7574 2b3d          output+=
-0000b1e0: 7374 7228 7365 6c66 2e64 7573 745f 746f  str(self.dust_to
-0000b1f0: 5f67 6173 292b 275c 6e5c 6e27 0a20 2020  _gas)+'\n\n'.   
-0000b200: 2020 2020 206f 7574 7075 742b 3d27 7674       output+='vt
-0000b210: 7572 6220 2020 2020 2020 2020 3d20 270a  urb         = '.
-0000b220: 2020 2020 2020 2020 6f75 7470 7574 2b3d          output+=
-0000b230: 7374 7228 7365 6c66 2e76 7475 7262 292b  str(self.vturb)+
-0000b240: 275c 6e5c 6e27 0a20 2020 2020 2020 206f  '\n\n'.        o
-0000b250: 7574 7075 742b 3d27 5467 2020 2020 2020  utput+='Tg      
-0000b260: 2020 2020 2020 3d20 270a 2020 2020 2020        = '.      
-0000b270: 2020 6f75 7470 7574 2b3d 7374 7228 7365    output+=str(se
-0000b280: 6c66 2e54 6729 2b27 5c6e 5c6e 270a 2020  lf.Tg)+'\n\n'.  
-0000b290: 2020 2020 2020 6f75 7470 7574 2b3d 2754        output+='T
-0000b2a0: 6420 2020 2020 2020 2020 2020 203d 2027  d            = '
-0000b2b0: 0a20 2020 2020 2020 206f 7574 7075 742b  .        output+
-0000b2c0: 3d73 7472 2873 656c 662e 5464 292b 275c  =str(self.Td)+'\
-0000b2d0: 6e5c 6e27 0a20 2020 2020 2020 206f 7574  n\n'.        out
-0000b2e0: 7075 742b 3d27 7370 6563 6965 735f 6e61  put+='species_na
-0000b2f0: 6d65 2020 203d 2027 0a20 2020 2020 2020  me   = '.       
-0000b300: 206f 7574 7075 742b 3d73 656c 662e 7370   output+=self.sp
-0000b310: 6563 6965 735f 6e61 6d65 2b27 5c6e 5c6e  ecies_name+'\n\n
-0000b320: 270a 2020 2020 2020 2020 6f75 7470 7574  '.        output
-0000b330: 2b3d 2761 6275 6e64 616e 6365 2020 2020  +='abundance    
-0000b340: 203d 2027 0a20 2020 2020 2020 206f 7574   = '.        out
-0000b350: 7075 742b 3d73 7472 2873 656c 662e 6162  put+=str(self.ab
-0000b360: 756e 6461 6e63 6529 2b27 5c6e 5c6e 270a  undance)+'\n\n'.
-0000b370: 2020 2020 2020 2020 6f75 7470 7574 2b3d          output+=
-0000b380: 2764 7620 2020 2020 2020 2020 2020 203d  'dv            =
-0000b390: 2027 0a20 2020 2020 2020 206f 7574 7075   '.        outpu
-0000b3a0: 742b 3d73 7472 2873 656c 662e 6476 292b  t+=str(self.dv)+
-0000b3b0: 275c 6e5c 6e27 0a20 2020 2020 2020 206f  '\n\n'.        o
-0000b3c0: 7574 7075 742b 3d27 6e6c 6576 656c 7320  utput+='nlevels 
-0000b3d0: 2020 2020 2020 3d20 270a 2020 2020 2020        = '.      
-0000b3e0: 2020 6f75 7470 7574 2b3d 7374 7228 7365    output+=str(se
-0000b3f0: 6c66 2e6e 6c65 7665 6c73 292b 275c 6e5c  lf.nlevels)+'\n\
-0000b400: 6e27 0a20 2020 2020 2020 206f 7574 7075  n'.        outpu
-0000b410: 742b 3d27 6e6c 696e 6573 2020 2020 2020  t+='nlines      
-0000b420: 2020 3d20 270a 2020 2020 2020 2020 6f75    = '.        ou
-0000b430: 7470 7574 2b3d 7374 7228 7365 6c66 2e6e  tput+=str(self.n
-0000b440: 6c69 6e65 7329 2b27 5c6e 5c6e 270a 2020  lines)+'\n\n'.  
-0000b450: 2020 2020 2020 6f75 7470 7574 2b3d 2763        output+='c
-0000b460: 6f6e 7654 7970 6520 2020 2020 2020 3d20  onvType       = 
-0000b470: 270a 2020 2020 2020 2020 6f75 7470 7574  '.        output
-0000b480: 2b3d 7374 7228 7365 6c66 2e63 6f6e 7654  +=str(self.convT
-0000b490: 7970 6529 2b27 5c6e 5c6e 270a 2020 2020  ype)+'\n\n'.    
-0000b4a0: 2020 2020 6f75 7470 7574 2b3d 2763 6f6e      output+='con
-0000b4b0: 7652 2020 2020 2020 2020 3d20 270a 2020  vR        = '.  
-0000b4c0: 2020 2020 2020 6f75 7470 7574 2b3d 7374        output+=st
-0000b4d0: 7228 7365 6c66 2e63 6f6e 7652 292b 275c  r(self.convR)+'\
-0000b4e0: 6e5c 6e27 0a20 2020 2020 2020 2072 6574  n\n'.        ret
-0000b4f0: 7572 6e20 6f75 7470 7574 0a0a 2020 2020  urn output..    
-0000b500: 6465 6620 636f 6e76 6f6c 7665 2873 656c  def convolve(sel
-0000b510: 662c 6672 6571 5f62 696e 733d 4e6f 6e65  f,freq_bins=None
-0000b520: 2c52 3d31 2c6c 616d 6264 615f 303d 312c  ,R=1,lambda_0=1,
-0000b530: 6c61 6d62 6461 5f6e 3d31 2c76 723d 3133  lambda_n=1,vr=13
-0000b540: 3030 2c4e 4c54 453d 4661 6c73 652c 636f  00,NLTE=False,co
-0000b550: 6e76 5f74 7970 653d 3129 3a0a 2020 2020  nv_type=1):.    
-0000b560: 2020 2020 743d 2746 4c54 4527 0a20 2020      t='FLTE'.   
-0000b570: 2020 2020 2069 6620 4e4c 5445 3a0a 2020       if NLTE:.  
-0000b580: 2020 2020 2020 2020 2020 743d 2746 4e4c            t='FNL
-0000b590: 5445 270a 2020 2020 2020 2020 6461 3d73  TE'.        da=s
-0000b5a0: 656c 662e 6c69 6e65 6461 7461 0a20 2020  elf.linedata.   
-0000b5b0: 2020 2020 2069 6620 6c61 6d62 6461 5f30       if lambda_0
-0000b5c0: 3d3d 6c61 6d62 6461 5f6e 3a0a 2020 2020  ==lambda_n:.    
-0000b5d0: 2020 2020 2020 2020 6c61 6d62 6461 5f30          lambda_0
-0000b5e0: 3d6e 702e 616d 696e 2864 615b 2747 487a  =np.amin(da['GHz
-0000b5f0: 275d 3e63 2f6c 616d 6264 615f 6e2a 3165  ']>c/lambda_n*1e
-0000b600: 2d33 290a 2020 2020 2020 2020 2020 2020  -3).            
-0000b610: 6c61 6d62 6461 5f6e 3d6e 702e 616d 6178  lambda_n=np.amax
-0000b620: 2864 615b 2747 487a 275d 3e63 2f6c 616d  (da['GHz']>c/lam
-0000b630: 6264 615f 6e2a 3165 2d33 290a 2020 2020  bda_n*1e-3).    
-0000b640: 2020 2020 2020 2020 6c61 6d62 6461 5f30          lambda_0
-0000b650: 3d6c 616d 6264 615f 302a 3130 2a2a 2d30  =lambda_0*10**-0
-0000b660: 2e30 350a 2020 2020 2020 2020 2020 2020  .05.            
-0000b670: 6c61 6d62 6461 5f6e 3d6c 616d 6264 615f  lambda_n=lambda_
-0000b680: 6e2a 3130 2a2a 302e 3035 0a20 2020 2020  n*10**0.05.     
-0000b690: 2020 2064 615f 7265 713d 6461 5b28 6461     da_req=da[(da
-0000b6a0: 5b27 4748 7a27 5d3e 632f 6c61 6d62 6461  ['GHz']>c/lambda
-0000b6b0: 5f6e 2a31 652d 3329 2628 6461 5b27 4748  _n*1e-3)&(da['GH
-0000b6c0: 7a27 5d3c 632f 6c61 6d62 6461 5f30 2a31  z']<c/lambda_0*1
-0000b6d0: 652d 3329 5d0a 2020 2020 2020 2020 6461  e-3)].        da
-0000b6e0: 5f72 6571 2e72 6573 6574 5f69 6e64 6578  _req.reset_index
-0000b6f0: 2864 726f 703d 5472 7565 2c69 6e70 6c61  (drop=True,inpla
-0000b700: 6365 3d54 7275 6529 0a20 2020 2020 2020  ce=True).       
-0000b710: 2069 6620 636f 6e76 5f74 7970 653d 3d31   if conv_type==1
-0000b720: 3a0a 2020 2020 2020 2020 2020 2020 6c2c  :.            l,
-0000b730: 663d 6765 6e65 7261 6c43 6f6e 766f 6c76  f=generalConvolv
-0000b740: 6528 6461 5f72 6571 5b74 5d2c 6461 5f72  e(da_req[t],da_r
-0000b750: 6571 5b27 4748 7a27 5d2c 523d 522c 6c61  eq['GHz'],R=R,la
-0000b760: 6d62 6461 5f30 3d6c 616d 6264 615f 302c  mbda_0=lambda_0,
-0000b770: 6c61 6d62 6461 5f6e 3d6c 616d 6264 615f  lambda_n=lambda_
-0000b780: 6e29 0a20 2020 2020 2020 2065 6c73 653a  n).        else:
-0000b790: 0a20 2020 2020 2020 2020 2020 206c 2c66  .            l,f
-0000b7a0: 3d73 7065 6343 6f6e 766f 6c76 6528 6461  =specConvolve(da
-0000b7b0: 5f72 6571 5b74 5d2c 6461 5f72 6571 5b27  _req[t],da_req['
-0000b7c0: 4748 7a27 5d2c 6672 6571 5f62 696e 733d  GHz'],freq_bins=
-0000b7d0: 6672 6571 5f62 696e 732c 523d 522c 6c61  freq_bins,R=R,la
-0000b7e0: 6d62 6461 5f30 3d6c 616d 6264 615f 302c  mbda_0=lambda_0,
-0000b7f0: 6c61 6d62 6461 5f6e 3d6c 616d 6264 615f  lambda_n=lambda_
-0000b800: 6e2c 7672 3d76 7229 0a20 2020 2020 2020  n,vr=vr).       
-0000b810: 2073 656c 662e 636f 6e76 5761 7665 6c65   self.convWavele
-0000b820: 6e67 7468 3d6c 0a20 2020 2020 2020 2073  ngth=l.        s
-0000b830: 656c 662e 636f 6e76 5479 7065 3d63 6f6e  elf.convType=con
-0000b840: 765f 7479 7065 0a20 2020 2020 2020 2073  v_type.        s
-0000b850: 656c 662e 636f 6e76 523d 520a 2020 2020  elf.convR=R.    
-0000b860: 2020 2020 6966 204e 4c54 453a 0a20 2020      if NLTE:.   
-0000b870: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
-0000b880: 6e76 4e4c 5445 666c 7578 3d66 0a20 2020  nvNLTEflux=f.   
-0000b890: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000b8a0: 2020 2020 2020 2073 656c 662e 636f 6e76         self.conv
-0000b8b0: 4c54 4566 6c75 783d 660a 0a20 2020 2064  LTEflux=f..    d
-0000b8c0: 6566 2063 6f6e 766f 6c76 655f 6f76 6572  ef convolve_over
-0000b8d0: 6c61 7028 7365 6c66 2c52 3d31 2c6c 616d  lap(self,R=1,lam
-0000b8e0: 6264 615f 303d 312c 6c61 6d62 6461 5f6e  bda_0=1,lambda_n
-0000b8f0: 3d31 293a 0a20 2020 2020 2020 2069 6620  =1):.        if 
-0000b900: 6c61 6d62 6461 5f30 3d3d 6c61 6d62 6461  lambda_0==lambda
-0000b910: 5f6e 3a0a 2020 2020 2020 2020 2020 2020  _n:.            
-0000b920: 6c61 6d62 6461 5f30 3d6e 702e 616d 696e  lambda_0=np.amin
-0000b930: 2863 2f73 656c 662e 6f76 6572 6c61 7046  (c/self.overlapF
-0000b940: 7265 712a 3165 2d33 290a 2020 2020 2020  req*1e-3).      
-0000b950: 2020 2020 2020 6c61 6d62 6461 5f6e 3d6e        lambda_n=n
-0000b960: 702e 616d 6178 2863 2f73 656c 662e 6f76  p.amax(c/self.ov
-0000b970: 6572 6c61 7046 7265 712a 3165 2d33 290a  erlapFreq*1e-3).
-0000b980: 2020 2020 2020 2020 2020 2020 6c61 6d62              lamb
-0000b990: 6461 5f30 3d6c 616d 6264 615f 302a 3130  da_0=lambda_0*10
-0000b9a0: 2a2a 2d30 2e30 350a 2020 2020 2020 2020  **-0.05.        
-0000b9b0: 2020 2020 6c61 6d62 6461 5f6e 3d6c 616d      lambda_n=lam
-0000b9c0: 6264 615f 6e2a 3130 2a2a 302e 3035 0a20  bda_n*10**0.05. 
-0000b9d0: 2020 2020 2020 206d 6173 6b3d 2873 656c         mask=(sel
-0000b9e0: 662e 6f76 6572 6c61 7046 7265 713e 632f  f.overlapFreq>c/
-0000b9f0: 6c61 6d62 6461 5f6e 2a31 652d 3329 2628  lambda_n*1e-3)&(
-0000ba00: 7365 6c66 2e6f 7665 726c 6170 4672 6571  self.overlapFreq
-0000ba10: 3c63 2f6c 616d 6264 615f 302a 3165 2d33  <c/lambda_0*1e-3
-0000ba20: 290a 2020 2020 2020 2020 4657 484d 3d73  ).        FWHM=s
-0000ba30: 656c 662e 6f76 6572 6c61 7052 2f52 2f32  elf.overlapR/R/2
-0000ba40: 2e33 3535 0a20 2020 2020 2020 2067 3d47  .355.        g=G
-0000ba50: 6175 7373 6961 6e31 444b 6572 6e65 6c28  aussian1DKernel(
-0000ba60: 7374 6464 6576 3d46 5748 4d2c 6661 6374  stddev=FWHM,fact
-0000ba70: 6f72 3d37 290a 2020 2020 2020 2020 7365  or=7).        se
-0000ba80: 6c66 2e63 6f6e 764f 7665 726c 6170 4c54  lf.convOverlapLT
-0000ba90: 453d 6170 795f 636f 6e76 6f6c 7665 2873  E=apy_convolve(s
-0000baa0: 656c 662e 6f76 6572 6c61 704c 5445 5b6d  elf.overlapLTE[m
-0000bab0: 6173 6b5d 2c67 290a 2020 2020 2020 2020  ask],g).        
-0000bac0: 2320 7365 6c66 2e63 6f6e 764f 7665 726c  # self.convOverl
-0000bad0: 6170 4e4c 5445 3d61 7079 5f63 6f6e 766f  apNLTE=apy_convo
-0000bae0: 6c76 6528 7365 6c66 2e6f 7665 726c 6170  lve(self.overlap
-0000baf0: 4e4c 5445 5b6d 6173 6b5d 2c67 290a 2020  NLTE[mask],g).  
-0000bb00: 2020 2020 2020 7365 6c66 2e63 6f6e 764f        self.convO
-0000bb10: 7665 726c 6170 4672 6571 3d73 656c 662e  verlapFreq=self.
-0000bb20: 6f76 6572 6c61 7046 7265 715b 6d61 736b  overlapFreq[mask
-0000bb30: 5d2a 312e 300a 2020 2020 2020 2020 7365  ]*1.0.        se
-0000bb40: 6c66 2e63 6f6e 764f 7665 726c 6170 5761  lf.convOverlapWa
-0000bb50: 7665 3d63 2f73 656c 662e 636f 6e76 4f76  ve=c/self.convOv
-0000bb60: 6572 6c61 7046 7265 712a 3165 2d33 0a20  erlapFreq*1e-3. 
-0000bb70: 2020 2020 2020 2073 656c 662e 636f 6e76         self.conv
-0000bb80: 4f76 6572 6c61 7052 3d52 0a0a 2020 2020  OverlapR=R..    
-0000bb90: 6465 6620 7368 6f77 2873 656c 6629 3a0a  def show(self):.
-0000bba0: 2020 2020 2020 2020 7072 696e 7428 7365          print(se
-0000bbb0: 6c66 290a 2020 2020 2020 2020 7072 696e  lf).        prin
-0000bbc0: 7428 276c 696e 6544 6174 6120 2020 203d  t('lineData    =
-0000bbd0: 2027 290a 2020 2020 2020 2020 7072 696e   ').        prin
-0000bbe0: 7428 7365 6c66 2e6c 696e 6564 6174 6129  t(self.linedata)
-0000bbf0: 0a20 2020 2020 2020 2070 7269 6e74 2827  .        print('
-0000bc00: 6c65 7665 6c44 6174 6120 2020 3d20 2729  levelData   = ')
-0000bc10: 0a20 2020 2020 2020 2070 7269 6e74 2873  .        print(s
-0000bc20: 656c 662e 6c65 7665 6c64 6174 6129 0a0a  elf.leveldata)..
-0000bc30: 0a63 6c61 7373 2073 6c61 6231 443a 0a20  .class slab1D:. 
-0000bc40: 2020 2022 2222 0a20 2020 2063 6c61 7373     """.    class
-0000bc50: 3a3a 2073 6c61 6231 440a 2020 2020 436c  :: slab1D.    Cl
-0000bc60: 6173 7320 746f 2068 6f6c 6420 7468 6520  ass to hold the 
-0000bc70: 6461 7461 206f 6620 3144 2073 6c61 6220  data of 1D slab 
-0000bc80: 6d6f 6465 6c73 0a20 2020 2022 2222 0a0a  models.    """..
-0000bc90: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-0000bca0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000bcb0: 7365 6c66 2e64 6972 6563 746f 7279 3d4e  self.directory=N
-0000bcc0: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
-0000bcd0: 2e66 6c75 783d 4e6f 6e65 0a20 2020 2020  .flux=None.     
-0000bce0: 2020 2073 656c 662e 6672 6571 7565 6e63     self.frequenc
-0000bcf0: 793d 4e6f 6e65 0a20 2020 2020 2020 2073  y=None.        s
-0000bd00: 656c 662e 4e73 7065 6369 6573 3d4e 6f6e  elf.Nspecies=Non
-0000bd10: 650a 2020 2020 2020 2020 7365 6c66 2e73  e.        self.s
-0000bd20: 7065 6369 6573 3d5b 5d0a 2020 2020 2020  pecies=[].      
-0000bd30: 2020 7365 6c66 2e4e 6772 6964 3d4e 6f6e    self.Ngrid=Non
-0000bd40: 650a 2020 2020 2020 2020 7365 6c66 2e52  e.        self.R
-0000bd50: 3d4e 6f6e 650a 2020 2020 2020 2020 7365  =None.        se
-0000bd60: 6c66 2e67 7269 643d 7064 2e44 6174 6146  lf.grid=pd.DataF
-0000bd70: 7261 6d65 2829 0a20 2020 2020 2020 2073  rame().        s
-0000bd80: 656c 662e 736f 7572 6365 5f66 756e 6374  elf.source_funct
-0000bd90: 696f 6e3d 4e6f 6e65 0a20 2020 2020 2020  ion=None.       
-0000bda0: 2073 656c 662e 736f 7572 6365 5f66 756e   self.source_fun
-0000bdb0: 6374 696f 6e5f 6761 733d 4e6f 6e65 0a20  ction_gas=None. 
-0000bdc0: 2020 2020 2020 2073 656c 662e 7461 755f         self.tau_
-0000bdd0: 6475 7374 3d4e 6f6e 650a 2020 2020 2020  dust=None.      
-0000bde0: 2020 7365 6c66 2e74 6175 5f67 6173 3d4e    self.tau_gas=N
-0000bdf0: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
-0000be00: 2e63 6f6e 7657 6176 656c 656e 6774 683d  .convWavelength=
-0000be10: 4e6f 6e65 0a20 2020 2020 2020 2073 656c  None.        sel
-0000be20: 662e 636f 6e76 4672 6571 7565 6e63 793d  f.convFrequency=
+00006fe0: 5472 7565 2c6f 7665 726c 6170 3d46 616c  True,overlap=Fal
+00006ff0: 7365 293a 0a20 2020 2020 2020 2066 6f72  se):.        for
+00007000: 2069 2c64 2069 6e20 656e 756d 6572 6174   i,d in enumerat
+00007010: 6528 7365 6c66 2e6d 6f64 656c 7329 3a0a  e(self.models):.
+00007020: 2020 2020 2020 2020 2020 2020 6966 2076              if v
+00007030: 6572 626f 7365 3a20 7072 696e 7428 275c  erbose: print('\
+00007040: 6e27 2c69 2b31 2c27 3b20 4d6f 6465 6c20  n',i+1,'; Model 
+00007050: 6e75 6d62 6572 2027 2c73 656c 662e 6d6f  number ',self.mo
+00007060: 6465 6c73 5b69 5d2e 6d6f 6465 6c5f 6e75  dels[i].model_nu
+00007070: 6d62 6572 2c27 3b20 5370 6563 6965 7320  mber,'; Species 
+00007080: 6e75 6d62 6572 2027 2c73 656c 662e 6d6f  number ',self.mo
+00007090: 6465 6c73 5b69 5d2e 7370 6563 6965 735f  dels[i].species_
+000070a0: 6e75 6d62 6572 290a 2020 2020 2020 2020  number).        
+000070b0: 2020 2020 642e 636f 6e76 6f6c 7665 2866      d.convolve(f
+000070c0: 7265 715f 6269 6e73 3d66 7265 715f 6269  req_bins=freq_bi
+000070d0: 6e73 2c52 3d52 2c6c 616d 6264 615f 303d  ns,R=R,lambda_0=
+000070e0: 6c61 6d62 6461 5f30 2c6c 616d 6264 615f  lambda_0,lambda_
+000070f0: 6e3d 6c61 6d62 6461 5f6e 2c76 723d 7672  n=lambda_n,vr=vr
+00007100: 2c4e 4c54 453d 4e4c 5445 2c63 6f6e 765f  ,NLTE=NLTE,conv_
+00007110: 7479 7065 3d63 6f6e 765f 7479 7065 2c6f  type=conv_type,o
+00007120: 7665 726c 6170 3d6f 7665 726c 6170 290a  verlap=overlap).
+00007130: 0a20 2020 2064 6566 2063 6f6e 766f 6c76  .    def convolv
+00007140: 655f 6f76 6572 6c61 7028 7365 6c66 2c52  e_overlap(self,R
+00007150: 3d31 2c6c 616d 6264 615f 303d 312c 6c61  =1,lambda_0=1,la
+00007160: 6d62 6461 5f6e 3d31 2c76 6572 626f 7365  mbda_n=1,verbose
+00007170: 3d54 7275 6529 3a0a 2020 2020 2020 2020  =True):.        
+00007180: 666f 7220 692c 6420 696e 2065 6e75 6d65  for i,d in enume
+00007190: 7261 7465 2873 656c 662e 6d6f 6465 6c73  rate(self.models
+000071a0: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
+000071b0: 6620 7665 7262 6f73 653a 2070 7269 6e74  f verbose: print
+000071c0: 2827 5c6e 272c 692b 312c 273b 204d 6f64  ('\n',i+1,'; Mod
+000071d0: 656c 206e 756d 6265 7220 272c 7365 6c66  el number ',self
+000071e0: 2e6d 6f64 656c 735b 695d 2e6d 6f64 656c  .models[i].model
+000071f0: 5f6e 756d 6265 7229 0a20 2020 2020 2020  _number).       
+00007200: 2020 2020 2064 2e63 6f6e 766f 6c76 655f       d.convolve_
+00007210: 6f76 6572 6c61 7028 523d 522c 6c61 6d62  overlap(R=R,lamb
+00007220: 6461 5f30 3d6c 616d 6264 615f 302c 6c61  da_0=lambda_0,la
+00007230: 6d62 6461 5f6e 3d6c 616d 6264 615f 6e29  mbda_n=lambda_n)
+00007240: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+00007250: 2020 2020 6465 6620 6e6d 6f64 656c 7328      def nmodels(
+00007260: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
+00007270: 656c 662e 5f6e 6d6f 6465 6c73 3d6c 656e  elf._nmodels=len
+00007280: 2873 656c 662e 6d6f 6465 6c73 290a 2020  (self.models).  
+00007290: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+000072a0: 662e 5f6e 6d6f 6465 6c73 0a0a 2020 2020  f._nmodels..    
+000072b0: 406e 6d6f 6465 6c73 2e73 6574 7465 720a  @nmodels.setter.
+000072c0: 2020 2020 6465 6620 6e6d 6f64 656c 7328      def nmodels(
+000072d0: 7365 6c66 2c76 616c 7565 293a 0a20 2020  self,value):.   
+000072e0: 2020 2020 2073 656c 662e 5f6e 6d6f 6465       self._nmode
+000072f0: 6c73 3d76 616c 7565 0a0a 2020 2020 4070  ls=value..    @p
+00007300: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+00007310: 7370 6563 6965 735f 6e75 6d62 6572 2873  species_number(s
+00007320: 656c 6629 3a0a 2020 2020 2020 2020 6966  elf):.        if
+00007330: 2073 656c 662e 6e6d 6f64 656c 733e 313a   self.nmodels>1:
+00007340: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00007350: 662e 5f73 7065 6369 6573 5f6e 756d 6265  f._species_numbe
+00007360: 723d 5b5d 0a20 2020 2020 2020 2020 2020  r=[].           
+00007370: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+00007380: 7365 6c66 2e6e 6d6f 6465 6c73 293a 0a20  self.nmodels):. 
+00007390: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000073a0: 656c 662e 5f73 7065 6369 6573 5f6e 756d  elf._species_num
+000073b0: 6265 722e 6170 7065 6e64 2873 656c 662e  ber.append(self.
+000073c0: 6d6f 6465 6c73 5b69 5d2e 7370 6563 6965  models[i].specie
+000073d0: 735f 6e75 6d62 6572 290a 2020 2020 2020  s_number).      
+000073e0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+000073f0: 2020 2020 7365 6c66 2e5f 7370 6563 6965      self._specie
+00007400: 735f 6e75 6d62 6572 3d73 656c 662e 6d6f  s_number=self.mo
+00007410: 6465 6c73 5b30 5d2e 7370 6563 6965 735f  dels[0].species_
+00007420: 6e75 6d62 6572 0a20 2020 2020 2020 2072  number.        r
+00007430: 6574 7572 6e20 7365 6c66 2e5f 7370 6563  eturn self._spec
+00007440: 6965 735f 6e75 6d62 6572 0a0a 2020 2020  ies_number..    
+00007450: 4073 7065 6369 6573 5f6e 756d 6265 722e  @species_number.
+00007460: 7365 7474 6572 0a20 2020 2064 6566 2073  setter.    def s
+00007470: 7065 6369 6573 5f6e 756d 6265 7228 7365  pecies_number(se
+00007480: 6c66 2c76 616c 7565 293a 0a20 2020 2020  lf,value):.     
+00007490: 2020 2073 656c 662e 5f73 7065 6369 6573     self._species
+000074a0: 5f6e 756d 6265 723d 7661 6c75 650a 0a20  _number=value.. 
+000074b0: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+000074c0: 2064 6566 206d 6f64 656c 5f6e 756d 6265   def model_numbe
+000074d0: 7228 7365 6c66 293a 0a20 2020 2020 2020  r(self):.       
+000074e0: 2069 6620 7365 6c66 2e6e 6d6f 6465 6c73   if self.nmodels
+000074f0: 3e31 3a0a 2020 2020 2020 2020 2020 2020  >1:.            
+00007500: 7365 6c66 2e5f 6d6f 6465 6c5f 6e75 6d62  self._model_numb
+00007510: 6572 3d5b 5d0a 2020 2020 2020 2020 2020  er=[].          
+00007520: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
+00007530: 2873 656c 662e 6e6d 6f64 656c 7329 3a0a  (self.nmodels):.
+00007540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007550: 7365 6c66 2e5f 6d6f 6465 6c5f 6e75 6d62  self._model_numb
+00007560: 6572 2e61 7070 656e 6428 7365 6c66 2e6d  er.append(self.m
+00007570: 6f64 656c 735b 695d 2e6d 6f64 656c 5f6e  odels[i].model_n
+00007580: 756d 6265 7229 0a20 2020 2020 2020 2065  umber).        e
+00007590: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+000075a0: 2073 656c 662e 5f6d 6f64 656c 5f6e 756d   self._model_num
+000075b0: 6265 723d 7365 6c66 2e6d 6f64 656c 735b  ber=self.models[
+000075c0: 305d 2e6d 6f64 656c 5f6e 756d 6265 720a  0].model_number.
+000075d0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+000075e0: 656c 662e 5f6d 6f64 656c 5f6e 756d 6265  elf._model_numbe
+000075f0: 720a 0a20 2020 2040 6d6f 6465 6c5f 6e75  r..    @model_nu
+00007600: 6d62 6572 2e73 6574 7465 720a 2020 2020  mber.setter.    
+00007610: 6465 6620 6d6f 6465 6c5f 6e75 6d62 6572  def model_number
+00007620: 2873 656c 662c 7661 6c75 6529 3a0a 2020  (self,value):.  
+00007630: 2020 2020 2020 7365 6c66 2e5f 6d6f 6465        self._mode
+00007640: 6c5f 6e75 6d62 6572 3d76 616c 7565 0a0a  l_number=value..
+00007650: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+00007660: 2020 6465 6620 4e48 2873 656c 6629 3a0a    def NH(self):.
+00007670: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00007680: 6e6d 6f64 656c 733e 313a 0a20 2020 2020  nmodels>1:.     
+00007690: 2020 2020 2020 2073 656c 662e 5f4e 483d         self._NH=
+000076a0: 5b5d 0a20 2020 2020 2020 2020 2020 2066  [].            f
+000076b0: 6f72 2069 2069 6e20 7261 6e67 6528 7365  or i in range(se
+000076c0: 6c66 2e6e 6d6f 6465 6c73 293a 0a20 2020  lf.nmodels):.   
+000076d0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000076e0: 662e 5f4e 482e 6170 7065 6e64 2873 656c  f._NH.append(sel
+000076f0: 662e 6d6f 6465 6c73 5b69 5d2e 4e48 290a  f.models[i].NH).
+00007700: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00007710: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00007720: 4e48 3d73 656c 662e 6d6f 6465 6c73 5b30  NH=self.models[0
+00007730: 5d2e 4e48 0a20 2020 2020 2020 2072 6574  ].NH.        ret
+00007740: 7572 6e20 7365 6c66 2e5f 4e48 0a0a 2020  urn self._NH..  
+00007750: 2020 404e 482e 7365 7474 6572 0a20 2020    @NH.setter.   
+00007760: 2064 6566 204e 4828 7365 6c66 2c76 616c   def NH(self,val
+00007770: 7565 293a 0a20 2020 2020 2020 2073 656c  ue):.        sel
+00007780: 662e 5f4e 483d 7661 6c75 650a 0a20 2020  f._NH=value..   
+00007790: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
+000077a0: 6566 206e 436f 6c6c 2873 656c 6629 3a0a  ef nColl(self):.
+000077b0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000077c0: 6e6d 6f64 656c 733e 313a 0a20 2020 2020  nmodels>1:.     
+000077d0: 2020 2020 2020 2073 656c 662e 5f6e 436f         self._nCo
+000077e0: 6c6c 3d5b 5d0a 2020 2020 2020 2020 2020  ll=[].          
+000077f0: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
+00007800: 2873 656c 662e 6e6d 6f64 656c 7329 3a0a  (self.nmodels):.
+00007810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007820: 7365 6c66 2e5f 6e43 6f6c 6c2e 6170 7065  self._nColl.appe
+00007830: 6e64 2873 656c 662e 6d6f 6465 6c73 5b69  nd(self.models[i
+00007840: 5d2e 6e43 6f6c 6c29 0a20 2020 2020 2020  ].nColl).       
+00007850: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00007860: 2020 2073 656c 662e 5f6e 436f 6c6c 3d73     self._nColl=s
+00007870: 656c 662e 6d6f 6465 6c73 5b30 5d2e 6e43  elf.models[0].nC
+00007880: 6f6c 6c0a 2020 2020 2020 2020 7265 7475  oll.        retu
+00007890: 726e 2073 656c 662e 5f6e 436f 6c6c 0a0a  rn self._nColl..
+000078a0: 2020 2020 406e 436f 6c6c 2e73 6574 7465      @nColl.sette
+000078b0: 720a 2020 2020 6465 6620 6e43 6f6c 6c28  r.    def nColl(
+000078c0: 7365 6c66 2c76 616c 7565 293a 0a20 2020  self,value):.   
+000078d0: 2020 2020 2073 656c 662e 5f6e 436f 6c6c       self._nColl
+000078e0: 3d76 616c 7565 0a0a 2020 2020 4070 726f  =value..    @pro
+000078f0: 7065 7274 790a 2020 2020 6465 6620 6e65  perty.    def ne
+00007900: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00007910: 6966 2073 656c 662e 6e6d 6f64 656c 733e  if self.nmodels>
+00007920: 313a 0a20 2020 2020 2020 2020 2020 2073  1:.            s
+00007930: 656c 662e 5f6e 653d 5b5d 0a20 2020 2020  elf._ne=[].     
+00007940: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+00007950: 7261 6e67 6528 7365 6c66 2e6e 6d6f 6465  range(self.nmode
+00007960: 6c73 293a 0a20 2020 2020 2020 2020 2020  ls):.           
+00007970: 2020 2020 2073 656c 662e 5f6e 652e 6170       self._ne.ap
+00007980: 7065 6e64 2873 656c 662e 6d6f 6465 6c73  pend(self.models
+00007990: 5b69 5d2e 6e65 290a 2020 2020 2020 2020  [i].ne).        
+000079a0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+000079b0: 2020 7365 6c66 2e5f 6e65 3d73 656c 662e    self._ne=self.
+000079c0: 6d6f 6465 6c73 5b30 5d2e 6e65 0a20 2020  models[0].ne.   
+000079d0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+000079e0: 2e5f 6e65 0a0a 2020 2020 406e 652e 7365  ._ne..    @ne.se
+000079f0: 7474 6572 0a20 2020 2064 6566 206e 6528  tter.    def ne(
+00007a00: 7365 6c66 2c76 616c 7565 293a 0a20 2020  self,value):.   
+00007a10: 2020 2020 2073 656c 662e 5f6e 653d 7661       self._ne=va
+00007a20: 6c75 650a 0a20 2020 2040 7072 6f70 6572  lue..    @proper
+00007a30: 7479 0a20 2020 2064 6566 206e 4865 2873  ty.    def nHe(s
+00007a40: 656c 6629 3a0a 2020 2020 2020 2020 6966  elf):.        if
+00007a50: 2073 656c 662e 6e6d 6f64 656c 733e 313a   self.nmodels>1:
+00007a60: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00007a70: 662e 5f6e 4865 3d5b 5d0a 2020 2020 2020  f._nHe=[].      
+00007a80: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
+00007a90: 616e 6765 2873 656c 662e 6e6d 6f64 656c  ange(self.nmodel
+00007aa0: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+00007ab0: 2020 2020 7365 6c66 2e5f 6e48 652e 6170      self._nHe.ap
+00007ac0: 7065 6e64 2873 656c 662e 6d6f 6465 6c73  pend(self.models
+00007ad0: 5b69 5d2e 6e48 6529 0a20 2020 2020 2020  [i].nHe).       
+00007ae0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00007af0: 2020 2073 656c 662e 5f6e 4865 3d73 656c     self._nHe=sel
+00007b00: 662e 6d6f 6465 6c73 5b30 5d2e 6e48 650a  f.models[0].nHe.
+00007b10: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00007b20: 656c 662e 5f6e 4865 0a0a 2020 2020 406e  elf._nHe..    @n
+00007b30: 4865 2e73 6574 7465 720a 2020 2020 6465  He.setter.    de
+00007b40: 6620 6e48 6528 7365 6c66 2c76 616c 7565  f nHe(self,value
+00007b50: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+00007b60: 5f6e 4865 3d76 616c 7565 0a0a 2020 2020  _nHe=value..    
+00007b70: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+00007b80: 6620 6e48 4949 2873 656c 6629 3a0a 2020  f nHII(self):.  
+00007b90: 2020 2020 2020 6966 2073 656c 662e 6e6d        if self.nm
+00007ba0: 6f64 656c 733e 313a 0a20 2020 2020 2020  odels>1:.       
+00007bb0: 2020 2020 2073 656c 662e 5f6e 4849 493d       self._nHII=
+00007bc0: 5b5d 0a20 2020 2020 2020 2020 2020 2066  [].            f
+00007bd0: 6f72 2069 2069 6e20 7261 6e67 6528 7365  or i in range(se
+00007be0: 6c66 2e6e 6d6f 6465 6c73 293a 0a20 2020  lf.nmodels):.   
+00007bf0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00007c00: 662e 5f6e 4849 492e 6170 7065 6e64 2873  f._nHII.append(s
+00007c10: 656c 662e 6d6f 6465 6c73 5b69 5d2e 6e48  elf.models[i].nH
+00007c20: 4949 290a 2020 2020 2020 2020 656c 7365  II).        else
+00007c30: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00007c40: 6c66 2e5f 6e48 4949 3d73 656c 662e 6d6f  lf._nHII=self.mo
+00007c50: 6465 6c73 5b30 5d2e 6e48 4949 0a20 2020  dels[0].nHII.   
+00007c60: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00007c70: 2e5f 6e48 4949 0a0a 2020 2020 406e 4849  ._nHII..    @nHI
+00007c80: 492e 7365 7474 6572 0a20 2020 2064 6566  I.setter.    def
+00007c90: 206e 4849 4928 7365 6c66 2c76 616c 7565   nHII(self,value
+00007ca0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+00007cb0: 5f6e 4849 493d 7661 6c75 650a 0a20 2020  _nHII=value..   
+00007cc0: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
+00007cd0: 6566 206e 4849 2873 656c 6629 3a0a 2020  ef nHI(self):.  
+00007ce0: 2020 2020 2020 6966 2073 656c 662e 6e6d        if self.nm
+00007cf0: 6f64 656c 733e 313a 0a20 2020 2020 2020  odels>1:.       
+00007d00: 2020 2020 2073 656c 662e 5f6e 4849 3d5b       self._nHI=[
+00007d10: 5d0a 2020 2020 2020 2020 2020 2020 666f  ].            fo
+00007d20: 7220 6920 696e 2072 616e 6765 2873 656c  r i in range(sel
+00007d30: 662e 6e6d 6f64 656c 7329 3a0a 2020 2020  f.nmodels):.    
+00007d40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00007d50: 2e5f 6e48 492e 6170 7065 6e64 2873 656c  ._nHI.append(sel
+00007d60: 662e 6d6f 6465 6c73 5b69 5d2e 6e48 4929  f.models[i].nHI)
+00007d70: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00007d80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00007d90: 5f6e 4849 3d73 656c 662e 6d6f 6465 6c73  _nHI=self.models
+00007da0: 5b30 5d2e 6e48 490a 2020 2020 2020 2020  [0].nHI.        
+00007db0: 7265 7475 726e 2073 656c 662e 5f6e 4849  return self._nHI
+00007dc0: 0a0a 2020 2020 406e 4849 2e73 6574 7465  ..    @nHI.sette
+00007dd0: 720a 2020 2020 6465 6620 6e48 4928 7365  r.    def nHI(se
+00007de0: 6c66 2c76 616c 7565 293a 0a20 2020 2020  lf,value):.     
+00007df0: 2020 2073 656c 662e 5f6e 4849 3d76 616c     self._nHI=val
+00007e00: 7565 0a0a 2020 2020 4070 726f 7065 7274  ue..    @propert
+00007e10: 790a 2020 2020 6465 6620 6e48 3228 7365  y.    def nH2(se
+00007e20: 6c66 293a 0a20 2020 2020 2020 2069 6620  lf):.        if 
+00007e30: 7365 6c66 2e6e 6d6f 6465 6c73 3e31 3a0a  self.nmodels>1:.
+00007e40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00007e50: 2e5f 6e48 323d 5b5d 0a20 2020 2020 2020  ._nH2=[].       
+00007e60: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
+00007e70: 6e67 6528 7365 6c66 2e6e 6d6f 6465 6c73  nge(self.nmodels
+00007e80: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00007e90: 2020 2073 656c 662e 5f6e 4832 2e61 7070     self._nH2.app
+00007ea0: 656e 6428 7365 6c66 2e6d 6f64 656c 735b  end(self.models[
+00007eb0: 695d 2e6e 4832 290a 2020 2020 2020 2020  i].nH2).        
+00007ec0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00007ed0: 2020 7365 6c66 2e5f 6e48 323d 7365 6c66    self._nH2=self
+00007ee0: 2e6d 6f64 656c 735b 305d 2e6e 4832 0a20  .models[0].nH2. 
+00007ef0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00007f00: 6c66 2e5f 6e48 320a 0a20 2020 2040 6e48  lf._nH2..    @nH
+00007f10: 322e 7365 7474 6572 0a20 2020 2064 6566  2.setter.    def
+00007f20: 206e 4832 2873 656c 662c 7661 6c75 6529   nH2(self,value)
+00007f30: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
+00007f40: 6e48 323d 7661 6c75 650a 0a20 2020 2040  nH2=value..    @
+00007f50: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+00007f60: 2064 7573 745f 746f 5f67 6173 2873 656c   dust_to_gas(sel
+00007f70: 6629 3a0a 2020 2020 2020 2020 6966 2073  f):.        if s
+00007f80: 656c 662e 6e6d 6f64 656c 733e 313a 0a20  elf.nmodels>1:. 
+00007f90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00007fa0: 5f64 7573 745f 746f 5f67 6173 3d5b 5d0a  _dust_to_gas=[].
+00007fb0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00007fc0: 6920 696e 2072 616e 6765 2873 656c 662e  i in range(self.
+00007fd0: 6e6d 6f64 656c 7329 3a0a 2020 2020 2020  nmodels):.      
+00007fe0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00007ff0: 6475 7374 5f74 6f5f 6761 732e 6170 7065  dust_to_gas.appe
+00008000: 6e64 2873 656c 662e 6d6f 6465 6c73 5b69  nd(self.models[i
+00008010: 5d2e 6475 7374 5f74 6f5f 6761 7329 0a20  ].dust_to_gas). 
+00008020: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00008030: 2020 2020 2020 2020 2073 656c 662e 5f64           self._d
+00008040: 7573 745f 746f 5f67 6173 3d73 656c 662e  ust_to_gas=self.
+00008050: 6d6f 6465 6c73 5b30 5d2e 6475 7374 5f74  models[0].dust_t
+00008060: 6f5f 6761 730a 2020 2020 2020 2020 7265  o_gas.        re
+00008070: 7475 726e 2073 656c 662e 5f64 7573 745f  turn self._dust_
+00008080: 746f 5f67 6173 0a0a 2020 2020 4064 7573  to_gas..    @dus
+00008090: 745f 746f 5f67 6173 2e73 6574 7465 720a  t_to_gas.setter.
+000080a0: 2020 2020 6465 6620 6475 7374 5f74 6f5f      def dust_to_
+000080b0: 6761 7328 7365 6c66 2c76 616c 7565 293a  gas(self,value):
+000080c0: 0a20 2020 2020 2020 2073 656c 662e 5f64  .        self._d
+000080d0: 7573 745f 746f 5f67 6173 3d76 616c 7565  ust_to_gas=value
+000080e0: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+000080f0: 2020 2020 6465 6620 7674 7572 6228 7365      def vturb(se
+00008100: 6c66 293a 0a20 2020 2020 2020 2069 6620  lf):.        if 
+00008110: 7365 6c66 2e6e 6d6f 6465 6c73 3e31 3a0a  self.nmodels>1:.
+00008120: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00008130: 2e5f 7674 7572 623d 5b5d 0a20 2020 2020  ._vturb=[].     
+00008140: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+00008150: 7261 6e67 6528 7365 6c66 2e6e 6d6f 6465  range(self.nmode
+00008160: 6c73 293a 0a20 2020 2020 2020 2020 2020  ls):.           
+00008170: 2020 2020 2073 656c 662e 5f76 7475 7262       self._vturb
+00008180: 2e61 7070 656e 6428 7365 6c66 2e6d 6f64  .append(self.mod
+00008190: 656c 735b 695d 2e76 7475 7262 290a 2020  els[i].vturb).  
+000081a0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+000081b0: 2020 2020 2020 2020 7365 6c66 2e5f 7674          self._vt
+000081c0: 7572 623d 7365 6c66 2e6d 6f64 656c 735b  urb=self.models[
+000081d0: 305d 2e76 7475 7262 0a20 2020 2020 2020  0].vturb.       
+000081e0: 2072 6574 7572 6e20 7365 6c66 2e5f 7674   return self._vt
+000081f0: 7572 620a 0a20 2020 2040 7674 7572 622e  urb..    @vturb.
+00008200: 7365 7474 6572 0a20 2020 2064 6566 2076  setter.    def v
+00008210: 7475 7262 2873 656c 662c 7661 6c75 6529  turb(self,value)
+00008220: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
+00008230: 7674 7572 623d 7661 6c75 650a 0a20 2020  vturb=value..   
+00008240: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
+00008250: 6566 2054 6728 7365 6c66 293a 0a20 2020  ef Tg(self):.   
+00008260: 2020 2020 2069 6620 7365 6c66 2e6e 6d6f       if self.nmo
+00008270: 6465 6c73 3e31 3a0a 2020 2020 2020 2020  dels>1:.        
+00008280: 2020 2020 7365 6c66 2e5f 5467 3d5b 5d0a      self._Tg=[].
+00008290: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000082a0: 6920 696e 2072 616e 6765 2873 656c 662e  i in range(self.
+000082b0: 6e6d 6f64 656c 7329 3a0a 2020 2020 2020  nmodels):.      
+000082c0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+000082d0: 5467 2e61 7070 656e 6428 7365 6c66 2e6d  Tg.append(self.m
+000082e0: 6f64 656c 735b 695d 2e54 6729 0a20 2020  odels[i].Tg).   
+000082f0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00008300: 2020 2020 2020 2073 656c 662e 5f54 673d         self._Tg=
+00008310: 7365 6c66 2e6d 6f64 656c 735b 305d 2e54  self.models[0].T
+00008320: 670a 2020 2020 2020 2020 7265 7475 726e  g.        return
+00008330: 2073 656c 662e 5f54 670a 0a20 2020 2040   self._Tg..    @
+00008340: 5467 2e73 6574 7465 720a 2020 2020 6465  Tg.setter.    de
+00008350: 6620 5467 2873 656c 662c 7661 6c75 6529  f Tg(self,value)
+00008360: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
+00008370: 5467 3d76 616c 7565 0a0a 2020 2020 4070  Tg=value..    @p
+00008380: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+00008390: 5464 2873 656c 6629 3a0a 2020 2020 2020  Td(self):.      
+000083a0: 2020 6966 2073 656c 662e 6e6d 6f64 656c    if self.nmodel
+000083b0: 733e 313a 0a20 2020 2020 2020 2020 2020  s>1:.           
+000083c0: 2073 656c 662e 5f54 643d 5b5d 0a20 2020   self._Td=[].   
+000083d0: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
+000083e0: 6e20 7261 6e67 6528 7365 6c66 2e6e 6d6f  n range(self.nmo
+000083f0: 6465 6c73 293a 0a20 2020 2020 2020 2020  dels):.         
+00008400: 2020 2020 2020 2073 656c 662e 5f54 642e         self._Td.
+00008410: 6170 7065 6e64 2873 656c 662e 6d6f 6465  append(self.mode
+00008420: 6c73 5b69 5d2e 5464 290a 2020 2020 2020  ls[i].Td).      
+00008430: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00008440: 2020 2020 7365 6c66 2e5f 5464 3d73 656c      self._Td=sel
+00008450: 662e 6d6f 6465 6c73 5b30 5d2e 5464 0a20  f.models[0].Td. 
+00008460: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00008470: 6c66 2e5f 5464 0a0a 2020 2020 4054 642e  lf._Td..    @Td.
+00008480: 7365 7474 6572 0a20 2020 2064 6566 2054  setter.    def T
+00008490: 6428 7365 6c66 2c76 616c 7565 293a 0a20  d(self,value):. 
+000084a0: 2020 2020 2020 2073 656c 662e 5f54 643d         self._Td=
+000084b0: 7661 6c75 650a 0a20 2020 2040 7072 6f70  value..    @prop
+000084c0: 6572 7479 0a20 2020 2064 6566 2073 7065  erty.    def spe
+000084d0: 6369 6573 5f6e 616d 6528 7365 6c66 293a  cies_name(self):
+000084e0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+000084f0: 2e6e 6d6f 6465 6c73 3e31 3a0a 2020 2020  .nmodels>1:.    
+00008500: 2020 2020 2020 2020 7365 6c66 2e5f 7370          self._sp
+00008510: 6563 6965 735f 6e61 6d65 3d5b 5d0a 2020  ecies_name=[].  
+00008520: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
+00008530: 696e 2072 616e 6765 2873 656c 662e 6e6d  in range(self.nm
+00008540: 6f64 656c 7329 3a0a 2020 2020 2020 2020  odels):.        
+00008550: 2020 2020 2020 2020 7365 6c66 2e5f 7370          self._sp
+00008560: 6563 6965 735f 6e61 6d65 2e61 7070 656e  ecies_name.appen
+00008570: 6428 7365 6c66 2e6d 6f64 656c 735b 695d  d(self.models[i]
+00008580: 2e73 7065 6369 6573 5f6e 616d 6529 0a20  .species_name). 
+00008590: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+000085a0: 2020 2020 2020 2020 2073 656c 662e 5f73           self._s
+000085b0: 7065 6369 6573 5f6e 616d 653d 7365 6c66  pecies_name=self
+000085c0: 2e6d 6f64 656c 735b 305d 2e73 7065 6369  .models[0].speci
+000085d0: 6573 5f6e 616d 650a 2020 2020 2020 2020  es_name.        
+000085e0: 7265 7475 726e 2073 656c 662e 5f73 7065  return self._spe
+000085f0: 6369 6573 5f6e 616d 650a 0a20 2020 2040  cies_name..    @
+00008600: 7370 6563 6965 735f 6e61 6d65 2e73 6574  species_name.set
+00008610: 7465 720a 2020 2020 6465 6620 7370 6563  ter.    def spec
+00008620: 6965 735f 6e61 6d65 2873 656c 662c 7661  ies_name(self,va
+00008630: 6c75 6529 3a0a 2020 2020 2020 2020 7365  lue):.        se
+00008640: 6c66 2e5f 7370 6563 6965 735f 6e61 6d65  lf._species_name
+00008650: 3d76 616c 7565 0a0a 2020 2020 4070 726f  =value..    @pro
+00008660: 7065 7274 790a 2020 2020 6465 6620 7370  perty.    def sp
+00008670: 6563 6965 735f 696e 6465 7828 7365 6c66  ecies_index(self
+00008680: 293a 0a20 2020 2020 2020 2069 6620 7365  ):.        if se
+00008690: 6c66 2e6e 6d6f 6465 6c73 3e31 3a0a 2020  lf.nmodels>1:.  
+000086a0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+000086b0: 7370 6563 6965 735f 696e 6465 783d 5b5d  species_index=[]
+000086c0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+000086d0: 2069 2069 6e20 7261 6e67 6528 7365 6c66   i in range(self
+000086e0: 2e6e 6d6f 6465 6c73 293a 0a20 2020 2020  .nmodels):.     
+000086f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00008700: 5f73 7065 6369 6573 5f69 6e64 6578 2e61  _species_index.a
+00008710: 7070 656e 6428 7365 6c66 2e6d 6f64 656c  ppend(self.model
+00008720: 735b 695d 2e73 7065 6369 6573 5f69 6e64  s[i].species_ind
+00008730: 6578 290a 2020 2020 2020 2020 656c 7365  ex).        else
+00008740: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00008750: 6c66 2e5f 7370 6563 6965 735f 696e 6465  lf._species_inde
+00008760: 783d 7365 6c66 2e6d 6f64 656c 735b 305d  x=self.models[0]
+00008770: 2e73 7065 6369 6573 5f69 6e64 6578 0a20  .species_index. 
+00008780: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00008790: 6c66 2e5f 7370 6563 6965 735f 696e 6465  lf._species_inde
+000087a0: 780a 0a20 2020 2040 7370 6563 6965 735f  x..    @species_
+000087b0: 696e 6465 782e 7365 7474 6572 0a20 2020  index.setter.   
+000087c0: 2064 6566 2073 7065 6369 6573 5f69 6e64   def species_ind
+000087d0: 6578 2873 656c 662c 7661 6c75 6529 3a0a  ex(self,value):.
+000087e0: 2020 2020 2020 2020 7365 6c66 2e5f 7370          self._sp
+000087f0: 6563 6965 735f 696e 6465 783d 7661 6c75  ecies_index=valu
+00008800: 650a 0a20 2020 2040 7072 6f70 6572 7479  e..    @property
+00008810: 0a20 2020 2064 6566 2061 6275 6e64 616e  .    def abundan
+00008820: 6365 2873 656c 6629 3a0a 2020 2020 2020  ce(self):.      
+00008830: 2020 6966 2073 656c 662e 6e6d 6f64 656c    if self.nmodel
+00008840: 733e 313a 0a20 2020 2020 2020 2020 2020  s>1:.           
+00008850: 2073 656c 662e 5f61 6275 6e64 616e 6365   self._abundance
+00008860: 3d5b 5d0a 2020 2020 2020 2020 2020 2020  =[].            
+00008870: 666f 7220 6920 696e 2072 616e 6765 2873  for i in range(s
+00008880: 656c 662e 6e6d 6f64 656c 7329 3a0a 2020  elf.nmodels):.  
+00008890: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000088a0: 6c66 2e5f 6162 756e 6461 6e63 652e 6170  lf._abundance.ap
+000088b0: 7065 6e64 2873 656c 662e 6d6f 6465 6c73  pend(self.models
+000088c0: 5b69 5d2e 6162 756e 6461 6e63 6529 0a20  [i].abundance). 
+000088d0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+000088e0: 2020 2020 2020 2020 2073 656c 662e 5f61           self._a
+000088f0: 6275 6e64 616e 6365 3d73 656c 662e 6d6f  bundance=self.mo
+00008900: 6465 6c73 5b30 5d2e 6162 756e 6461 6e63  dels[0].abundanc
+00008910: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
+00008920: 2073 656c 662e 5f61 6275 6e64 616e 6365   self._abundance
+00008930: 0a0a 2020 2020 4061 6275 6e64 616e 6365  ..    @abundance
+00008940: 2e73 6574 7465 720a 2020 2020 6465 6620  .setter.    def 
+00008950: 6162 756e 6461 6e63 6528 7365 6c66 2c76  abundance(self,v
+00008960: 616c 7565 293a 0a20 2020 2020 2020 2073  alue):.        s
+00008970: 656c 662e 5f61 6275 6e64 616e 6365 3d76  elf._abundance=v
+00008980: 616c 7565 0a0a 2020 2020 4070 726f 7065  alue..    @prope
+00008990: 7274 790a 2020 2020 6465 6620 6476 2873  rty.    def dv(s
+000089a0: 656c 6629 3a0a 2020 2020 2020 2020 6966  elf):.        if
+000089b0: 2073 656c 662e 6e6d 6f64 656c 733e 313a   self.nmodels>1:
+000089c0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000089d0: 662e 5f64 763d 5b5d 0a20 2020 2020 2020  f._dv=[].       
+000089e0: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
+000089f0: 6e67 6528 7365 6c66 2e6e 6d6f 6465 6c73  nge(self.nmodels
+00008a00: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00008a10: 2020 2073 656c 662e 5f64 762e 6170 7065     self._dv.appe
+00008a20: 6e64 2873 656c 662e 6d6f 6465 6c73 5b69  nd(self.models[i
+00008a30: 5d2e 6476 290a 2020 2020 2020 2020 656c  ].dv).        el
+00008a40: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00008a50: 7365 6c66 2e5f 6476 3d73 656c 662e 6d6f  self._dv=self.mo
+00008a60: 6465 6c73 5b30 5d2e 6476 0a20 2020 2020  dels[0].dv.     
+00008a70: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+00008a80: 6476 0a0a 2020 2020 4064 762e 7365 7474  dv..    @dv.sett
+00008a90: 6572 0a20 2020 2064 6566 2064 7628 7365  er.    def dv(se
+00008aa0: 6c66 2c76 616c 7565 293a 0a20 2020 2020  lf,value):.     
+00008ab0: 2020 2073 656c 662e 5f64 763d 7661 6c75     self._dv=valu
+00008ac0: 650a 0a20 2020 2040 7072 6f70 6572 7479  e..    @property
+00008ad0: 0a20 2020 2064 6566 206e 6c65 7665 6c73  .    def nlevels
+00008ae0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00008af0: 6966 2073 656c 662e 6e6d 6f64 656c 733e  if self.nmodels>
+00008b00: 313a 0a20 2020 2020 2020 2020 2020 2073  1:.            s
+00008b10: 656c 662e 5f6e 6c65 7665 6c73 3d5b 5d0a  elf._nlevels=[].
+00008b20: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00008b30: 6920 696e 2072 616e 6765 2873 656c 662e  i in range(self.
+00008b40: 6e6d 6f64 656c 7329 3a0a 2020 2020 2020  nmodels):.      
+00008b50: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00008b60: 6e6c 6576 656c 732e 6170 7065 6e64 2873  nlevels.append(s
+00008b70: 656c 662e 6d6f 6465 6c73 5b69 5d2e 6e6c  elf.models[i].nl
+00008b80: 6576 656c 7329 0a20 2020 2020 2020 2065  evels).        e
+00008b90: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00008ba0: 2073 656c 662e 5f6e 6c65 7665 6c73 3d73   self._nlevels=s
+00008bb0: 656c 662e 6d6f 6465 6c73 5b30 5d2e 6e6c  elf.models[0].nl
+00008bc0: 6576 656c 730a 2020 2020 2020 2020 7265  evels.        re
+00008bd0: 7475 726e 2073 656c 662e 5f6e 6c65 7665  turn self._nleve
+00008be0: 6c73 0a0a 2020 2020 406e 6c65 7665 6c73  ls..    @nlevels
+00008bf0: 2e73 6574 7465 720a 2020 2020 6465 6620  .setter.    def 
+00008c00: 6e6c 6576 656c 7328 7365 6c66 2c76 616c  nlevels(self,val
+00008c10: 7565 293a 0a20 2020 2020 2020 2073 656c  ue):.        sel
+00008c20: 662e 5f6e 6c65 7665 6c73 3d76 616c 7565  f._nlevels=value
+00008c30: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+00008c40: 2020 2020 6465 6620 6e6c 696e 6573 2873      def nlines(s
+00008c50: 656c 6629 3a0a 2020 2020 2020 2020 6966  elf):.        if
+00008c60: 2073 656c 662e 6e6d 6f64 656c 733e 313a   self.nmodels>1:
+00008c70: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00008c80: 662e 5f6e 6c69 6e65 733d 5b5d 0a20 2020  f._nlines=[].   
+00008c90: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
+00008ca0: 6e20 7261 6e67 6528 7365 6c66 2e6e 6d6f  n range(self.nmo
+00008cb0: 6465 6c73 293a 0a20 2020 2020 2020 2020  dels):.         
+00008cc0: 2020 2020 2020 2073 656c 662e 5f6e 6c69         self._nli
+00008cd0: 6e65 732e 6170 7065 6e64 2873 656c 662e  nes.append(self.
+00008ce0: 6d6f 6465 6c73 5b69 5d2e 6e6c 696e 6573  models[i].nlines
+00008cf0: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+00008d00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00008d10: 2e5f 6e6c 696e 6573 3d73 656c 662e 6d6f  ._nlines=self.mo
+00008d20: 6465 6c73 5b30 5d2e 6e6c 696e 6573 0a20  dels[0].nlines. 
+00008d30: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00008d40: 6c66 2e5f 6e6c 696e 6573 0a0a 2020 2020  lf._nlines..    
+00008d50: 406e 6c69 6e65 732e 7365 7474 6572 0a20  @nlines.setter. 
+00008d60: 2020 2064 6566 206e 6c69 6e65 7328 7365     def nlines(se
+00008d70: 6c66 2c76 616c 7565 293a 0a20 2020 2020  lf,value):.     
+00008d80: 2020 2073 656c 662e 5f6e 6c69 6e65 733d     self._nlines=
+00008d90: 7661 6c75 650a 0a20 2020 2040 7072 6f70  value..    @prop
+00008da0: 6572 7479 0a20 2020 2064 6566 206c 696e  erty.    def lin
+00008db0: 6564 6174 6128 7365 6c66 293a 0a20 2020  edata(self):.   
+00008dc0: 2020 2020 2069 6620 7365 6c66 2e6e 6d6f       if self.nmo
+00008dd0: 6465 6c73 3e31 3a0a 2020 2020 2020 2020  dels>1:.        
+00008de0: 2020 2020 7365 6c66 2e5f 6c69 6e65 6461      self._lineda
+00008df0: 7461 3d5b 5d0a 2020 2020 2020 2020 2020  ta=[].          
+00008e00: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
+00008e10: 2873 656c 662e 6e6d 6f64 656c 7329 3a0a  (self.nmodels):.
+00008e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008e30: 7365 6c66 2e5f 6c69 6e65 6461 7461 2e61  self._linedata.a
+00008e40: 7070 656e 6428 7365 6c66 2e6d 6f64 656c  ppend(self.model
+00008e50: 735b 695d 2e6c 696e 6564 6174 6129 0a20  s[i].linedata). 
+00008e60: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00008e70: 2020 2020 2020 2020 2073 656c 662e 5f6c           self._l
+00008e80: 696e 6564 6174 613d 7365 6c66 2e6d 6f64  inedata=self.mod
+00008e90: 656c 735b 305d 2e6c 696e 6564 6174 610a  els[0].linedata.
+00008ea0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00008eb0: 656c 662e 5f6c 696e 6564 6174 610a 0a20  elf._linedata.. 
+00008ec0: 2020 2040 6c69 6e65 6461 7461 2e73 6574     @linedata.set
+00008ed0: 7465 720a 2020 2020 6465 6620 6c69 6e65  ter.    def line
+00008ee0: 6461 7461 2873 656c 662c 7661 6c75 6529  data(self,value)
+00008ef0: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
+00008f00: 6c69 6e65 6461 7461 3d76 616c 7565 0a0a  linedata=value..
+00008f10: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+00008f20: 2020 6465 6620 6c65 7665 6c64 6174 6128    def leveldata(
+00008f30: 7365 6c66 293a 0a20 2020 2020 2020 2069  self):.        i
+00008f40: 6620 7365 6c66 2e6e 6d6f 6465 6c73 3e31  f self.nmodels>1
+00008f50: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00008f60: 6c66 2e5f 6c65 7665 6c64 6174 613d 5b5d  lf._leveldata=[]
+00008f70: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00008f80: 2069 2069 6e20 7261 6e67 6528 7365 6c66   i in range(self
+00008f90: 2e6e 6d6f 6465 6c73 293a 0a20 2020 2020  .nmodels):.     
+00008fa0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00008fb0: 5f6c 6576 656c 6461 7461 2e61 7070 656e  _leveldata.appen
+00008fc0: 6428 7365 6c66 2e6d 6f64 656c 735b 695d  d(self.models[i]
+00008fd0: 2e6c 6576 656c 6461 7461 290a 2020 2020  .leveldata).    
+00008fe0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00008ff0: 2020 2020 2020 7365 6c66 2e5f 6c65 7665        self._leve
+00009000: 6c64 6174 613d 7365 6c66 2e6d 6f64 656c  ldata=self.model
+00009010: 735b 305d 2e6c 6576 656c 6461 7461 0a20  s[0].leveldata. 
+00009020: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00009030: 6c66 2e5f 6c65 7665 6c64 6174 610a 0a20  lf._leveldata.. 
+00009040: 2020 2040 6c65 7665 6c64 6174 612e 7365     @leveldata.se
+00009050: 7474 6572 0a20 2020 2064 6566 206c 6576  tter.    def lev
+00009060: 656c 6461 7461 2873 656c 662c 7661 6c75  eldata(self,valu
+00009070: 6529 3a0a 2020 2020 2020 2020 7365 6c66  e):.        self
+00009080: 2e5f 6c65 7665 6c64 6174 613d 7661 6c75  ._leveldata=valu
+00009090: 650a 0a20 2020 2040 7072 6f70 6572 7479  e..    @property
+000090a0: 0a20 2020 2064 6566 2063 6f6e 7657 6176  .    def convWav
+000090b0: 656c 656e 6774 6828 7365 6c66 293a 0a20  elength(self):. 
+000090c0: 2020 2020 2020 2069 6620 7365 6c66 2e6e         if self.n
+000090d0: 6d6f 6465 6c73 3e31 3a0a 2020 2020 2020  models>1:.      
+000090e0: 2020 2020 2020 7365 6c66 2e5f 636f 6e76        self._conv
+000090f0: 5761 7665 6c65 6e67 7468 3d5b 5d0a 2020  Wavelength=[].  
+00009100: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
+00009110: 696e 2072 616e 6765 2873 656c 662e 6e6d  in range(self.nm
+00009120: 6f64 656c 7329 3a0a 2020 2020 2020 2020  odels):.        
+00009130: 2020 2020 2020 2020 7365 6c66 2e5f 636f          self._co
+00009140: 6e76 5761 7665 6c65 6e67 7468 2e61 7070  nvWavelength.app
+00009150: 656e 6428 7365 6c66 2e6d 6f64 656c 735b  end(self.models[
+00009160: 695d 2e63 6f6e 7657 6176 656c 656e 6774  i].convWavelengt
+00009170: 6829 0a20 2020 2020 2020 2065 6c73 653a  h).        else:
+00009180: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00009190: 662e 5f63 6f6e 7657 6176 656c 656e 6774  f._convWavelengt
+000091a0: 683d 7365 6c66 2e6d 6f64 656c 735b 305d  h=self.models[0]
+000091b0: 2e63 6f6e 7657 6176 656c 656e 6774 680a  .convWavelength.
+000091c0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+000091d0: 656c 662e 5f63 6f6e 7657 6176 656c 656e  elf._convWavelen
+000091e0: 6774 680a 0a20 2020 2040 636f 6e76 5761  gth..    @convWa
+000091f0: 7665 6c65 6e67 7468 2e73 6574 7465 720a  velength.setter.
+00009200: 2020 2020 6465 6620 636f 6e76 5761 7665      def convWave
+00009210: 6c65 6e67 7468 2873 656c 662c 7661 6c75  length(self,valu
+00009220: 6529 3a0a 2020 2020 2020 2020 7365 6c66  e):.        self
+00009230: 2e5f 636f 6e76 5761 7665 6c65 6e67 7468  ._convWavelength
+00009240: 3d76 616c 7565 0a0a 2020 2020 4070 726f  =value..    @pro
+00009250: 7065 7274 790a 2020 2020 6465 6620 636f  perty.    def co
+00009260: 6e76 4c54 4566 6c75 7828 7365 6c66 293a  nvLTEflux(self):
+00009270: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00009280: 2e6e 6d6f 6465 6c73 3e31 3a0a 2020 2020  .nmodels>1:.    
+00009290: 2020 2020 2020 2020 7365 6c66 2e5f 636f          self._co
+000092a0: 6e76 4c54 4566 6c75 783d 5b5d 0a20 2020  nvLTEflux=[].   
+000092b0: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
+000092c0: 6e20 7261 6e67 6528 7365 6c66 2e6e 6d6f  n range(self.nmo
+000092d0: 6465 6c73 293a 0a20 2020 2020 2020 2020  dels):.         
+000092e0: 2020 2020 2020 2073 656c 662e 5f63 6f6e         self._con
+000092f0: 764c 5445 666c 7578 2e61 7070 656e 6428  vLTEflux.append(
+00009300: 7365 6c66 2e6d 6f64 656c 735b 695d 2e63  self.models[i].c
+00009310: 6f6e 764c 5445 666c 7578 290a 2020 2020  onvLTEflux).    
+00009320: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00009330: 2020 2020 2020 7365 6c66 2e5f 636f 6e76        self._conv
+00009340: 4c54 4566 6c75 783d 7365 6c66 2e6d 6f64  LTEflux=self.mod
+00009350: 656c 735b 305d 2e63 6f6e 764c 5445 666c  els[0].convLTEfl
+00009360: 7578 0a20 2020 2020 2020 2072 6574 7572  ux.        retur
+00009370: 6e20 7365 6c66 2e5f 636f 6e76 4c54 4566  n self._convLTEf
+00009380: 6c75 780a 0a20 2020 2040 636f 6e76 4c54  lux..    @convLT
+00009390: 4566 6c75 782e 7365 7474 6572 0a20 2020  Eflux.setter.   
+000093a0: 2064 6566 2063 6f6e 764c 5445 666c 7578   def convLTEflux
+000093b0: 2873 656c 662c 7661 6c75 6529 3a0a 2020  (self,value):.  
+000093c0: 2020 2020 2020 7365 6c66 2e5f 636f 6e76        self._conv
+000093d0: 4c54 4566 6c75 783d 7661 6c75 650a 0a20  LTEflux=value.. 
+000093e0: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+000093f0: 2064 6566 2063 6f6e 764e 4c54 4566 6c75   def convNLTEflu
+00009400: 7828 7365 6c66 293a 0a20 2020 2020 2020  x(self):.       
+00009410: 2069 6620 7365 6c66 2e6e 6d6f 6465 6c73   if self.nmodels
+00009420: 3e31 3a0a 2020 2020 2020 2020 2020 2020  >1:.            
+00009430: 7365 6c66 2e5f 636f 6e76 4e4c 5445 666c  self._convNLTEfl
+00009440: 7578 3d5b 5d0a 2020 2020 2020 2020 2020  ux=[].          
+00009450: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
+00009460: 2873 656c 662e 6e6d 6f64 656c 7329 3a0a  (self.nmodels):.
+00009470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009480: 7365 6c66 2e5f 636f 6e76 4e4c 5445 666c  self._convNLTEfl
+00009490: 7578 2e61 7070 656e 6428 7365 6c66 2e6d  ux.append(self.m
+000094a0: 6f64 656c 735b 695d 2e63 6f6e 764e 4c54  odels[i].convNLT
+000094b0: 4566 6c75 7829 0a20 2020 2020 2020 2065  Eflux).        e
+000094c0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+000094d0: 2073 656c 662e 5f63 6f6e 764e 4c54 4566   self._convNLTEf
+000094e0: 6c75 783d 7365 6c66 2e6d 6f64 656c 735b  lux=self.models[
+000094f0: 305d 2e63 6f6e 764e 4c54 4566 6c75 780a  0].convNLTEflux.
+00009500: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00009510: 656c 662e 5f63 6f6e 764e 4c54 4566 6c75  elf._convNLTEflu
+00009520: 780a 0a20 2020 2040 636f 6e76 4e4c 5445  x..    @convNLTE
+00009530: 666c 7578 2e73 6574 7465 720a 2020 2020  flux.setter.    
+00009540: 6465 6620 636f 6e76 4e4c 5445 666c 7578  def convNLTEflux
+00009550: 2873 656c 662c 7661 6c75 6529 3a0a 2020  (self,value):.  
+00009560: 2020 2020 2020 7365 6c66 2e5f 636f 6e76        self._conv
+00009570: 4e4c 5445 666c 7578 3d76 616c 7565 0a0a  NLTEflux=value..
+00009580: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+00009590: 2020 6465 6620 636f 6e76 5479 7065 2873    def convType(s
+000095a0: 656c 6629 3a0a 2020 2020 2020 2020 6966  elf):.        if
+000095b0: 2073 656c 662e 6e6d 6f64 656c 733e 313a   self.nmodels>1:
+000095c0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000095d0: 662e 5f63 6f6e 7654 7970 653d 5b5d 0a20  f._convType=[]. 
+000095e0: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+000095f0: 2069 6e20 7261 6e67 6528 7365 6c66 2e6e   in range(self.n
+00009600: 6d6f 6465 6c73 293a 0a20 2020 2020 2020  models):.       
+00009610: 2020 2020 2020 2020 2073 656c 662e 5f63           self._c
+00009620: 6f6e 7654 7970 652e 6170 7065 6e64 2873  onvType.append(s
+00009630: 656c 662e 6d6f 6465 6c73 5b69 5d2e 636f  elf.models[i].co
+00009640: 6e76 5479 7065 290a 2020 2020 2020 2020  nvType).        
+00009650: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00009660: 2020 7365 6c66 2e5f 636f 6e76 5479 7065    self._convType
+00009670: 3d73 656c 662e 6d6f 6465 6c73 5b30 5d2e  =self.models[0].
+00009680: 636f 6e76 5479 7065 0a20 2020 2020 2020  convType.       
+00009690: 2072 6574 7572 6e20 7365 6c66 2e5f 636f   return self._co
+000096a0: 6e76 5479 7065 0a0a 2020 2020 4063 6f6e  nvType..    @con
+000096b0: 7654 7970 652e 7365 7474 6572 0a20 2020  vType.setter.   
+000096c0: 2064 6566 2063 6f6e 7654 7970 6528 7365   def convType(se
+000096d0: 6c66 2c76 616c 7565 293a 0a20 2020 2020  lf,value):.     
+000096e0: 2020 2073 656c 662e 5f63 6f6e 7654 7970     self._convTyp
+000096f0: 653d 7661 6c75 650a 0a20 2020 2040 7072  e=value..    @pr
+00009700: 6f70 6572 7479 0a20 2020 2064 6566 2063  operty.    def c
+00009710: 6f6e 7652 2873 656c 6629 3a0a 2020 2020  onvR(self):.    
+00009720: 2020 2020 6966 2073 656c 662e 6e6d 6f64      if self.nmod
+00009730: 656c 733e 313a 0a20 2020 2020 2020 2020  els>1:.         
+00009740: 2020 2073 656c 662e 5f63 6f6e 7652 3d5b     self._convR=[
+00009750: 5d0a 2020 2020 2020 2020 2020 2020 666f  ].            fo
+00009760: 7220 6920 696e 2072 616e 6765 2873 656c  r i in range(sel
+00009770: 662e 6e6d 6f64 656c 7329 3a0a 2020 2020  f.nmodels):.    
+00009780: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00009790: 2e5f 636f 6e76 522e 6170 7065 6e64 2873  ._convR.append(s
+000097a0: 656c 662e 6d6f 6465 6c73 5b69 5d2e 636f  elf.models[i].co
+000097b0: 6e76 5229 0a20 2020 2020 2020 2065 6c73  nvR).        els
+000097c0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+000097d0: 656c 662e 5f63 6f6e 7652 3d73 656c 662e  elf._convR=self.
+000097e0: 6d6f 6465 6c73 5b30 5d2e 636f 6e76 520a  models[0].convR.
+000097f0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00009800: 656c 662e 5f63 6f6e 7652 0a0a 2020 2020  elf._convR..    
+00009810: 4063 6f6e 7652 2e73 6574 7465 720a 2020  @convR.setter.  
+00009820: 2020 6465 6620 636f 6e76 5228 7365 6c66    def convR(self
+00009830: 2c76 616c 7565 293a 0a20 2020 2020 2020  ,value):.       
+00009840: 2073 656c 662e 5f63 6f6e 7652 3d76 616c   self._convR=val
+00009850: 7565 0a0a 2020 2020 4070 726f 7065 7274  ue..    @propert
+00009860: 790a 2020 2020 6465 6620 636f 6e76 4f76  y.    def convOv
+00009870: 6572 6c61 7046 7265 7128 7365 6c66 293a  erlapFreq(self):
+00009880: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00009890: 2e6e 6d6f 6465 6c73 3e31 3a0a 2020 2020  .nmodels>1:.    
+000098a0: 2020 2020 2020 2020 7365 6c66 2e5f 636f          self._co
+000098b0: 6e76 4f76 6572 6c61 7046 7265 713d 5b5d  nvOverlapFreq=[]
+000098c0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+000098d0: 2069 2069 6e20 7261 6e67 6528 7365 6c66   i in range(self
+000098e0: 2e6e 6d6f 6465 6c73 293a 0a20 2020 2020  .nmodels):.     
+000098f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00009900: 5f63 6f6e 764f 7665 726c 6170 4672 6571  _convOverlapFreq
+00009910: 2e61 7070 656e 6428 7365 6c66 2e6d 6f64  .append(self.mod
+00009920: 656c 735b 695d 2e63 6f6e 764f 7665 726c  els[i].convOverl
+00009930: 6170 4672 6571 290a 2020 2020 2020 2020  apFreq).        
+00009940: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00009950: 2020 7365 6c66 2e5f 636f 6e76 4f76 6572    self._convOver
+00009960: 6c61 7046 7265 713d 7365 6c66 2e6d 6f64  lapFreq=self.mod
+00009970: 656c 735b 305d 2e63 6f6e 764f 7665 726c  els[0].convOverl
+00009980: 6170 4672 6571 0a20 2020 2020 2020 2072  apFreq.        r
+00009990: 6574 7572 6e20 7365 6c66 2e5f 636f 6e76  eturn self._conv
+000099a0: 4f76 6572 6c61 7046 7265 710a 0a20 2020  OverlapFreq..   
+000099b0: 2040 636f 6e76 4f76 6572 6c61 7046 7265   @convOverlapFre
+000099c0: 712e 7365 7474 6572 0a20 2020 2064 6566  q.setter.    def
+000099d0: 2063 6f6e 764f 7665 726c 6170 4672 6571   convOverlapFreq
+000099e0: 2873 656c 662c 7661 6c75 6529 3a0a 2020  (self,value):.  
+000099f0: 2020 2020 2020 7365 6c66 2e5f 636f 6e76        self._conv
+00009a00: 4f76 6572 6c61 7046 7265 713d 7661 6c75  OverlapFreq=valu
+00009a10: 650a 0a20 2020 2040 7072 6f70 6572 7479  e..    @property
+00009a20: 0a20 2020 2064 6566 2063 6f6e 764f 7665  .    def convOve
+00009a30: 726c 6170 5761 7665 2873 656c 6629 3a0a  rlapWave(self):.
+00009a40: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00009a50: 6e6d 6f64 656c 733e 313a 0a20 2020 2020  nmodels>1:.     
+00009a60: 2020 2020 2020 2073 656c 662e 5f63 6f6e         self._con
+00009a70: 764f 7665 726c 6170 5761 7665 3d5b 5d0a  vOverlapWave=[].
+00009a80: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00009a90: 6920 696e 2072 616e 6765 2873 656c 662e  i in range(self.
+00009aa0: 6e6d 6f64 656c 7329 3a0a 2020 2020 2020  nmodels):.      
+00009ab0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00009ac0: 636f 6e76 4f76 6572 6c61 7057 6176 652e  convOverlapWave.
+00009ad0: 6170 7065 6e64 2873 656c 662e 6d6f 6465  append(self.mode
+00009ae0: 6c73 5b69 5d2e 636f 6e76 4f76 6572 6c61  ls[i].convOverla
+00009af0: 7057 6176 6529 0a20 2020 2020 2020 2065  pWave).        e
+00009b00: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00009b10: 2073 656c 662e 5f63 6f6e 764f 7665 726c   self._convOverl
+00009b20: 6170 5761 7665 3d73 656c 662e 6d6f 6465  apWave=self.mode
+00009b30: 6c73 5b30 5d2e 636f 6e76 4f76 6572 6c61  ls[0].convOverla
+00009b40: 7057 6176 650a 2020 2020 2020 2020 7265  pWave.        re
+00009b50: 7475 726e 2073 656c 662e 5f63 6f6e 764f  turn self._convO
+00009b60: 7665 726c 6170 5761 7665 0a0a 2020 2020  verlapWave..    
+00009b70: 4063 6f6e 764f 7665 726c 6170 5761 7665  @convOverlapWave
+00009b80: 2e73 6574 7465 720a 2020 2020 6465 6620  .setter.    def 
+00009b90: 636f 6e76 4f76 6572 6c61 7057 6176 6528  convOverlapWave(
+00009ba0: 7365 6c66 2c76 616c 7565 293a 0a20 2020  self,value):.   
+00009bb0: 2020 2020 2073 656c 662e 5f63 6f6e 764f       self._convO
+00009bc0: 7665 726c 6170 5761 7665 3d76 616c 7565  verlapWave=value
+00009bd0: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+00009be0: 2020 2020 6465 6620 6f76 6572 6c61 7046      def overlapF
+00009bf0: 7265 7128 7365 6c66 293a 0a20 2020 2020  req(self):.     
+00009c00: 2020 2069 6620 7365 6c66 2e6e 6d6f 6465     if self.nmode
+00009c10: 6c73 3e31 3a0a 2020 2020 2020 2020 2020  ls>1:.          
+00009c20: 2020 7365 6c66 2e5f 6f76 6572 6c61 7046    self._overlapF
+00009c30: 7265 713d 5b5d 0a20 2020 2020 2020 2020  req=[].         
+00009c40: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
+00009c50: 6528 7365 6c66 2e6e 6d6f 6465 6c73 293a  e(self.nmodels):
+00009c60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009c70: 2073 656c 662e 5f6f 7665 726c 6170 4672   self._overlapFr
+00009c80: 6571 2e61 7070 656e 6428 7365 6c66 2e6d  eq.append(self.m
+00009c90: 6f64 656c 735b 695d 2e6f 7665 726c 6170  odels[i].overlap
+00009ca0: 4672 6571 290a 2020 2020 2020 2020 656c  Freq).        el
+00009cb0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00009cc0: 7365 6c66 2e5f 6f76 6572 6c61 7046 7265  self._overlapFre
+00009cd0: 713d 7365 6c66 2e6d 6f64 656c 735b 305d  q=self.models[0]
+00009ce0: 2e6f 7665 726c 6170 4672 6571 0a20 2020  .overlapFreq.   
+00009cf0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00009d00: 2e5f 6f76 6572 6c61 7046 7265 710a 0a20  ._overlapFreq.. 
+00009d10: 2020 2040 6f76 6572 6c61 7046 7265 712e     @overlapFreq.
+00009d20: 7365 7474 6572 0a20 2020 2064 6566 206f  setter.    def o
+00009d30: 7665 726c 6170 4672 6571 2873 656c 662c  verlapFreq(self,
+00009d40: 7661 6c75 6529 3a0a 2020 2020 2020 2020  value):.        
+00009d50: 7365 6c66 2e5f 6f76 6572 6c61 7046 7265  self._overlapFre
+00009d60: 713d 7661 6c75 650a 0a20 2020 2040 7072  q=value..    @pr
+00009d70: 6f70 6572 7479 0a20 2020 2064 6566 2063  operty.    def c
+00009d80: 6f6e 764f 7665 726c 6170 4c54 4528 7365  onvOverlapLTE(se
+00009d90: 6c66 293a 0a20 2020 2020 2020 2069 6620  lf):.        if 
+00009da0: 7365 6c66 2e6e 6d6f 6465 6c73 3e31 3a0a  self.nmodels>1:.
+00009db0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00009dc0: 2e5f 636f 6e76 4f76 6572 6c61 704c 5445  ._convOverlapLTE
+00009dd0: 3d5b 5d0a 2020 2020 2020 2020 2020 2020  =[].            
+00009de0: 666f 7220 6920 696e 2072 616e 6765 2873  for i in range(s
+00009df0: 656c 662e 6e6d 6f64 656c 7329 3a0a 2020  elf.nmodels):.  
+00009e00: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00009e10: 6c66 2e5f 636f 6e76 4f76 6572 6c61 704c  lf._convOverlapL
+00009e20: 5445 2e61 7070 656e 6428 7365 6c66 2e6d  TE.append(self.m
+00009e30: 6f64 656c 735b 695d 2e63 6f6e 764f 7665  odels[i].convOve
+00009e40: 726c 6170 4c54 4529 0a20 2020 2020 2020  rlapLTE).       
+00009e50: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00009e60: 2020 2073 656c 662e 5f63 6f6e 764f 7665     self._convOve
+00009e70: 726c 6170 4c54 453d 7365 6c66 2e6d 6f64  rlapLTE=self.mod
+00009e80: 656c 735b 305d 2e63 6f6e 764f 7665 726c  els[0].convOverl
+00009e90: 6170 4c54 450a 2020 2020 2020 2020 7265  apLTE.        re
+00009ea0: 7475 726e 2073 656c 662e 5f63 6f6e 764f  turn self._convO
+00009eb0: 7665 726c 6170 4c54 450a 0a20 2020 2040  verlapLTE..    @
+00009ec0: 636f 6e76 4f76 6572 6c61 704c 5445 2e73  convOverlapLTE.s
+00009ed0: 6574 7465 720a 2020 2020 6465 6620 636f  etter.    def co
+00009ee0: 6e76 4f76 6572 6c61 704c 5445 2873 656c  nvOverlapLTE(sel
+00009ef0: 662c 7661 6c75 6529 3a0a 2020 2020 2020  f,value):.      
+00009f00: 2020 7365 6c66 2e5f 636f 6e76 4f76 6572    self._convOver
+00009f10: 6c61 704c 5445 3d76 616c 7565 0a0a 2020  lapLTE=value..  
+00009f20: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+00009f30: 6465 6620 636f 6e76 4f76 6572 6c61 704e  def convOverlapN
+00009f40: 4c54 4528 7365 6c66 293a 0a20 2020 2020  LTE(self):.     
+00009f50: 2020 2069 6620 7365 6c66 2e6e 6d6f 6465     if self.nmode
+00009f60: 6c73 3e31 3a0a 2020 2020 2020 2020 2020  ls>1:.          
+00009f70: 2020 7365 6c66 2e5f 636f 6e76 4f76 6572    self._convOver
+00009f80: 6c61 704e 4c54 453d 5b5d 0a20 2020 2020  lapNLTE=[].     
+00009f90: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+00009fa0: 7261 6e67 6528 7365 6c66 2e6e 6d6f 6465  range(self.nmode
+00009fb0: 6c73 293a 0a20 2020 2020 2020 2020 2020  ls):.           
+00009fc0: 2020 2020 2073 656c 662e 5f63 6f6e 764f       self._convO
+00009fd0: 7665 726c 6170 4e4c 5445 2e61 7070 656e  verlapNLTE.appen
+00009fe0: 6428 7365 6c66 2e6d 6f64 656c 735b 695d  d(self.models[i]
+00009ff0: 2e63 6f6e 764f 7665 726c 6170 4e4c 5445  .convOverlapNLTE
+0000a000: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+0000a010: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000a020: 2e5f 636f 6e76 4f76 6572 6c61 704e 4c54  ._convOverlapNLT
+0000a030: 453d 7365 6c66 2e6d 6f64 656c 735b 305d  E=self.models[0]
+0000a040: 2e63 6f6e 764f 7665 726c 6170 4e4c 5445  .convOverlapNLTE
+0000a050: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000a060: 7365 6c66 2e5f 636f 6e76 4f76 6572 6c61  self._convOverla
+0000a070: 704e 4c54 450a 0a20 2020 2040 636f 6e76  pNLTE..    @conv
+0000a080: 4f76 6572 6c61 704e 4c54 452e 7365 7474  OverlapNLTE.sett
+0000a090: 6572 0a20 2020 2064 6566 2063 6f6e 764f  er.    def convO
+0000a0a0: 7665 726c 6170 4e4c 5445 2873 656c 662c  verlapNLTE(self,
+0000a0b0: 7661 6c75 6529 3a0a 2020 2020 2020 2020  value):.        
+0000a0c0: 7365 6c66 2e5f 636f 6e76 4f76 6572 6c61  self._convOverla
+0000a0d0: 704e 4c54 453d 7661 6c75 650a 0a20 2020  pNLTE=value..   
+0000a0e0: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
+0000a0f0: 6566 206f 7665 726c 6170 4c54 4528 7365  ef overlapLTE(se
+0000a100: 6c66 293a 0a20 2020 2020 2020 2069 6620  lf):.        if 
+0000a110: 7365 6c66 2e6e 6d6f 6465 6c73 3e31 3a0a  self.nmodels>1:.
+0000a120: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000a130: 2e5f 6f76 6572 6c61 704c 5445 3d5b 5d0a  ._overlapLTE=[].
+0000a140: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000a150: 6920 696e 2072 616e 6765 2873 656c 662e  i in range(self.
+0000a160: 6e6d 6f64 656c 7329 3a0a 2020 2020 2020  nmodels):.      
+0000a170: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+0000a180: 6f76 6572 6c61 704c 5445 2e61 7070 656e  overlapLTE.appen
+0000a190: 6428 7365 6c66 2e6d 6f64 656c 735b 695d  d(self.models[i]
+0000a1a0: 2e6f 7665 726c 6170 4c54 4529 0a20 2020  .overlapLTE).   
+0000a1b0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000a1c0: 2020 2020 2020 2073 656c 662e 5f6f 7665         self._ove
+0000a1d0: 726c 6170 4c54 453d 7365 6c66 2e6d 6f64  rlapLTE=self.mod
+0000a1e0: 656c 735b 305d 2e6f 7665 726c 6170 4c54  els[0].overlapLT
+0000a1f0: 450a 2020 2020 2020 2020 7265 7475 726e  E.        return
+0000a200: 2073 656c 662e 5f6f 7665 726c 6170 4c54   self._overlapLT
+0000a210: 450a 0a20 2020 2040 6f76 6572 6c61 704c  E..    @overlapL
+0000a220: 5445 2e73 6574 7465 720a 2020 2020 6465  TE.setter.    de
+0000a230: 6620 6f76 6572 6c61 704c 5445 2873 656c  f overlapLTE(sel
+0000a240: 662c 7661 6c75 6529 3a0a 2020 2020 2020  f,value):.      
+0000a250: 2020 7365 6c66 2e5f 6f76 6572 6c61 704c    self._overlapL
+0000a260: 5445 3d76 616c 7565 0a0a 2020 2020 4070  TE=value..    @p
+0000a270: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+0000a280: 6f76 6572 6c61 704e 4c54 4528 7365 6c66  overlapNLTE(self
+0000a290: 293a 0a20 2020 2020 2020 2069 6620 7365  ):.        if se
+0000a2a0: 6c66 2e6e 6d6f 6465 6c73 3e31 3a0a 2020  lf.nmodels>1:.  
+0000a2b0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+0000a2c0: 6f76 6572 6c61 704e 4c54 453d 5b5d 0a20  overlapNLTE=[]. 
+0000a2d0: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+0000a2e0: 2069 6e20 7261 6e67 6528 7365 6c66 2e6e   in range(self.n
+0000a2f0: 6d6f 6465 6c73 293a 0a20 2020 2020 2020  models):.       
+0000a300: 2020 2020 2020 2020 2073 656c 662e 5f6f           self._o
+0000a310: 7665 726c 6170 4e4c 5445 2e61 7070 656e  verlapNLTE.appen
+0000a320: 6428 7365 6c66 2e6d 6f64 656c 735b 695d  d(self.models[i]
+0000a330: 2e6f 7665 726c 6170 4e4c 5445 290a 2020  .overlapNLTE).  
+0000a340: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000a350: 2020 2020 2020 2020 7365 6c66 2e5f 6f76          self._ov
+0000a360: 6572 6c61 704e 4c54 453d 7365 6c66 2e6d  erlapNLTE=self.m
+0000a370: 6f64 656c 735b 305d 2e6f 7665 726c 6170  odels[0].overlap
+0000a380: 4e4c 5445 0a20 2020 2020 2020 2072 6574  NLTE.        ret
+0000a390: 7572 6e20 7365 6c66 2e5f 6f76 6572 6c61  urn self._overla
+0000a3a0: 704e 4c54 450a 0a20 2020 2040 6f76 6572  pNLTE..    @over
+0000a3b0: 6c61 704e 4c54 452e 7365 7474 6572 0a20  lapNLTE.setter. 
+0000a3c0: 2020 2064 6566 206f 7665 726c 6170 4e4c     def overlapNL
+0000a3d0: 5445 2873 656c 662c 7661 6c75 6529 3a0a  TE(self,value):.
+0000a3e0: 2020 2020 2020 2020 7365 6c66 2e5f 6f76          self._ov
+0000a3f0: 6572 6c61 704e 4c54 453d 7661 6c75 650a  erlapNLTE=value.
+0000a400: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+0000a410: 2020 2064 6566 206f 7665 726c 6170 5461     def overlapTa
+0000a420: 754c 5445 2873 656c 6629 3a0a 2020 2020  uLTE(self):.    
+0000a430: 2020 2020 6966 2073 656c 662e 6e6d 6f64      if self.nmod
+0000a440: 656c 733e 313a 0a20 2020 2020 2020 2020  els>1:.         
+0000a450: 2020 2073 656c 662e 5f6f 7665 726c 6170     self._overlap
+0000a460: 5461 754c 5445 3d5b 5d0a 2020 2020 2020  TauLTE=[].      
+0000a470: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
+0000a480: 616e 6765 2873 656c 662e 6e6d 6f64 656c  ange(self.nmodel
+0000a490: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+0000a4a0: 2020 2020 7365 6c66 2e5f 6f76 6572 6c61      self._overla
+0000a4b0: 7054 6175 4c54 452e 6170 7065 6e64 2873  pTauLTE.append(s
+0000a4c0: 656c 662e 6d6f 6465 6c73 5b69 5d2e 6f76  elf.models[i].ov
+0000a4d0: 6572 6c61 7054 6175 4c54 4529 0a20 2020  erlapTauLTE).   
+0000a4e0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000a4f0: 2020 2020 2020 2073 656c 662e 5f6f 7665         self._ove
+0000a500: 726c 6170 5461 754c 5445 3d73 656c 662e  rlapTauLTE=self.
+0000a510: 6d6f 6465 6c73 5b30 5d2e 6f76 6572 6c61  models[0].overla
+0000a520: 7054 6175 4c54 450a 2020 2020 2020 2020  pTauLTE.        
+0000a530: 7265 7475 726e 2073 656c 662e 5f6f 7665  return self._ove
+0000a540: 726c 6170 5461 754c 5445 0a0a 2020 2020  rlapTauLTE..    
+0000a550: 406f 7665 726c 6170 5461 754c 5445 2e73  @overlapTauLTE.s
+0000a560: 6574 7465 720a 2020 2020 6465 6620 6f76  etter.    def ov
+0000a570: 6572 6c61 7054 6175 4c54 4528 7365 6c66  erlapTauLTE(self
+0000a580: 2c76 616c 7565 293a 0a20 2020 2020 2020  ,value):.       
+0000a590: 2073 656c 662e 5f6f 7665 726c 6170 5461   self._overlapTa
+0000a5a0: 754c 5445 3d76 616c 7565 0a0a 2020 2020  uLTE=value..    
+0000a5b0: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+0000a5c0: 6620 6f76 6572 6c61 7054 6175 4e4c 5445  f overlapTauNLTE
+0000a5d0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000a5e0: 6966 2073 656c 662e 6e6d 6f64 656c 733e  if self.nmodels>
+0000a5f0: 313a 0a20 2020 2020 2020 2020 2020 2073  1:.            s
+0000a600: 656c 662e 5f6f 7665 726c 6170 5461 754e  elf._overlapTauN
+0000a610: 4c54 453d 5b5d 0a20 2020 2020 2020 2020  LTE=[].         
+0000a620: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
+0000a630: 6528 7365 6c66 2e6e 6d6f 6465 6c73 293a  e(self.nmodels):
+0000a640: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a650: 2073 656c 662e 5f6f 7665 726c 6170 5461   self._overlapTa
+0000a660: 754e 4c54 452e 6170 7065 6e64 2873 656c  uNLTE.append(sel
+0000a670: 662e 6d6f 6465 6c73 5b69 5d2e 6f76 6572  f.models[i].over
+0000a680: 6c61 7054 6175 4e4c 5445 290a 2020 2020  lapTauNLTE).    
+0000a690: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000a6a0: 2020 2020 2020 7365 6c66 2e5f 6f76 6572        self._over
+0000a6b0: 6c61 7054 6175 4e4c 5445 3d73 656c 662e  lapTauNLTE=self.
+0000a6c0: 6d6f 6465 6c73 5b30 5d2e 6f76 6572 6c61  models[0].overla
+0000a6d0: 7054 6175 4e4c 5445 0a20 2020 2020 2020  pTauNLTE.       
+0000a6e0: 2072 6574 7572 6e20 7365 6c66 2e5f 6f76   return self._ov
+0000a6f0: 6572 6c61 7054 6175 4e4c 5445 0a0a 2020  erlapTauNLTE..  
+0000a700: 2020 406f 7665 726c 6170 5461 754e 4c54    @overlapTauNLT
+0000a710: 452e 7365 7474 6572 0a20 2020 2064 6566  E.setter.    def
+0000a720: 206f 7665 726c 6170 5461 754e 4c54 4528   overlapTauNLTE(
+0000a730: 7365 6c66 2c76 616c 7565 293a 0a20 2020  self,value):.   
+0000a740: 2020 2020 2073 656c 662e 5f6f 7665 726c       self._overl
+0000a750: 6170 5461 754e 4c54 453d 7661 6c75 650a  apTauNLTE=value.
+0000a760: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+0000a770: 2020 2064 6566 2063 6f6e 764f 7665 726c     def convOverl
+0000a780: 6170 5228 7365 6c66 293a 0a20 2020 2020  apR(self):.     
+0000a790: 2020 2069 6620 7365 6c66 2e6e 6d6f 6465     if self.nmode
+0000a7a0: 6c73 3e31 3a0a 2020 2020 2020 2020 2020  ls>1:.          
+0000a7b0: 2020 7365 6c66 2e5f 636f 6e76 4f76 6572    self._convOver
+0000a7c0: 6c61 7052 3d5b 5d0a 2020 2020 2020 2020  lapR=[].        
+0000a7d0: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+0000a7e0: 6765 2873 656c 662e 6e6d 6f64 656c 7329  ge(self.nmodels)
+0000a7f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000a800: 2020 7365 6c66 2e5f 636f 6e76 4f76 6572    self._convOver
+0000a810: 6c61 7052 2e61 7070 656e 6428 7365 6c66  lapR.append(self
+0000a820: 2e6d 6f64 656c 735b 695d 2e63 6f6e 764f  .models[i].convO
+0000a830: 7665 726c 6170 5229 0a20 2020 2020 2020  verlapR).       
+0000a840: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000a850: 2020 2073 656c 662e 5f63 6f6e 764f 7665     self._convOve
+0000a860: 726c 6170 523d 7365 6c66 2e6d 6f64 656c  rlapR=self.model
+0000a870: 735b 305d 2e63 6f6e 764f 7665 726c 6170  s[0].convOverlap
+0000a880: 520a 2020 2020 2020 2020 7265 7475 726e  R.        return
+0000a890: 2073 656c 662e 5f63 6f6e 764f 7665 726c   self._convOverl
+0000a8a0: 6170 520a 0a20 2020 2040 636f 6e76 4f76  apR..    @convOv
+0000a8b0: 6572 6c61 7052 2e73 6574 7465 720a 2020  erlapR.setter.  
+0000a8c0: 2020 6465 6620 636f 6e76 4f76 6572 6c61    def convOverla
+0000a8d0: 7052 2873 656c 662c 7661 6c75 6529 3a0a  pR(self,value):.
+0000a8e0: 2020 2020 2020 2020 7365 6c66 2e5f 636f          self._co
+0000a8f0: 6e76 4f76 6572 6c61 7052 3d76 616c 7565  nvOverlapR=value
+0000a900: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+0000a910: 2020 2020 6465 6620 6f76 6572 6c61 7052      def overlapR
+0000a920: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000a930: 6966 2073 656c 662e 6e6d 6f64 656c 733e  if self.nmodels>
+0000a940: 313a 0a20 2020 2020 2020 2020 2020 2073  1:.            s
+0000a950: 656c 662e 5f6f 7665 726c 6170 523d 5b5d  elf._overlapR=[]
+0000a960: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+0000a970: 2069 2069 6e20 7261 6e67 6528 7365 6c66   i in range(self
+0000a980: 2e6e 6d6f 6465 6c73 293a 0a20 2020 2020  .nmodels):.     
+0000a990: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000a9a0: 5f6f 7665 726c 6170 522e 6170 7065 6e64  _overlapR.append
+0000a9b0: 2873 656c 662e 6d6f 6465 6c73 5b69 5d2e  (self.models[i].
+0000a9c0: 6f76 6572 6c61 7052 290a 2020 2020 2020  overlapR).      
+0000a9d0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000a9e0: 2020 2020 7365 6c66 2e5f 6f76 6572 6c61      self._overla
+0000a9f0: 7052 3d73 656c 662e 6d6f 6465 6c73 5b30  pR=self.models[0
+0000aa00: 5d2e 6f76 6572 6c61 7052 0a20 2020 2020  ].overlapR.     
+0000aa10: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+0000aa20: 6f76 6572 6c61 7052 0a0a 2020 2020 406f  overlapR..    @o
+0000aa30: 7665 726c 6170 522e 7365 7474 6572 0a20  verlapR.setter. 
+0000aa40: 2020 2064 6566 206f 7665 726c 6170 5228     def overlapR(
+0000aa50: 7365 6c66 2c76 616c 7565 293a 0a20 2020  self,value):.   
+0000aa60: 2020 2020 2073 656c 662e 5f6f 7665 726c       self._overl
+0000aa70: 6170 523d 7661 6c75 650a 0a0a 636c 6173  apR=value...clas
+0000aa80: 7320 736c 6162 3a0a 2020 2020 2222 220a  s slab:.    """.
+0000aa90: 2020 2020 636c 6173 733a 3a20 736c 6162      class:: slab
+0000aaa0: 0a20 2020 2043 6c61 7373 2074 6f20 686f  .    Class to ho
+0000aab0: 6c64 2074 6865 2064 6174 6120 6f66 2069  ld the data of i
+0000aac0: 6e64 6976 6964 7561 6c20 736c 6162 206d  ndividual slab m
+0000aad0: 6f64 656c 730a 2020 2020 2222 220a 0a20  odels.    """.. 
+0000aae0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+0000aaf0: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
+0000ab00: 656c 662e 7370 6563 6965 735f 6e75 6d62  elf.species_numb
+0000ab10: 6572 3d4e 6f6e 650a 2020 2020 2020 2020  er=None.        
+0000ab20: 7365 6c66 2e6d 6f64 656c 5f6e 756d 6265  self.model_numbe
+0000ab30: 723d 4e6f 6e65 0a20 2020 2020 2020 2073  r=None.        s
+0000ab40: 656c 662e 4e48 3d4e 6f6e 650a 2020 2020  elf.NH=None.    
+0000ab50: 2020 2020 7365 6c66 2e6e 436f 6c6c 3d4e      self.nColl=N
+0000ab60: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
+0000ab70: 2e6e 653d 4e6f 6e65 0a20 2020 2020 2020  .ne=None.       
+0000ab80: 2073 656c 662e 6e48 653d 4e6f 6e65 0a20   self.nHe=None. 
+0000ab90: 2020 2020 2020 2073 656c 662e 6e48 4949         self.nHII
+0000aba0: 3d4e 6f6e 650a 2020 2020 2020 2020 7365  =None.        se
+0000abb0: 6c66 2e6e 4849 3d4e 6f6e 650a 2020 2020  lf.nHI=None.    
+0000abc0: 2020 2020 7365 6c66 2e6e 4832 3d4e 6f6e      self.nH2=Non
+0000abd0: 650a 2020 2020 2020 2020 7365 6c66 2e64  e.        self.d
+0000abe0: 7573 745f 746f 5f67 6173 3d4e 6f6e 650a  ust_to_gas=None.
+0000abf0: 2020 2020 2020 2020 7365 6c66 2e76 7475          self.vtu
+0000ac00: 7262 3d4e 6f6e 650a 2020 2020 2020 2020  rb=None.        
+0000ac10: 7365 6c66 2e54 673d 4e6f 6e65 0a20 2020  self.Tg=None.   
+0000ac20: 2020 2020 2073 656c 662e 5464 3d4e 6f6e       self.Td=Non
+0000ac30: 650a 2020 2020 2020 2020 7365 6c66 2e73  e.        self.s
+0000ac40: 7065 6369 6573 5f6e 616d 653d 4e6f 6e65  pecies_name=None
+0000ac50: 0a20 2020 2020 2020 2073 656c 662e 7370  .        self.sp
+0000ac60: 6563 6965 735f 696e 6465 783d 4e6f 6e65  ecies_index=None
+0000ac70: 0a20 2020 2020 2020 2073 656c 662e 6162  .        self.ab
+0000ac80: 756e 6461 6e63 653d 4e6f 6e65 0a20 2020  undance=None.   
+0000ac90: 2020 2020 2073 656c 662e 6476 3d4e 6f6e       self.dv=Non
+0000aca0: 650a 2020 2020 2020 2020 7365 6c66 2e6e  e.        self.n
+0000acb0: 6c65 7665 6c73 3d4e 6f6e 650a 2020 2020  levels=None.    
+0000acc0: 2020 2020 7365 6c66 2e6e 6c69 6e65 733d      self.nlines=
+0000acd0: 4e6f 6e65 0a20 2020 2020 2020 2073 656c  None.        sel
+0000ace0: 662e 6c69 6e65 6461 7461 3d4e 6f6e 650a  f.linedata=None.
+0000acf0: 2020 2020 2020 2020 7365 6c66 2e6c 6576          self.lev
+0000ad00: 656c 6461 7461 3d4e 6f6e 650a 2020 2020  eldata=None.    
+0000ad10: 2020 2020 7365 6c66 2e63 6f6e 7657 6176      self.convWav
+0000ad20: 656c 656e 6774 683d 4e6f 6e65 0a20 2020  elength=None.   
+0000ad30: 2020 2020 2073 656c 662e 636f 6e76 4c54       self.convLT
+0000ad40: 4566 6c75 783d 4e6f 6e65 0a20 2020 2020  Eflux=None.     
+0000ad50: 2020 2073 656c 662e 636f 6e76 4e4c 5445     self.convNLTE
+0000ad60: 666c 7578 3d4e 6f6e 650a 2020 2020 2020  flux=None.      
+0000ad70: 2020 7365 6c66 2e63 6f6e 7654 7970 653d    self.convType=
+0000ad80: 4e6f 6e65 0a20 2020 2020 2020 2073 656c  None.        sel
+0000ad90: 662e 636f 6e76 523d 4e6f 6e65 0a20 2020  f.convR=None.   
+0000ada0: 2020 2020 2073 656c 662e 6f76 6572 6c61       self.overla
+0000adb0: 704c 5445 3d4e 6f6e 650a 2020 2020 2020  pLTE=None.      
+0000adc0: 2020 7365 6c66 2e6f 7665 726c 6170 4e4c    self.overlapNL
+0000add0: 5445 3d4e 6f6e 650a 2020 2020 2020 2020  TE=None.        
+0000ade0: 7365 6c66 2e6f 7665 726c 6170 5461 754c  self.overlapTauL
+0000adf0: 5445 3d4e 6f6e 650a 2020 2020 2020 2020  TE=None.        
+0000ae00: 7365 6c66 2e6f 7665 726c 6170 5461 754e  self.overlapTauN
+0000ae10: 4c54 453d 4e6f 6e65 0a20 2020 2020 2020  LTE=None.       
+0000ae20: 2073 656c 662e 6f76 6572 6c61 7046 7265   self.overlapFre
+0000ae30: 713d 4e6f 6e65 0a20 2020 2020 2020 2073  q=None.        s
+0000ae40: 656c 662e 636f 6e76 4f76 6572 6c61 704c  elf.convOverlapL
+0000ae50: 5445 3d4e 6f6e 650a 2020 2020 2020 2020  TE=None.        
+0000ae60: 7365 6c66 2e63 6f6e 764f 7665 726c 6170  self.convOverlap
+0000ae70: 4e4c 5445 3d4e 6f6e 650a 2020 2020 2020  NLTE=None.      
+0000ae80: 2020 7365 6c66 2e63 6f6e 764f 7665 726c    self.convOverl
+0000ae90: 6170 4672 6571 3d4e 6f6e 650a 2020 2020  apFreq=None.    
+0000aea0: 2020 2020 7365 6c66 2e63 6f6e 764f 7665      self.convOve
+0000aeb0: 726c 6170 5761 7665 3d4e 6f6e 650a 2020  rlapWave=None.  
+0000aec0: 2020 2020 2020 7365 6c66 2e63 6f6e 764f        self.convO
+0000aed0: 7665 726c 6170 523d 3165 350a 2020 2020  verlapR=1e5.    
+0000aee0: 2020 2020 7365 6c66 2e6f 7665 726c 6170      self.overlap
+0000aef0: 523d 3165 350a 0a20 2020 2064 6566 205f  R=1e5..    def _
+0000af00: 5f73 7472 5f5f 2873 656c 6629 3a0a 2020  _str__(self):.  
+0000af10: 2020 2020 2020 6f75 7470 7574 3d22 496e        output="In
+0000af20: 666f 204d 6f64 656c 3a20 5c6e 220a 2020  fo Model: \n".  
+0000af30: 2020 2020 2020 6f75 7470 7574 2b3d 2773        output+='s
+0000af40: 7065 6369 6573 5f6e 756d 6265 723d 2027  pecies_number= '
+0000af50: 0a20 2020 2020 2020 206f 7574 7075 742b  .        output+
+0000af60: 3d73 7472 2873 656c 662e 7370 6563 6965  =str(self.specie
+0000af70: 735f 6e75 6d62 6572 292b 275c 6e5c 6e27  s_number)+'\n\n'
+0000af80: 0a20 2020 2020 2020 206f 7574 7075 742b  .        output+
+0000af90: 3d27 6d6f 6465 6c5f 6e75 6d62 6572 2020  ='model_number  
+0000afa0: 3d20 270a 2020 2020 2020 2020 6f75 7470  = '.        outp
+0000afb0: 7574 2b3d 7374 7228 7365 6c66 2e6d 6f64  ut+=str(self.mod
+0000afc0: 656c 5f6e 756d 6265 7229 2b27 5c6e 5c6e  el_number)+'\n\n
+0000afd0: 270a 2020 2020 2020 2020 6f75 7470 7574  '.        output
+0000afe0: 2b3d 274e 4820 2020 2020 2020 2020 2020  +='NH           
+0000aff0: 203d 2027 0a20 2020 2020 2020 206f 7574   = '.        out
+0000b000: 7075 742b 3d73 7472 2873 656c 662e 4e48  put+=str(self.NH
+0000b010: 292b 275c 6e5c 6e27 0a20 2020 2020 2020  )+'\n\n'.       
+0000b020: 206f 7574 7075 742b 3d27 6e43 6f6c 6c20   output+='nColl 
+0000b030: 2020 2020 2020 2020 3d20 270a 2020 2020          = '.    
+0000b040: 2020 2020 6f75 7470 7574 2b3d 7374 7228      output+=str(
+0000b050: 7365 6c66 2e6e 436f 6c6c 292b 275c 6e5c  self.nColl)+'\n\
+0000b060: 6e27 0a20 2020 2020 2020 206f 7574 7075  n'.        outpu
+0000b070: 742b 3d27 6e65 2020 2020 2020 2020 2020  t+='ne          
+0000b080: 2020 3d20 270a 2020 2020 2020 2020 6f75    = '.        ou
+0000b090: 7470 7574 2b3d 7374 7228 7365 6c66 2e6e  tput+=str(self.n
+0000b0a0: 6529 2b27 5c6e 5c6e 270a 2020 2020 2020  e)+'\n\n'.      
+0000b0b0: 2020 6f75 7470 7574 2b3d 276e 4865 2020    output+='nHe  
+0000b0c0: 2020 2020 2020 2020 203d 2027 0a20 2020           = '.   
+0000b0d0: 2020 2020 206f 7574 7075 742b 3d73 7472       output+=str
+0000b0e0: 2873 656c 662e 6e48 6529 2b27 5c6e 5c6e  (self.nHe)+'\n\n
+0000b0f0: 270a 2020 2020 2020 2020 6f75 7470 7574  '.        output
+0000b100: 2b3d 276e 4849 4920 2020 2020 2020 2020  +='nHII         
+0000b110: 203d 2027 0a20 2020 2020 2020 206f 7574   = '.        out
+0000b120: 7075 742b 3d73 7472 2873 656c 662e 6e48  put+=str(self.nH
+0000b130: 4949 292b 275c 6e5c 6e27 0a20 2020 2020  II)+'\n\n'.     
+0000b140: 2020 206f 7574 7075 742b 3d27 6e48 4920     output+='nHI 
+0000b150: 2020 2020 2020 2020 2020 3d20 270a 2020            = '.  
+0000b160: 2020 2020 2020 6f75 7470 7574 2b3d 7374        output+=st
+0000b170: 7228 7365 6c66 2e6e 4849 292b 275c 6e5c  r(self.nHI)+'\n\
+0000b180: 6e27 0a20 2020 2020 2020 206f 7574 7075  n'.        outpu
+0000b190: 742b 3d27 6e48 3220 2020 2020 2020 2020  t+='nH2         
+0000b1a0: 2020 3d20 270a 2020 2020 2020 2020 6f75    = '.        ou
+0000b1b0: 7470 7574 2b3d 7374 7228 7365 6c66 2e6e  tput+=str(self.n
+0000b1c0: 4832 292b 275c 6e5c 6e27 0a20 2020 2020  H2)+'\n\n'.     
+0000b1d0: 2020 206f 7574 7075 742b 3d27 6475 7374     output+='dust
+0000b1e0: 5f74 6f5f 6761 7320 2020 3d20 270a 2020  _to_gas   = '.  
+0000b1f0: 2020 2020 2020 6f75 7470 7574 2b3d 7374        output+=st
+0000b200: 7228 7365 6c66 2e64 7573 745f 746f 5f67  r(self.dust_to_g
+0000b210: 6173 292b 275c 6e5c 6e27 0a20 2020 2020  as)+'\n\n'.     
+0000b220: 2020 206f 7574 7075 742b 3d27 7674 7572     output+='vtur
+0000b230: 6220 2020 2020 2020 2020 3d20 270a 2020  b         = '.  
+0000b240: 2020 2020 2020 6f75 7470 7574 2b3d 7374        output+=st
+0000b250: 7228 7365 6c66 2e76 7475 7262 292b 275c  r(self.vturb)+'\
+0000b260: 6e5c 6e27 0a20 2020 2020 2020 206f 7574  n\n'.        out
+0000b270: 7075 742b 3d27 5467 2020 2020 2020 2020  put+='Tg        
+0000b280: 2020 2020 3d20 270a 2020 2020 2020 2020      = '.        
+0000b290: 6f75 7470 7574 2b3d 7374 7228 7365 6c66  output+=str(self
+0000b2a0: 2e54 6729 2b27 5c6e 5c6e 270a 2020 2020  .Tg)+'\n\n'.    
+0000b2b0: 2020 2020 6f75 7470 7574 2b3d 2754 6420      output+='Td 
+0000b2c0: 2020 2020 2020 2020 2020 203d 2027 0a20             = '. 
+0000b2d0: 2020 2020 2020 206f 7574 7075 742b 3d73         output+=s
+0000b2e0: 7472 2873 656c 662e 5464 292b 275c 6e5c  tr(self.Td)+'\n\
+0000b2f0: 6e27 0a20 2020 2020 2020 206f 7574 7075  n'.        outpu
+0000b300: 742b 3d27 7370 6563 6965 735f 6e61 6d65  t+='species_name
+0000b310: 2020 203d 2027 0a20 2020 2020 2020 206f     = '.        o
+0000b320: 7574 7075 742b 3d73 656c 662e 7370 6563  utput+=self.spec
+0000b330: 6965 735f 6e61 6d65 2b27 5c6e 5c6e 270a  ies_name+'\n\n'.
+0000b340: 2020 2020 2020 2020 6f75 7470 7574 2b3d          output+=
+0000b350: 2761 6275 6e64 616e 6365 2020 2020 203d  'abundance     =
+0000b360: 2027 0a20 2020 2020 2020 206f 7574 7075   '.        outpu
+0000b370: 742b 3d73 7472 2873 656c 662e 6162 756e  t+=str(self.abun
+0000b380: 6461 6e63 6529 2b27 5c6e 5c6e 270a 2020  dance)+'\n\n'.  
+0000b390: 2020 2020 2020 6f75 7470 7574 2b3d 2764        output+='d
+0000b3a0: 7620 2020 2020 2020 2020 2020 203d 2027  v            = '
+0000b3b0: 0a20 2020 2020 2020 206f 7574 7075 742b  .        output+
+0000b3c0: 3d73 7472 2873 656c 662e 6476 292b 275c  =str(self.dv)+'\
+0000b3d0: 6e5c 6e27 0a20 2020 2020 2020 206f 7574  n\n'.        out
+0000b3e0: 7075 742b 3d27 6e6c 6576 656c 7320 2020  put+='nlevels   
+0000b3f0: 2020 2020 3d20 270a 2020 2020 2020 2020      = '.        
+0000b400: 6f75 7470 7574 2b3d 7374 7228 7365 6c66  output+=str(self
+0000b410: 2e6e 6c65 7665 6c73 292b 275c 6e5c 6e27  .nlevels)+'\n\n'
+0000b420: 0a20 2020 2020 2020 206f 7574 7075 742b  .        output+
+0000b430: 3d27 6e6c 696e 6573 2020 2020 2020 2020  ='nlines        
+0000b440: 3d20 270a 2020 2020 2020 2020 6f75 7470  = '.        outp
+0000b450: 7574 2b3d 7374 7228 7365 6c66 2e6e 6c69  ut+=str(self.nli
+0000b460: 6e65 7329 2b27 5c6e 5c6e 270a 2020 2020  nes)+'\n\n'.    
+0000b470: 2020 2020 6f75 7470 7574 2b3d 2763 6f6e      output+='con
+0000b480: 7654 7970 6520 2020 2020 2020 3d20 270a  vType       = '.
+0000b490: 2020 2020 2020 2020 6f75 7470 7574 2b3d          output+=
+0000b4a0: 7374 7228 7365 6c66 2e63 6f6e 7654 7970  str(self.convTyp
+0000b4b0: 6529 2b27 5c6e 5c6e 270a 2020 2020 2020  e)+'\n\n'.      
+0000b4c0: 2020 6f75 7470 7574 2b3d 2763 6f6e 7652    output+='convR
+0000b4d0: 2020 2020 2020 2020 3d20 270a 2020 2020          = '.    
+0000b4e0: 2020 2020 6f75 7470 7574 2b3d 7374 7228      output+=str(
+0000b4f0: 7365 6c66 2e63 6f6e 7652 292b 275c 6e5c  self.convR)+'\n\
+0000b500: 6e27 0a20 2020 2020 2020 2072 6574 7572  n'.        retur
+0000b510: 6e20 6f75 7470 7574 0a0a 2020 2020 6465  n output..    de
+0000b520: 6620 636f 6e76 6f6c 7665 2873 656c 662c  f convolve(self,
+0000b530: 6672 6571 5f62 696e 733d 4e6f 6e65 2c52  freq_bins=None,R
+0000b540: 3d31 2c6c 616d 6264 615f 303d 312c 6c61  =1,lambda_0=1,la
+0000b550: 6d62 6461 5f6e 3d31 2c76 723d 3133 3030  mbda_n=1,vr=1300
+0000b560: 2c4e 4c54 453d 4661 6c73 652c 636f 6e76  ,NLTE=False,conv
+0000b570: 5f74 7970 653d 312c 6f76 6572 6c61 703d  _type=1,overlap=
+0000b580: 4661 6c73 6529 3a0a 2020 2020 2020 2020  False):.        
+0000b590: 6966 206f 7665 726c 6170 3a0a 2020 2020  if overlap:.    
+0000b5a0: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+0000b5b0: 766f 6c76 655f 6f76 6572 6c61 7028 523d  volve_overlap(R=
+0000b5c0: 522c 6c61 6d62 6461 5f30 3d6c 616d 6264  R,lambda_0=lambd
+0000b5d0: 615f 302c 6c61 6d62 6461 5f6e 3d6c 616d  a_0,lambda_n=lam
+0000b5e0: 6264 615f 6e29 0a20 2020 2020 2020 2020  bda_n).         
+0000b5f0: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
+0000b600: 2020 743d 2746 4c54 4527 0a20 2020 2020    t='FLTE'.     
+0000b610: 2020 2069 6620 4e4c 5445 3a0a 2020 2020     if NLTE:.    
+0000b620: 2020 2020 2020 2020 743d 2746 4e4c 5445          t='FNLTE
+0000b630: 270a 2020 2020 2020 2020 6461 3d73 656c  '.        da=sel
+0000b640: 662e 6c69 6e65 6461 7461 0a20 2020 2020  f.linedata.     
+0000b650: 2020 2069 6620 6c61 6d62 6461 5f30 3d3d     if lambda_0==
+0000b660: 6c61 6d62 6461 5f6e 3a0a 2020 2020 2020  lambda_n:.      
+0000b670: 2020 2020 2020 6c61 6d62 6461 5f30 3d6e        lambda_0=n
+0000b680: 702e 616d 696e 2864 615b 2747 487a 275d  p.amin(da['GHz']
+0000b690: 3e63 2f6c 616d 6264 615f 6e2a 3165 2d33  >c/lambda_n*1e-3
+0000b6a0: 290a 2020 2020 2020 2020 2020 2020 6c61  ).            la
+0000b6b0: 6d62 6461 5f6e 3d6e 702e 616d 6178 2864  mbda_n=np.amax(d
+0000b6c0: 615b 2747 487a 275d 3e63 2f6c 616d 6264  a['GHz']>c/lambd
+0000b6d0: 615f 6e2a 3165 2d33 290a 2020 2020 2020  a_n*1e-3).      
+0000b6e0: 2020 2020 2020 6c61 6d62 6461 5f30 3d6c        lambda_0=l
+0000b6f0: 616d 6264 615f 302a 3130 2a2a 2d30 2e30  ambda_0*10**-0.0
+0000b700: 350a 2020 2020 2020 2020 2020 2020 6c61  5.            la
+0000b710: 6d62 6461 5f6e 3d6c 616d 6264 615f 6e2a  mbda_n=lambda_n*
+0000b720: 3130 2a2a 302e 3035 0a20 2020 2020 2020  10**0.05.       
+0000b730: 2064 615f 7265 713d 6461 5b28 6461 5b27   da_req=da[(da['
+0000b740: 4748 7a27 5d3e 632f 6c61 6d62 6461 5f6e  GHz']>c/lambda_n
+0000b750: 2a31 652d 3329 2628 6461 5b27 4748 7a27  *1e-3)&(da['GHz'
+0000b760: 5d3c 632f 6c61 6d62 6461 5f30 2a31 652d  ]<c/lambda_0*1e-
+0000b770: 3329 5d0a 2020 2020 2020 2020 6461 5f72  3)].        da_r
+0000b780: 6571 2e72 6573 6574 5f69 6e64 6578 2864  eq.reset_index(d
+0000b790: 726f 703d 5472 7565 2c69 6e70 6c61 6365  rop=True,inplace
+0000b7a0: 3d54 7275 6529 0a20 2020 2020 2020 2069  =True).        i
+0000b7b0: 6620 636f 6e76 5f74 7970 653d 3d31 3a0a  f conv_type==1:.
+0000b7c0: 2020 2020 2020 2020 2020 2020 6c2c 663d              l,f=
+0000b7d0: 6765 6e65 7261 6c43 6f6e 766f 6c76 6528  generalConvolve(
+0000b7e0: 6461 5f72 6571 5b74 5d2c 6461 5f72 6571  da_req[t],da_req
+0000b7f0: 5b27 4748 7a27 5d2c 523d 522c 6c61 6d62  ['GHz'],R=R,lamb
+0000b800: 6461 5f30 3d6c 616d 6264 615f 302c 6c61  da_0=lambda_0,la
+0000b810: 6d62 6461 5f6e 3d6c 616d 6264 615f 6e29  mbda_n=lambda_n)
+0000b820: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+0000b830: 2020 2020 2020 2020 2020 206c 2c66 3d73             l,f=s
+0000b840: 7065 6343 6f6e 766f 6c76 6528 6461 5f72  pecConvolve(da_r
+0000b850: 6571 5b74 5d2c 6461 5f72 6571 5b27 4748  eq[t],da_req['GH
+0000b860: 7a27 5d2c 6672 6571 5f62 696e 733d 6672  z'],freq_bins=fr
+0000b870: 6571 5f62 696e 732c 523d 522c 6c61 6d62  eq_bins,R=R,lamb
+0000b880: 6461 5f30 3d6c 616d 6264 615f 302c 6c61  da_0=lambda_0,la
+0000b890: 6d62 6461 5f6e 3d6c 616d 6264 615f 6e2c  mbda_n=lambda_n,
+0000b8a0: 7672 3d76 7229 0a20 2020 2020 2020 2073  vr=vr).        s
+0000b8b0: 656c 662e 636f 6e76 5761 7665 6c65 6e67  elf.convWaveleng
+0000b8c0: 7468 3d6c 0a20 2020 2020 2020 2073 656c  th=l.        sel
+0000b8d0: 662e 636f 6e76 5479 7065 3d63 6f6e 765f  f.convType=conv_
+0000b8e0: 7479 7065 0a20 2020 2020 2020 2073 656c  type.        sel
+0000b8f0: 662e 636f 6e76 523d 520a 2020 2020 2020  f.convR=R.      
+0000b900: 2020 6966 204e 4c54 453a 0a20 2020 2020    if NLTE:.     
+0000b910: 2020 2020 2020 2073 656c 662e 636f 6e76         self.conv
+0000b920: 4e4c 5445 666c 7578 3d66 0a20 2020 2020  NLTEflux=f.     
+0000b930: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000b940: 2020 2020 2073 656c 662e 636f 6e76 4c54       self.convLT
+0000b950: 4566 6c75 783d 660a 0a20 2020 2064 6566  Eflux=f..    def
+0000b960: 2063 6f6e 766f 6c76 655f 6f76 6572 6c61   convolve_overla
+0000b970: 7028 7365 6c66 2c52 3d31 2c6c 616d 6264  p(self,R=1,lambd
+0000b980: 615f 303d 312c 6c61 6d62 6461 5f6e 3d31  a_0=1,lambda_n=1
+0000b990: 293a 0a20 2020 2020 2020 2069 6620 6c61  ):.        if la
+0000b9a0: 6d62 6461 5f30 3d3d 6c61 6d62 6461 5f6e  mbda_0==lambda_n
+0000b9b0: 3a0a 2020 2020 2020 2020 2020 2020 6c61  :.            la
+0000b9c0: 6d62 6461 5f30 3d6e 702e 616d 696e 2863  mbda_0=np.amin(c
+0000b9d0: 2f73 656c 662e 6f76 6572 6c61 7046 7265  /self.overlapFre
+0000b9e0: 712a 3165 2d33 290a 2020 2020 2020 2020  q*1e-3).        
+0000b9f0: 2020 2020 6c61 6d62 6461 5f6e 3d6e 702e      lambda_n=np.
+0000ba00: 616d 6178 2863 2f73 656c 662e 6f76 6572  amax(c/self.over
+0000ba10: 6c61 7046 7265 712a 3165 2d33 290a 2020  lapFreq*1e-3).  
+0000ba20: 2020 2020 2020 2020 2020 6c61 6d62 6461            lambda
+0000ba30: 5f30 3d6c 616d 6264 615f 302a 3130 2a2a  _0=lambda_0*10**
+0000ba40: 2d30 2e30 350a 2020 2020 2020 2020 2020  -0.05.          
+0000ba50: 2020 6c61 6d62 6461 5f6e 3d6c 616d 6264    lambda_n=lambd
+0000ba60: 615f 6e2a 3130 2a2a 302e 3035 0a20 2020  a_n*10**0.05.   
+0000ba70: 2020 2020 206d 6173 6b3d 2873 656c 662e       mask=(self.
+0000ba80: 6f76 6572 6c61 7046 7265 713e 632f 6c61  overlapFreq>c/la
+0000ba90: 6d62 6461 5f6e 2a31 652d 3329 2628 7365  mbda_n*1e-3)&(se
+0000baa0: 6c66 2e6f 7665 726c 6170 4672 6571 3c63  lf.overlapFreq<c
+0000bab0: 2f6c 616d 6264 615f 302a 3165 2d33 290a  /lambda_0*1e-3).
+0000bac0: 2020 2020 2020 2020 4657 484d 3d73 656c          FWHM=sel
+0000bad0: 662e 6f76 6572 6c61 7052 2f52 2f32 2e33  f.overlapR/R/2.3
+0000bae0: 3535 0a20 2020 2020 2020 2067 3d47 6175  55.        g=Gau
+0000baf0: 7373 6961 6e31 444b 6572 6e65 6c28 7374  ssian1DKernel(st
+0000bb00: 6464 6576 3d46 5748 4d2c 6661 6374 6f72  ddev=FWHM,factor
+0000bb10: 3d37 290a 2020 2020 2020 2020 7365 6c66  =7).        self
+0000bb20: 2e63 6f6e 764f 7665 726c 6170 4c54 453d  .convOverlapLTE=
+0000bb30: 6170 795f 636f 6e76 6f6c 7665 2873 656c  apy_convolve(sel
+0000bb40: 662e 6f76 6572 6c61 704c 5445 5b6d 6173  f.overlapLTE[mas
+0000bb50: 6b5d 2c67 290a 2020 2020 2020 2020 7365  k],g).        se
+0000bb60: 6c66 2e63 6f6e 764f 7665 726c 6170 4e4c  lf.convOverlapNL
+0000bb70: 5445 3d61 7079 5f63 6f6e 766f 6c76 6528  TE=apy_convolve(
+0000bb80: 7365 6c66 2e6f 7665 726c 6170 4e4c 5445  self.overlapNLTE
+0000bb90: 5b6d 6173 6b5d 2c67 290a 2020 2020 2020  [mask],g).      
+0000bba0: 2020 7365 6c66 2e63 6f6e 764f 7665 726c    self.convOverl
+0000bbb0: 6170 4672 6571 3d73 656c 662e 6f76 6572  apFreq=self.over
+0000bbc0: 6c61 7046 7265 715b 6d61 736b 5d2a 312e  lapFreq[mask]*1.
+0000bbd0: 300a 2020 2020 2020 2020 7365 6c66 2e63  0.        self.c
+0000bbe0: 6f6e 764f 7665 726c 6170 5761 7665 3d63  onvOverlapWave=c
+0000bbf0: 2f73 656c 662e 636f 6e76 4f76 6572 6c61  /self.convOverla
+0000bc00: 7046 7265 712a 3165 2d33 0a20 2020 2020  pFreq*1e-3.     
+0000bc10: 2020 2073 656c 662e 636f 6e76 4f76 6572     self.convOver
+0000bc20: 6c61 7052 3d52 0a0a 2020 2020 6465 6620  lapR=R..    def 
+0000bc30: 7368 6f77 2873 656c 6629 3a0a 2020 2020  show(self):.    
+0000bc40: 2020 2020 7072 696e 7428 7365 6c66 290a      print(self).
+0000bc50: 2020 2020 2020 2020 7072 696e 7428 276c          print('l
+0000bc60: 696e 6544 6174 6120 2020 203d 2027 290a  ineData    = ').
+0000bc70: 2020 2020 2020 2020 7072 696e 7428 7365          print(se
+0000bc80: 6c66 2e6c 696e 6564 6174 6129 0a20 2020  lf.linedata).   
+0000bc90: 2020 2020 2070 7269 6e74 2827 6c65 7665       print('leve
+0000bca0: 6c44 6174 6120 2020 3d20 2729 0a20 2020  lData   = ').   
+0000bcb0: 2020 2020 2070 7269 6e74 2873 656c 662e       print(self.
+0000bcc0: 6c65 7665 6c64 6174 6129 0a0a 0a63 6c61  leveldata)...cla
+0000bcd0: 7373 2073 6c61 6231 443a 0a20 2020 2022  ss slab1D:.    "
+0000bce0: 2222 0a20 2020 2063 6c61 7373 3a3a 2073  "".    class:: s
+0000bcf0: 6c61 6231 440a 2020 2020 436c 6173 7320  lab1D.    Class 
+0000bd00: 746f 2068 6f6c 6420 7468 6520 6461 7461  to hold the data
+0000bd10: 206f 6620 3144 2073 6c61 6220 6d6f 6465   of 1D slab mode
+0000bd20: 6c73 0a20 2020 2022 2222 0a0a 2020 2020  ls.    """..    
+0000bd30: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+0000bd40: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
+0000bd50: 2e64 6972 6563 746f 7279 3d4e 6f6e 650a  .directory=None.
+0000bd60: 2020 2020 2020 2020 7365 6c66 2e66 6c75          self.flu
+0000bd70: 783d 4e6f 6e65 0a20 2020 2020 2020 2073  x=None.        s
+0000bd80: 656c 662e 6672 6571 7565 6e63 793d 4e6f  elf.frequency=No
+0000bd90: 6e65 0a20 2020 2020 2020 2073 656c 662e  ne.        self.
+0000bda0: 4e73 7065 6369 6573 3d4e 6f6e 650a 2020  Nspecies=None.  
+0000bdb0: 2020 2020 2020 7365 6c66 2e73 7065 6369        self.speci
+0000bdc0: 6573 3d5b 5d0a 2020 2020 2020 2020 7365  es=[].        se
+0000bdd0: 6c66 2e4e 6772 6964 3d4e 6f6e 650a 2020  lf.Ngrid=None.  
+0000bde0: 2020 2020 2020 7365 6c66 2e52 3d4e 6f6e        self.R=Non
+0000bdf0: 650a 2020 2020 2020 2020 7365 6c66 2e67  e.        self.g
+0000be00: 7269 643d 7064 2e44 6174 6146 7261 6d65  rid=pd.DataFrame
+0000be10: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+0000be20: 736f 7572 6365 5f66 756e 6374 696f 6e3d  source_function=
 0000be30: 4e6f 6e65 0a20 2020 2020 2020 2073 656c  None.        sel
-0000be40: 662e 636f 6e76 5f66 6c75 783d 4e6f 6e65  f.conv_flux=None
-0000be50: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
-0000be60: 6e76 523d 4e6f 6e65 0a0a 2020 2020 6465  nvR=None..    de
-0000be70: 6620 5f5f 7374 725f 5f28 7365 6c66 293a  f __str__(self):
-0000be80: 0a20 2020 2020 2020 206f 7574 7075 743d  .        output=
-0000be90: 2249 6e66 6f20 4d6f 6465 6c3a 205c 6e22  "Info Model: \n"
-0000bea0: 0a20 2020 2020 2020 206f 7574 7075 742b  .        output+
-0000beb0: 3d27 4e75 6d62 6572 206f 6620 7370 6563  ='Number of spec
-0000bec0: 6965 7320 2020 2020 2020 2020 203d 2027  ies          = '
-0000bed0: 0a20 2020 2020 2020 206f 7574 7075 742b  .        output+
-0000bee0: 3d73 7472 2873 656c 662e 4e73 7065 6369  =str(self.Nspeci
-0000bef0: 6573 292b 275c 6e5c 6e27 0a20 2020 2020  es)+'\n\n'.     
-0000bf00: 2020 206f 7574 7075 742b 3d27 4772 6964     output+='Grid
-0000bf10: 2073 697a 6520 2020 2020 2020 2020 2020   size           
-0000bf20: 2020 2020 2020 203d 2027 0a20 2020 2020         = '.     
-0000bf30: 2020 206f 7574 7075 742b 3d73 7472 2873     output+=str(s
-0000bf40: 656c 662e 4e67 7269 6429 2b27 5c6e 5c6e  elf.Ngrid)+'\n\n
-0000bf50: 270a 2020 2020 2020 2020 6f75 7470 7574  '.        output
-0000bf60: 2b3d 2752 6573 6f6c 7669 6e67 2070 6f77  +='Resolving pow
-0000bf70: 6572 206f 6620 7370 6563 7472 6120 3d20  er of spectra = 
-0000bf80: 270a 2020 2020 2020 2020 6f75 7470 7574  '.        output
-0000bf90: 2b3d 7374 7228 7365 6c66 2e52 292b 275c  +=str(self.R)+'\
-0000bfa0: 6e5c 6e27 0a20 2020 2020 2020 206f 7574  n\n'.        out
-0000bfb0: 7075 742b 3d27 4f75 7470 7574 2066 696c  put+='Output fil
-0000bfc0: 6520 7061 7468 203d 2027 0a20 2020 2020  e path = '.     
-0000bfd0: 2020 206f 7574 7075 742b 3d73 7472 2873     output+=str(s
-0000bfe0: 656c 662e 6469 7265 6374 6f72 7929 2b27  elf.directory)+'
-0000bff0: 5c6e 5c6e 270a 2020 2020 2020 2020 7265  \n\n'.        re
-0000c000: 7475 726e 206f 7574 7075 740a 0a20 2020  turn output..   
-0000c010: 2064 6566 2063 6f6e 766f 6c76 6528 7365   def convolve(se
-0000c020: 6c66 2c52 3d31 2c6c 616d 6264 615f 303d  lf,R=1,lambda_0=
-0000c030: 312c 6c61 6d62 6461 5f6e 3d31 2c76 6572  1,lambda_n=1,ver
-0000c040: 626f 7365 3d54 7275 6529 3a0a 2020 2020  bose=True):.    
-0000c050: 2020 2020 6966 2076 6572 626f 7365 3a20      if verbose: 
-0000c060: 7072 696e 7428 2243 6f6e 766f 6c76 696e  print("Convolvin
-0000c070: 6720 746f 2022 2c52 290a 2020 2020 2020  g to ",R).      
-0000c080: 2020 6966 206c 616d 6264 615f 303d 3d6c    if lambda_0==l
-0000c090: 616d 6264 615f 6e3a 0a20 2020 2020 2020  ambda_n:.       
-0000c0a0: 2020 2020 206c 616d 6264 615f 303d 6e70       lambda_0=np
-0000c0b0: 2e61 6d69 6e28 632f 7365 6c66 2e66 7265  .amin(c/self.fre
-0000c0c0: 7175 656e 6379 2a31 652d 3329 0a20 2020  quency*1e-3).   
-0000c0d0: 2020 2020 2020 2020 206c 616d 6264 615f           lambda_
-0000c0e0: 6e3d 6e70 2e61 6d61 7828 632f 7365 6c66  n=np.amax(c/self
-0000c0f0: 2e66 7265 7175 656e 6379 2a31 652d 3329  .frequency*1e-3)
-0000c100: 0a20 2020 2020 2020 2020 2020 206c 616d  .            lam
-0000c110: 6264 615f 303d 6c61 6d62 6461 5f30 2a31  bda_0=lambda_0*1
-0000c120: 302a 2a2d 302e 3035 0a20 2020 2020 2020  0**-0.05.       
-0000c130: 2020 2020 206c 616d 6264 615f 6e3d 6c61       lambda_n=la
-0000c140: 6d62 6461 5f6e 2a31 302a 2a30 2e30 350a  mbda_n*10**0.05.
-0000c150: 2020 2020 2020 2020 6d61 736b 3d28 7365          mask=(se
-0000c160: 6c66 2e66 7265 7175 656e 6379 3e63 2f6c  lf.frequency>c/l
-0000c170: 616d 6264 615f 6e2a 3165 2d33 2926 2873  ambda_n*1e-3)&(s
-0000c180: 656c 662e 6672 6571 7565 6e63 793c 632f  elf.frequency<c/
-0000c190: 6c61 6d62 6461 5f30 2a31 652d 3329 0a20  lambda_0*1e-3). 
-0000c1a0: 2020 2020 2020 2046 5748 4d3d 7365 6c66         FWHM=self
-0000c1b0: 2e52 2f52 2f32 2e33 3535 0a20 2020 2020  .R/R/2.355.     
-0000c1c0: 2020 2067 3d47 6175 7373 6961 6e31 444b     g=Gaussian1DK
-0000c1d0: 6572 6e65 6c28 7374 6464 6576 3d46 5748  ernel(stddev=FWH
-0000c1e0: 4d2c 6661 6374 6f72 3d37 290a 2020 2020  M,factor=7).    
-0000c1f0: 2020 2020 7365 6c66 2e63 6f6e 765f 666c      self.conv_fl
-0000c200: 7578 3d61 7079 5f63 6f6e 766f 6c76 6528  ux=apy_convolve(
-0000c210: 7365 6c66 2e66 6c75 785b 6d61 736b 5d2c  self.flux[mask],
-0000c220: 6729 0a20 2020 2020 2020 2073 656c 662e  g).        self.
-0000c230: 636f 6e76 4672 6571 7565 6e63 793d 7365  convFrequency=se
-0000c240: 6c66 2e66 7265 7175 656e 6379 5b6d 6173  lf.frequency[mas
-0000c250: 6b5d 2a31 2e30 0a20 2020 2020 2020 2073  k]*1.0.        s
-0000c260: 656c 662e 636f 6e76 523d 520a 2020 2020  elf.convR=R.    
-0000c270: 2020 2020 7365 6c66 2e63 6f6e 7657 6176      self.convWav
-0000c280: 656c 656e 6774 683d 632f 7365 6c66 2e63  elength=c/self.c
-0000c290: 6f6e 7646 7265 7175 656e 6379 2a31 652d  onvFrequency*1e-
-0000c2a0: 330a 0a20 2020 2064 6566 2073 686f 7728  3..    def show(
-0000c2b0: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
-0000c2c0: 7269 6e74 2873 656c 6629 0a20 2020 2020  rint(self).     
-0000c2d0: 2020 2070 7269 6e74 2827 4772 6964 2020     print('Grid  
-0000c2e0: 2020 3d20 2729 0a20 2020 2020 2020 2070    = ').        p
-0000c2f0: 7269 6e74 2873 656c 662e 6772 6964 290a  rint(self.grid).
-0000c300: 2020 2020 2020 2020 7072 696e 7428 2753          print('S
-0000c310: 6f75 7263 6520 6675 6e63 7469 6f6e 2020  ource function  
-0000c320: 203d 2027 290a 2020 2020 2020 2020 7072   = ').        pr
-0000c330: 696e 7428 7365 6c66 2e73 6f75 7263 655f  int(self.source_
-0000c340: 6675 6e63 7469 6f6e 290a 2020 2020 2020  function).      
-0000c350: 2020 7072 696e 7428 2747 6173 206f 6e6c    print('Gas onl
-0000c360: 7920 736f 7572 6365 2066 756e 6374 696f  y source functio
-0000c370: 6e20 2020 3d20 2729 0a20 2020 2020 2020  n   = ').       
-0000c380: 2070 7269 6e74 2873 656c 662e 736f 7572   print(self.sour
-0000c390: 6365 5f66 756e 6374 696f 6e5f 6761 7329  ce_function_gas)
-0000c3a0: 0a20 2020 2020 2020 2070 7269 6e74 2827  .        print('
-0000c3b0: 4475 7374 206f 7074 6963 616c 2064 6570  Dust optical dep
-0000c3c0: 7468 2020 203d 2027 290a 2020 2020 2020  th   = ').      
-0000c3d0: 2020 7072 696e 7428 7365 6c66 2e74 6175    print(self.tau
-0000c3e0: 5f64 7573 7429 0a20 2020 2020 2020 2070  _dust).        p
-0000c3f0: 7269 6e74 2827 4761 7320 6f70 7469 6361  rint('Gas optica
-0000c400: 6c20 6465 7074 6820 2020 3d20 2729 0a20  l depth   = '). 
-0000c410: 2020 2020 2020 2070 7269 6e74 2873 656c         print(sel
-0000c420: 662e 7461 755f 6761 7329 0a0a 0a64 6566  f.tau_gas)...def
-0000c430: 2072 6561 645f 3144 5f73 6c61 6228 6d6f   read_1D_slab(mo
-0000c440: 6465 6c5f 7061 7468 3d27 536c 6162 5265  del_path='SlabRe
-0000c450: 7375 6c74 732e 6669 7473 2e67 7a27 2c76  sults.fits.gz',v
-0000c460: 6572 626f 7365 3d54 7275 6529 3a0a 2020  erbose=True):.  
-0000c470: 2020 2222 220a 2020 2020 4675 6e63 7469    """.    Functi
-0000c480: 6f6e 2074 6f20 7265 6164 2031 4420 7072  on to read 1D pr
-0000c490: 6f64 696d 6f20 736c 6162 206d 6f64 656c  odimo slab model
-0000c4a0: 206f 7574 7075 740a 2020 2020 2222 220a   output.    """.
-0000c4b0: 2020 2020 6966 2076 6572 626f 7365 3a20      if verbose: 
-0000c4c0: 7072 696e 7428 2252 6561 6469 6e67 2031  print("Reading 1
-0000c4d0: 4420 736c 6162 206d 6f64 656c 206f 7574  D slab model out
-0000c4e0: 7075 7420 6672 6f6d 3a20 222c 6d6f 6465  put from: ",mode
-0000c4f0: 6c5f 7061 7468 290a 2020 2020 6966 2027  l_path).    if '
-0000c500: 2e66 6974 732e 677a 2720 696e 206d 6f64  .fits.gz' in mod
-0000c510: 656c 5f70 6174 683a 0a20 2020 2020 2020  el_path:.       
-0000c520: 2068 6475 6c3d 6669 7473 2e6f 7065 6e28   hdul=fits.open(
-0000c530: 6d6f 6465 6c5f 7061 7468 290a 2020 2020  model_path).    
-0000c540: 2020 2020 6461 7461 3d73 6c61 6231 4428      data=slab1D(
-0000c550: 290a 2020 2020 2020 2020 6461 7461 2e64  ).        data.d
-0000c560: 6972 6563 746f 7279 3d6d 6f64 656c 5f70  irectory=model_p
-0000c570: 6174 680a 2020 2020 2020 2020 6461 7461  ath.        data
-0000c580: 2e66 6c75 783d 6864 756c 5b30 5d2e 6461  .flux=hdul[0].da
-0000c590: 7461 2e54 5b3a 2c31 5d0a 2020 2020 2020  ta.T[:,1].      
-0000c5a0: 2020 6461 7461 2e66 7265 7175 656e 6379    data.frequency
-0000c5b0: 3d68 6475 6c5b 305d 2e64 6174 612e 545b  =hdul[0].data.T[
-0000c5c0: 3a2c 305d 0a20 2020 2020 2020 2064 6174  :,0].        dat
-0000c5d0: 612e 4e73 7065 6369 6573 3d68 6475 6c5b  a.Nspecies=hdul[
-0000c5e0: 305d 2e68 6561 6465 725b 274e 5350 4543  0].header['NSPEC
-0000c5f0: 4945 5327 5d0a 2020 2020 2020 2020 6461  IES'].        da
-0000c600: 7461 2e73 7065 6369 6573 3d68 6475 6c5b  ta.species=hdul[
-0000c610: 305d 2e68 6561 6465 722e 636f 6d6d 656e  0].header.commen
-0000c620: 7473 5b27 4e53 5045 4349 4553 275d 2e73  ts['NSPECIES'].s
-0000c630: 706c 6974 2827 2c27 290a 2020 2020 2020  plit(',').      
-0000c640: 2020 6461 7461 2e4e 6772 6964 3d68 6475    data.Ngrid=hdu
-0000c650: 6c5b 305d 2e68 6561 6465 725b 274e 4752  l[0].header['NGR
-0000c660: 4944 275d 0a20 2020 2020 2020 2064 6174  ID'].        dat
-0000c670: 612e 523d 6864 756c 5b30 5d2e 6865 6164  a.R=hdul[0].head
-0000c680: 6572 5b27 525f 4f56 4c50 275d 0a20 2020  er['R_OVLP'].   
-0000c690: 2020 2020 2069 6620 2828 392b 6461 7461       if ((9+data
-0000c6a0: 2e4e 7370 6563 6965 732a 3229 2c64 6174  .Nspecies*2),dat
-0000c6b0: 612e 4e67 7269 6429 3d3d 6864 756c 5b31  a.Ngrid)==hdul[1
-0000c6c0: 5d2e 6461 7461 2e54 2e73 6861 7065 3a0a  ].data.T.shape:.
-0000c6d0: 2020 2020 2020 2020 2020 2020 6772 6964              grid
-0000c6e0: 3d68 6475 6c5b 315d 2e64 6174 610a 2020  =hdul[1].data.  
-0000c6f0: 2020 2020 2020 2020 2020 6461 7461 2e67            data.g
-0000c700: 7269 645b 2764 7a27 5d3d 6772 6964 5b3a  rid['dz']=grid[:
-0000c710: 2c30 5d0a 2020 2020 2020 2020 2020 2020  ,0].            
-0000c720: 6461 7461 2e67 7269 645b 2776 7475 7262  data.grid['vturb
-0000c730: 275d 3d67 7269 645b 3a2c 315d 0a20 2020  ']=grid[:,1].   
-0000c740: 2020 2020 2020 2020 2064 6174 612e 6772           data.gr
-0000c750: 6964 5b27 6e64 275d 3d67 7269 645b 3a2c  id['nd']=grid[:,
-0000c760: 325d 0a20 2020 2020 2020 2020 2020 2064  2].            d
-0000c770: 6174 612e 6772 6964 5b27 5464 275d 3d67  ata.grid['Td']=g
-0000c780: 7269 645b 3a2c 335d 0a20 2020 2020 2020  rid[:,3].       
-0000c790: 2020 2020 2064 6174 612e 6772 6964 5b27       data.grid['
-0000c7a0: 6e48 3227 5d3d 6772 6964 5b3a 2c34 5d0a  nH2']=grid[:,4].
+0000be40: 662e 736f 7572 6365 5f66 756e 6374 696f  f.source_functio
+0000be50: 6e5f 6761 733d 4e6f 6e65 0a20 2020 2020  n_gas=None.     
+0000be60: 2020 2073 656c 662e 7461 755f 6475 7374     self.tau_dust
+0000be70: 3d4e 6f6e 650a 2020 2020 2020 2020 7365  =None.        se
+0000be80: 6c66 2e74 6175 5f67 6173 3d4e 6f6e 650a  lf.tau_gas=None.
+0000be90: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+0000bea0: 7657 6176 656c 656e 6774 683d 4e6f 6e65  vWavelength=None
+0000beb0: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
+0000bec0: 6e76 4672 6571 7565 6e63 793d 4e6f 6e65  nvFrequency=None
+0000bed0: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
+0000bee0: 6e76 5f66 6c75 783d 4e6f 6e65 0a20 2020  nv_flux=None.   
+0000bef0: 2020 2020 2073 656c 662e 636f 6e76 523d       self.convR=
+0000bf00: 4e6f 6e65 0a0a 2020 2020 6465 6620 5f5f  None..    def __
+0000bf10: 7374 725f 5f28 7365 6c66 293a 0a20 2020  str__(self):.   
+0000bf20: 2020 2020 206f 7574 7075 743d 2249 6e66       output="Inf
+0000bf30: 6f20 4d6f 6465 6c3a 205c 6e22 0a20 2020  o Model: \n".   
+0000bf40: 2020 2020 206f 7574 7075 742b 3d27 4e75       output+='Nu
+0000bf50: 6d62 6572 206f 6620 7370 6563 6965 7320  mber of species 
+0000bf60: 2020 2020 2020 2020 203d 2027 0a20 2020           = '.   
+0000bf70: 2020 2020 206f 7574 7075 742b 3d73 7472       output+=str
+0000bf80: 2873 656c 662e 4e73 7065 6369 6573 292b  (self.Nspecies)+
+0000bf90: 275c 6e5c 6e27 0a20 2020 2020 2020 206f  '\n\n'.        o
+0000bfa0: 7574 7075 742b 3d27 4772 6964 2073 697a  utput+='Grid siz
+0000bfb0: 6520 2020 2020 2020 2020 2020 2020 2020  e               
+0000bfc0: 2020 203d 2027 0a20 2020 2020 2020 206f     = '.        o
+0000bfd0: 7574 7075 742b 3d73 7472 2873 656c 662e  utput+=str(self.
+0000bfe0: 4e67 7269 6429 2b27 5c6e 5c6e 270a 2020  Ngrid)+'\n\n'.  
+0000bff0: 2020 2020 2020 6f75 7470 7574 2b3d 2752        output+='R
+0000c000: 6573 6f6c 7669 6e67 2070 6f77 6572 206f  esolving power o
+0000c010: 6620 7370 6563 7472 6120 3d20 270a 2020  f spectra = '.  
+0000c020: 2020 2020 2020 6f75 7470 7574 2b3d 7374        output+=st
+0000c030: 7228 7365 6c66 2e52 292b 275c 6e5c 6e27  r(self.R)+'\n\n'
+0000c040: 0a20 2020 2020 2020 206f 7574 7075 742b  .        output+
+0000c050: 3d27 4f75 7470 7574 2066 696c 6520 7061  ='Output file pa
+0000c060: 7468 203d 2027 0a20 2020 2020 2020 206f  th = '.        o
+0000c070: 7574 7075 742b 3d73 7472 2873 656c 662e  utput+=str(self.
+0000c080: 6469 7265 6374 6f72 7929 2b27 5c6e 5c6e  directory)+'\n\n
+0000c090: 270a 2020 2020 2020 2020 7265 7475 726e  '.        return
+0000c0a0: 206f 7574 7075 740a 0a20 2020 2064 6566   output..    def
+0000c0b0: 2063 6f6e 766f 6c76 6528 7365 6c66 2c52   convolve(self,R
+0000c0c0: 3d31 2c6c 616d 6264 615f 303d 312c 6c61  =1,lambda_0=1,la
+0000c0d0: 6d62 6461 5f6e 3d31 2c76 6572 626f 7365  mbda_n=1,verbose
+0000c0e0: 3d54 7275 6529 3a0a 2020 2020 2020 2020  =True):.        
+0000c0f0: 6966 2076 6572 626f 7365 3a20 7072 696e  if verbose: prin
+0000c100: 7428 2243 6f6e 766f 6c76 696e 6720 746f  t("Convolving to
+0000c110: 2022 2c52 290a 2020 2020 2020 2020 6966   ",R).        if
+0000c120: 206c 616d 6264 615f 303d 3d6c 616d 6264   lambda_0==lambd
+0000c130: 615f 6e3a 0a20 2020 2020 2020 2020 2020  a_n:.           
+0000c140: 206c 616d 6264 615f 303d 6e70 2e61 6d69   lambda_0=np.ami
+0000c150: 6e28 632f 7365 6c66 2e66 7265 7175 656e  n(c/self.frequen
+0000c160: 6379 2a31 652d 3329 0a20 2020 2020 2020  cy*1e-3).       
+0000c170: 2020 2020 206c 616d 6264 615f 6e3d 6e70       lambda_n=np
+0000c180: 2e61 6d61 7828 632f 7365 6c66 2e66 7265  .amax(c/self.fre
+0000c190: 7175 656e 6379 2a31 652d 3329 0a20 2020  quency*1e-3).   
+0000c1a0: 2020 2020 2020 2020 206c 616d 6264 615f           lambda_
+0000c1b0: 303d 6c61 6d62 6461 5f30 2a31 302a 2a2d  0=lambda_0*10**-
+0000c1c0: 302e 3035 0a20 2020 2020 2020 2020 2020  0.05.           
+0000c1d0: 206c 616d 6264 615f 6e3d 6c61 6d62 6461   lambda_n=lambda
+0000c1e0: 5f6e 2a31 302a 2a30 2e30 350a 2020 2020  _n*10**0.05.    
+0000c1f0: 2020 2020 6d61 736b 3d28 7365 6c66 2e66      mask=(self.f
+0000c200: 7265 7175 656e 6379 3e63 2f6c 616d 6264  requency>c/lambd
+0000c210: 615f 6e2a 3165 2d33 2926 2873 656c 662e  a_n*1e-3)&(self.
+0000c220: 6672 6571 7565 6e63 793c 632f 6c61 6d62  frequency<c/lamb
+0000c230: 6461 5f30 2a31 652d 3329 0a20 2020 2020  da_0*1e-3).     
+0000c240: 2020 2046 5748 4d3d 7365 6c66 2e52 2f52     FWHM=self.R/R
+0000c250: 2f32 2e33 3535 0a20 2020 2020 2020 2067  /2.355.        g
+0000c260: 3d47 6175 7373 6961 6e31 444b 6572 6e65  =Gaussian1DKerne
+0000c270: 6c28 7374 6464 6576 3d46 5748 4d2c 6661  l(stddev=FWHM,fa
+0000c280: 6374 6f72 3d37 290a 2020 2020 2020 2020  ctor=7).        
+0000c290: 7365 6c66 2e63 6f6e 765f 666c 7578 3d61  self.conv_flux=a
+0000c2a0: 7079 5f63 6f6e 766f 6c76 6528 7365 6c66  py_convolve(self
+0000c2b0: 2e66 6c75 785b 6d61 736b 5d2c 6729 0a20  .flux[mask],g). 
+0000c2c0: 2020 2020 2020 2073 656c 662e 636f 6e76         self.conv
+0000c2d0: 4672 6571 7565 6e63 793d 7365 6c66 2e66  Frequency=self.f
+0000c2e0: 7265 7175 656e 6379 5b6d 6173 6b5d 2a31  requency[mask]*1
+0000c2f0: 2e30 0a20 2020 2020 2020 2073 656c 662e  .0.        self.
+0000c300: 636f 6e76 523d 520a 2020 2020 2020 2020  convR=R.        
+0000c310: 7365 6c66 2e63 6f6e 7657 6176 656c 656e  self.convWavelen
+0000c320: 6774 683d 632f 7365 6c66 2e63 6f6e 7646  gth=c/self.convF
+0000c330: 7265 7175 656e 6379 2a31 652d 330a 0a20  requency*1e-3.. 
+0000c340: 2020 2064 6566 2073 686f 7728 7365 6c66     def show(self
+0000c350: 293a 0a20 2020 2020 2020 2070 7269 6e74  ):.        print
+0000c360: 2873 656c 6629 0a20 2020 2020 2020 2070  (self).        p
+0000c370: 7269 6e74 2827 4772 6964 2020 2020 3d20  rint('Grid    = 
+0000c380: 2729 0a20 2020 2020 2020 2070 7269 6e74  ').        print
+0000c390: 2873 656c 662e 6772 6964 290a 2020 2020  (self.grid).    
+0000c3a0: 2020 2020 7072 696e 7428 2753 6f75 7263      print('Sourc
+0000c3b0: 6520 6675 6e63 7469 6f6e 2020 203d 2027  e function   = '
+0000c3c0: 290a 2020 2020 2020 2020 7072 696e 7428  ).        print(
+0000c3d0: 7365 6c66 2e73 6f75 7263 655f 6675 6e63  self.source_func
+0000c3e0: 7469 6f6e 290a 2020 2020 2020 2020 7072  tion).        pr
+0000c3f0: 696e 7428 2747 6173 206f 6e6c 7920 736f  int('Gas only so
+0000c400: 7572 6365 2066 756e 6374 696f 6e20 2020  urce function   
+0000c410: 3d20 2729 0a20 2020 2020 2020 2070 7269  = ').        pri
+0000c420: 6e74 2873 656c 662e 736f 7572 6365 5f66  nt(self.source_f
+0000c430: 756e 6374 696f 6e5f 6761 7329 0a20 2020  unction_gas).   
+0000c440: 2020 2020 2070 7269 6e74 2827 4475 7374       print('Dust
+0000c450: 206f 7074 6963 616c 2064 6570 7468 2020   optical depth  
+0000c460: 203d 2027 290a 2020 2020 2020 2020 7072   = ').        pr
+0000c470: 696e 7428 7365 6c66 2e74 6175 5f64 7573  int(self.tau_dus
+0000c480: 7429 0a20 2020 2020 2020 2070 7269 6e74  t).        print
+0000c490: 2827 4761 7320 6f70 7469 6361 6c20 6465  ('Gas optical de
+0000c4a0: 7074 6820 2020 3d20 2729 0a20 2020 2020  pth   = ').     
+0000c4b0: 2020 2070 7269 6e74 2873 656c 662e 7461     print(self.ta
+0000c4c0: 755f 6761 7329 0a0a 0a64 6566 2072 6561  u_gas)...def rea
+0000c4d0: 645f 3144 5f73 6c61 6228 6d6f 6465 6c5f  d_1D_slab(model_
+0000c4e0: 7061 7468 3d27 536c 6162 5265 7375 6c74  path='SlabResult
+0000c4f0: 732e 6669 7473 2e67 7a27 2c76 6572 626f  s.fits.gz',verbo
+0000c500: 7365 3d54 7275 6529 3a0a 2020 2020 2222  se=True):.    ""
+0000c510: 220a 2020 2020 4675 6e63 7469 6f6e 2074  ".    Function t
+0000c520: 6f20 7265 6164 2031 4420 7072 6f64 696d  o read 1D prodim
+0000c530: 6f20 736c 6162 206d 6f64 656c 206f 7574  o slab model out
+0000c540: 7075 740a 2020 2020 2222 220a 2020 2020  put.    """.    
+0000c550: 6966 2076 6572 626f 7365 3a20 7072 696e  if verbose: prin
+0000c560: 7428 2252 6561 6469 6e67 2031 4420 736c  t("Reading 1D sl
+0000c570: 6162 206d 6f64 656c 206f 7574 7075 7420  ab model output 
+0000c580: 6672 6f6d 3a20 222c 6d6f 6465 6c5f 7061  from: ",model_pa
+0000c590: 7468 290a 2020 2020 6966 2027 2e66 6974  th).    if '.fit
+0000c5a0: 732e 677a 2720 696e 206d 6f64 656c 5f70  s.gz' in model_p
+0000c5b0: 6174 683a 0a20 2020 2020 2020 2068 6475  ath:.        hdu
+0000c5c0: 6c3d 6669 7473 2e6f 7065 6e28 6d6f 6465  l=fits.open(mode
+0000c5d0: 6c5f 7061 7468 290a 2020 2020 2020 2020  l_path).        
+0000c5e0: 6461 7461 3d73 6c61 6231 4428 290a 2020  data=slab1D().  
+0000c5f0: 2020 2020 2020 6461 7461 2e64 6972 6563        data.direc
+0000c600: 746f 7279 3d6d 6f64 656c 5f70 6174 680a  tory=model_path.
+0000c610: 2020 2020 2020 2020 6461 7461 2e66 6c75          data.flu
+0000c620: 783d 6864 756c 5b30 5d2e 6461 7461 2e54  x=hdul[0].data.T
+0000c630: 5b3a 2c31 5d0a 2020 2020 2020 2020 6461  [:,1].        da
+0000c640: 7461 2e66 7265 7175 656e 6379 3d68 6475  ta.frequency=hdu
+0000c650: 6c5b 305d 2e64 6174 612e 545b 3a2c 305d  l[0].data.T[:,0]
+0000c660: 0a20 2020 2020 2020 2064 6174 612e 4e73  .        data.Ns
+0000c670: 7065 6369 6573 3d68 6475 6c5b 305d 2e68  pecies=hdul[0].h
+0000c680: 6561 6465 725b 274e 5350 4543 4945 5327  eader['NSPECIES'
+0000c690: 5d0a 2020 2020 2020 2020 6461 7461 2e73  ].        data.s
+0000c6a0: 7065 6369 6573 3d68 6475 6c5b 305d 2e68  pecies=hdul[0].h
+0000c6b0: 6561 6465 722e 636f 6d6d 656e 7473 5b27  eader.comments['
+0000c6c0: 4e53 5045 4349 4553 275d 2e73 706c 6974  NSPECIES'].split
+0000c6d0: 2827 2c27 290a 2020 2020 2020 2020 6461  (',').        da
+0000c6e0: 7461 2e4e 6772 6964 3d68 6475 6c5b 305d  ta.Ngrid=hdul[0]
+0000c6f0: 2e68 6561 6465 725b 274e 4752 4944 275d  .header['NGRID']
+0000c700: 0a20 2020 2020 2020 2064 6174 612e 523d  .        data.R=
+0000c710: 6864 756c 5b30 5d2e 6865 6164 6572 5b27  hdul[0].header['
+0000c720: 525f 4f56 4c50 275d 0a20 2020 2020 2020  R_OVLP'].       
+0000c730: 2069 6620 2828 392b 6461 7461 2e4e 7370   if ((9+data.Nsp
+0000c740: 6563 6965 732a 3229 2c64 6174 612e 4e67  ecies*2),data.Ng
+0000c750: 7269 6429 3d3d 6864 756c 5b31 5d2e 6461  rid)==hdul[1].da
+0000c760: 7461 2e54 2e73 6861 7065 3a0a 2020 2020  ta.T.shape:.    
+0000c770: 2020 2020 2020 2020 6772 6964 3d68 6475          grid=hdu
+0000c780: 6c5b 315d 2e64 6174 610a 2020 2020 2020  l[1].data.      
+0000c790: 2020 2020 2020 6461 7461 2e67 7269 645b        data.grid[
+0000c7a0: 2764 7a27 5d3d 6772 6964 5b3a 2c30 5d0a  'dz']=grid[:,0].
 0000c7b0: 2020 2020 2020 2020 2020 2020 6461 7461              data
-0000c7c0: 2e67 7269 645b 276e 4849 275d 3d67 7269  .grid['nHI']=gri
-0000c7d0: 645b 3a2c 355d 0a20 2020 2020 2020 2020  d[:,5].         
-0000c7e0: 2020 2064 6174 612e 6772 6964 5b27 6e48     data.grid['nH
-0000c7f0: 4949 275d 3d67 7269 645b 3a2c 365d 0a20  II']=grid[:,6]. 
+0000c7c0: 2e67 7269 645b 2776 7475 7262 275d 3d67  .grid['vturb']=g
+0000c7d0: 7269 645b 3a2c 315d 0a20 2020 2020 2020  rid[:,1].       
+0000c7e0: 2020 2020 2064 6174 612e 6772 6964 5b27       data.grid['
+0000c7f0: 6e64 275d 3d67 7269 645b 3a2c 325d 0a20  nd']=grid[:,2]. 
 0000c800: 2020 2020 2020 2020 2020 2064 6174 612e             data.
-0000c810: 6772 6964 5b27 6e48 6527 5d3d 6772 6964  grid['nHe']=grid
-0000c820: 5b3a 2c37 5d0a 2020 2020 2020 2020 2020  [:,7].          
-0000c830: 2020 6461 7461 2e67 7269 645b 276e 656c    data.grid['nel
-0000c840: 6563 275d 3d67 7269 645b 3a2c 385d 0a20  ec']=grid[:,8]. 
-0000c850: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-0000c860: 2069 6e20 7261 6e67 6528 6461 7461 2e4e   in range(data.N
-0000c870: 7370 6563 6965 7329 3a0a 2020 2020 2020  species):.      
-0000c880: 2020 2020 2020 2020 2020 6b65 793d 276e            key='n
-0000c890: 272b 6461 7461 2e73 7065 6369 6573 5b69  '+data.species[i
-0000c8a0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-0000c8b0: 2020 6461 7461 2e67 7269 645b 6b65 795d    data.grid[key]
-0000c8c0: 3d67 7269 645b 3a2c 392b 695d 0a20 2020  =grid[:,9+i].   
-0000c8d0: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
-0000c8e0: 6e20 7261 6e67 6528 6461 7461 2e4e 7370  n range(data.Nsp
-0000c8f0: 6563 6965 7329 3a0a 2020 2020 2020 2020  ecies):.        
-0000c900: 2020 2020 2020 2020 6b65 793d 2754 675f          key='Tg_
-0000c910: 272b 6461 7461 2e73 7065 6369 6573 5b69  '+data.species[i
-0000c920: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-0000c930: 2020 6461 7461 2e67 7269 645b 6b65 795d    data.grid[key]
-0000c940: 3d67 7269 645b 3a2c 392b 6461 7461 2e4e  =grid[:,9+data.N
-0000c950: 7370 6563 6965 732b 695d 0a20 2020 2020  species+i].     
-0000c960: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000c970: 2020 2020 2072 6169 7365 2041 7373 6572       raise Asser
-0000c980: 7469 6f6e 4572 726f 7228 2747 7269 6420  tionError('Grid 
-0000c990: 696e 206f 7574 7075 7420 6669 6c65 2064  in output file d
-0000c9a0: 6f65 7320 6e6f 7420 6d61 7463 6820 7468  oes not match th
-0000c9b0: 6520 6163 7475 616c 2067 7269 6420 6f75  e actual grid ou
-0000c9c0: 7470 7574 2061 7272 6179 2729 0a0a 2020  tput array')..  
-0000c9d0: 2020 2020 2020 6966 2028 6c65 6e28 6461        if (len(da
-0000c9e0: 7461 2e66 7265 7175 656e 6379 292c 6461  ta.frequency),da
-0000c9f0: 7461 2e4e 6772 6964 293d 3d68 6475 6c5b  ta.Ngrid)==hdul[
-0000ca00: 325d 2e64 6174 612e 542e 7368 6170 653a  2].data.T.shape:
-0000ca10: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-0000ca20: 612e 736f 7572 6365 5f66 756e 6374 696f  a.source_functio
-0000ca30: 6e3d 6864 756c 5b32 5d2e 6461 7461 0a20  n=hdul[2].data. 
-0000ca40: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0000ca50: 2020 2020 2020 2020 2072 6169 7365 2041           raise A
-0000ca60: 7373 6572 7469 6f6e 4572 726f 7228 2753  ssertionError('S
-0000ca70: 6f75 7263 6520 6675 6e63 7469 6f6e 2067  ource function g
-0000ca80: 7269 6420 696e 206f 7574 7075 7420 6669  rid in output fi
-0000ca90: 6c65 2064 6f65 7320 6e6f 7420 6d61 7463  le does not matc
-0000caa0: 6820 7468 6520 7370 6174 6961 6c20 616e  h the spatial an
-0000cab0: 6420 6672 6571 7565 6e63 7920 6772 6964  d frequency grid
-0000cac0: 2073 697a 6527 290a 0a20 2020 2020 2020   size')..       
-0000cad0: 2069 6620 286c 656e 2864 6174 612e 6672   if (len(data.fr
-0000cae0: 6571 7565 6e63 7929 2c64 6174 612e 4e67  equency),data.Ng
-0000caf0: 7269 6429 3d3d 6864 756c 5b33 5d2e 6461  rid)==hdul[3].da
-0000cb00: 7461 2e54 2e73 6861 7065 3a0a 2020 2020  ta.T.shape:.    
-0000cb10: 2020 2020 2020 2020 6461 7461 2e73 6f75          data.sou
-0000cb20: 7263 655f 6675 6e63 7469 6f6e 5f67 6173  rce_function_gas
-0000cb30: 3d68 6475 6c5b 335d 2e64 6174 610a 2020  =hdul[3].data.  
-0000cb40: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0000cb50: 2020 2020 2020 2020 7261 6973 6520 4173          raise As
-0000cb60: 7365 7274 696f 6e45 7272 6f72 2827 4761  sertionError('Ga
-0000cb70: 7320 736f 7572 6365 2066 756e 6374 696f  s source functio
-0000cb80: 6e20 6772 6964 2069 6e20 6f75 7470 7574  n grid in output
-0000cb90: 2066 696c 6520 646f 6573 206e 6f74 206d   file does not m
-0000cba0: 6174 6368 2074 6865 2073 7061 7469 616c  atch the spatial
-0000cbb0: 2061 6e64 2066 7265 7175 656e 6379 2067   and frequency g
-0000cbc0: 7269 6420 7369 7a65 2729 0a0a 2020 2020  rid size')..    
-0000cbd0: 2020 2020 6966 2028 6c65 6e28 6461 7461      if (len(data
-0000cbe0: 2e66 7265 7175 656e 6379 292c 6461 7461  .frequency),data
-0000cbf0: 2e4e 6772 6964 293d 3d68 6475 6c5b 345d  .Ngrid)==hdul[4]
-0000cc00: 2e64 6174 612e 542e 7368 6170 653a 0a20  .data.T.shape:. 
-0000cc10: 2020 2020 2020 2020 2020 2064 6174 612e             data.
-0000cc20: 7461 755f 6475 7374 3d68 6475 6c5b 345d  tau_dust=hdul[4]
-0000cc30: 2e64 6174 610a 2020 2020 2020 2020 656c  .data.        el
-0000cc40: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000cc50: 7261 6973 6520 4173 7365 7274 696f 6e45  raise AssertionE
-0000cc60: 7272 6f72 2827 4475 7374 206f 7074 6963  rror('Dust optic
-0000cc70: 616c 2064 6570 7468 2067 7269 6420 696e  al depth grid in
-0000cc80: 206f 7574 7075 7420 6669 6c65 2064 6f65   output file doe
-0000cc90: 7320 6e6f 7420 6d61 7463 6820 7468 6520  s not match the 
-0000cca0: 7370 6174 6961 6c20 616e 6420 6672 6571  spatial and freq
-0000ccb0: 7565 6e63 7920 6772 6964 2073 697a 6527  uency grid size'
-0000ccc0: 290a 0a20 2020 2020 2020 2069 6620 286c  )..        if (l
-0000ccd0: 656e 2864 6174 612e 6672 6571 7565 6e63  en(data.frequenc
-0000cce0: 7929 2c64 6174 612e 4e67 7269 6429 3d3d  y),data.Ngrid)==
-0000ccf0: 6864 756c 5b35 5d2e 6461 7461 2e54 2e73  hdul[5].data.T.s
-0000cd00: 6861 7065 3a0a 2020 2020 2020 2020 2020  hape:.          
-0000cd10: 2020 6461 7461 2e74 6175 5f67 6173 3d68    data.tau_gas=h
-0000cd20: 6475 6c5b 355d 2e64 6174 610a 2020 2020  dul[5].data.    
-0000cd30: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000cd40: 2020 2020 2020 7261 6973 6520 4173 7365        raise Asse
-0000cd50: 7274 696f 6e45 7272 6f72 2827 4761 7320  rtionError('Gas 
-0000cd60: 6f70 7469 6361 6c20 6465 7074 6820 6772  optical depth gr
-0000cd70: 6964 2069 6e20 6f75 7470 7574 2066 696c  id in output fil
-0000cd80: 6520 646f 6573 206e 6f74 206d 6174 6368  e does not match
-0000cd90: 2074 6865 2073 7061 7469 616c 2061 6e64   the spatial and
-0000cda0: 2066 7265 7175 656e 6379 2067 7269 6420   frequency grid 
-0000cdb0: 7369 7a65 2729 0a20 2020 2065 6c73 653a  size').    else:
-0000cdc0: 0a20 2020 2020 2020 2064 6174 615f 7265  .        data_re
-0000cdd0: 6164 3d6e 702e 6c6f 6164 7478 7428 6d6f  ad=np.loadtxt(mo
-0000cde0: 6465 6c5f 7061 7468 2c73 6b69 7072 6f77  del_path,skiprow
-0000cdf0: 733d 3129 0a20 2020 2020 2020 2064 6174  s=1).        dat
-0000ce00: 613d 736c 6162 3144 2829 0a20 2020 2020  a=slab1D().     
-0000ce10: 2020 2064 6174 612e 6469 7265 6374 6f72     data.director
-0000ce20: 793d 6d6f 6465 6c5f 7061 7468 0a20 2020  y=model_path.   
-0000ce30: 2020 2020 2064 6174 612e 666c 7578 3d64       data.flux=d
-0000ce40: 6174 615f 7265 6164 5b3a 2c31 5d0a 2020  ata_read[:,1].  
-0000ce50: 2020 2020 2020 6461 7461 2e66 7265 7175        data.frequ
-0000ce60: 656e 6379 3d64 6174 615f 7265 6164 5b3a  ency=data_read[:
-0000ce70: 2c30 5d0a 2020 2020 7265 7475 726e 2864  ,0].    return(d
-0000ce80: 6174 6129 0a0a 0a64 6566 2072 6561 645f  ata)...def read_
-0000ce90: 736c 6162 286d 6f64 656c 5f70 6174 683d  slab(model_path=
-0000cea0: 2753 6c61 6252 6573 756c 7473 2e6f 7574  'SlabResults.out
-0000ceb0: 272c 7665 7262 6f73 653d 5472 7565 2c73  ',verbose=True,s
-0000cec0: 686f 7274 5f66 6f72 6d61 743d 4661 6c73  hort_format=Fals
-0000ced0: 6529 3a0a 2020 2020 2222 220a 2020 2020  e):.    """.    
-0000cee0: 4675 6e63 7469 6f6e 2074 6f20 7265 6164  Function to read
-0000cef0: 2073 6c61 6220 6d6f 6465 6c20 6f75 7470   slab model outp
-0000cf00: 7574 0a20 2020 2022 2222 0a20 2020 2069  ut.    """.    i
-0000cf10: 6620 6973 696e 7374 616e 6365 286d 6f64  f isinstance(mod
-0000cf20: 656c 5f70 6174 682c 6c69 7374 293a 0a20  el_path,list):. 
-0000cf30: 2020 2020 2020 2064 6174 613d 736c 6162         data=slab
-0000cf40: 5f64 6174 6128 290a 2020 2020 2020 2020  _data().        
-0000cf50: 6461 7461 2e64 6972 6563 746f 7279 3d6d  data.directory=m
-0000cf60: 6f64 656c 5f70 6174 680a 2020 2020 2020  odel_path.      
-0000cf70: 2020 666f 7220 6920 696e 206d 6f64 656c    for i in model
-0000cf80: 5f70 6174 683a 0a20 2020 2020 2020 2020  _path:.         
-0000cf90: 2020 2072 6461 7461 3d72 6561 645f 736c     rdata=read_sl
-0000cfa0: 6162 2869 2c76 6572 626f 7365 3d76 6572  ab(i,verbose=ver
-0000cfb0: 626f 7365 2c73 686f 7274 5f66 6f72 6d61  bose,short_forma
-0000cfc0: 743d 7368 6f72 745f 666f 726d 6174 290a  t=short_format).
-0000cfd0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000cfe0: 6a20 696e 2072 616e 6765 2872 6461 7461  j in range(rdata
-0000cff0: 2e6e 6d6f 6465 6c73 293a 0a20 2020 2020  .nmodels):.     
-0000d000: 2020 2020 2020 2020 2020 2064 6174 612e             data.
-0000d010: 6164 645f 6d6f 6465 6c28 7264 6174 612e  add_model(rdata.
-0000d020: 6d6f 6465 6c73 5b6a 5d29 0a20 2020 2020  models[j]).     
-0000d030: 2020 2072 6574 7572 6e28 6461 7461 290a     return(data).
-0000d040: 0a20 2020 2069 6620 7665 7262 6f73 653a  .    if verbose:
-0000d050: 2070 7269 6e74 2822 5265 6164 696e 6720   print("Reading 
-0000d060: 736c 6162 206d 6f64 656c 206f 7574 7075  slab model outpu
-0000d070: 7420 6672 6f6d 3a20 222c 6d6f 6465 6c5f  t from: ",model_
-0000d080: 7061 7468 290a 2020 2020 663d 6f70 656e  path).    f=open
-0000d090: 286d 6f64 656c 5f70 6174 6829 0a20 2020  (model_path).   
-0000d0a0: 2064 6174 613d 736c 6162 5f64 6174 6128   data=slab_data(
-0000d0b0: 290a 2020 2020 6e6d 6f64 656c 733d 696e  ).    nmodels=in
-0000d0c0: 7428 662e 7265 6164 6c69 6e65 2829 2e73  t(f.readline().s
-0000d0d0: 706c 6974 2829 5b30 5d29 0a20 2020 2064  plit()[0]).    d
-0000d0e0: 6174 612e 6469 7265 6374 6f72 793d 6d6f  ata.directory=mo
-0000d0f0: 6465 6c5f 7061 7468 0a20 2020 2066 6f72  del_path.    for
-0000d100: 2069 2069 6e20 7261 6e67 6528 6e6d 6f64   i in range(nmod
-0000d110: 656c 7329 3a0a 2320 2020 2020 2020 2020  els):.#         
-0000d120: 7465 6d70 6f20 2020 2020 2020 2020 2020  tempo           
-0000d130: 2020 2020 203d 2020 2073 6c61 6228 290a       =   slab().
-0000d140: 2020 2020 2020 2020 7465 6d70 6f5f 6d6f          tempo_mo
-0000d150: 6465 6c5f 6e75 6d62 6572 3d69 6e74 2866  del_number=int(f
-0000d160: 2e72 6561 646c 696e 6528 292e 7370 6c69  .readline().spli
-0000d170: 7428 295b 305d 290a 2020 2020 2020 2020  t()[0]).        
-0000d180: 6e73 7065 6369 6573 3d69 6e74 2866 2e72  nspecies=int(f.r
-0000d190: 6561 646c 696e 6528 292e 7370 6c69 7428  eadline().split(
-0000d1a0: 295b 305d 290a 2320 2020 2020 2020 2020  )[0]).#         
-0000d1b0: 7465 6d70 6f2e 7370 6563 6965 735f 6e75  tempo.species_nu
-0000d1c0: 6d62 6572 203d 2020 2069 6e74 2866 2e72  mber =   int(f.r
-0000d1d0: 6561 646c 696e 6528 292e 7370 6c69 7428  eadline().split(
-0000d1e0: 295b 305d 290a 2020 2020 2020 2020 7465  )[0]).        te
-0000d1f0: 6d70 6f5f 6e48 746f 743d 666c 6f61 7428  mpo_nHtot=float(
-0000d200: 662e 7265 6164 6c69 6e65 2829 2e73 706c  f.readline().spl
-0000d210: 6974 2829 5b30 5d29 0a20 2020 2020 2020  it()[0]).       
-0000d220: 2074 656d 706f 5f67 6173 4465 6e73 3d66   tempo_gasDens=f
-0000d230: 6c6f 6174 2866 2e72 6561 646c 696e 6528  loat(f.readline(
-0000d240: 292e 7370 6c69 7428 295b 305d 290a 2020  ).split()[0]).  
-0000d250: 2020 2020 2020 7465 6d70 6f5f 6e65 6c65        tempo_nele
-0000d260: 633d 666c 6f61 7428 662e 7265 6164 6c69  c=float(f.readli
-0000d270: 6e65 2829 2e73 706c 6974 2829 5b30 5d29  ne().split()[0])
-0000d280: 0a20 2020 2020 2020 2074 656d 706f 5f6e  .        tempo_n
-0000d290: 4865 3d66 6c6f 6174 2866 2e72 6561 646c  He=float(f.readl
-0000d2a0: 696e 6528 292e 7370 6c69 7428 295b 305d  ine().split()[0]
-0000d2b0: 290a 2020 2020 2020 2020 7465 6d70 6f5f  ).        tempo_
-0000d2c0: 6e48 4949 3d66 6c6f 6174 2866 2e72 6561  nHII=float(f.rea
-0000d2d0: 646c 696e 6528 292e 7370 6c69 7428 295b  dline().split()[
-0000d2e0: 305d 290a 2020 2020 2020 2020 7465 6d70  0]).        temp
-0000d2f0: 6f5f 6e48 493d 666c 6f61 7428 662e 7265  o_nHI=float(f.re
-0000d300: 6164 6c69 6e65 2829 2e73 706c 6974 2829  adline().split()
-0000d310: 5b30 5d29 0a20 2020 2020 2020 2074 656d  [0]).        tem
-0000d320: 706f 5f6e 4832 3d66 6c6f 6174 2866 2e72  po_nH2=float(f.r
-0000d330: 6561 646c 696e 6528 292e 7370 6c69 7428  eadline().split(
-0000d340: 295b 305d 290a 2020 2020 2020 2020 7465  )[0]).        te
-0000d350: 6d70 6f5f 6475 7374 5f74 6f5f 6761 733d  mpo_dust_to_gas=
-0000d360: 666c 6f61 7428 662e 7265 6164 6c69 6e65  float(f.readline
-0000d370: 2829 2e73 706c 6974 2829 5b30 5d29 0a20  ().split()[0]). 
-0000d380: 2020 2020 2020 2074 656d 706f 5f76 7475         tempo_vtu
-0000d390: 7262 3d66 6c6f 6174 2866 2e72 6561 646c  rb=float(f.readl
-0000d3a0: 696e 6528 292e 7370 6c69 7428 295b 305d  ine().split()[0]
-0000d3b0: 290a 2020 2020 2020 2020 7465 6d70 6f5f  ).        tempo_
-0000d3c0: 5467 3d66 6c6f 6174 2866 2e72 6561 646c  Tg=float(f.readl
-0000d3d0: 696e 6528 292e 7370 6c69 7428 295b 305d  ine().split()[0]
-0000d3e0: 290a 2020 2020 2020 2020 7465 6d70 6f5f  ).        tempo_
-0000d3f0: 5464 3d66 6c6f 6174 2866 2e72 6561 646c  Td=float(f.readl
-0000d400: 696e 6528 292e 7370 6c69 7428 295b 305d  ine().split()[0]
-0000d410: 290a 2020 2020 2020 2020 6966 2073 686f  ).        if sho
-0000d420: 7274 5f66 6f72 6d61 743a 0a20 2020 2020  rt_format:.     
-0000d430: 2020 2020 2020 2066 6f72 206a 2069 6e20         for j in 
-0000d440: 7261 6e67 6528 6e73 7065 6369 6573 293a  range(nspecies):
-0000d450: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d460: 2074 656d 706f 3d73 6c61 6228 290a 2020   tempo=slab().  
-0000d470: 2020 2020 2020 2020 2020 2020 2020 7465                te
-0000d480: 6d70 6f2e 6d6f 6465 6c5f 6e75 6d62 6572  mpo.model_number
-0000d490: 3d74 656d 706f 5f6d 6f64 656c 5f6e 756d  =tempo_model_num
-0000d4a0: 6265 720a 2020 2020 2020 2020 2020 2020  ber.            
-0000d4b0: 2020 2020 7465 6d70 6f2e 4e48 3d74 656d      tempo.NH=tem
-0000d4c0: 706f 5f6e 4874 6f74 0a20 2020 2020 2020  po_nHtot.       
-0000d4d0: 2020 2020 2020 2020 2074 656d 706f 2e6e           tempo.n
-0000d4e0: 436f 6c6c 3d74 656d 706f 5f67 6173 4465  Coll=tempo_gasDe
-0000d4f0: 6e73 0a20 2020 2020 2020 2020 2020 2020  ns.             
-0000d500: 2020 2074 656d 706f 2e6e 653d 7465 6d70     tempo.ne=temp
-0000d510: 6f5f 6e65 6c65 630a 2020 2020 2020 2020  o_nelec.        
-0000d520: 2020 2020 2020 2020 7465 6d70 6f2e 6e48          tempo.nH
-0000d530: 653d 7465 6d70 6f5f 6e48 650a 2020 2020  e=tempo_nHe.    
-0000d540: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-0000d550: 6f2e 6e48 4949 3d74 656d 706f 5f6e 4849  o.nHII=tempo_nHI
-0000d560: 490a 2020 2020 2020 2020 2020 2020 2020  I.              
-0000d570: 2020 7465 6d70 6f2e 6e48 493d 7465 6d70    tempo.nHI=temp
-0000d580: 6f5f 6e48 490a 2020 2020 2020 2020 2020  o_nHI.          
-0000d590: 2020 2020 2020 7465 6d70 6f2e 6e48 323d        tempo.nH2=
-0000d5a0: 7465 6d70 6f5f 6e48 320a 2020 2020 2020  tempo_nH2.      
-0000d5b0: 2020 2020 2020 2020 2020 7465 6d70 6f2e            tempo.
-0000d5c0: 6475 7374 5f74 6f5f 6761 733d 7465 6d70  dust_to_gas=temp
-0000d5d0: 6f5f 6475 7374 5f74 6f5f 6761 730a 2020  o_dust_to_gas.  
-0000d5e0: 2020 2020 2020 2020 2020 2020 2020 7465                te
-0000d5f0: 6d70 6f2e 7674 7572 623d 7465 6d70 6f5f  mpo.vturb=tempo_
-0000d600: 7674 7572 620a 2020 2020 2020 2020 2020  vturb.          
-0000d610: 2020 2020 2020 7465 6d70 6f2e 5467 3d74        tempo.Tg=t
-0000d620: 656d 706f 5f54 670a 2020 2020 2020 2020  empo_Tg.        
-0000d630: 2020 2020 2020 2020 7465 6d70 6f2e 5464          tempo.Td
-0000d640: 3d74 656d 706f 5f54 640a 0a20 2020 2020  =tempo_Td..     
-0000d650: 2020 2020 2020 2020 2020 2074 656d 706f             tempo
-0000d660: 2e73 7065 6369 6573 5f69 6e64 6578 3d69  .species_index=i
-0000d670: 6e74 2866 2e72 6561 646c 696e 6528 292e  nt(f.readline().
-0000d680: 7370 6c69 7428 295b 305d 290a 2020 2020  split()[0]).    
-0000d690: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-0000d6a0: 6f2e 7370 6563 6965 735f 6e75 6d62 6572  o.species_number
-0000d6b0: 3d6a 2b31 0a20 2020 2020 2020 2020 2020  =j+1.           
-0000d6c0: 2020 2020 2074 656d 706f 2e73 7065 6369       tempo.speci
-0000d6d0: 6573 5f6e 616d 653d 662e 7265 6164 6c69  es_name=f.readli
-0000d6e0: 6e65 2829 2e73 706c 6974 2829 5b30 5d0a  ne().split()[0].
-0000d6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d700: 7465 6d70 6f2e 6162 756e 6461 6e63 653d  tempo.abundance=
-0000d710: 666c 6f61 7428 662e 7265 6164 6c69 6e65  float(f.readline
-0000d720: 2829 2e73 706c 6974 2829 5b30 5d29 0a20  ().split()[0]). 
-0000d730: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000d740: 656d 706f 2e64 763d 666c 6f61 7428 662e  empo.dv=float(f.
-0000d750: 7265 6164 6c69 6e65 2829 2e73 706c 6974  readline().split
-0000d760: 2829 5b30 5d29 0a20 2020 2020 2020 2020  ()[0]).         
-0000d770: 2020 2020 2020 2074 656d 706f 2e6e 6c69         tempo.nli
-0000d780: 6e65 733d 696e 7428 662e 7265 6164 6c69  nes=int(f.readli
-0000d790: 6e65 2829 2e73 706c 6974 2829 5b30 5d29  ne().split()[0])
-0000d7a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d7b0: 206c 696e 6573 3d66 2e72 6561 646c 696e   lines=f.readlin
-0000d7c0: 6528 290a 0a20 2020 2020 2020 2020 2020  e()..           
-0000d7d0: 2020 2020 2023 2074 656d 706f 2e6e 6c69       # tempo.nli
-0000d7e0: 6e65 733d 4e6f 6e65 0a20 2020 2020 2020  nes=None.       
-0000d7f0: 2020 2020 2020 2020 2074 656d 706f 2e6c           tempo.l
-0000d800: 696e 6564 6174 613d 4e6f 6e65 0a20 2020  inedata=None.   
-0000d810: 2020 2020 2020 2020 2020 2020 2074 656d               tem
-0000d820: 706f 2e6c 6576 656c 6461 7461 3d4e 6f6e  po.leveldata=Non
-0000d830: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-0000d840: 2020 7465 6d70 6f2e 636f 6e76 5761 7665    tempo.convWave
-0000d850: 6c65 6e67 7468 3d4e 6f6e 650a 2020 2020  length=None.    
-0000d860: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-0000d870: 6f2e 636f 6e76 4c54 4566 6c75 783d 4e6f  o.convLTEflux=No
-0000d880: 6e65 0a20 2020 2020 2020 2020 2020 2020  ne.             
-0000d890: 2020 2074 656d 706f 2e63 6f6e 764e 4c54     tempo.convNLT
-0000d8a0: 4566 6c75 783d 4e6f 6e65 0a20 2020 2020  Eflux=None.     
-0000d8b0: 2020 2020 2020 2020 2020 2074 656d 706f             tempo
-0000d8c0: 2e63 6f6e 7654 7970 653d 4e6f 6e65 0a20  .convType=None. 
-0000d8d0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000d8e0: 656d 706f 2e63 6f6e 7652 3d4e 6f6e 650a  empo.convR=None.
-0000d8f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d900: 2064 6174 3d5b 5d0a 2020 2020 2020 2020   dat=[].        
-0000d910: 2020 2020 2020 2020 2320 666f 7220 6b20          # for k 
-0000d920: 696e 2072 616e 6765 2874 656d 706f 2e6e  in range(tempo.n
-0000d930: 6c65 7665 6c73 293a 0a20 2020 2020 2020  levels):.       
-0000d940: 2020 2020 2020 2020 2023 2020 2020 2064           #     d
-0000d950: 6174 5b30 5d5b 6b2c 3a5d 3d6e 702e 6173  at[0][k,:]=np.as
-0000d960: 6172 7261 7928 5b66 6c6f 6174 2878 2920  array([float(x) 
-0000d970: 666f 7220 7820 696e 2066 2e72 6561 646c  for x in f.readl
-0000d980: 696e 6528 292e 7370 6c69 7428 295d 290a  ine().split()]).
-0000d990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d9a0: 2023 206c 696e 6573 3d66 2e72 6561 646c   # lines=f.readl
-0000d9b0: 696e 6528 290a 2020 2020 2020 2020 2020  ine().          
-0000d9c0: 2020 2020 2020 2320 6c69 6e65 733d 662e        # lines=f.
-0000d9d0: 7265 6164 6c69 6e65 2829 0a20 2020 2020  readline().     
-0000d9e0: 2020 2020 2020 2020 2020 2064 6174 3d6e             dat=n
-0000d9f0: 702e 7a65 726f 7328 2874 656d 706f 2e6e  p.zeros((tempo.n
-0000da00: 6c69 6e65 732c 3429 290a 2020 2020 2020  lines,4)).      
-0000da10: 2020 2020 2020 2020 2020 736c 6162 4f75            slabOu
-0000da20: 7446 6f72 6d61 743d 5b38 2c31 342c 3135  tFormat=[8,14,15
-0000da30: 2c31 355d 0a20 2020 2020 2020 2020 2020  ,15].           
-0000da40: 2020 2020 2066 6f72 206b 2069 6e20 7261       for k in ra
-0000da50: 6e67 6528 7465 6d70 6f2e 6e6c 696e 6573  nge(tempo.nlines
-0000da60: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000da70: 2020 2020 2020 206c 696e 6552 6561 643d         lineRead=
-0000da80: 5b5d 0a20 2020 2020 2020 2020 2020 2020  [].             
-0000da90: 2020 2020 2020 206c 696e 6573 3d66 2e72         lines=f.r
-0000daa0: 6561 646c 696e 6528 290a 2020 2020 2020  eadline().      
-0000dab0: 2020 2020 2020 2020 2020 2020 2020 6c3d                l=
-0000dac0: 300a 2020 2020 2020 2020 2020 2020 2020  0.              
-0000dad0: 2020 2020 2020 666f 7220 6c65 6e67 7468        for length
-0000dae0: 2069 6e20 736c 6162 4f75 7446 6f72 6d61   in slabOutForma
-0000daf0: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
-0000db00: 2020 2020 2020 2020 2020 206c 696e 6552             lineR
-0000db10: 6561 642e 6170 7065 6e64 286c 696e 6573  ead.append(lines
-0000db20: 5b6c 3a6c 2b6c 656e 6774 685d 290a 2020  [l:l+length]).  
-0000db30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db40: 2020 2020 2020 6c2b 3d6c 656e 6774 680a        l+=length.
-0000db50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db60: 2020 2020 6461 745b 6b2c 3a5d 3d6e 702e      dat[k,:]=np.
-0000db70: 6173 6172 7261 7928 5b66 6c6f 6174 2878  asarray([float(x
-0000db80: 2920 666f 7220 7820 696e 206c 696e 6552  ) for x in lineR
-0000db90: 6561 645d 290a 2020 2020 2020 2020 2020  ead]).          
-0000dba0: 2020 2020 2020 6c69 6e65 4461 7461 3d70        lineData=p
-0000dbb0: 642e 4461 7461 4672 616d 6528 6461 742c  d.DataFrame(dat,
-0000dbc0: 636f 6c75 6d6e 733d 5b27 6927 2c27 4748  columns=['i','GH
-0000dbd0: 7a27 2c27 464e 4c54 4527 2c27 464c 5445  z','FNLTE','FLTE
-0000dbe0: 275d 290a 2020 2020 2020 2020 2020 2020  ']).            
-0000dbf0: 2020 2020 7465 6d70 6f2e 6c69 6e65 6461      tempo.lineda
-0000dc00: 7461 3d6c 696e 6544 6174 610a 2020 2020  ta=lineData.    
-0000dc10: 2020 2020 2020 2020 2020 2020 6461 7461              data
-0000dc20: 2e61 6464 5f6d 6f64 656c 2874 656d 706f  .add_model(tempo
-0000dc30: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-0000dc40: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000dc50: 6a20 696e 2072 616e 6765 286e 7370 6563  j in range(nspec
-0000dc60: 6965 7329 3a0a 2020 2020 2020 2020 2020  ies):.          
-0000dc70: 2020 2020 2020 7465 6d70 6f3d 736c 6162        tempo=slab
-0000dc80: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-0000dc90: 2020 2074 656d 706f 2e6d 6f64 656c 5f6e     tempo.model_n
-0000dca0: 756d 6265 723d 7465 6d70 6f5f 6d6f 6465  umber=tempo_mode
-0000dcb0: 6c5f 6e75 6d62 6572 0a20 2020 2020 2020  l_number.       
-0000dcc0: 2020 2020 2020 2020 2074 656d 706f 2e4e           tempo.N
-0000dcd0: 483d 7465 6d70 6f5f 6e48 746f 740a 2020  H=tempo_nHtot.  
-0000dce0: 2020 2020 2020 2020 2020 2020 2020 7465                te
-0000dcf0: 6d70 6f2e 6e43 6f6c 6c3d 7465 6d70 6f5f  mpo.nColl=tempo_
-0000dd00: 6761 7344 656e 730a 2020 2020 2020 2020  gasDens.        
-0000dd10: 2020 2020 2020 2020 7465 6d70 6f2e 6e65          tempo.ne
-0000dd20: 3d74 656d 706f 5f6e 656c 6563 0a20 2020  =tempo_nelec.   
-0000dd30: 2020 2020 2020 2020 2020 2020 2074 656d               tem
-0000dd40: 706f 2e6e 4865 3d74 656d 706f 5f6e 4865  po.nHe=tempo_nHe
-0000dd50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000dd60: 2074 656d 706f 2e6e 4849 493d 7465 6d70   tempo.nHII=temp
-0000dd70: 6f5f 6e48 4949 0a20 2020 2020 2020 2020  o_nHII.         
-0000dd80: 2020 2020 2020 2074 656d 706f 2e6e 4849         tempo.nHI
-0000dd90: 3d74 656d 706f 5f6e 4849 0a20 2020 2020  =tempo_nHI.     
-0000dda0: 2020 2020 2020 2020 2020 2074 656d 706f             tempo
-0000ddb0: 2e6e 4832 3d74 656d 706f 5f6e 4832 0a20  .nH2=tempo_nH2. 
-0000ddc0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000ddd0: 656d 706f 2e64 7573 745f 746f 5f67 6173  empo.dust_to_gas
-0000dde0: 3d74 656d 706f 5f64 7573 745f 746f 5f67  =tempo_dust_to_g
-0000ddf0: 6173 0a20 2020 2020 2020 2020 2020 2020  as.             
-0000de00: 2020 2074 656d 706f 2e76 7475 7262 3d74     tempo.vturb=t
-0000de10: 656d 706f 5f76 7475 7262 0a20 2020 2020  empo_vturb.     
-0000de20: 2020 2020 2020 2020 2020 2074 656d 706f             tempo
-0000de30: 2e54 673d 7465 6d70 6f5f 5467 0a20 2020  .Tg=tempo_Tg.   
-0000de40: 2020 2020 2020 2020 2020 2020 2074 656d               tem
-0000de50: 706f 2e54 643d 7465 6d70 6f5f 5464 0a0a  po.Td=tempo_Td..
-0000de60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de70: 7465 6d70 6f2e 7370 6563 6965 735f 696e  tempo.species_in
-0000de80: 6465 783d 696e 7428 662e 7265 6164 6c69  dex=int(f.readli
-0000de90: 6e65 2829 2e73 706c 6974 2829 5b30 5d29  ne().split()[0])
-0000dea0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000deb0: 2074 656d 706f 2e73 7065 6369 6573 5f6e   tempo.species_n
-0000dec0: 756d 6265 723d 6a2b 310a 2020 2020 2020  umber=j+1.      
-0000ded0: 2020 2020 2020 2020 2020 7465 6d70 6f2e            tempo.
-0000dee0: 7370 6563 6965 735f 6e61 6d65 3d66 2e72  species_name=f.r
-0000def0: 6561 646c 696e 6528 292e 7370 6c69 7428  eadline().split(
-0000df00: 295b 305d 0a20 2020 2020 2020 2020 2020  )[0].           
-0000df10: 2020 2020 2074 656d 706f 2e61 6275 6e64       tempo.abund
-0000df20: 616e 6365 3d66 6c6f 6174 2866 2e72 6561  ance=float(f.rea
-0000df30: 646c 696e 6528 292e 7370 6c69 7428 295b  dline().split()[
-0000df40: 305d 290a 2020 2020 2020 2020 2020 2020  0]).            
-0000df50: 2020 2020 7465 6d70 6f2e 6476 3d66 6c6f      tempo.dv=flo
-0000df60: 6174 2866 2e72 6561 646c 696e 6528 292e  at(f.readline().
-0000df70: 7370 6c69 7428 295b 305d 290a 2020 2020  split()[0]).    
-0000df80: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-0000df90: 6f2e 6e6c 6576 656c 733d 696e 7428 662e  o.nlevels=int(f.
-0000dfa0: 7265 6164 6c69 6e65 2829 2e73 706c 6974  readline().split
-0000dfb0: 2829 5b30 5d29 0a20 2020 2020 2020 2020  ()[0]).         
-0000dfc0: 2020 2020 2020 206c 696e 6573 3d66 2e72         lines=f.r
-0000dfd0: 6561 646c 696e 6528 290a 0a20 2020 2020  eadline()..     
-0000dfe0: 2020 2020 2020 2020 2020 2074 656d 706f             tempo
-0000dff0: 2e6e 6c69 6e65 733d 4e6f 6e65 0a20 2020  .nlines=None.   
-0000e000: 2020 2020 2020 2020 2020 2020 2074 656d               tem
-0000e010: 706f 2e6c 696e 6564 6174 613d 4e6f 6e65  po.linedata=None
-0000e020: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e030: 2074 656d 706f 2e6c 6576 656c 6461 7461   tempo.leveldata
-0000e040: 3d4e 6f6e 650a 2020 2020 2020 2020 2020  =None.          
-0000e050: 2020 2020 2020 7465 6d70 6f2e 636f 6e76        tempo.conv
-0000e060: 5761 7665 6c65 6e67 7468 3d4e 6f6e 650a  Wavelength=None.
-0000e070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e080: 7465 6d70 6f2e 636f 6e76 4c54 4566 6c75  tempo.convLTEflu
-0000e090: 783d 4e6f 6e65 0a20 2020 2020 2020 2020  x=None.         
-0000e0a0: 2020 2020 2020 2074 656d 706f 2e63 6f6e         tempo.con
-0000e0b0: 764e 4c54 4566 6c75 783d 4e6f 6e65 0a20  vNLTEflux=None. 
-0000e0c0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000e0d0: 656d 706f 2e63 6f6e 7654 7970 653d 4e6f  empo.convType=No
-0000e0e0: 6e65 0a20 2020 2020 2020 2020 2020 2020  ne.             
-0000e0f0: 2020 2074 656d 706f 2e63 6f6e 7652 3d4e     tempo.convR=N
-0000e100: 6f6e 650a 0a20 2020 2020 2020 2020 2020  one..           
-0000e110: 2020 2020 2064 6174 3d5b 6e70 2e7a 6572       dat=[np.zer
-0000e120: 6f73 2828 7465 6d70 6f2e 6e6c 6576 656c  os((tempo.nlevel
-0000e130: 732c 3829 292c 5b5d 2c5b 5d5d 0a20 2020  s,8)),[],[]].   
-0000e140: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0000e150: 206b 2069 6e20 7261 6e67 6528 7465 6d70   k in range(temp
-0000e160: 6f2e 6e6c 6576 656c 7329 3a0a 2020 2020  o.nlevels):.    
-0000e170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e180: 6461 745b 305d 5b6b 2c3a 5d3d 6e70 2e61  dat[0][k,:]=np.a
-0000e190: 7361 7272 6179 285b 666c 6f61 7428 7829  sarray([float(x)
-0000e1a0: 2066 6f72 2078 2069 6e20 662e 7265 6164   for x in f.read
-0000e1b0: 6c69 6e65 2829 2e73 706c 6974 2829 5d29  line().split()])
-0000e1c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e1d0: 2074 656d 706f 2e6e 6c69 6e65 733d 696e   tempo.nlines=in
-0000e1e0: 7428 662e 7265 6164 6c69 6e65 2829 2e73  t(f.readline().s
-0000e1f0: 706c 6974 2829 5b30 5d29 0a20 2020 2020  plit()[0]).     
-0000e200: 2020 2020 2020 2020 2020 206c 696e 6573             lines
-0000e210: 3d66 2e72 6561 646c 696e 6528 290a 2020  =f.readline().  
-0000e220: 2020 2020 2020 2020 2020 2020 2020 6c69                li
-0000e230: 6e65 733d 662e 7265 6164 6c69 6e65 2829  nes=f.readline()
-0000e240: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e250: 2064 6174 5b31 5d3d 6e70 2e7a 6572 6f73   dat[1]=np.zeros
-0000e260: 2828 7465 6d70 6f2e 6e6c 696e 6573 2c32  ((tempo.nlines,2
-0000e270: 3329 290a 2020 2020 2020 2020 2020 2020  3)).            
-0000e280: 2020 2020 736c 6162 4f75 7446 6f72 6d61      slabOutForma
-0000e290: 743d 5b39 2c39 2c39 2c35 2c35 2c35 2c31  t=[9,9,9,5,5,5,1
-0000e2a0: 352c 3135 2c31 352c 3135 2c31 352c 3135  5,15,15,15,15,15
-0000e2b0: 2c31 352c 3135 2c31 352c 3135 2c31 352c  ,15,15,15,15,15,
-0000e2c0: 3135 2c31 352c 3135 2c31 352c 3135 2c31  15,15,15,15,15,1
-0000e2d0: 352c 3231 2c32 312c 3231 2c32 315d 0a20  5,21,21,21,21]. 
-0000e2e0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000e2f0: 6f72 206b 2069 6e20 7261 6e67 6528 7465  or k in range(te
-0000e300: 6d70 6f2e 6e6c 696e 6573 293a 0a20 2020  mpo.nlines):.   
-0000e310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e320: 206c 696e 6552 6561 643d 5b5d 0a20 2020   lineRead=[].   
-0000e330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e340: 206c 696e 6573 3d66 2e72 6561 646c 696e   lines=f.readlin
-0000e350: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
-0000e360: 2020 2020 2020 2020 6c3d 300a 2020 2020          l=0.    
-0000e370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e380: 666f 7220 6c65 6e67 7468 2069 6e20 736c  for length in sl
-0000e390: 6162 4f75 7446 6f72 6d61 743a 0a20 2020  abOutFormat:.   
-0000e3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e3b0: 2020 2020 206c 696e 6552 6561 642e 6170       lineRead.ap
-0000e3c0: 7065 6e64 286c 696e 6573 5b6c 3a6c 2b6c  pend(lines[l:l+l
-0000e3d0: 656e 6774 685d 290a 2020 2020 2020 2020  ength]).        
-0000e3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e3f0: 6c2b 3d6c 656e 6774 680a 2020 2020 2020  l+=length.      
-0000e400: 2020 2020 2020 2020 2020 2020 2020 6461                da
-0000e410: 745b 315d 5b6b 2c3a 5d3d 6e70 2e61 7361  t[1][k,:]=np.asa
-0000e420: 7272 6179 285b 666c 6f61 7428 7829 2066  rray([float(x) f
-0000e430: 6f72 2078 2069 6e20 6c69 6e65 5265 6164  or x in lineRead
-0000e440: 5b30 3a2d 345d 5d29 0a20 2020 2020 2020  [0:-4]]).       
-0000e450: 2020 2020 2020 2020 2020 2020 2064 6174               dat
-0000e460: 5b32 5d2e 6170 7065 6e64 285b 612e 7374  [2].append([a.st
-0000e470: 7269 7028 2920 666f 7220 6120 696e 206c  rip() for a in l
-0000e480: 696e 6552 6561 645b 2d34 3a5d 5d29 0a0a  ineRead[-4:]])..
-0000e490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e4a0: 6c69 6e65 4461 7461 3d70 642e 4461 7461  lineData=pd.Data
-0000e4b0: 4672 616d 6528 6461 745b 315d 2c63 6f6c  Frame(dat[1],col
-0000e4c0: 756d 6e73 3d5b 2769 272c 2775 272c 276c  umns=['i','u','l
-0000e4d0: 272c 2765 272c 2776 272c 274a 272c 2767  ','e','v','J','g
-0000e4e0: 7527 2c27 4575 272c 2741 272c 2742 272c  u','Eu','A','B',
-0000e4f0: 2747 487a 272c 2774 6175 4427 2c27 4a62  'GHz','tauD','Jb
-0000e500: 6163 6b27 2c27 706f 7027 2c27 6c74 6570  ack','pop','ltep
-0000e510: 6f70 272c 2774 6175 4e4c 5445 272c 2774  op','tauNLTE','t
-0000e520: 6175 4c54 4527 2c27 624e 4c54 4527 2c27  auLTE','bNLTE','
-0000e530: 624c 5445 272c 2770 4e4c 5445 272c 2770  bLTE','pNLTE','p
-0000e540: 4c54 4527 2c27 464e 4c54 4527 2c27 464c  LTE','FNLTE','FL
-0000e550: 5445 275d 290a 2020 2020 2020 2020 2020  TE']).          
-0000e560: 2020 2020 2020 6c69 6e65 4461 7461 5b27        lineData['
-0000e570: 676c 6f62 616c 5f75 275d 3d5b 615b 305d  global_u']=[a[0]
-0000e580: 2066 6f72 2061 2069 6e20 6461 745b 325d   for a in dat[2]
-0000e590: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-0000e5a0: 2020 6c69 6e65 4461 7461 5b27 676c 6f62    lineData['glob
-0000e5b0: 616c 5f6c 275d 3d5b 615b 315d 2066 6f72  al_l']=[a[1] for
-0000e5c0: 2061 2069 6e20 6461 745b 325d 5d0a 2020   a in dat[2]].  
-0000e5d0: 2020 2020 2020 2020 2020 2020 2020 6c69                li
-0000e5e0: 6e65 4461 7461 5b27 6c6f 6361 6c5f 7527  neData['local_u'
-0000e5f0: 5d3d 5b61 5b32 5d20 666f 7220 6120 696e  ]=[a[2] for a in
-0000e600: 2064 6174 5b32 5d5d 0a20 2020 2020 2020   dat[2]].       
-0000e610: 2020 2020 2020 2020 206c 696e 6544 6174           lineDat
-0000e620: 615b 276c 6f63 616c 5f6c 275d 3d5b 615b  a['local_l']=[a[
-0000e630: 335d 2066 6f72 2061 2069 6e20 6461 745b  3] for a in dat[
-0000e640: 325d 5d0a 2020 2020 2020 2020 2020 2020  2]].            
-0000e650: 2020 2020 6c65 7644 6174 613d 7064 2e44      levData=pd.D
-0000e660: 6174 6146 7261 6d65 2864 6174 5b30 5d2c  ataFrame(dat[0],
-0000e670: 636f 6c75 6d6e 733d 5b27 6927 2c27 6727  columns=['i','g'
-0000e680: 2c27 4527 2c27 706f 7027 2c27 6c74 6570  ,'E','pop','ltep
-0000e690: 6f70 272c 2765 272c 2776 272c 274a 275d  op','e','v','J']
-0000e6a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000e6b0: 2020 7465 6d70 6f2e 6c69 6e65 6461 7461    tempo.linedata
-0000e6c0: 3d6c 696e 6544 6174 610a 2020 2020 2020  =lineData.      
-0000e6d0: 2020 2020 2020 2020 2020 7465 6d70 6f2e            tempo.
-0000e6e0: 6c65 7665 6c64 6174 613d 6c65 7644 6174  leveldata=levDat
-0000e6f0: 610a 2020 2020 2020 2020 2020 2020 2020  a.              
-0000e700: 2020 6461 7461 2e61 6464 5f6d 6f64 656c    data.add_model
-0000e710: 2874 656d 706f 290a 2020 2020 7265 7475  (tempo).    retu
-0000e720: 726e 2864 6174 6129 0a0a 0a64 6566 2072  rn(data)...def r
-0000e730: 6561 645f 6f76 6572 6c61 705f 7370 6563  ead_overlap_spec
-0000e740: 7472 6128 7061 7468 3d27 536c 6162 4f76  tra(path='SlabOv
-0000e750: 6572 6c61 702e 6f75 7427 2c76 6572 626f  erlap.out',verbo
-0000e760: 7365 3d54 7275 6529 3a0a 2020 2020 2222  se=True):.    ""
-0000e770: 220a 2020 2020 4675 6e63 7469 6f6e 2074  ".    Function t
-0000e780: 6f20 7265 6164 206f 4420 7072 6f64 696d  o read oD prodim
-0000e790: 6f20 736c 6162 206d 6f64 656c 206f 7574  o slab model out
-0000e7a0: 7075 7420 7769 7468 206c 696e 6520 6f76  put with line ov
-0000e7b0: 6572 6c61 700a 2020 2020 2222 220a 0a20  erlap.    """.. 
-0000e7c0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-0000e7d0: 2870 6174 682c 6c69 7374 293a 0a20 2020  (path,list):.   
-0000e7e0: 2020 2020 2064 6174 613d 736c 6162 5f64       data=slab_d
-0000e7f0: 6174 6128 290a 2020 2020 2020 2020 6461  ata().        da
-0000e800: 7461 2e64 6972 6563 746f 7279 3d70 6174  ta.directory=pat
-0000e810: 680a 2020 2020 2020 2020 666f 7220 6920  h.        for i 
-0000e820: 696e 2070 6174 683a 0a20 2020 2020 2020  in path:.       
-0000e830: 2020 2020 2072 6461 7461 3d72 6561 645f       rdata=read_
-0000e840: 6f76 6572 6c61 705f 7370 6563 7472 6128  overlap_spectra(
-0000e850: 692c 7665 7262 6f73 653d 7665 7262 6f73  i,verbose=verbos
-0000e860: 6529 0a20 2020 2020 2020 2020 2020 2066  e).            f
-0000e870: 6f72 206a 2069 6e20 7261 6e67 6528 7264  or j in range(rd
-0000e880: 6174 612e 6e6d 6f64 656c 7329 3a0a 2020  ata.nmodels):.  
-0000e890: 2020 2020 2020 2020 2020 2020 2020 6461                da
-0000e8a0: 7461 2e61 6464 5f6d 6f64 656c 2872 6461  ta.add_model(rda
-0000e8b0: 7461 2e6d 6f64 656c 735b 6a5d 290a 2020  ta.models[j]).  
-0000e8c0: 2020 2020 2020 7265 7475 726e 2864 6174        return(dat
-0000e8d0: 6129 0a0a 2020 2020 6966 2076 6572 626f  a)..    if verbo
-0000e8e0: 7365 3a20 7072 696e 7428 2252 6561 6469  se: print("Readi
-0000e8f0: 6e67 2073 6c61 6220 6c69 6e65 206f 7665  ng slab line ove
-0000e900: 726c 6170 206d 6f64 656c 206f 7574 7075  rlap model outpu
-0000e910: 7420 6672 6f6d 3a20 222c 7061 7468 290a  t from: ",path).
-0000e920: 2020 2020 6966 2027 2e66 6974 732e 677a      if '.fits.gz
-0000e930: 2720 696e 2070 6174 683a 0a20 2020 2020  ' in path:.     
-0000e940: 2020 2068 6475 6c3d 6669 7473 2e6f 7065     hdul=fits.ope
-0000e950: 6e28 7061 7468 290a 2020 2020 2020 2020  n(path).        
-0000e960: 6461 7461 3d73 6c61 625f 6461 7461 2829  data=slab_data()
-0000e970: 0a20 2020 2020 2020 206e 6d6f 6465 6c73  .        nmodels
-0000e980: 3d68 6475 6c5b 305d 2e68 6561 6465 725b  =hdul[0].header[
-0000e990: 274e 4d4f 4445 4c53 275d 0a20 2020 2020  'NMODELS'].     
-0000e9a0: 2020 2064 6174 612e 6469 7265 6374 6f72     data.director
-0000e9b0: 793d 7061 7468 0a20 2020 2020 2020 2066  y=path.        f
-0000e9c0: 6f72 2069 2069 6e20 7261 6e67 6528 6e6d  or i in range(nm
-0000e9d0: 6f64 656c 7329 3a0a 2020 2020 2020 2020  odels):.        
-0000e9e0: 2020 2020 7465 6d70 6f3d 736c 6162 2829      tempo=slab()
-0000e9f0: 0a20 2020 2020 2020 2020 2020 2074 656d  .            tem
-0000ea00: 706f 5f6d 6f64 656c 5f6e 756d 6265 723d  po_model_number=
-0000ea10: 6864 756c 5b69 2b31 5d2e 6865 6164 6572  hdul[i+1].header
-0000ea20: 5b27 4d4f 4445 4c27 5d0a 2020 2020 2020  ['MODEL'].      
-0000ea30: 2020 2020 2020 7465 6d70 6f5f 4e6c 696e        tempo_Nlin
-0000ea40: 653d 6864 756c 5b69 2b31 5d2e 6865 6164  e=hdul[i+1].head
-0000ea50: 6572 5b27 4e4c 494e 4527 5d0a 2020 2020  er['NLINE'].    
-0000ea60: 2020 2020 2020 2020 7465 6d70 6f5f 523d          tempo_R=
-0000ea70: 6864 756c 5b69 2b31 5d2e 6865 6164 6572  hdul[i+1].header
-0000ea80: 5b27 525f 4f56 4c50 275d 0a20 2020 2020  ['R_OVLP'].     
-0000ea90: 2020 2020 2020 2064 6174 7461 3d5b 5d0a         datta=[].
-0000eaa0: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-0000eab0: 6f2e 6f76 6572 6c61 7046 7265 713d 6864  o.overlapFreq=hd
-0000eac0: 756c 5b69 2b31 5d2e 6461 7461 5b3a 2c2d  ul[i+1].data[:,-
-0000ead0: 315d 0a20 2020 2020 2020 2020 2020 2074  1].            t
-0000eae0: 656d 706f 2e6f 7665 726c 6170 4c54 453d  empo.overlapLTE=
-0000eaf0: 6864 756c 5b69 2b31 5d2e 6461 7461 5b3a  hdul[i+1].data[:
-0000eb00: 2c30 5d0a 2020 2020 2020 2020 2020 2020  ,0].            
-0000eb10: 7465 6d70 6f2e 6f76 6572 6c61 7054 6175  tempo.overlapTau
-0000eb20: 4c54 453d 6864 756c 5b69 2b31 5d2e 6461  LTE=hdul[i+1].da
-0000eb30: 7461 5b3a 2c31 5d0a 2020 2020 2020 2020  ta[:,1].        
-0000eb40: 2020 2020 7465 6d70 6f2e 6f76 6572 6c61      tempo.overla
-0000eb50: 704e 4c54 453d 6864 756c 5b69 2b31 5d2e  pNLTE=hdul[i+1].
-0000eb60: 6461 7461 5b3a 2c32 5d0a 2020 2020 2020  data[:,2].      
-0000eb70: 2020 2020 2020 7465 6d70 6f2e 6f76 6572        tempo.over
-0000eb80: 6c61 7054 6175 4e4c 5445 3d68 6475 6c5b  lapTauNLTE=hdul[
-0000eb90: 692b 315d 2e64 6174 615b 3a2c 335d 0a20  i+1].data[:,3]. 
-0000eba0: 2020 2020 2020 2020 2020 2074 656d 706f             tempo
-0000ebb0: 2e6f 7665 726c 6170 523d 7465 6d70 6f5f  .overlapR=tempo_
-0000ebc0: 520a 2020 2020 2020 2020 2020 2020 7465  R.            te
-0000ebd0: 6d70 6f2e 6d6f 6465 6c5f 6e75 6d62 6572  mpo.model_number
-0000ebe0: 3d68 6475 6c5b 692b 315d 2e68 6561 6465  =hdul[i+1].heade
-0000ebf0: 725b 274d 4f44 454c 275d 0a20 2020 2020  r['MODEL'].     
-0000ec00: 2020 2020 2020 2074 656d 706f 2e54 673d         tempo.Tg=
-0000ec10: 6864 756c 5b69 2b31 5d2e 6865 6164 6572  hdul[i+1].header
-0000ec20: 5b27 5447 275d 0a20 2020 2020 2020 2020  ['TG'].         
-0000ec30: 2020 2074 656d 706f 2e54 643d 6864 756c     tempo.Td=hdul
-0000ec40: 5b69 2b31 5d2e 6865 6164 6572 5b27 5444  [i+1].header['TD
-0000ec50: 275d 0a20 2020 2020 2020 2020 2020 2074  '].            t
-0000ec60: 656d 706f 2e76 7475 7262 3d68 6475 6c5b  empo.vturb=hdul[
-0000ec70: 692b 315d 2e68 6561 6465 725b 2756 5455  i+1].header['VTU
-0000ec80: 5242 275d 0a20 2020 2020 2020 2020 2020  RB'].           
-0000ec90: 2074 656d 706f 2e4e 483d 6864 756c 5b69   tempo.NH=hdul[i
-0000eca0: 2b31 5d2e 6865 6164 6572 5b27 4e48 544f  +1].header['NHTO
-0000ecb0: 5427 5d0a 2020 2020 2020 2020 2020 2020  T'].            
-0000ecc0: 6461 7461 2e61 6464 5f6d 6f64 656c 2874  data.add_model(t
-0000ecd0: 656d 706f 290a 2020 2020 2020 2020 2020  empo).          
-0000ece0: 2020 2320 7072 696e 7428 2772 6561 6420    # print('read 
-0000ecf0: 272c 692c 2720 6d6f 6465 6c27 290a 2020  ',i,' model').  
-0000ed00: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000ed10: 663d 6f70 656e 2870 6174 6829 0a20 2020  f=open(path).   
-0000ed20: 2020 2020 2064 6174 613d 736c 6162 5f64       data=slab_d
-0000ed30: 6174 6128 290a 2020 2020 2020 2020 6e6d  ata().        nm
-0000ed40: 6f64 656c 733d 696e 7428 662e 7265 6164  odels=int(f.read
-0000ed50: 6c69 6e65 2829 2e73 706c 6974 2829 5b30  line().split()[0
-0000ed60: 5d29 0a20 2020 2020 2020 2064 6174 612e  ]).        data.
-0000ed70: 6469 7265 6374 6f72 793d 7061 7468 0a20  directory=path. 
-0000ed80: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-0000ed90: 7261 6e67 6528 6e6d 6f64 656c 7329 3a0a  range(nmodels):.
-0000eda0: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-0000edb0: 6f3d 736c 6162 2829 0a20 2020 2020 2020  o=slab().       
-0000edc0: 2020 2020 2074 656d 706f 5f6d 6f64 656c       tempo_model
-0000edd0: 5f6e 756d 6265 723d 696e 7428 662e 7265  _number=int(f.re
-0000ede0: 6164 6c69 6e65 2829 2e73 706c 6974 2829  adline().split()
-0000edf0: 5b30 5d29 0a20 2020 2020 2020 2020 2020  [0]).           
-0000ee00: 2074 656d 706f 5f4e 6c69 6e65 3d69 6e74   tempo_Nline=int
-0000ee10: 2866 2e72 6561 646c 696e 6528 292e 7370  (f.readline().sp
-0000ee20: 6c69 7428 295b 305d 290a 2020 2020 2020  lit()[0]).      
-0000ee30: 2020 2020 2020 7465 6d70 6f5f 523d 666c        tempo_R=fl
-0000ee40: 6f61 7428 662e 7265 6164 6c69 6e65 2829  oat(f.readline()
-0000ee50: 2e73 706c 6974 2829 5b30 5d29 0a20 2020  .split()[0]).   
-0000ee60: 2020 2020 2020 2020 2064 6174 7461 3d5b           datta=[
-0000ee70: 5d0a 2020 2020 2020 2020 2020 2020 6c69  ].            li
-0000ee80: 6e65 733d 662e 7265 6164 6c69 6e65 2829  nes=f.readline()
-0000ee90: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-0000eea0: 206a 2069 6e20 7261 6e67 6528 7465 6d70   j in range(temp
-0000eeb0: 6f5f 4e6c 696e 6529 3a0a 2020 2020 2020  o_Nline):.      
-0000eec0: 2020 2020 2020 2020 2020 6c69 6e65 733d            lines=
-0000eed0: 662e 7265 6164 6c69 6e65 2829 0a20 2020  f.readline().   
-0000eee0: 2020 2020 2020 2020 2020 2020 2064 6174               dat
-0000eef0: 7461 2e61 7070 656e 6428 6e70 2e61 7272  ta.append(np.arr
-0000ef00: 6179 286c 696e 6573 2e73 706c 6974 2829  ay(lines.split()
-0000ef10: 2c64 7479 7065 3d66 6c6f 6174 2929 0a20  ,dtype=float)). 
-0000ef20: 2020 2020 2020 2020 2020 2064 6174 7461             datta
-0000ef30: 3d6e 702e 6172 7261 7928 6461 7474 6129  =np.array(datta)
-0000ef40: 0a20 2020 2020 2020 2020 2020 2074 656d  .            tem
-0000ef50: 706f 2e6f 7665 726c 6170 4672 6571 3d64  po.overlapFreq=d
-0000ef60: 6174 7461 5b3a 2c30 5d0a 2020 2020 2020  atta[:,0].      
-0000ef70: 2020 2020 2020 7465 6d70 6f2e 6f76 6572        tempo.over
-0000ef80: 6c61 704c 5445 3d64 6174 7461 5b3a 2c31  lapLTE=datta[:,1
-0000ef90: 5d0a 2020 2020 2020 2020 2020 2020 7465  ].            te
-0000efa0: 6d70 6f2e 6f76 6572 6c61 7054 6175 4c54  mpo.overlapTauLT
-0000efb0: 453d 6461 7474 615b 3a2c 325d 0a20 2020  E=datta[:,2].   
-0000efc0: 2020 2020 2020 2020 2074 656d 706f 2e6f           tempo.o
-0000efd0: 7665 726c 6170 4e4c 5445 3d64 6174 7461  verlapNLTE=datta
-0000efe0: 5b3a 2c33 5d0a 2020 2020 2020 2020 2020  [:,3].          
-0000eff0: 2020 7465 6d70 6f2e 6f76 6572 6c61 7054    tempo.overlapT
-0000f000: 6175 4e4c 5445 3d64 6174 7461 5b3a 2c34  auNLTE=datta[:,4
-0000f010: 5d0a 2020 2020 2020 2020 2020 2020 7465  ].            te
-0000f020: 6d70 6f2e 6f76 6572 6c61 7052 3d74 656d  mpo.overlapR=tem
-0000f030: 706f 5f52 0a20 2020 2020 2020 2020 2020  po_R.           
-0000f040: 2064 6174 612e 6164 645f 6d6f 6465 6c28   data.add_model(
-0000f050: 7465 6d70 6f29 0a20 2020 2020 2020 2020  tempo).         
-0000f060: 2020 206c 696e 6573 3d66 2e72 6561 646c     lines=f.readl
-0000f070: 696e 6528 290a 2020 2020 2020 2020 2020  ine().          
-0000f080: 2020 2320 7072 696e 7428 2772 6561 6420    # print('read 
-0000f090: 272c 692c 2720 6d6f 6465 6c27 290a 0a20  ',i,' model').. 
-0000f0a0: 2020 2072 6574 7572 6e28 6461 7461 290a     return(data).
-0000f0b0: 0a0a 6465 6620 7370 6563 436f 6e76 6f6c  ..def specConvol
-0000f0c0: 7665 286c 696e 6553 7472 656e 6774 6873  ve(lineStrengths
-0000f0d0: 2c6c 696e 6546 7265 712c 6672 6571 5f62  ,lineFreq,freq_b
-0000f0e0: 696e 733d 4e6f 6e65 2c52 3d31 2c6c 616d  ins=None,R=1,lam
-0000f0f0: 6264 615f 303d 312c 6c61 6d62 6461 5f6e  bda_0=1,lambda_n
-0000f100: 3d31 2c76 723d 3133 3030 293a 0a20 2020  =1,vr=1300):.   
-0000f110: 2022 2222 0a20 2020 204e 4f54 2055 5345   """.    NOT USE
-0000f120: 4420 414e 594d 4f52 450a 2020 2020 4675  D ANYMORE.    Fu
-0000f130: 6e63 7469 6f6e 2074 6f20 636f 6e76 6f6c  nction to convol
-0000f140: 7665 206c 696e 6573 2069 6e74 6f20 7370  ve lines into sp
-0000f150: 6563 7472 6120 6279 2073 696d 706c 7920  ectra by simply 
-0000f160: 6269 6e6e 696e 6720 7468 656d 2069 6e74  binning them int
-0000f170: 6f20 6120 7761 7665 6c65 6e67 7468 2067  o a wavelength g
-0000f180: 7269 640a 2020 2020 2222 220a 2020 2020  rid.    """.    
-0000f190: 6750 6572 633d 6c61 6d62 6461 2078 2c6d  gPerc=lambda x,m
-0000f1a0: 2c73 3a20 7365 7266 2828 782d 6d29 2f73  ,s: serf((x-m)/s
-0000f1b0: 292a 302e 352b 302e 350a 2020 2020 6e75  )*0.5+0.5.    nu
-0000f1c0: 5f69 6a3d 6c69 6e65 4672 6571 2a31 6539  _ij=lineFreq*1e9
-0000f1d0: 0a20 2020 2069 6620 6c61 6d62 6461 5f6e  .    if lambda_n
-0000f1e0: 3d3d 6c61 6d62 6461 5f30 3a0a 2020 2020  ==lambda_0:.    
-0000f1f0: 2020 2020 6c61 6d62 6461 5f6e 3d6e 702e      lambda_n=np.
-0000f200: 616d 6178 2863 2f6e 755f 696a 2a31 6536  amax(c/nu_ij*1e6
-0000f210: 292a 320a 2020 2020 6966 2074 7970 6528  )*2.    if type(
-0000f220: 6672 6571 5f62 696e 7329 3d3d 7479 7065  freq_bins)==type
-0000f230: 284e 6f6e 6529 3a0a 2020 2020 2020 2020  (None):.        
-0000f240: 6e75 3d67 656e 6572 6174 655f 6772 6964  nu=generate_grid
-0000f250: 2852 3d52 2c6c 616d 6264 615f 303d 6c61  (R=R,lambda_0=la
-0000f260: 6d62 6461 5f30 2c6c 616d 6264 615f 6e3d  mbda_0,lambda_n=
-0000f270: 6c61 6d62 6461 5f6e 292a 3165 390a 2020  lambda_n)*1e9.  
-0000f280: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000f290: 6672 6571 5f62 696e 733d 6e70 2e63 6f6e  freq_bins=np.con
-0000f2a0: 6361 7465 6e61 7465 2828 6672 6571 5f62  catenate((freq_b
-0000f2b0: 696e 732c 6e70 2e61 7272 6179 285b 2866  ins,np.array([(f
-0000f2c0: 7265 715f 6269 6e73 5b2d 315d 2d66 7265  req_bins[-1]-fre
-0000f2d0: 715f 6269 6e73 5b2d 325d 292b 6672 6571  q_bins[-2])+freq
-0000f2e0: 5f62 696e 735b 2d31 5d5d 2929 290a 2020  _bins[-1]]))).  
-0000f2f0: 2020 2020 2020 6e75 3d66 7265 715f 6269        nu=freq_bi
-0000f300: 6e73 2a31 6539 0a20 2020 206e 755f 696a  ns*1e9.    nu_ij
-0000f310: 5f74 696c 653d 6e70 2e74 696c 6528 6e75  _tile=np.tile(nu
-0000f320: 5f69 6a2c 5b6c 656e 286e 7529 2c31 5d29  _ij,[len(nu),1])
-0000f330: 0a20 2020 206e 755f 7469 6c65 3d6e 702e  .    nu_tile=np.
-0000f340: 7469 6c65 286e 752c 5b6c 656e 286e 755f  tile(nu,[len(nu_
-0000f350: 696a 292c 315d 290a 2020 2020 6c69 6e65  ij),1]).    line
-0000f360: 5374 7265 6e67 7468 735f 7469 6c65 3d6e  Strengths_tile=n
-0000f370: 702e 7469 6c65 286c 696e 6553 7472 656e  p.tile(lineStren
-0000f380: 6774 6873 2c5b 6c65 6e28 6e75 292c 315d  gths,[len(nu),1]
-0000f390: 290a 2020 2020 7065 7263 5f74 696c 653d  ).    perc_tile=
-0000f3a0: 6750 6572 6328 6e75 5f74 696c 652c 6e75  gPerc(nu_tile,nu
-0000f3b0: 5f69 6a5f 7469 6c65 2e54 2c6e 755f 696a  _ij_tile.T,nu_ij
-0000f3c0: 5f74 696c 652e 542f 632a 7672 290a 2020  _tile.T/c*vr).  
-0000f3d0: 2020 783d 7065 7263 5f74 696c 655b 3a2c    x=perc_tile[:,
-0000f3e0: 3a2d 315d 2d70 6572 635f 7469 6c65 5b3a  :-1]-perc_tile[:
-0000f3f0: 2c31 3a5d 0a20 2020 2077 6176 656c 656e  ,1:].    wavelen
-0000f400: 6774 682c 666c 7578 3d63 2f6e 755b 3a2d  gth,flux=c/nu[:-
-0000f410: 315d 2a31 6536 2c6e 702e 7375 6d28 782a  1]*1e6,np.sum(x*
-0000f420: 6c69 6e65 5374 7265 6e67 7468 735f 7469  lineStrengths_ti
-0000f430: 6c65 5b3a 2d31 2c3a 5d2e 542c 6178 6973  le[:-1,:].T,axis
-0000f440: 3d30 292f 286e 755b 3a2d 315d 2d6e 755b  =0)/(nu[:-1]-nu[
-0000f450: 313a 5d29 0a20 2020 2072 6574 7572 6e20  1:]).    return 
-0000f460: 7761 7665 6c65 6e67 7468 2c66 6c75 780a  wavelength,flux.
-0000f470: 0a0a 6465 6620 6765 6e65 7261 6c43 6f6e  ..def generalCon
-0000f480: 766f 6c76 6528 6c69 6e65 5374 7265 6e67  volve(lineStreng
-0000f490: 7468 732c 6c69 6e65 4672 6571 2c52 3d31  ths,lineFreq,R=1
-0000f4a0: 2c6c 616d 6264 615f 303d 312c 6c61 6d62  ,lambda_0=1,lamb
-0000f4b0: 6461 5f6e 3d31 2c52 5f62 6163 6b3d 3165  da_n=1,R_back=1e
-0000f4c0: 3629 3a0a 2020 2020 2222 220a 2020 2020  6):.    """.    
-0000f4d0: 4675 6e63 7469 6f6e 2074 6f20 636f 6e76  Function to conv
-0000f4e0: 6f6c 7665 206c 696e 6520 666c 7578 6573  olve line fluxes
-0000f4f0: 2069 6e74 6f20 6c69 6e65 2073 7065 6374   into line spect
-0000f500: 7261 2062 6173 6564 206f 6e20 6120 7573  ra based on a us
-0000f510: 6572 2064 6566 696e 6564 2073 7065 6374  er defined spect
-0000f520: 7261 6c20 7265 736f 6c76 696e 6720 706f  ral resolving po
-0000f530: 7765 7220 520a 2020 2020 2222 220a 2020  wer R.    """.  
-0000f540: 2020 6966 206c 616d 6264 615f 6e3d 3d6c    if lambda_n==l
-0000f550: 616d 6264 615f 303a 0a20 2020 2020 2020  ambda_0:.       
-0000f560: 206c 616d 6264 615f 6e3d 632f 6e70 2e61   lambda_n=c/np.a
-0000f570: 6d69 6e28 6c69 6e65 4672 6571 292a 3165  min(lineFreq)*1e
-0000f580: 2d33 2a32 0a20 2020 2066 7265 715f 6269  -3*2.    freq_bi
-0000f590: 6e73 3d67 656e 6572 6174 655f 6772 6964  ns=generate_grid
-0000f5a0: 2852 5f62 6163 6b2c 6c61 6d62 6461 5f30  (R_back,lambda_0
-0000f5b0: 2c6c 616d 6264 615f 6e29 0a20 2020 2077  ,lambda_n).    w
-0000f5c0: 6176 655f 6269 6e73 3d63 2f66 7265 715f  ave_bins=c/freq_
-0000f5d0: 6269 6e73 2a31 652d 330a 2020 2020 666c  bins*1e-3.    fl
-0000f5e0: 7578 5f62 696e 733d 7761 7665 5f62 696e  ux_bins=wave_bin
-0000f5f0: 732a 302e 300a 2020 2020 693d 360a 2020  s*0.0.    i=6.  
-0000f600: 2020 533d 6c69 6e65 5374 7265 6e67 7468    S=lineStrength
-0000f610: 730a 2020 2020 463d 6c69 6e65 4672 6571  s.    F=lineFreq
-0000f620: 0a20 2020 2069 6e64 3d6e 702e 6469 6769  .    ind=np.digi
-0000f630: 7469 7a65 2846 2c6e 702e 666c 6970 2866  tize(F,np.flip(f
-0000f640: 7265 715f 6269 6e73 295b 3a2d 315d 290a  req_bins)[:-1]).
-0000f650: 2020 2020 666f 7220 692c 6964 7820 696e      for i,idx in
-0000f660: 2065 6e75 6d65 7261 7465 2869 6e64 293a   enumerate(ind):
-0000f670: 0a20 2020 2020 2020 2066 6c75 785f 6269  .        flux_bi
-0000f680: 6e73 5b69 6478 5d2b 3d53 5b69 5d0a 0a20  ns[idx]+=S[i].. 
-0000f690: 2020 2046 5748 4d3d 525f 6261 636b 2f52     FWHM=R_back/R
-0000f6a0: 2f32 2e33 3535 0a20 2020 2067 3d47 6175  /2.355.    g=Gau
-0000f6b0: 7373 6961 6e31 444b 6572 6e65 6c28 7374  ssian1DKernel(st
-0000f6c0: 6464 6576 3d46 5748 4d2c 6661 6374 6f72  ddev=FWHM,factor
-0000f6d0: 3d37 290a 2020 2020 413d 6170 795f 636f  =7).    A=apy_co
-0000f6e0: 6e76 6f6c 7665 2866 6c75 785f 6269 6e73  nvolve(flux_bins
-0000f6f0: 2c67 290a 2020 2020 413d 415b 313a 5d2f  ,g).    A=A[1:]/
-0000f700: 286e 702e 666c 6970 2866 7265 715f 6269  (np.flip(freq_bi
-0000f710: 6e73 295b 313a 5d2d 6e70 2e66 6c69 7028  ns)[1:]-np.flip(
-0000f720: 6672 6571 5f62 696e 7329 5b3a 2d31 5d29  freq_bins)[:-1])
-0000f730: 2a31 652d 390a 2020 2020 573d 6e70 2e66  *1e-9.    W=np.f
-0000f740: 6c69 7028 7761 7665 5f62 696e 735b 313a  lip(wave_bins[1:
-0000f750: 5d29 0a20 2020 2072 6574 7572 6e20 6e70  ]).    return np
-0000f760: 2e66 6c69 7028 5729 2c6e 702e 666c 6970  .flip(W),np.flip
-0000f770: 2841 290a 0a0a 6465 6620 6765 6e65 7261  (A)...def genera
-0000f780: 7465 5f67 7269 6428 523d 312c 6c61 6d62  te_grid(R=1,lamb
-0000f790: 6461 5f30 3d31 2c6c 616d 6264 615f 6e3d  da_0=1,lambda_n=
-0000f7a0: 312c 7361 6d70 6c69 6e67 3d31 293a 0a20  1,sampling=1):. 
-0000f7b0: 2020 2022 2222 0a20 2020 2047 656e 6572     """.    Gener
-0000f7c0: 6174 6520 6120 7370 6563 7472 616c 2067  ate a spectral g
-0000f7d0: 7269 6420 696e 2047 487a 0a20 2020 2022  rid in GHz.    "
-0000f7e0: 2222 0a20 2020 2064 656c 5f6c 6f67 6c61  "".    del_logla
-0000f7f0: 6d3d 6e70 2e6c 6f67 3130 2831 2e30 2b31  m=np.log10(1.0+1
-0000f800: 2e30 2f52 290a 2020 2020 4e3d 312b 696e  .0/R).    N=1+in
-0000f810: 7428 6e70 2e6c 6f67 3130 286c 616d 6264  t(np.log10(lambd
-0000f820: 615f 6e2f 6c61 6d62 6461 5f30 292f 6465  a_n/lambda_0)/de
-0000f830: 6c5f 6c6f 676c 616d 290a 2020 2020 6d77  l_loglam).    mw
-0000f840: 6c73 6c69 6e65 3d6e 702e 6c6f 6773 7061  lsline=np.logspa
-0000f850: 6365 286e 702e 6c6f 6731 3028 6c61 6d62  ce(np.log10(lamb
-0000f860: 6461 5f30 292c 6e70 2e6c 6f67 3130 286c  da_0),np.log10(l
-0000f870: 616d 6264 615f 6e29 2c69 6e74 284e 2a73  ambda_n),int(N*s
-0000f880: 616d 706c 696e 6729 290a 2020 2020 6e75  ampling)).    nu
-0000f890: 3d63 2f6d 776c 736c 696e 652a 3165 360a  =c/mwlsline*1e6.
-0000f8a0: 2020 2020 7265 7475 726e 286e 752a 3165      return(nu*1e
-0000f8b0: 2d39 290a 0a0a 6465 6620 636f 6e76 6f6c  -9)...def convol
-0000f8c0: 7665 286d 6f64 656c 732c 6672 6571 5f62  ve(models,freq_b
-0000f8d0: 696e 733d 4e6f 6e65 2c52 3d31 2c6c 616d  ins=None,R=1,lam
-0000f8e0: 6264 615f 303d 312c 6c61 6d62 6461 5f6e  bda_0=1,lambda_n
-0000f8f0: 3d31 2c76 723d 3133 3030 2c4e 4c54 453d  =1,vr=1300,NLTE=
-0000f900: 4661 6c73 652c 636f 6e76 5f74 7970 653d  False,conv_type=
-0000f910: 312c 7665 7262 6f73 653d 5472 7565 293a  1,verbose=True):
-0000f920: 0a20 2020 2022 2222 0a20 2020 2053 616d  .    """.    Sam
-0000f930: 6520 6173 202e 636f 6e76 6f6c 7665 2829  e as .convolve()
-0000f940: 206d 6574 686f 640a 2020 2020 2222 220a   method.    """.
-0000f950: 2020 2020 666f 7220 692c 6420 696e 2065      for i,d in e
-0000f960: 6e75 6d65 7261 7465 286d 6f64 656c 7329  numerate(models)
-0000f970: 3a0a 2020 2020 2020 2020 6966 2076 6572  :.        if ver
-0000f980: 626f 7365 3a20 7072 696e 7428 275c 6e5c  bose: print('\n\
-0000f990: 6e4d 6f64 656c 2027 2c69 2b31 290a 2020  nModel ',i+1).  
-0000f9a0: 2020 2020 2020 642e 636f 6e76 6f6c 7665        d.convolve
-0000f9b0: 2866 7265 715f 6269 6e73 3d66 7265 715f  (freq_bins=freq_
-0000f9c0: 6269 6e73 2c52 3d52 2c6c 616d 6264 615f  bins,R=R,lambda_
-0000f9d0: 303d 6c61 6d62 6461 5f30 2c6c 616d 6264  0=lambda_0,lambd
-0000f9e0: 615f 6e3d 6c61 6d62 6461 5f6e 2c76 723d  a_n=lambda_n,vr=
-0000f9f0: 7672 2c4e 4c54 453d 4e4c 5445 2c63 6f6e  vr,NLTE=NLTE,con
-0000fa00: 765f 7479 7065 3d63 6f6e 765f 7479 7065  v_type=conv_type
-0000fa10: 290a 2020 2020 7265 7475 726e 206d 6f64  ).    return mod
-0000fa20: 656c 730a 0a0a 6465 6620 6765 6e65 7261  els...def genera
-0000fa30: 7465 5f73 6c61 625f 6772 6964 2864 6972  te_slab_grid(dir
-0000fa40: 6563 746f 7279 3d27 2e27 2c67 7269 645f  ectory='.',grid_
-0000fa50: 7061 7261 6d65 7465 7273 3d7b 7d2c 636f  parameters={},co
-0000fa60: 6d62 696e 6174 696f 6e3d 4661 6c73 652c  mbination=False,
-0000fa70: 4e74 6f74 3d4e 6f6e 652c 5467 3d4e 6f6e  Ntot=None,Tg=Non
-0000fa80: 652c 6e48 706c 7573 3d4e 6f6e 652c 6e48  e,nHplus=None,nH
-0000fa90: 313d 4e6f 6e65 2c6e 4832 3d4e 6f6e 652c  1=None,nH2=None,
-0000faa0: 6e48 653d 4e6f 6e65 2c6e 656c 6563 3d4e  nHe=None,nelec=N
-0000fab0: 6f6e 652c 5464 3d4e 6f6e 652c 7674 7572  one,Td=None,vtur
-0000fac0: 623d 4e6f 6e65 2c64 7573 745f 746f 5f67  b=None,dust_to_g
-0000fad0: 6173 3d4e 6f6e 652c 525f 6f76 6572 6c61  as=None,R_overla
-0000fae0: 703d 4e6f 6e65 2c6c 696e 655f 6f76 6572  p=None,line_over
-0000faf0: 6c61 703d 4e6f 6e65 2c73 7065 6369 6573  lap=None,species
-0000fb00: 5f6c 6973 743d 7b7d 2c6f 7574 7075 745f  _list={},output_
-0000fb10: 6669 6c65 6e61 6d65 3d27 536c 6162 5265  filename='SlabRe
-0000fb20: 7375 6c74 732e 6f75 7427 2c6f 7665 726c  sults.out',overl
-0000fb30: 6170 5f66 696c 656e 616d 653d 2753 6c61  ap_filename='Sla
-0000fb40: 624f 7665 726c 6170 2e6f 7574 272c 7365  bOverlap.out',se
-0000fb50: 7061 7261 7465 5f6f 705f 6669 6c65 733d  parate_op_files=
-0000fb60: 5472 7565 2c73 6c61 625f 5254 3d54 7275  True,slab_RT=Tru
-0000fb70: 652c 7368 6f72 745f 666f 726d 6174 3d46  e,short_format=F
-0000fb80: 616c 7365 2c6e 6f5f 696e 6469 7669 6475  alse,no_individu
-0000fb90: 616c 5f6c 696e 6573 3d46 616c 7365 2c66  al_lines=False,f
-0000fba0: 6974 735f 6f70 5f66 696c 6573 3d46 616c  its_op_files=Fal
-0000fbb0: 7365 293a 0a20 2020 2022 2222 0a20 2020  se):.    """.   
-0000fbc0: 2046 756e 6374 696f 6e20 746f 2067 656e   Function to gen
-0000fbd0: 6572 6174 6520 536c 6162 496e 7075 742e  erate SlabInput.
-0000fbe0: 696e 2069 6e70 7574 2066 696c 6520 636f  in input file co
-0000fbf0: 6e74 6169 6e69 6e67 2074 6865 2064 6574  ntaining the det
-0000fc00: 6169 6c73 206f 6620 7468 6520 736c 6162  ails of the slab
-0000fc10: 206d 6f64 656c 2067 7269 640a 2020 2020   model grid.    
-0000fc20: 2222 220a 2020 2020 6e6d 6f64 656c 733d  """.    nmodels=
-0000fc30: 310a 2020 2020 636f 6d62 696e 6174 696f  1.    combinatio
-0000fc40: 6e3d 4661 6c73 650a 2020 2020 6966 206c  n=False.    if l
-0000fc50: 656e 2867 7269 645f 7061 7261 6d65 7465  en(grid_paramete
-0000fc60: 7273 293e 303a 0a20 2020 2020 2020 2069  rs)>0:.        i
-0000fc70: 6620 6e6f 7420 636f 6d62 696e 6174 696f  f not combinatio
-0000fc80: 6e3a 0a20 2020 2020 2020 2020 2020 206e  n:.            n
-0000fc90: 6d6f 6465 6c73 3d6c 656e 2867 7269 645f  models=len(grid_
-0000fca0: 7061 7261 6d65 7465 7273 5b6c 6973 7428  parameters[list(
-0000fcb0: 6772 6964 5f70 6172 616d 6574 6572 732e  grid_parameters.
-0000fcc0: 6b65 7973 2829 295b 305d 5d29 0a20 2020  keys())[0]]).   
-0000fcd0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000fce0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-0000fcf0: 7261 6e67 6528 6c65 6e28 6772 6964 5f70  range(len(grid_p
-0000fd00: 6172 616d 6574 6572 7329 293a 0a20 2020  arameters)):.   
-0000fd10: 2020 2020 2020 2020 2020 2020 206e 6d6f               nmo
-0000fd20: 6465 6c73 2a3d 6c65 6e28 6772 6964 5f70  dels*=len(grid_p
-0000fd30: 6172 616d 6574 6572 735b 6c69 7374 2867  arameters[list(g
-0000fd40: 7269 645f 7061 7261 6d65 7465 7273 2e6b  rid_parameters.k
-0000fd50: 6579 7328 2929 5b69 5d5d 290a 0a20 2020  eys())[i]])..   
-0000fd60: 204e 746f 745f 6c69 7374 3d6e 702e 6f6e   Ntot_list=np.on
-0000fd70: 6573 2828 6e6d 6f64 656c 7329 290a 2020  es((nmodels)).  
-0000fd80: 2020 5467 5f6c 6973 743d 6e70 2e6f 6e65    Tg_list=np.one
-0000fd90: 7328 286e 6d6f 6465 6c73 2929 0a20 2020  s((nmodels)).   
-0000fda0: 206e 4870 6c75 735f 6c69 7374 3d6e 702e   nHplus_list=np.
-0000fdb0: 6f6e 6573 2828 6e6d 6f64 656c 7329 290a  ones((nmodels)).
-0000fdc0: 2020 2020 6e48 315f 6c69 7374 3d6e 702e      nH1_list=np.
-0000fdd0: 6f6e 6573 2828 6e6d 6f64 656c 7329 290a  ones((nmodels)).
-0000fde0: 2020 2020 6e48 325f 6c69 7374 3d6e 702e      nH2_list=np.
-0000fdf0: 6f6e 6573 2828 6e6d 6f64 656c 7329 290a  ones((nmodels)).
-0000fe00: 2020 2020 6e48 655f 6c69 7374 3d6e 702e      nHe_list=np.
-0000fe10: 6f6e 6573 2828 6e6d 6f64 656c 7329 290a  ones((nmodels)).
-0000fe20: 2020 2020 6e65 6c65 635f 6c69 7374 3d6e      nelec_list=n
-0000fe30: 702e 6f6e 6573 2828 6e6d 6f64 656c 7329  p.ones((nmodels)
-0000fe40: 290a 2020 2020 5464 5f6c 6973 743d 6e70  ).    Td_list=np
-0000fe50: 2e6f 6e65 7328 286e 6d6f 6465 6c73 2929  .ones((nmodels))
-0000fe60: 0a20 2020 2076 7475 7262 5f6c 6973 743d  .    vturb_list=
-0000fe70: 6e70 2e6f 6e65 7328 286e 6d6f 6465 6c73  np.ones((nmodels
-0000fe80: 2929 0a20 2020 2064 7573 745f 746f 5f67  )).    dust_to_g
-0000fe90: 6173 5f6c 6973 743d 6e70 2e6f 6e65 7328  as_list=np.ones(
-0000fea0: 286e 6d6f 6465 6c73 2929 0a20 2020 2052  (nmodels)).    R
-0000feb0: 5f6f 7665 726c 6170 5f6c 6973 743d 6e70  _overlap_list=np
+0000c810: 6772 6964 5b27 5464 275d 3d67 7269 645b  grid['Td']=grid[
+0000c820: 3a2c 335d 0a20 2020 2020 2020 2020 2020  :,3].           
+0000c830: 2064 6174 612e 6772 6964 5b27 6e48 3227   data.grid['nH2'
+0000c840: 5d3d 6772 6964 5b3a 2c34 5d0a 2020 2020  ]=grid[:,4].    
+0000c850: 2020 2020 2020 2020 6461 7461 2e67 7269          data.gri
+0000c860: 645b 276e 4849 275d 3d67 7269 645b 3a2c  d['nHI']=grid[:,
+0000c870: 355d 0a20 2020 2020 2020 2020 2020 2064  5].            d
+0000c880: 6174 612e 6772 6964 5b27 6e48 4949 275d  ata.grid['nHII']
+0000c890: 3d67 7269 645b 3a2c 365d 0a20 2020 2020  =grid[:,6].     
+0000c8a0: 2020 2020 2020 2064 6174 612e 6772 6964         data.grid
+0000c8b0: 5b27 6e48 6527 5d3d 6772 6964 5b3a 2c37  ['nHe']=grid[:,7
+0000c8c0: 5d0a 2020 2020 2020 2020 2020 2020 6461  ].            da
+0000c8d0: 7461 2e67 7269 645b 276e 656c 6563 275d  ta.grid['nelec']
+0000c8e0: 3d67 7269 645b 3a2c 385d 0a20 2020 2020  =grid[:,8].     
+0000c8f0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+0000c900: 7261 6e67 6528 6461 7461 2e4e 7370 6563  range(data.Nspec
+0000c910: 6965 7329 3a0a 2020 2020 2020 2020 2020  ies):.          
+0000c920: 2020 2020 2020 6b65 793d 276e 272b 6461        key='n'+da
+0000c930: 7461 2e73 7065 6369 6573 5b69 5d0a 2020  ta.species[i].  
+0000c940: 2020 2020 2020 2020 2020 2020 2020 6461                da
+0000c950: 7461 2e67 7269 645b 6b65 795d 3d67 7269  ta.grid[key]=gri
+0000c960: 645b 3a2c 392b 695d 0a20 2020 2020 2020  d[:,9+i].       
+0000c970: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
+0000c980: 6e67 6528 6461 7461 2e4e 7370 6563 6965  nge(data.Nspecie
+0000c990: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+0000c9a0: 2020 2020 6b65 793d 2754 675f 272b 6461      key='Tg_'+da
+0000c9b0: 7461 2e73 7065 6369 6573 5b69 5d0a 2020  ta.species[i].  
+0000c9c0: 2020 2020 2020 2020 2020 2020 2020 6461                da
+0000c9d0: 7461 2e67 7269 645b 6b65 795d 3d67 7269  ta.grid[key]=gri
+0000c9e0: 645b 3a2c 392b 6461 7461 2e4e 7370 6563  d[:,9+data.Nspec
+0000c9f0: 6965 732b 695d 0a20 2020 2020 2020 2065  ies+i].        e
+0000ca00: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0000ca10: 2072 6169 7365 2041 7373 6572 7469 6f6e   raise Assertion
+0000ca20: 4572 726f 7228 2747 7269 6420 696e 206f  Error('Grid in o
+0000ca30: 7574 7075 7420 6669 6c65 2064 6f65 7320  utput file does 
+0000ca40: 6e6f 7420 6d61 7463 6820 7468 6520 6163  not match the ac
+0000ca50: 7475 616c 2067 7269 6420 6f75 7470 7574  tual grid output
+0000ca60: 2061 7272 6179 2729 0a0a 2020 2020 2020   array')..      
+0000ca70: 2020 6966 2028 6c65 6e28 6461 7461 2e66    if (len(data.f
+0000ca80: 7265 7175 656e 6379 292c 6461 7461 2e4e  requency),data.N
+0000ca90: 6772 6964 293d 3d68 6475 6c5b 325d 2e64  grid)==hdul[2].d
+0000caa0: 6174 612e 542e 7368 6170 653a 0a20 2020  ata.T.shape:.   
+0000cab0: 2020 2020 2020 2020 2064 6174 612e 736f           data.so
+0000cac0: 7572 6365 5f66 756e 6374 696f 6e3d 6864  urce_function=hd
+0000cad0: 756c 5b32 5d2e 6461 7461 0a20 2020 2020  ul[2].data.     
+0000cae0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000caf0: 2020 2020 2072 6169 7365 2041 7373 6572       raise Asser
+0000cb00: 7469 6f6e 4572 726f 7228 2753 6f75 7263  tionError('Sourc
+0000cb10: 6520 6675 6e63 7469 6f6e 2067 7269 6420  e function grid 
+0000cb20: 696e 206f 7574 7075 7420 6669 6c65 2064  in output file d
+0000cb30: 6f65 7320 6e6f 7420 6d61 7463 6820 7468  oes not match th
+0000cb40: 6520 7370 6174 6961 6c20 616e 6420 6672  e spatial and fr
+0000cb50: 6571 7565 6e63 7920 6772 6964 2073 697a  equency grid siz
+0000cb60: 6527 290a 0a20 2020 2020 2020 2069 6620  e')..        if 
+0000cb70: 286c 656e 2864 6174 612e 6672 6571 7565  (len(data.freque
+0000cb80: 6e63 7929 2c64 6174 612e 4e67 7269 6429  ncy),data.Ngrid)
+0000cb90: 3d3d 6864 756c 5b33 5d2e 6461 7461 2e54  ==hdul[3].data.T
+0000cba0: 2e73 6861 7065 3a0a 2020 2020 2020 2020  .shape:.        
+0000cbb0: 2020 2020 6461 7461 2e73 6f75 7263 655f      data.source_
+0000cbc0: 6675 6e63 7469 6f6e 5f67 6173 3d68 6475  function_gas=hdu
+0000cbd0: 6c5b 335d 2e64 6174 610a 2020 2020 2020  l[3].data.      
+0000cbe0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000cbf0: 2020 2020 7261 6973 6520 4173 7365 7274      raise Assert
+0000cc00: 696f 6e45 7272 6f72 2827 4761 7320 736f  ionError('Gas so
+0000cc10: 7572 6365 2066 756e 6374 696f 6e20 6772  urce function gr
+0000cc20: 6964 2069 6e20 6f75 7470 7574 2066 696c  id in output fil
+0000cc30: 6520 646f 6573 206e 6f74 206d 6174 6368  e does not match
+0000cc40: 2074 6865 2073 7061 7469 616c 2061 6e64   the spatial and
+0000cc50: 2066 7265 7175 656e 6379 2067 7269 6420   frequency grid 
+0000cc60: 7369 7a65 2729 0a0a 2020 2020 2020 2020  size')..        
+0000cc70: 6966 2028 6c65 6e28 6461 7461 2e66 7265  if (len(data.fre
+0000cc80: 7175 656e 6379 292c 6461 7461 2e4e 6772  quency),data.Ngr
+0000cc90: 6964 293d 3d68 6475 6c5b 345d 2e64 6174  id)==hdul[4].dat
+0000cca0: 612e 542e 7368 6170 653a 0a20 2020 2020  a.T.shape:.     
+0000ccb0: 2020 2020 2020 2064 6174 612e 7461 755f         data.tau_
+0000ccc0: 6475 7374 3d68 6475 6c5b 345d 2e64 6174  dust=hdul[4].dat
+0000ccd0: 610a 2020 2020 2020 2020 656c 7365 3a0a  a.        else:.
+0000cce0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+0000ccf0: 6520 4173 7365 7274 696f 6e45 7272 6f72  e AssertionError
+0000cd00: 2827 4475 7374 206f 7074 6963 616c 2064  ('Dust optical d
+0000cd10: 6570 7468 2067 7269 6420 696e 206f 7574  epth grid in out
+0000cd20: 7075 7420 6669 6c65 2064 6f65 7320 6e6f  put file does no
+0000cd30: 7420 6d61 7463 6820 7468 6520 7370 6174  t match the spat
+0000cd40: 6961 6c20 616e 6420 6672 6571 7565 6e63  ial and frequenc
+0000cd50: 7920 6772 6964 2073 697a 6527 290a 0a20  y grid size').. 
+0000cd60: 2020 2020 2020 2069 6620 286c 656e 2864         if (len(d
+0000cd70: 6174 612e 6672 6571 7565 6e63 7929 2c64  ata.frequency),d
+0000cd80: 6174 612e 4e67 7269 6429 3d3d 6864 756c  ata.Ngrid)==hdul
+0000cd90: 5b35 5d2e 6461 7461 2e54 2e73 6861 7065  [5].data.T.shape
+0000cda0: 3a0a 2020 2020 2020 2020 2020 2020 6461  :.            da
+0000cdb0: 7461 2e74 6175 5f67 6173 3d68 6475 6c5b  ta.tau_gas=hdul[
+0000cdc0: 355d 2e64 6174 610a 2020 2020 2020 2020  5].data.        
+0000cdd0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000cde0: 2020 7261 6973 6520 4173 7365 7274 696f    raise Assertio
+0000cdf0: 6e45 7272 6f72 2827 4761 7320 6f70 7469  nError('Gas opti
+0000ce00: 6361 6c20 6465 7074 6820 6772 6964 2069  cal depth grid i
+0000ce10: 6e20 6f75 7470 7574 2066 696c 6520 646f  n output file do
+0000ce20: 6573 206e 6f74 206d 6174 6368 2074 6865  es not match the
+0000ce30: 2073 7061 7469 616c 2061 6e64 2066 7265   spatial and fre
+0000ce40: 7175 656e 6379 2067 7269 6420 7369 7a65  quency grid size
+0000ce50: 2729 0a20 2020 2065 6c73 653a 0a20 2020  ').    else:.   
+0000ce60: 2020 2020 2064 6174 615f 7265 6164 3d6e       data_read=n
+0000ce70: 702e 6c6f 6164 7478 7428 6d6f 6465 6c5f  p.loadtxt(model_
+0000ce80: 7061 7468 2c73 6b69 7072 6f77 733d 3129  path,skiprows=1)
+0000ce90: 0a20 2020 2020 2020 2064 6174 613d 736c  .        data=sl
+0000cea0: 6162 3144 2829 0a20 2020 2020 2020 2064  ab1D().        d
+0000ceb0: 6174 612e 6469 7265 6374 6f72 793d 6d6f  ata.directory=mo
+0000cec0: 6465 6c5f 7061 7468 0a20 2020 2020 2020  del_path.       
+0000ced0: 2064 6174 612e 666c 7578 3d64 6174 615f   data.flux=data_
+0000cee0: 7265 6164 5b3a 2c31 5d0a 2020 2020 2020  read[:,1].      
+0000cef0: 2020 6461 7461 2e66 7265 7175 656e 6379    data.frequency
+0000cf00: 3d64 6174 615f 7265 6164 5b3a 2c30 5d0a  =data_read[:,0].
+0000cf10: 2020 2020 7265 7475 726e 2864 6174 6129      return(data)
+0000cf20: 0a0a 0a64 6566 2072 6561 645f 736c 6162  ...def read_slab
+0000cf30: 286d 6f64 656c 5f70 6174 683d 2753 6c61  (model_path='Sla
+0000cf40: 6252 6573 756c 7473 2e6f 7574 272c 7665  bResults.out',ve
+0000cf50: 7262 6f73 653d 5472 7565 2c73 686f 7274  rbose=True,short
+0000cf60: 5f66 6f72 6d61 743d 4661 6c73 652c 6f76  _format=False,ov
+0000cf70: 6572 6c61 705f 6d6f 6465 6c3d 4661 6c73  erlap_model=Fals
+0000cf80: 6529 3a0a 2020 2020 2222 220a 2020 2020  e):.    """.    
+0000cf90: 4675 6e63 7469 6f6e 2074 6f20 7265 6164  Function to read
+0000cfa0: 2073 6c61 6220 6d6f 6465 6c20 6f75 7470   slab model outp
+0000cfb0: 7574 0a20 2020 2022 2222 0a20 2020 2069  ut.    """.    i
+0000cfc0: 6620 6973 696e 7374 616e 6365 286d 6f64  f isinstance(mod
+0000cfd0: 656c 5f70 6174 682c 6c69 7374 293a 0a20  el_path,list):. 
+0000cfe0: 2020 2020 2020 2064 6174 613d 736c 6162         data=slab
+0000cff0: 5f64 6174 6128 290a 2020 2020 2020 2020  _data().        
+0000d000: 6461 7461 2e64 6972 6563 746f 7279 3d6d  data.directory=m
+0000d010: 6f64 656c 5f70 6174 680a 2020 2020 2020  odel_path.      
+0000d020: 2020 666f 7220 6920 696e 206d 6f64 656c    for i in model
+0000d030: 5f70 6174 683a 0a20 2020 2020 2020 2020  _path:.         
+0000d040: 2020 2072 6461 7461 3d72 6561 645f 736c     rdata=read_sl
+0000d050: 6162 2869 2c76 6572 626f 7365 3d76 6572  ab(i,verbose=ver
+0000d060: 626f 7365 2c73 686f 7274 5f66 6f72 6d61  bose,short_forma
+0000d070: 743d 7368 6f72 745f 666f 726d 6174 290a  t=short_format).
+0000d080: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000d090: 6a20 696e 2072 616e 6765 2872 6461 7461  j in range(rdata
+0000d0a0: 2e6e 6d6f 6465 6c73 293a 0a20 2020 2020  .nmodels):.     
+0000d0b0: 2020 2020 2020 2020 2020 2064 6174 612e             data.
+0000d0c0: 6164 645f 6d6f 6465 6c28 7264 6174 612e  add_model(rdata.
+0000d0d0: 6d6f 6465 6c73 5b6a 5d29 0a20 2020 2020  models[j]).     
+0000d0e0: 2020 2072 6574 7572 6e28 6461 7461 290a     return(data).
+0000d0f0: 2020 2020 0a20 2020 2069 6620 6f76 6572      .    if over
+0000d100: 6c61 705f 6d6f 6465 6c3a 2072 6574 7572  lap_model: retur
+0000d110: 6e28 7265 6164 5f6f 7665 726c 6170 5f73  n(read_overlap_s
+0000d120: 7065 6374 7261 2870 6174 683d 6d6f 6465  pectra(path=mode
+0000d130: 6c5f 7061 7468 2c76 6572 626f 7365 3d76  l_path,verbose=v
+0000d140: 6572 626f 7365 2929 0a20 2020 200a 2020  erbose)).    .  
+0000d150: 2020 6966 2076 6572 626f 7365 3a20 7072    if verbose: pr
+0000d160: 696e 7428 2252 6561 6469 6e67 2073 6c61  int("Reading sla
+0000d170: 6220 6d6f 6465 6c20 6f75 7470 7574 2066  b model output f
+0000d180: 726f 6d3a 2022 2c6d 6f64 656c 5f70 6174  rom: ",model_pat
+0000d190: 6829 0a20 2020 2066 3d6f 7065 6e28 6d6f  h).    f=open(mo
+0000d1a0: 6465 6c5f 7061 7468 290a 2020 2020 6461  del_path).    da
+0000d1b0: 7461 3d73 6c61 625f 6461 7461 2829 0a20  ta=slab_data(). 
+0000d1c0: 2020 206e 6d6f 6465 6c73 3d69 6e74 2866     nmodels=int(f
+0000d1d0: 2e72 6561 646c 696e 6528 292e 7370 6c69  .readline().spli
+0000d1e0: 7428 295b 305d 290a 2020 2020 6461 7461  t()[0]).    data
+0000d1f0: 2e64 6972 6563 746f 7279 3d6d 6f64 656c  .directory=model
+0000d200: 5f70 6174 680a 2020 2020 666f 7220 6920  _path.    for i 
+0000d210: 696e 2072 616e 6765 286e 6d6f 6465 6c73  in range(nmodels
+0000d220: 293a 0a23 2020 2020 2020 2020 2074 656d  ):.#         tem
+0000d230: 706f 2020 2020 2020 2020 2020 2020 2020  po              
+0000d240: 2020 3d20 2020 736c 6162 2829 0a20 2020    =   slab().   
+0000d250: 2020 2020 2074 656d 706f 5f6d 6f64 656c       tempo_model
+0000d260: 5f6e 756d 6265 723d 696e 7428 662e 7265  _number=int(f.re
+0000d270: 6164 6c69 6e65 2829 2e73 706c 6974 2829  adline().split()
+0000d280: 5b30 5d29 0a20 2020 2020 2020 206e 7370  [0]).        nsp
+0000d290: 6563 6965 733d 696e 7428 662e 7265 6164  ecies=int(f.read
+0000d2a0: 6c69 6e65 2829 2e73 706c 6974 2829 5b30  line().split()[0
+0000d2b0: 5d29 0a23 2020 2020 2020 2020 2074 656d  ]).#         tem
+0000d2c0: 706f 2e73 7065 6369 6573 5f6e 756d 6265  po.species_numbe
+0000d2d0: 7220 3d20 2020 696e 7428 662e 7265 6164  r =   int(f.read
+0000d2e0: 6c69 6e65 2829 2e73 706c 6974 2829 5b30  line().split()[0
+0000d2f0: 5d29 0a20 2020 2020 2020 2074 656d 706f  ]).        tempo
+0000d300: 5f6e 4874 6f74 3d66 6c6f 6174 2866 2e72  _nHtot=float(f.r
+0000d310: 6561 646c 696e 6528 292e 7370 6c69 7428  eadline().split(
+0000d320: 295b 305d 290a 2020 2020 2020 2020 7465  )[0]).        te
+0000d330: 6d70 6f5f 6761 7344 656e 733d 666c 6f61  mpo_gasDens=floa
+0000d340: 7428 662e 7265 6164 6c69 6e65 2829 2e73  t(f.readline().s
+0000d350: 706c 6974 2829 5b30 5d29 0a20 2020 2020  plit()[0]).     
+0000d360: 2020 2074 656d 706f 5f6e 656c 6563 3d66     tempo_nelec=f
+0000d370: 6c6f 6174 2866 2e72 6561 646c 696e 6528  loat(f.readline(
+0000d380: 292e 7370 6c69 7428 295b 305d 290a 2020  ).split()[0]).  
+0000d390: 2020 2020 2020 7465 6d70 6f5f 6e48 653d        tempo_nHe=
+0000d3a0: 666c 6f61 7428 662e 7265 6164 6c69 6e65  float(f.readline
+0000d3b0: 2829 2e73 706c 6974 2829 5b30 5d29 0a20  ().split()[0]). 
+0000d3c0: 2020 2020 2020 2074 656d 706f 5f6e 4849         tempo_nHI
+0000d3d0: 493d 666c 6f61 7428 662e 7265 6164 6c69  I=float(f.readli
+0000d3e0: 6e65 2829 2e73 706c 6974 2829 5b30 5d29  ne().split()[0])
+0000d3f0: 0a20 2020 2020 2020 2074 656d 706f 5f6e  .        tempo_n
+0000d400: 4849 3d66 6c6f 6174 2866 2e72 6561 646c  HI=float(f.readl
+0000d410: 696e 6528 292e 7370 6c69 7428 295b 305d  ine().split()[0]
+0000d420: 290a 2020 2020 2020 2020 7465 6d70 6f5f  ).        tempo_
+0000d430: 6e48 323d 666c 6f61 7428 662e 7265 6164  nH2=float(f.read
+0000d440: 6c69 6e65 2829 2e73 706c 6974 2829 5b30  line().split()[0
+0000d450: 5d29 0a20 2020 2020 2020 2074 656d 706f  ]).        tempo
+0000d460: 5f64 7573 745f 746f 5f67 6173 3d66 6c6f  _dust_to_gas=flo
+0000d470: 6174 2866 2e72 6561 646c 696e 6528 292e  at(f.readline().
+0000d480: 7370 6c69 7428 295b 305d 290a 2020 2020  split()[0]).    
+0000d490: 2020 2020 7465 6d70 6f5f 7674 7572 623d      tempo_vturb=
+0000d4a0: 666c 6f61 7428 662e 7265 6164 6c69 6e65  float(f.readline
+0000d4b0: 2829 2e73 706c 6974 2829 5b30 5d29 0a20  ().split()[0]). 
+0000d4c0: 2020 2020 2020 2074 656d 706f 5f54 673d         tempo_Tg=
+0000d4d0: 666c 6f61 7428 662e 7265 6164 6c69 6e65  float(f.readline
+0000d4e0: 2829 2e73 706c 6974 2829 5b30 5d29 0a20  ().split()[0]). 
+0000d4f0: 2020 2020 2020 2074 656d 706f 5f54 643d         tempo_Td=
+0000d500: 666c 6f61 7428 662e 7265 6164 6c69 6e65  float(f.readline
+0000d510: 2829 2e73 706c 6974 2829 5b30 5d29 0a20  ().split()[0]). 
+0000d520: 2020 2020 2020 2069 6620 7368 6f72 745f         if short_
+0000d530: 666f 726d 6174 3a0a 2020 2020 2020 2020  format:.        
+0000d540: 2020 2020 666f 7220 6a20 696e 2072 616e      for j in ran
+0000d550: 6765 286e 7370 6563 6965 7329 3a0a 2020  ge(nspecies):.  
+0000d560: 2020 2020 2020 2020 2020 2020 2020 7465                te
+0000d570: 6d70 6f3d 736c 6162 2829 0a20 2020 2020  mpo=slab().     
+0000d580: 2020 2020 2020 2020 2020 2074 656d 706f             tempo
+0000d590: 2e6d 6f64 656c 5f6e 756d 6265 723d 7465  .model_number=te
+0000d5a0: 6d70 6f5f 6d6f 6465 6c5f 6e75 6d62 6572  mpo_model_number
+0000d5b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d5c0: 2074 656d 706f 2e4e 483d 7465 6d70 6f5f   tempo.NH=tempo_
+0000d5d0: 6e48 746f 740a 2020 2020 2020 2020 2020  nHtot.          
+0000d5e0: 2020 2020 2020 7465 6d70 6f2e 6e43 6f6c        tempo.nCol
+0000d5f0: 6c3d 7465 6d70 6f5f 6761 7344 656e 730a  l=tempo_gasDens.
+0000d600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d610: 7465 6d70 6f2e 6e65 3d74 656d 706f 5f6e  tempo.ne=tempo_n
+0000d620: 656c 6563 0a20 2020 2020 2020 2020 2020  elec.           
+0000d630: 2020 2020 2074 656d 706f 2e6e 4865 3d74       tempo.nHe=t
+0000d640: 656d 706f 5f6e 4865 0a20 2020 2020 2020  empo_nHe.       
+0000d650: 2020 2020 2020 2020 2074 656d 706f 2e6e           tempo.n
+0000d660: 4849 493d 7465 6d70 6f5f 6e48 4949 0a20  HII=tempo_nHII. 
+0000d670: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000d680: 656d 706f 2e6e 4849 3d74 656d 706f 5f6e  empo.nHI=tempo_n
+0000d690: 4849 0a20 2020 2020 2020 2020 2020 2020  HI.             
+0000d6a0: 2020 2074 656d 706f 2e6e 4832 3d74 656d     tempo.nH2=tem
+0000d6b0: 706f 5f6e 4832 0a20 2020 2020 2020 2020  po_nH2.         
+0000d6c0: 2020 2020 2020 2074 656d 706f 2e64 7573         tempo.dus
+0000d6d0: 745f 746f 5f67 6173 3d74 656d 706f 5f64  t_to_gas=tempo_d
+0000d6e0: 7573 745f 746f 5f67 6173 0a20 2020 2020  ust_to_gas.     
+0000d6f0: 2020 2020 2020 2020 2020 2074 656d 706f             tempo
+0000d700: 2e76 7475 7262 3d74 656d 706f 5f76 7475  .vturb=tempo_vtu
+0000d710: 7262 0a20 2020 2020 2020 2020 2020 2020  rb.             
+0000d720: 2020 2074 656d 706f 2e54 673d 7465 6d70     tempo.Tg=temp
+0000d730: 6f5f 5467 0a20 2020 2020 2020 2020 2020  o_Tg.           
+0000d740: 2020 2020 2074 656d 706f 2e54 643d 7465       tempo.Td=te
+0000d750: 6d70 6f5f 5464 0a0a 2020 2020 2020 2020  mpo_Td..        
+0000d760: 2020 2020 2020 2020 7465 6d70 6f2e 7370          tempo.sp
+0000d770: 6563 6965 735f 696e 6465 783d 696e 7428  ecies_index=int(
+0000d780: 662e 7265 6164 6c69 6e65 2829 2e73 706c  f.readline().spl
+0000d790: 6974 2829 5b30 5d29 0a20 2020 2020 2020  it()[0]).       
+0000d7a0: 2020 2020 2020 2020 2074 656d 706f 2e73           tempo.s
+0000d7b0: 7065 6369 6573 5f6e 756d 6265 723d 6a2b  pecies_number=j+
+0000d7c0: 310a 2020 2020 2020 2020 2020 2020 2020  1.              
+0000d7d0: 2020 7465 6d70 6f2e 7370 6563 6965 735f    tempo.species_
+0000d7e0: 6e61 6d65 3d66 2e72 6561 646c 696e 6528  name=f.readline(
+0000d7f0: 292e 7370 6c69 7428 295b 305d 0a20 2020  ).split()[0].   
+0000d800: 2020 2020 2020 2020 2020 2020 2074 656d               tem
+0000d810: 706f 2e61 6275 6e64 616e 6365 3d66 6c6f  po.abundance=flo
+0000d820: 6174 2866 2e72 6561 646c 696e 6528 292e  at(f.readline().
+0000d830: 7370 6c69 7428 295b 305d 290a 2020 2020  split()[0]).    
+0000d840: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
+0000d850: 6f2e 6476 3d66 6c6f 6174 2866 2e72 6561  o.dv=float(f.rea
+0000d860: 646c 696e 6528 292e 7370 6c69 7428 295b  dline().split()[
+0000d870: 305d 290a 2020 2020 2020 2020 2020 2020  0]).            
+0000d880: 2020 2020 7465 6d70 6f2e 6e6c 696e 6573      tempo.nlines
+0000d890: 3d69 6e74 2866 2e72 6561 646c 696e 6528  =int(f.readline(
+0000d8a0: 292e 7370 6c69 7428 295b 305d 290a 2020  ).split()[0]).  
+0000d8b0: 2020 2020 2020 2020 2020 2020 2020 6c69                li
+0000d8c0: 6e65 733d 662e 7265 6164 6c69 6e65 2829  nes=f.readline()
+0000d8d0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000d8e0: 2020 2320 7465 6d70 6f2e 6e6c 696e 6573    # tempo.nlines
+0000d8f0: 3d4e 6f6e 650a 2020 2020 2020 2020 2020  =None.          
+0000d900: 2020 2020 2020 7465 6d70 6f2e 6c69 6e65        tempo.line
+0000d910: 6461 7461 3d4e 6f6e 650a 2020 2020 2020  data=None.      
+0000d920: 2020 2020 2020 2020 2020 7465 6d70 6f2e            tempo.
+0000d930: 6c65 7665 6c64 6174 613d 4e6f 6e65 0a20  leveldata=None. 
+0000d940: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000d950: 656d 706f 2e63 6f6e 7657 6176 656c 656e  empo.convWavelen
+0000d960: 6774 683d 4e6f 6e65 0a20 2020 2020 2020  gth=None.       
+0000d970: 2020 2020 2020 2020 2074 656d 706f 2e63           tempo.c
+0000d980: 6f6e 764c 5445 666c 7578 3d4e 6f6e 650a  onvLTEflux=None.
+0000d990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d9a0: 7465 6d70 6f2e 636f 6e76 4e4c 5445 666c  tempo.convNLTEfl
+0000d9b0: 7578 3d4e 6f6e 650a 2020 2020 2020 2020  ux=None.        
+0000d9c0: 2020 2020 2020 2020 7465 6d70 6f2e 636f          tempo.co
+0000d9d0: 6e76 5479 7065 3d4e 6f6e 650a 2020 2020  nvType=None.    
+0000d9e0: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
+0000d9f0: 6f2e 636f 6e76 523d 4e6f 6e65 0a0a 2020  o.convR=None..  
+0000da00: 2020 2020 2020 2020 2020 2020 2020 6461                da
+0000da10: 743d 5b5d 0a20 2020 2020 2020 2020 2020  t=[].           
+0000da20: 2020 2020 2023 2066 6f72 206b 2069 6e20       # for k in 
+0000da30: 7261 6e67 6528 7465 6d70 6f2e 6e6c 6576  range(tempo.nlev
+0000da40: 656c 7329 3a0a 2020 2020 2020 2020 2020  els):.          
+0000da50: 2020 2020 2020 2320 2020 2020 6461 745b        #     dat[
+0000da60: 305d 5b6b 2c3a 5d3d 6e70 2e61 7361 7272  0][k,:]=np.asarr
+0000da70: 6179 285b 666c 6f61 7428 7829 2066 6f72  ay([float(x) for
+0000da80: 2078 2069 6e20 662e 7265 6164 6c69 6e65   x in f.readline
+0000da90: 2829 2e73 706c 6974 2829 5d29 0a0a 2020  ().split()])..  
+0000daa0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0000dab0: 6c69 6e65 733d 662e 7265 6164 6c69 6e65  lines=f.readline
+0000dac0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+0000dad0: 2020 2023 206c 696e 6573 3d66 2e72 6561     # lines=f.rea
+0000dae0: 646c 696e 6528 290a 2020 2020 2020 2020  dline().        
+0000daf0: 2020 2020 2020 2020 6461 743d 6e70 2e7a          dat=np.z
+0000db00: 6572 6f73 2828 7465 6d70 6f2e 6e6c 696e  eros((tempo.nlin
+0000db10: 6573 2c34 2929 0a20 2020 2020 2020 2020  es,4)).         
+0000db20: 2020 2020 2020 2073 6c61 624f 7574 466f         slabOutFo
+0000db30: 726d 6174 3d5b 382c 3134 2c31 352c 3135  rmat=[8,14,15,15
+0000db40: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+0000db50: 2020 666f 7220 6b20 696e 2072 616e 6765    for k in range
+0000db60: 2874 656d 706f 2e6e 6c69 6e65 7329 3a0a  (tempo.nlines):.
+0000db70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db80: 2020 2020 6c69 6e65 5265 6164 3d5b 5d0a      lineRead=[].
+0000db90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dba0: 2020 2020 6c69 6e65 733d 662e 7265 6164      lines=f.read
+0000dbb0: 6c69 6e65 2829 0a20 2020 2020 2020 2020  line().         
+0000dbc0: 2020 2020 2020 2020 2020 206c 3d30 0a20             l=0. 
+0000dbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dbe0: 2020 2066 6f72 206c 656e 6774 6820 696e     for length in
+0000dbf0: 2073 6c61 624f 7574 466f 726d 6174 3a0a   slabOutFormat:.
+0000dc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc10: 2020 2020 2020 2020 6c69 6e65 5265 6164          lineRead
+0000dc20: 2e61 7070 656e 6428 6c69 6e65 735b 6c3a  .append(lines[l:
+0000dc30: 6c2b 6c65 6e67 7468 5d29 0a20 2020 2020  l+length]).     
+0000dc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc50: 2020 206c 2b3d 6c65 6e67 7468 0a20 2020     l+=length.   
+0000dc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc70: 2064 6174 5b6b 2c3a 5d3d 6e70 2e61 7361   dat[k,:]=np.asa
+0000dc80: 7272 6179 285b 666c 6f61 7428 7829 2066  rray([float(x) f
+0000dc90: 6f72 2078 2069 6e20 6c69 6e65 5265 6164  or x in lineRead
+0000dca0: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
+0000dcb0: 2020 206c 696e 6544 6174 613d 7064 2e44     lineData=pd.D
+0000dcc0: 6174 6146 7261 6d65 2864 6174 2c63 6f6c  ataFrame(dat,col
+0000dcd0: 756d 6e73 3d5b 2769 272c 2747 487a 272c  umns=['i','GHz',
+0000dce0: 2746 4e4c 5445 272c 2746 4c54 4527 5d29  'FNLTE','FLTE'])
+0000dcf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dd00: 2074 656d 706f 2e6c 696e 6564 6174 613d   tempo.linedata=
+0000dd10: 6c69 6e65 4461 7461 0a20 2020 2020 2020  lineData.       
+0000dd20: 2020 2020 2020 2020 2064 6174 612e 6164           data.ad
+0000dd30: 645f 6d6f 6465 6c28 7465 6d70 6f29 0a20  d_model(tempo). 
+0000dd40: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0000dd50: 2020 2020 2020 2020 2066 6f72 206a 2069           for j i
+0000dd60: 6e20 7261 6e67 6528 6e73 7065 6369 6573  n range(nspecies
+0000dd70: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000dd80: 2020 2074 656d 706f 3d73 6c61 6228 290a     tempo=slab().
+0000dd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dda0: 7465 6d70 6f2e 6d6f 6465 6c5f 6e75 6d62  tempo.model_numb
+0000ddb0: 6572 3d74 656d 706f 5f6d 6f64 656c 5f6e  er=tempo_model_n
+0000ddc0: 756d 6265 720a 2020 2020 2020 2020 2020  umber.          
+0000ddd0: 2020 2020 2020 7465 6d70 6f2e 4e48 3d74        tempo.NH=t
+0000dde0: 656d 706f 5f6e 4874 6f74 0a20 2020 2020  empo_nHtot.     
+0000ddf0: 2020 2020 2020 2020 2020 2074 656d 706f             tempo
+0000de00: 2e6e 436f 6c6c 3d74 656d 706f 5f67 6173  .nColl=tempo_gas
+0000de10: 4465 6e73 0a20 2020 2020 2020 2020 2020  Dens.           
+0000de20: 2020 2020 2074 656d 706f 2e6e 653d 7465       tempo.ne=te
+0000de30: 6d70 6f5f 6e65 6c65 630a 2020 2020 2020  mpo_nelec.      
+0000de40: 2020 2020 2020 2020 2020 7465 6d70 6f2e            tempo.
+0000de50: 6e48 653d 7465 6d70 6f5f 6e48 650a 2020  nHe=tempo_nHe.  
+0000de60: 2020 2020 2020 2020 2020 2020 2020 7465                te
+0000de70: 6d70 6f2e 6e48 4949 3d74 656d 706f 5f6e  mpo.nHII=tempo_n
+0000de80: 4849 490a 2020 2020 2020 2020 2020 2020  HII.            
+0000de90: 2020 2020 7465 6d70 6f2e 6e48 493d 7465      tempo.nHI=te
+0000dea0: 6d70 6f5f 6e48 490a 2020 2020 2020 2020  mpo_nHI.        
+0000deb0: 2020 2020 2020 2020 7465 6d70 6f2e 6e48          tempo.nH
+0000dec0: 323d 7465 6d70 6f5f 6e48 320a 2020 2020  2=tempo_nH2.    
+0000ded0: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
+0000dee0: 6f2e 6475 7374 5f74 6f5f 6761 733d 7465  o.dust_to_gas=te
+0000def0: 6d70 6f5f 6475 7374 5f74 6f5f 6761 730a  mpo_dust_to_gas.
+0000df00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000df10: 7465 6d70 6f2e 7674 7572 623d 7465 6d70  tempo.vturb=temp
+0000df20: 6f5f 7674 7572 620a 2020 2020 2020 2020  o_vturb.        
+0000df30: 2020 2020 2020 2020 7465 6d70 6f2e 5467          tempo.Tg
+0000df40: 3d74 656d 706f 5f54 670a 2020 2020 2020  =tempo_Tg.      
+0000df50: 2020 2020 2020 2020 2020 7465 6d70 6f2e            tempo.
+0000df60: 5464 3d74 656d 706f 5f54 640a 0a20 2020  Td=tempo_Td..   
+0000df70: 2020 2020 2020 2020 2020 2020 2074 656d               tem
+0000df80: 706f 2e73 7065 6369 6573 5f69 6e64 6578  po.species_index
+0000df90: 3d69 6e74 2866 2e72 6561 646c 696e 6528  =int(f.readline(
+0000dfa0: 292e 7370 6c69 7428 295b 305d 290a 2020  ).split()[0]).  
+0000dfb0: 2020 2020 2020 2020 2020 2020 2020 7465                te
+0000dfc0: 6d70 6f2e 7370 6563 6965 735f 6e75 6d62  mpo.species_numb
+0000dfd0: 6572 3d6a 2b31 0a20 2020 2020 2020 2020  er=j+1.         
+0000dfe0: 2020 2020 2020 2074 656d 706f 2e73 7065         tempo.spe
+0000dff0: 6369 6573 5f6e 616d 653d 662e 7265 6164  cies_name=f.read
+0000e000: 6c69 6e65 2829 2e73 706c 6974 2829 5b30  line().split()[0
+0000e010: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+0000e020: 2020 7465 6d70 6f2e 6162 756e 6461 6e63    tempo.abundanc
+0000e030: 653d 666c 6f61 7428 662e 7265 6164 6c69  e=float(f.readli
+0000e040: 6e65 2829 2e73 706c 6974 2829 5b30 5d29  ne().split()[0])
+0000e050: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e060: 2074 656d 706f 2e64 763d 666c 6f61 7428   tempo.dv=float(
+0000e070: 662e 7265 6164 6c69 6e65 2829 2e73 706c  f.readline().spl
+0000e080: 6974 2829 5b30 5d29 0a20 2020 2020 2020  it()[0]).       
+0000e090: 2020 2020 2020 2020 2074 656d 706f 2e6e           tempo.n
+0000e0a0: 6c65 7665 6c73 3d69 6e74 2866 2e72 6561  levels=int(f.rea
+0000e0b0: 646c 696e 6528 292e 7370 6c69 7428 295b  dline().split()[
+0000e0c0: 305d 290a 2020 2020 2020 2020 2020 2020  0]).            
+0000e0d0: 2020 2020 6c69 6e65 733d 662e 7265 6164      lines=f.read
+0000e0e0: 6c69 6e65 2829 0a0a 2020 2020 2020 2020  line()..        
+0000e0f0: 2020 2020 2020 2020 7465 6d70 6f2e 6e6c          tempo.nl
+0000e100: 696e 6573 3d4e 6f6e 650a 2020 2020 2020  ines=None.      
+0000e110: 2020 2020 2020 2020 2020 7465 6d70 6f2e            tempo.
+0000e120: 6c69 6e65 6461 7461 3d4e 6f6e 650a 2020  linedata=None.  
+0000e130: 2020 2020 2020 2020 2020 2020 2020 7465                te
+0000e140: 6d70 6f2e 6c65 7665 6c64 6174 613d 4e6f  mpo.leveldata=No
+0000e150: 6e65 0a20 2020 2020 2020 2020 2020 2020  ne.             
+0000e160: 2020 2074 656d 706f 2e63 6f6e 7657 6176     tempo.convWav
+0000e170: 656c 656e 6774 683d 4e6f 6e65 0a20 2020  elength=None.   
+0000e180: 2020 2020 2020 2020 2020 2020 2074 656d               tem
+0000e190: 706f 2e63 6f6e 764c 5445 666c 7578 3d4e  po.convLTEflux=N
+0000e1a0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+0000e1b0: 2020 2020 7465 6d70 6f2e 636f 6e76 4e4c      tempo.convNL
+0000e1c0: 5445 666c 7578 3d4e 6f6e 650a 2020 2020  TEflux=None.    
+0000e1d0: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
+0000e1e0: 6f2e 636f 6e76 5479 7065 3d4e 6f6e 650a  o.convType=None.
+0000e1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e200: 7465 6d70 6f2e 636f 6e76 523d 4e6f 6e65  tempo.convR=None
+0000e210: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000e220: 2020 6461 743d 5b6e 702e 7a65 726f 7328    dat=[np.zeros(
+0000e230: 2874 656d 706f 2e6e 6c65 7665 6c73 2c38  (tempo.nlevels,8
+0000e240: 2929 2c5b 5d2c 5b5d 5d0a 2020 2020 2020  )),[],[]].      
+0000e250: 2020 2020 2020 2020 2020 666f 7220 6b20            for k 
+0000e260: 696e 2072 616e 6765 2874 656d 706f 2e6e  in range(tempo.n
+0000e270: 6c65 7665 6c73 293a 0a20 2020 2020 2020  levels):.       
+0000e280: 2020 2020 2020 2020 2020 2020 2064 6174               dat
+0000e290: 5b30 5d5b 6b2c 3a5d 3d6e 702e 6173 6172  [0][k,:]=np.asar
+0000e2a0: 7261 7928 5b66 6c6f 6174 2878 2920 666f  ray([float(x) fo
+0000e2b0: 7220 7820 696e 2066 2e72 6561 646c 696e  r x in f.readlin
+0000e2c0: 6528 292e 7370 6c69 7428 295d 290a 2020  e().split()]).  
+0000e2d0: 2020 2020 2020 2020 2020 2020 2020 7465                te
+0000e2e0: 6d70 6f2e 6e6c 696e 6573 3d69 6e74 2866  mpo.nlines=int(f
+0000e2f0: 2e72 6561 646c 696e 6528 292e 7370 6c69  .readline().spli
+0000e300: 7428 295b 305d 290a 2020 2020 2020 2020  t()[0]).        
+0000e310: 2020 2020 2020 2020 6c69 6e65 733d 662e          lines=f.
+0000e320: 7265 6164 6c69 6e65 2829 0a20 2020 2020  readline().     
+0000e330: 2020 2020 2020 2020 2020 206c 696e 6573             lines
+0000e340: 3d66 2e72 6561 646c 696e 6528 290a 2020  =f.readline().  
+0000e350: 2020 2020 2020 2020 2020 2020 2020 6461                da
+0000e360: 745b 315d 3d6e 702e 7a65 726f 7328 2874  t[1]=np.zeros((t
+0000e370: 656d 706f 2e6e 6c69 6e65 732c 3233 2929  empo.nlines,23))
+0000e380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e390: 2073 6c61 624f 7574 466f 726d 6174 3d5b   slabOutFormat=[
+0000e3a0: 392c 392c 392c 352c 352c 352c 3135 2c31  9,9,9,5,5,5,15,1
+0000e3b0: 352c 3135 2c31 352c 3135 2c31 352c 3135  5,15,15,15,15,15
+0000e3c0: 2c31 352c 3135 2c31 352c 3135 2c31 352c  ,15,15,15,15,15,
+0000e3d0: 3135 2c31 352c 3135 2c31 352c 3135 2c32  15,15,15,15,15,2
+0000e3e0: 312c 3231 2c32 312c 3231 5d0a 2020 2020  1,21,21,21].    
+0000e3f0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000e400: 6b20 696e 2072 616e 6765 2874 656d 706f  k in range(tempo
+0000e410: 2e6e 6c69 6e65 7329 3a0a 2020 2020 2020  .nlines):.      
+0000e420: 2020 2020 2020 2020 2020 2020 2020 6c69                li
+0000e430: 6e65 5265 6164 3d5b 5d0a 2020 2020 2020  neRead=[].      
+0000e440: 2020 2020 2020 2020 2020 2020 2020 6c69                li
+0000e450: 6e65 733d 662e 7265 6164 6c69 6e65 2829  nes=f.readline()
+0000e460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e470: 2020 2020 206c 3d30 0a20 2020 2020 2020       l=0.       
+0000e480: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0000e490: 206c 656e 6774 6820 696e 2073 6c61 624f   length in slabO
+0000e4a0: 7574 466f 726d 6174 3a0a 2020 2020 2020  utFormat:.      
+0000e4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e4c0: 2020 6c69 6e65 5265 6164 2e61 7070 656e    lineRead.appen
+0000e4d0: 6428 6c69 6e65 735b 6c3a 6c2b 6c65 6e67  d(lines[l:l+leng
+0000e4e0: 7468 5d29 0a20 2020 2020 2020 2020 2020  th]).           
+0000e4f0: 2020 2020 2020 2020 2020 2020 206c 2b3d               l+=
+0000e500: 6c65 6e67 7468 0a20 2020 2020 2020 2020  length.         
+0000e510: 2020 2020 2020 2020 2020 2064 6174 5b31             dat[1
+0000e520: 5d5b 6b2c 3a5d 3d6e 702e 6173 6172 7261  ][k,:]=np.asarra
+0000e530: 7928 5b66 6c6f 6174 2878 2920 666f 7220  y([float(x) for 
+0000e540: 7820 696e 206c 696e 6552 6561 645b 303a  x in lineRead[0:
+0000e550: 2d34 5d5d 290a 2020 2020 2020 2020 2020  -4]]).          
+0000e560: 2020 2020 2020 2020 2020 6461 745b 325d            dat[2]
+0000e570: 2e61 7070 656e 6428 5b61 2e73 7472 6970  .append([a.strip
+0000e580: 2829 2066 6f72 2061 2069 6e20 6c69 6e65  () for a in line
+0000e590: 5265 6164 5b2d 343a 5d5d 290a 0a20 2020  Read[-4:]])..   
+0000e5a0: 2020 2020 2020 2020 2020 2020 206c 696e               lin
+0000e5b0: 6544 6174 613d 7064 2e44 6174 6146 7261  eData=pd.DataFra
+0000e5c0: 6d65 2864 6174 5b31 5d2c 636f 6c75 6d6e  me(dat[1],column
+0000e5d0: 733d 5b27 6927 2c27 7527 2c27 6c27 2c27  s=['i','u','l','
+0000e5e0: 6527 2c27 7627 2c27 4a27 2c27 6775 272c  e','v','J','gu',
+0000e5f0: 2745 7527 2c27 4127 2c27 4227 2c27 4748  'Eu','A','B','GH
+0000e600: 7a27 2c27 7461 7544 272c 274a 6261 636b  z','tauD','Jback
+0000e610: 272c 2770 6f70 272c 276c 7465 706f 7027  ','pop','ltepop'
+0000e620: 2c27 7461 754e 4c54 4527 2c27 7461 754c  ,'tauNLTE','tauL
+0000e630: 5445 272c 2762 4e4c 5445 272c 2762 4c54  TE','bNLTE','bLT
+0000e640: 4527 2c27 704e 4c54 4527 2c27 704c 5445  E','pNLTE','pLTE
+0000e650: 272c 2746 4e4c 5445 272c 2746 4c54 4527  ','FNLTE','FLTE'
+0000e660: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
+0000e670: 2020 206c 696e 6544 6174 615b 2767 6c6f     lineData['glo
+0000e680: 6261 6c5f 7527 5d3d 5b61 5b30 5d20 666f  bal_u']=[a[0] fo
+0000e690: 7220 6120 696e 2064 6174 5b32 5d5d 0a20  r a in dat[2]]. 
+0000e6a0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+0000e6b0: 696e 6544 6174 615b 2767 6c6f 6261 6c5f  ineData['global_
+0000e6c0: 6c27 5d3d 5b61 5b31 5d20 666f 7220 6120  l']=[a[1] for a 
+0000e6d0: 696e 2064 6174 5b32 5d5d 0a20 2020 2020  in dat[2]].     
+0000e6e0: 2020 2020 2020 2020 2020 206c 696e 6544             lineD
+0000e6f0: 6174 615b 276c 6f63 616c 5f75 275d 3d5b  ata['local_u']=[
+0000e700: 615b 325d 2066 6f72 2061 2069 6e20 6461  a[2] for a in da
+0000e710: 745b 325d 5d0a 2020 2020 2020 2020 2020  t[2]].          
+0000e720: 2020 2020 2020 6c69 6e65 4461 7461 5b27        lineData['
+0000e730: 6c6f 6361 6c5f 6c27 5d3d 5b61 5b33 5d20  local_l']=[a[3] 
+0000e740: 666f 7220 6120 696e 2064 6174 5b32 5d5d  for a in dat[2]]
+0000e750: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e760: 206c 6576 4461 7461 3d70 642e 4461 7461   levData=pd.Data
+0000e770: 4672 616d 6528 6461 745b 305d 2c63 6f6c  Frame(dat[0],col
+0000e780: 756d 6e73 3d5b 2769 272c 2767 272c 2745  umns=['i','g','E
+0000e790: 272c 2770 6f70 272c 276c 7465 706f 7027  ','pop','ltepop'
+0000e7a0: 2c27 6527 2c27 7627 2c27 4a27 5d29 0a20  ,'e','v','J']). 
+0000e7b0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000e7c0: 656d 706f 2e6c 696e 6564 6174 613d 6c69  empo.linedata=li
+0000e7d0: 6e65 4461 7461 0a20 2020 2020 2020 2020  neData.         
+0000e7e0: 2020 2020 2020 2074 656d 706f 2e6c 6576         tempo.lev
+0000e7f0: 656c 6461 7461 3d6c 6576 4461 7461 0a20  eldata=levData. 
+0000e800: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+0000e810: 6174 612e 6164 645f 6d6f 6465 6c28 7465  ata.add_model(te
+0000e820: 6d70 6f29 0a20 2020 2072 6574 7572 6e28  mpo).    return(
+0000e830: 6461 7461 290a 0a0a 6465 6620 7265 6164  data)...def read
+0000e840: 5f6f 7665 726c 6170 5f73 7065 6374 7261  _overlap_spectra
+0000e850: 2870 6174 683d 2753 6c61 624f 7665 726c  (path='SlabOverl
+0000e860: 6170 2e6f 7574 272c 7665 7262 6f73 653d  ap.out',verbose=
+0000e870: 5472 7565 293a 0a20 2020 2022 2222 0a20  True):.    """. 
+0000e880: 2020 2046 756e 6374 696f 6e20 746f 2072     Function to r
+0000e890: 6561 6420 3044 2070 726f 6469 6d6f 2073  ead 0D prodimo s
+0000e8a0: 6c61 6220 6d6f 6465 6c20 6f75 7470 7574  lab model output
+0000e8b0: 2077 6974 6820 6c69 6e65 206f 7665 726c   with line overl
+0000e8c0: 6170 0a20 2020 2022 2222 0a0a 2020 2020  ap.    """..    
+0000e8d0: 6966 2069 7369 6e73 7461 6e63 6528 7061  if isinstance(pa
+0000e8e0: 7468 2c6c 6973 7429 3a0a 2020 2020 2020  th,list):.      
+0000e8f0: 2020 6461 7461 3d73 6c61 625f 6461 7461    data=slab_data
+0000e900: 2829 0a20 2020 2020 2020 2064 6174 612e  ().        data.
+0000e910: 6469 7265 6374 6f72 793d 7061 7468 0a20  directory=path. 
+0000e920: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+0000e930: 7061 7468 3a0a 2020 2020 2020 2020 2020  path:.          
+0000e940: 2020 7264 6174 613d 7265 6164 5f6f 7665    rdata=read_ove
+0000e950: 726c 6170 5f73 7065 6374 7261 2869 2c76  rlap_spectra(i,v
+0000e960: 6572 626f 7365 3d76 6572 626f 7365 290a  erbose=verbose).
+0000e970: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000e980: 6a20 696e 2072 616e 6765 2872 6461 7461  j in range(rdata
+0000e990: 2e6e 6d6f 6465 6c73 293a 0a20 2020 2020  .nmodels):.     
+0000e9a0: 2020 2020 2020 2020 2020 2064 6174 612e             data.
+0000e9b0: 6164 645f 6d6f 6465 6c28 7264 6174 612e  add_model(rdata.
+0000e9c0: 6d6f 6465 6c73 5b6a 5d29 0a20 2020 2020  models[j]).     
+0000e9d0: 2020 2072 6574 7572 6e28 6461 7461 290a     return(data).
+0000e9e0: 0a20 2020 2069 6620 7665 7262 6f73 653a  .    if verbose:
+0000e9f0: 2070 7269 6e74 2822 5265 6164 696e 6720   print("Reading 
+0000ea00: 736c 6162 206c 696e 6520 6f76 6572 6c61  slab line overla
+0000ea10: 7020 6d6f 6465 6c20 6f75 7470 7574 2066  p model output f
+0000ea20: 726f 6d3a 2022 2c70 6174 6829 0a20 2020  rom: ",path).   
+0000ea30: 2069 6620 272e 6669 7473 2e67 7a27 2069   if '.fits.gz' i
+0000ea40: 6e20 7061 7468 3a0a 2020 2020 2020 2020  n path:.        
+0000ea50: 6864 756c 3d66 6974 732e 6f70 656e 2870  hdul=fits.open(p
+0000ea60: 6174 6829 0a20 2020 2020 2020 2064 6174  ath).        dat
+0000ea70: 613d 736c 6162 5f64 6174 6128 290a 2020  a=slab_data().  
+0000ea80: 2020 2020 2020 6e6d 6f64 656c 733d 6864        nmodels=hd
+0000ea90: 756c 5b30 5d2e 6865 6164 6572 5b27 4e4d  ul[0].header['NM
+0000eaa0: 4f44 454c 5327 5d0a 2020 2020 2020 2020  ODELS'].        
+0000eab0: 6461 7461 2e64 6972 6563 746f 7279 3d70  data.directory=p
+0000eac0: 6174 680a 2020 2020 2020 2020 666f 7220  ath.        for 
+0000ead0: 6920 696e 2072 616e 6765 286e 6d6f 6465  i in range(nmode
+0000eae0: 6c73 293a 0a20 2020 2020 2020 2020 2020  ls):.           
+0000eaf0: 2074 656d 706f 3d73 6c61 6228 290a 2020   tempo=slab().  
+0000eb00: 2020 2020 2020 2020 2020 7465 6d70 6f5f            tempo_
+0000eb10: 6d6f 6465 6c5f 6e75 6d62 6572 3d68 6475  model_number=hdu
+0000eb20: 6c5b 692b 315d 2e68 6561 6465 725b 274d  l[i+1].header['M
+0000eb30: 4f44 454c 275d 0a20 2020 2020 2020 2020  ODEL'].         
+0000eb40: 2020 2074 656d 706f 5f4e 6c69 6e65 3d68     tempo_Nline=h
+0000eb50: 6475 6c5b 692b 315d 2e68 6561 6465 725b  dul[i+1].header[
+0000eb60: 274e 4c49 4e45 275d 0a20 2020 2020 2020  'NLINE'].       
+0000eb70: 2020 2020 2074 656d 706f 5f52 3d68 6475       tempo_R=hdu
+0000eb80: 6c5b 692b 315d 2e68 6561 6465 725b 2752  l[i+1].header['R
+0000eb90: 5f4f 564c 5027 5d0a 2020 2020 2020 2020  _OVLP'].        
+0000eba0: 2020 2020 6461 7474 613d 5b5d 0a20 2020      datta=[].   
+0000ebb0: 2020 2020 2020 2020 2074 656d 706f 2e6f           tempo.o
+0000ebc0: 7665 726c 6170 4672 6571 3d68 6475 6c5b  verlapFreq=hdul[
+0000ebd0: 692b 315d 2e64 6174 615b 3a2c 2d31 5d0a  i+1].data[:,-1].
+0000ebe0: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
+0000ebf0: 6f2e 6f76 6572 6c61 704c 5445 3d68 6475  o.overlapLTE=hdu
+0000ec00: 6c5b 692b 315d 2e64 6174 615b 3a2c 305d  l[i+1].data[:,0]
+0000ec10: 0a20 2020 2020 2020 2020 2020 2074 656d  .            tem
+0000ec20: 706f 2e6f 7665 726c 6170 5461 754c 5445  po.overlapTauLTE
+0000ec30: 3d68 6475 6c5b 692b 315d 2e64 6174 615b  =hdul[i+1].data[
+0000ec40: 3a2c 315d 0a20 2020 2020 2020 2020 2020  :,1].           
+0000ec50: 2074 656d 706f 2e6f 7665 726c 6170 4e4c   tempo.overlapNL
+0000ec60: 5445 3d68 6475 6c5b 692b 315d 2e64 6174  TE=hdul[i+1].dat
+0000ec70: 615b 3a2c 325d 0a20 2020 2020 2020 2020  a[:,2].         
+0000ec80: 2020 2074 656d 706f 2e6f 7665 726c 6170     tempo.overlap
+0000ec90: 5461 754e 4c54 453d 6864 756c 5b69 2b31  TauNLTE=hdul[i+1
+0000eca0: 5d2e 6461 7461 5b3a 2c33 5d0a 2020 2020  ].data[:,3].    
+0000ecb0: 2020 2020 2020 2020 7465 6d70 6f2e 6f76          tempo.ov
+0000ecc0: 6572 6c61 7052 3d74 656d 706f 5f52 0a20  erlapR=tempo_R. 
+0000ecd0: 2020 2020 2020 2020 2020 2074 656d 706f             tempo
+0000ece0: 2e6d 6f64 656c 5f6e 756d 6265 723d 6864  .model_number=hd
+0000ecf0: 756c 5b69 2b31 5d2e 6865 6164 6572 5b27  ul[i+1].header['
+0000ed00: 4d4f 4445 4c27 5d0a 2020 2020 2020 2020  MODEL'].        
+0000ed10: 2020 2020 7465 6d70 6f2e 5467 3d68 6475      tempo.Tg=hdu
+0000ed20: 6c5b 692b 315d 2e68 6561 6465 725b 2754  l[i+1].header['T
+0000ed30: 4727 5d0a 2020 2020 2020 2020 2020 2020  G'].            
+0000ed40: 7465 6d70 6f2e 5464 3d68 6475 6c5b 692b  tempo.Td=hdul[i+
+0000ed50: 315d 2e68 6561 6465 725b 2754 4427 5d0a  1].header['TD'].
+0000ed60: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
+0000ed70: 6f2e 7674 7572 623d 6864 756c 5b69 2b31  o.vturb=hdul[i+1
+0000ed80: 5d2e 6865 6164 6572 5b27 5654 5552 4227  ].header['VTURB'
+0000ed90: 5d0a 2020 2020 2020 2020 2020 2020 7465  ].            te
+0000eda0: 6d70 6f2e 4e48 3d68 6475 6c5b 692b 315d  mpo.NH=hdul[i+1]
+0000edb0: 2e68 6561 6465 725b 274e 4854 4f54 275d  .header['NHTOT']
+0000edc0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+0000edd0: 612e 6164 645f 6d6f 6465 6c28 7465 6d70  a.add_model(temp
+0000ede0: 6f29 0a20 2020 2020 2020 2020 2020 2023  o).            #
+0000edf0: 2070 7269 6e74 2827 7265 6164 2027 2c69   print('read ',i
+0000ee00: 2c27 206d 6f64 656c 2729 0a20 2020 2065  ,' model').    e
+0000ee10: 6c73 653a 0a20 2020 2020 2020 2066 3d6f  lse:.        f=o
+0000ee20: 7065 6e28 7061 7468 290a 2020 2020 2020  pen(path).      
+0000ee30: 2020 6461 7461 3d73 6c61 625f 6461 7461    data=slab_data
+0000ee40: 2829 0a20 2020 2020 2020 206e 6d6f 6465  ().        nmode
+0000ee50: 6c73 3d69 6e74 2866 2e72 6561 646c 696e  ls=int(f.readlin
+0000ee60: 6528 292e 7370 6c69 7428 295b 305d 290a  e().split()[0]).
+0000ee70: 2020 2020 2020 2020 6461 7461 2e64 6972          data.dir
+0000ee80: 6563 746f 7279 3d70 6174 680a 2020 2020  ectory=path.    
+0000ee90: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+0000eea0: 6765 286e 6d6f 6465 6c73 293a 0a20 2020  ge(nmodels):.   
+0000eeb0: 2020 2020 2020 2020 2074 656d 706f 3d73           tempo=s
+0000eec0: 6c61 6228 290a 2020 2020 2020 2020 2020  lab().          
+0000eed0: 2020 7465 6d70 6f5f 6d6f 6465 6c5f 6e75    tempo_model_nu
+0000eee0: 6d62 6572 3d69 6e74 2866 2e72 6561 646c  mber=int(f.readl
+0000eef0: 696e 6528 292e 7370 6c69 7428 295b 305d  ine().split()[0]
+0000ef00: 290a 2020 2020 2020 2020 2020 2020 7465  ).            te
+0000ef10: 6d70 6f5f 4e6c 696e 653d 696e 7428 662e  mpo_Nline=int(f.
+0000ef20: 7265 6164 6c69 6e65 2829 2e73 706c 6974  readline().split
+0000ef30: 2829 5b30 5d29 0a20 2020 2020 2020 2020  ()[0]).         
+0000ef40: 2020 2074 656d 706f 5f52 3d66 6c6f 6174     tempo_R=float
+0000ef50: 2866 2e72 6561 646c 696e 6528 292e 7370  (f.readline().sp
+0000ef60: 6c69 7428 295b 305d 290a 2020 2020 2020  lit()[0]).      
+0000ef70: 2020 2020 2020 6461 7474 613d 5b5d 0a20        datta=[]. 
+0000ef80: 2020 2020 2020 2020 2020 206c 696e 6573             lines
+0000ef90: 3d66 2e72 6561 646c 696e 6528 290a 2020  =f.readline().  
+0000efa0: 2020 2020 2020 2020 2020 666f 7220 6a20            for j 
+0000efb0: 696e 2072 616e 6765 2874 656d 706f 5f4e  in range(tempo_N
+0000efc0: 6c69 6e65 293a 0a20 2020 2020 2020 2020  line):.         
+0000efd0: 2020 2020 2020 206c 696e 6573 3d66 2e72         lines=f.r
+0000efe0: 6561 646c 696e 6528 290a 2020 2020 2020  eadline().      
+0000eff0: 2020 2020 2020 2020 2020 6461 7474 612e            datta.
+0000f000: 6170 7065 6e64 286e 702e 6172 7261 7928  append(np.array(
+0000f010: 6c69 6e65 732e 7370 6c69 7428 292c 6474  lines.split(),dt
+0000f020: 7970 653d 666c 6f61 7429 290a 2020 2020  ype=float)).    
+0000f030: 2020 2020 2020 2020 6461 7474 613d 6e70          datta=np
+0000f040: 2e61 7272 6179 2864 6174 7461 290a 2020  .array(datta).  
+0000f050: 2020 2020 2020 2020 2020 7465 6d70 6f2e            tempo.
+0000f060: 6f76 6572 6c61 7046 7265 713d 6461 7474  overlapFreq=datt
+0000f070: 615b 3a2c 305d 0a20 2020 2020 2020 2020  a[:,0].         
+0000f080: 2020 2074 656d 706f 2e6f 7665 726c 6170     tempo.overlap
+0000f090: 4c54 453d 6461 7474 615b 3a2c 315d 0a20  LTE=datta[:,1]. 
+0000f0a0: 2020 2020 2020 2020 2020 2074 656d 706f             tempo
+0000f0b0: 2e6f 7665 726c 6170 5461 754c 5445 3d64  .overlapTauLTE=d
+0000f0c0: 6174 7461 5b3a 2c32 5d0a 2020 2020 2020  atta[:,2].      
+0000f0d0: 2020 2020 2020 7465 6d70 6f2e 6f76 6572        tempo.over
+0000f0e0: 6c61 704e 4c54 453d 6461 7474 615b 3a2c  lapNLTE=datta[:,
+0000f0f0: 335d 0a20 2020 2020 2020 2020 2020 2074  3].            t
+0000f100: 656d 706f 2e6f 7665 726c 6170 5461 754e  empo.overlapTauN
+0000f110: 4c54 453d 6461 7474 615b 3a2c 345d 0a20  LTE=datta[:,4]. 
+0000f120: 2020 2020 2020 2020 2020 2074 656d 706f             tempo
+0000f130: 2e6f 7665 726c 6170 523d 7465 6d70 6f5f  .overlapR=tempo_
+0000f140: 520a 2020 2020 2020 2020 2020 2020 6461  R.            da
+0000f150: 7461 2e61 6464 5f6d 6f64 656c 2874 656d  ta.add_model(tem
+0000f160: 706f 290a 2020 2020 2020 2020 2020 2020  po).            
+0000f170: 6c69 6e65 733d 662e 7265 6164 6c69 6e65  lines=f.readline
+0000f180: 2829 0a20 2020 2020 2020 2020 2020 2023  ().            #
+0000f190: 2070 7269 6e74 2827 7265 6164 2027 2c69   print('read ',i
+0000f1a0: 2c27 206d 6f64 656c 2729 0a20 2020 200a  ,' model').    .
+0000f1b0: 2020 2020 7265 7475 726e 2864 6174 6129      return(data)
+0000f1c0: 0a0a 0a64 6566 2073 7065 6343 6f6e 766f  ...def specConvo
+0000f1d0: 6c76 6528 6c69 6e65 5374 7265 6e67 7468  lve(lineStrength
+0000f1e0: 732c 6c69 6e65 4672 6571 2c66 7265 715f  s,lineFreq,freq_
+0000f1f0: 6269 6e73 3d4e 6f6e 652c 523d 312c 6c61  bins=None,R=1,la
+0000f200: 6d62 6461 5f30 3d31 2c6c 616d 6264 615f  mbda_0=1,lambda_
+0000f210: 6e3d 312c 7672 3d31 3330 3029 3a0a 2020  n=1,vr=1300):.  
+0000f220: 2020 2222 220a 2020 2020 4e4f 5420 5553    """.    NOT US
+0000f230: 4544 2041 4e59 4d4f 5245 0a20 2020 2046  ED ANYMORE.    F
+0000f240: 756e 6374 696f 6e20 746f 2063 6f6e 766f  unction to convo
+0000f250: 6c76 6520 6c69 6e65 7320 696e 746f 2073  lve lines into s
+0000f260: 7065 6374 7261 2062 7920 7369 6d70 6c79  pectra by simply
+0000f270: 2062 696e 6e69 6e67 2074 6865 6d20 696e   binning them in
+0000f280: 746f 2061 2077 6176 656c 656e 6774 6820  to a wavelength 
+0000f290: 6772 6964 0a20 2020 2022 2222 0a20 2020  grid.    """.   
+0000f2a0: 2067 5065 7263 3d6c 616d 6264 6120 782c   gPerc=lambda x,
+0000f2b0: 6d2c 733a 2073 6572 6628 2878 2d6d 292f  m,s: serf((x-m)/
+0000f2c0: 7329 2a30 2e35 2b30 2e35 0a20 2020 206e  s)*0.5+0.5.    n
+0000f2d0: 755f 696a 3d6c 696e 6546 7265 712a 3165  u_ij=lineFreq*1e
+0000f2e0: 390a 2020 2020 6966 206c 616d 6264 615f  9.    if lambda_
+0000f2f0: 6e3d 3d6c 616d 6264 615f 303a 0a20 2020  n==lambda_0:.   
+0000f300: 2020 2020 206c 616d 6264 615f 6e3d 6e70       lambda_n=np
+0000f310: 2e61 6d61 7828 632f 6e75 5f69 6a2a 3165  .amax(c/nu_ij*1e
+0000f320: 3629 2a32 0a20 2020 2069 6620 7479 7065  6)*2.    if type
+0000f330: 2866 7265 715f 6269 6e73 293d 3d74 7970  (freq_bins)==typ
+0000f340: 6528 4e6f 6e65 293a 0a20 2020 2020 2020  e(None):.       
+0000f350: 206e 753d 6765 6e65 7261 7465 5f67 7269   nu=generate_gri
+0000f360: 6428 523d 522c 6c61 6d62 6461 5f30 3d6c  d(R=R,lambda_0=l
+0000f370: 616d 6264 615f 302c 6c61 6d62 6461 5f6e  ambda_0,lambda_n
+0000f380: 3d6c 616d 6264 615f 6e29 2a31 6539 0a20  =lambda_n)*1e9. 
+0000f390: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000f3a0: 2066 7265 715f 6269 6e73 3d6e 702e 636f   freq_bins=np.co
+0000f3b0: 6e63 6174 656e 6174 6528 2866 7265 715f  ncatenate((freq_
+0000f3c0: 6269 6e73 2c6e 702e 6172 7261 7928 5b28  bins,np.array([(
+0000f3d0: 6672 6571 5f62 696e 735b 2d31 5d2d 6672  freq_bins[-1]-fr
+0000f3e0: 6571 5f62 696e 735b 2d32 5d29 2b66 7265  eq_bins[-2])+fre
+0000f3f0: 715f 6269 6e73 5b2d 315d 5d29 2929 0a20  q_bins[-1]]))). 
+0000f400: 2020 2020 2020 206e 753d 6672 6571 5f62         nu=freq_b
+0000f410: 696e 732a 3165 390a 2020 2020 6e75 5f69  ins*1e9.    nu_i
+0000f420: 6a5f 7469 6c65 3d6e 702e 7469 6c65 286e  j_tile=np.tile(n
+0000f430: 755f 696a 2c5b 6c65 6e28 6e75 292c 315d  u_ij,[len(nu),1]
+0000f440: 290a 2020 2020 6e75 5f74 696c 653d 6e70  ).    nu_tile=np
+0000f450: 2e74 696c 6528 6e75 2c5b 6c65 6e28 6e75  .tile(nu,[len(nu
+0000f460: 5f69 6a29 2c31 5d29 0a20 2020 206c 696e  _ij),1]).    lin
+0000f470: 6553 7472 656e 6774 6873 5f74 696c 653d  eStrengths_tile=
+0000f480: 6e70 2e74 696c 6528 6c69 6e65 5374 7265  np.tile(lineStre
+0000f490: 6e67 7468 732c 5b6c 656e 286e 7529 2c31  ngths,[len(nu),1
+0000f4a0: 5d29 0a20 2020 2070 6572 635f 7469 6c65  ]).    perc_tile
+0000f4b0: 3d67 5065 7263 286e 755f 7469 6c65 2c6e  =gPerc(nu_tile,n
+0000f4c0: 755f 696a 5f74 696c 652e 542c 6e75 5f69  u_ij_tile.T,nu_i
+0000f4d0: 6a5f 7469 6c65 2e54 2f63 2a76 7229 0a20  j_tile.T/c*vr). 
+0000f4e0: 2020 2078 3d70 6572 635f 7469 6c65 5b3a     x=perc_tile[:
+0000f4f0: 2c3a 2d31 5d2d 7065 7263 5f74 696c 655b  ,:-1]-perc_tile[
+0000f500: 3a2c 313a 5d0a 2020 2020 7761 7665 6c65  :,1:].    wavele
+0000f510: 6e67 7468 2c66 6c75 783d 632f 6e75 5b3a  ngth,flux=c/nu[:
+0000f520: 2d31 5d2a 3165 362c 6e70 2e73 756d 2878  -1]*1e6,np.sum(x
+0000f530: 2a6c 696e 6553 7472 656e 6774 6873 5f74  *lineStrengths_t
+0000f540: 696c 655b 3a2d 312c 3a5d 2e54 2c61 7869  ile[:-1,:].T,axi
+0000f550: 733d 3029 2f28 6e75 5b3a 2d31 5d2d 6e75  s=0)/(nu[:-1]-nu
+0000f560: 5b31 3a5d 290a 2020 2020 7265 7475 726e  [1:]).    return
+0000f570: 2077 6176 656c 656e 6774 682c 666c 7578   wavelength,flux
+0000f580: 0a0a 0a64 6566 2067 656e 6572 616c 436f  ...def generalCo
+0000f590: 6e76 6f6c 7665 286c 696e 6553 7472 656e  nvolve(lineStren
+0000f5a0: 6774 6873 2c6c 696e 6546 7265 712c 523d  gths,lineFreq,R=
+0000f5b0: 312c 6c61 6d62 6461 5f30 3d31 2c6c 616d  1,lambda_0=1,lam
+0000f5c0: 6264 615f 6e3d 312c 525f 6261 636b 3d31  bda_n=1,R_back=1
+0000f5d0: 6536 293a 0a20 2020 2022 2222 0a20 2020  e6):.    """.   
+0000f5e0: 2046 756e 6374 696f 6e20 746f 2063 6f6e   Function to con
+0000f5f0: 766f 6c76 6520 6c69 6e65 2066 6c75 7865  volve line fluxe
+0000f600: 7320 696e 746f 206c 696e 6520 7370 6563  s into line spec
+0000f610: 7472 6120 6261 7365 6420 6f6e 2061 2075  tra based on a u
+0000f620: 7365 7220 6465 6669 6e65 6420 7370 6563  ser defined spec
+0000f630: 7472 616c 2072 6573 6f6c 7669 6e67 2070  tral resolving p
+0000f640: 6f77 6572 2052 0a20 2020 2022 2222 0a20  ower R.    """. 
+0000f650: 2020 2069 6620 6c61 6d62 6461 5f6e 3d3d     if lambda_n==
+0000f660: 6c61 6d62 6461 5f30 3a0a 2020 2020 2020  lambda_0:.      
+0000f670: 2020 6c61 6d62 6461 5f6e 3d63 2f6e 702e    lambda_n=c/np.
+0000f680: 616d 696e 286c 696e 6546 7265 7129 2a31  amin(lineFreq)*1
+0000f690: 652d 332a 320a 2020 2020 6672 6571 5f62  e-3*2.    freq_b
+0000f6a0: 696e 733d 6765 6e65 7261 7465 5f67 7269  ins=generate_gri
+0000f6b0: 6428 525f 6261 636b 2c6c 616d 6264 615f  d(R_back,lambda_
+0000f6c0: 302c 6c61 6d62 6461 5f6e 290a 2020 2020  0,lambda_n).    
+0000f6d0: 7761 7665 5f62 696e 733d 632f 6672 6571  wave_bins=c/freq
+0000f6e0: 5f62 696e 732a 3165 2d33 0a20 2020 2066  _bins*1e-3.    f
+0000f6f0: 6c75 785f 6269 6e73 3d77 6176 655f 6269  lux_bins=wave_bi
+0000f700: 6e73 2a30 2e30 0a20 2020 2069 3d36 0a20  ns*0.0.    i=6. 
+0000f710: 2020 2053 3d6c 696e 6553 7472 656e 6774     S=lineStrengt
+0000f720: 6873 0a20 2020 2046 3d6c 696e 6546 7265  hs.    F=lineFre
+0000f730: 710a 2020 2020 696e 643d 6e70 2e64 6967  q.    ind=np.dig
+0000f740: 6974 697a 6528 462c 6e70 2e66 6c69 7028  itize(F,np.flip(
+0000f750: 6672 6571 5f62 696e 7329 5b3a 2d31 5d29  freq_bins)[:-1])
+0000f760: 0a20 2020 2066 6f72 2069 2c69 6478 2069  .    for i,idx i
+0000f770: 6e20 656e 756d 6572 6174 6528 696e 6429  n enumerate(ind)
+0000f780: 3a0a 2020 2020 2020 2020 666c 7578 5f62  :.        flux_b
+0000f790: 696e 735b 6964 785d 2b3d 535b 695d 0a0a  ins[idx]+=S[i]..
+0000f7a0: 2020 2020 4657 484d 3d52 5f62 6163 6b2f      FWHM=R_back/
+0000f7b0: 522f 322e 3335 350a 2020 2020 673d 4761  R/2.355.    g=Ga
+0000f7c0: 7573 7369 616e 3144 4b65 726e 656c 2873  ussian1DKernel(s
+0000f7d0: 7464 6465 763d 4657 484d 2c66 6163 746f  tddev=FWHM,facto
+0000f7e0: 723d 3729 0a20 2020 2041 3d61 7079 5f63  r=7).    A=apy_c
+0000f7f0: 6f6e 766f 6c76 6528 666c 7578 5f62 696e  onvolve(flux_bin
+0000f800: 732c 6729 0a20 2020 2041 3d41 5b31 3a5d  s,g).    A=A[1:]
+0000f810: 2f28 6e70 2e66 6c69 7028 6672 6571 5f62  /(np.flip(freq_b
+0000f820: 696e 7329 5b31 3a5d 2d6e 702e 666c 6970  ins)[1:]-np.flip
+0000f830: 2866 7265 715f 6269 6e73 295b 3a2d 315d  (freq_bins)[:-1]
+0000f840: 292a 3165 2d39 0a20 2020 2057 3d6e 702e  )*1e-9.    W=np.
+0000f850: 666c 6970 2877 6176 655f 6269 6e73 5b31  flip(wave_bins[1
+0000f860: 3a5d 290a 2020 2020 7265 7475 726e 206e  :]).    return n
+0000f870: 702e 666c 6970 2857 292c 6e70 2e66 6c69  p.flip(W),np.fli
+0000f880: 7028 4129 0a0a 0a64 6566 2067 656e 6572  p(A)...def gener
+0000f890: 6174 655f 6772 6964 2852 3d31 2c6c 616d  ate_grid(R=1,lam
+0000f8a0: 6264 615f 303d 312c 6c61 6d62 6461 5f6e  bda_0=1,lambda_n
+0000f8b0: 3d31 2c73 616d 706c 696e 673d 3129 3a0a  =1,sampling=1):.
+0000f8c0: 2020 2020 2222 220a 2020 2020 4765 6e65      """.    Gene
+0000f8d0: 7261 7465 2061 2073 7065 6374 7261 6c20  rate a spectral 
+0000f8e0: 6772 6964 2069 6e20 4748 7a0a 2020 2020  grid in GHz.    
+0000f8f0: 2222 220a 2020 2020 6465 6c5f 6c6f 676c  """.    del_logl
+0000f900: 616d 3d6e 702e 6c6f 6731 3028 312e 302b  am=np.log10(1.0+
+0000f910: 312e 302f 5229 0a20 2020 204e 3d31 2b69  1.0/R).    N=1+i
+0000f920: 6e74 286e 702e 6c6f 6731 3028 6c61 6d62  nt(np.log10(lamb
+0000f930: 6461 5f6e 2f6c 616d 6264 615f 3029 2f64  da_n/lambda_0)/d
+0000f940: 656c 5f6c 6f67 6c61 6d29 0a20 2020 206d  el_loglam).    m
+0000f950: 776c 736c 696e 653d 6e70 2e6c 6f67 7370  wlsline=np.logsp
+0000f960: 6163 6528 6e70 2e6c 6f67 3130 286c 616d  ace(np.log10(lam
+0000f970: 6264 615f 3029 2c6e 702e 6c6f 6731 3028  bda_0),np.log10(
+0000f980: 6c61 6d62 6461 5f6e 292c 696e 7428 4e2a  lambda_n),int(N*
+0000f990: 7361 6d70 6c69 6e67 2929 0a20 2020 206e  sampling)).    n
+0000f9a0: 753d 632f 6d77 6c73 6c69 6e65 2a31 6536  u=c/mwlsline*1e6
+0000f9b0: 0a20 2020 2072 6574 7572 6e28 6e75 2a31  .    return(nu*1
+0000f9c0: 652d 3929 0a0a 0a64 6566 2063 6f6e 766f  e-9)...def convo
+0000f9d0: 6c76 6528 6d6f 6465 6c73 2c66 7265 715f  lve(models,freq_
+0000f9e0: 6269 6e73 3d4e 6f6e 652c 523d 312c 6c61  bins=None,R=1,la
+0000f9f0: 6d62 6461 5f30 3d31 2c6c 616d 6264 615f  mbda_0=1,lambda_
+0000fa00: 6e3d 312c 7672 3d31 3330 302c 4e4c 5445  n=1,vr=1300,NLTE
+0000fa10: 3d46 616c 7365 2c63 6f6e 765f 7479 7065  =False,conv_type
+0000fa20: 3d31 2c76 6572 626f 7365 3d54 7275 6529  =1,verbose=True)
+0000fa30: 3a0a 2020 2020 2222 220a 2020 2020 5361  :.    """.    Sa
+0000fa40: 6d65 2061 7320 2e63 6f6e 766f 6c76 6528  me as .convolve(
+0000fa50: 2920 6d65 7468 6f64 0a20 2020 2022 2222  ) method.    """
+0000fa60: 0a20 2020 2066 6f72 2069 2c64 2069 6e20  .    for i,d in 
+0000fa70: 656e 756d 6572 6174 6528 6d6f 6465 6c73  enumerate(models
+0000fa80: 293a 0a20 2020 2020 2020 2069 6620 7665  ):.        if ve
+0000fa90: 7262 6f73 653a 2070 7269 6e74 2827 5c6e  rbose: print('\n
+0000faa0: 5c6e 4d6f 6465 6c20 272c 692b 3129 0a20  \nModel ',i+1). 
+0000fab0: 2020 2020 2020 2064 2e63 6f6e 766f 6c76         d.convolv
+0000fac0: 6528 6672 6571 5f62 696e 733d 6672 6571  e(freq_bins=freq
+0000fad0: 5f62 696e 732c 523d 522c 6c61 6d62 6461  _bins,R=R,lambda
+0000fae0: 5f30 3d6c 616d 6264 615f 302c 6c61 6d62  _0=lambda_0,lamb
+0000faf0: 6461 5f6e 3d6c 616d 6264 615f 6e2c 7672  da_n=lambda_n,vr
+0000fb00: 3d76 722c 4e4c 5445 3d4e 4c54 452c 636f  =vr,NLTE=NLTE,co
+0000fb10: 6e76 5f74 7970 653d 636f 6e76 5f74 7970  nv_type=conv_typ
+0000fb20: 6529 0a20 2020 2072 6574 7572 6e20 6d6f  e).    return mo
+0000fb30: 6465 6c73 0a0a 0a64 6566 2067 656e 6572  dels...def gener
+0000fb40: 6174 655f 736c 6162 5f67 7269 6428 6469  ate_slab_grid(di
+0000fb50: 7265 6374 6f72 793d 272e 272c 6772 6964  rectory='.',grid
+0000fb60: 5f70 6172 616d 6574 6572 733d 7b7d 2c63  _parameters={},c
+0000fb70: 6f6d 6269 6e61 7469 6f6e 3d46 616c 7365  ombination=False
+0000fb80: 2c4e 746f 743d 4e6f 6e65 2c54 673d 4e6f  ,Ntot=None,Tg=No
+0000fb90: 6e65 2c6e 4870 6c75 733d 4e6f 6e65 2c6e  ne,nHplus=None,n
+0000fba0: 4831 3d4e 6f6e 652c 6e48 323d 4e6f 6e65  H1=None,nH2=None
+0000fbb0: 2c6e 4865 3d4e 6f6e 652c 6e65 6c65 633d  ,nHe=None,nelec=
+0000fbc0: 4e6f 6e65 2c54 643d 4e6f 6e65 2c76 7475  None,Td=None,vtu
+0000fbd0: 7262 3d4e 6f6e 652c 6475 7374 5f74 6f5f  rb=None,dust_to_
+0000fbe0: 6761 733d 4e6f 6e65 2c52 5f6f 7665 726c  gas=None,R_overl
+0000fbf0: 6170 3d4e 6f6e 652c 6c69 6e65 5f6f 7665  ap=None,line_ove
+0000fc00: 726c 6170 3d4e 6f6e 652c 7370 6563 6965  rlap=None,specie
+0000fc10: 735f 6c69 7374 3d7b 7d2c 6f75 7470 7574  s_list={},output
+0000fc20: 5f66 696c 656e 616d 653d 2753 6c61 6252  _filename='SlabR
+0000fc30: 6573 756c 7473 2e6f 7574 272c 6f76 6572  esults.out',over
+0000fc40: 6c61 705f 6669 6c65 6e61 6d65 3d27 536c  lap_filename='Sl
+0000fc50: 6162 4f76 6572 6c61 702e 6f75 7427 2c73  abOverlap.out',s
+0000fc60: 6570 6172 6174 655f 6f70 5f66 696c 6573  eparate_op_files
+0000fc70: 3d54 7275 652c 736c 6162 5f52 543d 5472  =True,slab_RT=Tr
+0000fc80: 7565 2c73 686f 7274 5f66 6f72 6d61 743d  ue,short_format=
+0000fc90: 4661 6c73 652c 6e6f 5f69 6e64 6976 6964  False,no_individ
+0000fca0: 7561 6c5f 6c69 6e65 733d 4661 6c73 652c  ual_lines=False,
+0000fcb0: 6669 7473 5f6f 705f 6669 6c65 733d 4661  fits_op_files=Fa
+0000fcc0: 6c73 6529 3a0a 2020 2020 2222 220a 2020  lse):.    """.  
+0000fcd0: 2020 4675 6e63 7469 6f6e 2074 6f20 6765    Function to ge
+0000fce0: 6e65 7261 7465 2053 6c61 6249 6e70 7574  nerate SlabInput
+0000fcf0: 2e69 6e20 696e 7075 7420 6669 6c65 2063  .in input file c
+0000fd00: 6f6e 7461 696e 696e 6720 7468 6520 6465  ontaining the de
+0000fd10: 7461 696c 7320 6f66 2074 6865 2073 6c61  tails of the sla
+0000fd20: 6220 6d6f 6465 6c20 6772 6964 0a20 2020  b model grid.   
+0000fd30: 2022 2222 0a20 2020 206e 6d6f 6465 6c73   """.    nmodels
+0000fd40: 3d31 0a20 2020 2063 6f6d 6269 6e61 7469  =1.    combinati
+0000fd50: 6f6e 3d46 616c 7365 0a20 2020 2069 6620  on=False.    if 
+0000fd60: 6c65 6e28 6772 6964 5f70 6172 616d 6574  len(grid_paramet
+0000fd70: 6572 7329 3e30 3a0a 2020 2020 2020 2020  ers)>0:.        
+0000fd80: 6966 206e 6f74 2063 6f6d 6269 6e61 7469  if not combinati
+0000fd90: 6f6e 3a0a 2020 2020 2020 2020 2020 2020  on:.            
+0000fda0: 6e6d 6f64 656c 733d 6c65 6e28 6772 6964  nmodels=len(grid
+0000fdb0: 5f70 6172 616d 6574 6572 735b 6c69 7374  _parameters[list
+0000fdc0: 2867 7269 645f 7061 7261 6d65 7465 7273  (grid_parameters
+0000fdd0: 2e6b 6579 7328 2929 5b30 5d5d 290a 2020  .keys())[0]]).  
+0000fde0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000fdf0: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+0000fe00: 2072 616e 6765 286c 656e 2867 7269 645f   range(len(grid_
+0000fe10: 7061 7261 6d65 7465 7273 2929 3a0a 2020  parameters)):.  
+0000fe20: 2020 2020 2020 2020 2020 2020 2020 6e6d                nm
+0000fe30: 6f64 656c 732a 3d6c 656e 2867 7269 645f  odels*=len(grid_
+0000fe40: 7061 7261 6d65 7465 7273 5b6c 6973 7428  parameters[list(
+0000fe50: 6772 6964 5f70 6172 616d 6574 6572 732e  grid_parameters.
+0000fe60: 6b65 7973 2829 295b 695d 5d29 0a0a 2020  keys())[i]])..  
+0000fe70: 2020 4e74 6f74 5f6c 6973 743d 6e70 2e6f    Ntot_list=np.o
+0000fe80: 6e65 7328 286e 6d6f 6465 6c73 2929 0a20  nes((nmodels)). 
+0000fe90: 2020 2054 675f 6c69 7374 3d6e 702e 6f6e     Tg_list=np.on
+0000fea0: 6573 2828 6e6d 6f64 656c 7329 290a 2020  es((nmodels)).  
+0000feb0: 2020 6e48 706c 7573 5f6c 6973 743d 6e70    nHplus_list=np
 0000fec0: 2e6f 6e65 7328 286e 6d6f 6465 6c73 2929  .ones((nmodels))
-0000fed0: 0a20 2020 206c 696e 655f 6f76 6572 6c61  .    line_overla
-0000fee0: 705f 6c69 7374 3d6e 702e 6f6e 6573 2828  p_list=np.ones((
-0000fef0: 6e6d 6f64 656c 732c 3229 290a 2020 2020  nmodels,2)).    
-0000ff00: 6966 206c 656e 2873 7065 6369 6573 5f6c  if len(species_l
-0000ff10: 6973 7429 3c31 3a20 7261 6973 6520 5661  ist)<1: raise Va
-0000ff20: 6c75 6545 7272 6f72 2827 5468 6520 7370  lueError('The sp
-0000ff30: 6563 6965 735f 6c69 7374 2063 616e 6e6f  ecies_list canno
-0000ff40: 7420 6265 2065 6d70 7479 2729 0a0a 2020  t be empty')..  
-0000ff50: 2020 6966 206e 6f74 2063 6f6d 6269 6e61    if not combina
-0000ff60: 7469 6f6e 3a0a 2020 2020 2020 2020 666f  tion:.        fo
-0000ff70: 7220 6920 696e 2072 616e 6765 286c 656e  r i in range(len
-0000ff80: 2867 7269 645f 7061 7261 6d65 7465 7273  (grid_parameters
-0000ff90: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
-0000ffa0: 6966 206c 6973 7428 6772 6964 5f70 6172  if list(grid_par
-0000ffb0: 616d 6574 6572 732e 6b65 7973 2829 295b  ameters.keys())[
-0000ffc0: 695d 3d3d 274e 746f 7427 3a0a 2020 2020  i]=='Ntot':.    
-0000ffd0: 2020 2020 2020 2020 2020 2020 4e74 6f74              Ntot
-0000ffe0: 5f6c 6973 742a 3d67 7269 645f 7061 7261  _list*=grid_para
-0000fff0: 6d65 7465 7273 5b27 4e74 6f74 275d 0a20  meters['Ntot']. 
-00010000: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-00010010: 6c69 7374 2867 7269 645f 7061 7261 6d65  list(grid_parame
-00010020: 7465 7273 2e6b 6579 7328 2929 5b69 5d3d  ters.keys())[i]=
-00010030: 3d27 5467 273a 0a20 2020 2020 2020 2020  ='Tg':.         
-00010040: 2020 2020 2020 2054 675f 6c69 7374 2a3d         Tg_list*=
-00010050: 6772 6964 5f70 6172 616d 6574 6572 735b  grid_parameters[
-00010060: 2754 6727 5d0a 2020 2020 2020 2020 2020  'Tg'].          
-00010070: 2020 656c 6966 206c 6973 7428 6772 6964    elif list(grid
-00010080: 5f70 6172 616d 6574 6572 732e 6b65 7973  _parameters.keys
-00010090: 2829 295b 695d 3d3d 276e 4870 6c75 7327  ())[i]=='nHplus'
-000100a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000100b0: 2020 6e48 706c 7573 5f6c 6973 742a 3d67    nHplus_list*=g
-000100c0: 7269 645f 7061 7261 6d65 7465 7273 5b27  rid_parameters['
-000100d0: 6e48 706c 7573 275d 0a20 2020 2020 2020  nHplus'].       
-000100e0: 2020 2020 2065 6c69 6620 6c69 7374 2867       elif list(g
-000100f0: 7269 645f 7061 7261 6d65 7465 7273 2e6b  rid_parameters.k
-00010100: 6579 7328 2929 5b69 5d3d 3d27 6e48 3127  eys())[i]=='nH1'
-00010110: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00010120: 2020 6e48 315f 6c69 7374 2a3d 6772 6964    nH1_list*=grid
-00010130: 5f70 6172 616d 6574 6572 735b 276e 4831  _parameters['nH1
-00010140: 275d 0a20 2020 2020 2020 2020 2020 2065  '].            e
-00010150: 6c69 6620 6c69 7374 2867 7269 645f 7061  lif list(grid_pa
-00010160: 7261 6d65 7465 7273 2e6b 6579 7328 2929  rameters.keys())
-00010170: 5b69 5d3d 3d27 6e48 3227 3a0a 2020 2020  [i]=='nH2':.    
-00010180: 2020 2020 2020 2020 2020 2020 6e48 325f              nH2_
-00010190: 6c69 7374 2a3d 6772 6964 5f70 6172 616d  list*=grid_param
-000101a0: 6574 6572 735b 276e 4832 275d 0a20 2020  eters['nH2'].   
-000101b0: 2020 2020 2020 2020 2065 6c69 6620 6c69           elif li
-000101c0: 7374 2867 7269 645f 7061 7261 6d65 7465  st(grid_paramete
-000101d0: 7273 2e6b 6579 7328 2929 5b69 5d3d 3d27  rs.keys())[i]=='
-000101e0: 6e48 6527 3a0a 2020 2020 2020 2020 2020  nHe':.          
-000101f0: 2020 2020 2020 6e48 655f 6c69 7374 2a3d        nHe_list*=
-00010200: 6772 6964 5f70 6172 616d 6574 6572 735b  grid_parameters[
-00010210: 276e 4865 275d 0a20 2020 2020 2020 2020  'nHe'].         
-00010220: 2020 2065 6c69 6620 6c69 7374 2867 7269     elif list(gri
-00010230: 645f 7061 7261 6d65 7465 7273 2e6b 6579  d_parameters.key
-00010240: 7328 2929 5b69 5d3d 3d27 6e65 6c65 6327  s())[i]=='nelec'
-00010250: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00010260: 2020 6e65 6c65 635f 6c69 7374 2a3d 6772    nelec_list*=gr
-00010270: 6964 5f70 6172 616d 6574 6572 735b 276e  id_parameters['n
-00010280: 656c 6563 275d 0a20 2020 2020 2020 2020  elec'].         
-00010290: 2020 2065 6c69 6620 6c69 7374 2867 7269     elif list(gri
-000102a0: 645f 7061 7261 6d65 7465 7273 2e6b 6579  d_parameters.key
-000102b0: 7328 2929 5b69 5d3d 3d27 5464 273a 0a20  s())[i]=='Td':. 
-000102c0: 2020 2020 2020 2020 2020 2020 2020 2054                 T
-000102d0: 645f 6c69 7374 2a3d 6772 6964 5f70 6172  d_list*=grid_par
-000102e0: 616d 6574 6572 735b 2754 6427 5d0a 2020  ameters['Td'].  
-000102f0: 2020 2020 2020 2020 2020 656c 6966 206c            elif l
-00010300: 6973 7428 6772 6964 5f70 6172 616d 6574  ist(grid_paramet
-00010310: 6572 732e 6b65 7973 2829 295b 695d 3d3d  ers.keys())[i]==
-00010320: 2776 7475 7262 273a 0a20 2020 2020 2020  'vturb':.       
-00010330: 2020 2020 2020 2020 2076 7475 7262 5f6c           vturb_l
-00010340: 6973 742a 3d67 7269 645f 7061 7261 6d65  ist*=grid_parame
-00010350: 7465 7273 5b27 7674 7572 6227 5d0a 2020  ters['vturb'].  
-00010360: 2020 2020 2020 2020 2020 656c 6966 206c            elif l
-00010370: 6973 7428 6772 6964 5f70 6172 616d 6574  ist(grid_paramet
-00010380: 6572 732e 6b65 7973 2829 295b 695d 3d3d  ers.keys())[i]==
-00010390: 2764 7573 745f 746f 5f67 6173 273a 0a20  'dust_to_gas':. 
-000103a0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-000103b0: 7573 745f 746f 5f67 6173 5f6c 6973 742a  ust_to_gas_list*
-000103c0: 3d67 7269 645f 7061 7261 6d65 7465 7273  =grid_parameters
-000103d0: 5b27 6475 7374 5f74 6f5f 6761 7327 5d0a  ['dust_to_gas'].
-000103e0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-000103f0: 206c 6973 7428 6772 6964 5f70 6172 616d   list(grid_param
-00010400: 6574 6572 732e 6b65 7973 2829 295b 695d  eters.keys())[i]
-00010410: 3d3d 2752 5f6f 7665 726c 6170 273a 0a20  =='R_overlap':. 
-00010420: 2020 2020 2020 2020 2020 2020 2020 2052                 R
-00010430: 5f6f 7665 726c 6170 5f6c 6973 742a 3d67  _overlap_list*=g
-00010440: 7269 645f 7061 7261 6d65 7465 7273 5b27  rid_parameters['
-00010450: 525f 6f76 6572 6c61 7027 5d0a 2020 2020  R_overlap'].    
-00010460: 2020 2020 2020 2020 656c 6966 206c 6973          elif lis
-00010470: 7428 6772 6964 5f70 6172 616d 6574 6572  t(grid_parameter
-00010480: 732e 6b65 7973 2829 295b 695d 3d3d 276c  s.keys())[i]=='l
-00010490: 696e 655f 6f76 6572 6c61 7027 3a0a 2020  ine_overlap':.  
-000104a0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-000104b0: 7220 6a20 696e 2072 616e 6765 286c 656e  r j in range(len
-000104c0: 2867 7269 645f 7061 7261 6d65 7465 7273  (grid_parameters
-000104d0: 5b27 6c69 6e65 5f6f 7665 726c 6170 275d  ['line_overlap']
-000104e0: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
-000104f0: 2020 2020 2020 2020 6c69 6e65 5f6f 7665          line_ove
-00010500: 726c 6170 5f6c 6973 745b 6a2c 3a5d 3d6e  rlap_list[j,:]=n
-00010510: 702e 6172 7261 7928 6772 6964 5f70 6172  p.array(grid_par
-00010520: 616d 6574 6572 735b 276c 696e 655f 6f76  ameters['line_ov
-00010530: 6572 6c61 7027 5d5b 6a5d 290a 2020 2020  erlap'][j]).    
-00010540: 2020 2020 2020 2020 656c 7365 3a20 7261          else: ra
-00010550: 6973 6520 4b65 7945 7272 6f72 2866 2755  ise KeyError(f'U
-00010560: 6e69 6465 6e74 6966 6965 6420 6772 6964  nidentified grid
-00010570: 2070 6172 616d 6574 6572 207b 6c69 7374   parameter {list
-00010580: 2867 7269 645f 7061 7261 6d65 7465 7273  (grid_parameters
-00010590: 2e6b 6579 7328 2929 5b69 5d7d 2729 0a20  .keys())[i]}'). 
-000105a0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000105b0: 2072 6169 7365 204b 6579 4572 726f 7228   raise KeyError(
-000105c0: 2743 6f6d 6269 6e61 7469 6f6e 2069 7320  'Combination is 
-000105d0: 7374 696c 6c20 6e6f 7420 7375 7070 6f72  still not suppor
-000105e0: 7465 6427 290a 0a20 2020 2069 6620 6e70  ted')..    if np
-000105f0: 2e73 756d 284e 746f 745f 6c69 7374 293d  .sum(Ntot_list)=
-00010600: 3d6e 6d6f 6465 6c73 3a0a 2020 2020 2020  =nmodels:.      
-00010610: 2020 6966 206e 6f74 2028 4e74 6f74 2020    if not (Ntot  
-00010620: 2020 2020 2020 6973 204e 6f6e 6529 3a0a        is None):.
-00010630: 2020 2020 2020 2020 2020 2020 4e74 6f74              Ntot
-00010640: 5f6c 6973 742a 3d4e 746f 740a 2020 2020  _list*=Ntot.    
-00010650: 2020 2020 2320 656c 7365 3a0a 2020 2020      # else:.    
-00010660: 2020 2020 2320 2020 2020 4e74 6f74 5f6c      #     Ntot_l
-00010670: 6973 742a 3d31 6531 350a 2020 2020 6966  ist*=1e15.    if
-00010680: 206e 702e 7375 6d28 5467 5f6c 6973 7429   np.sum(Tg_list)
-00010690: 3d3d 6e6d 6f64 656c 733a 0a20 2020 2020  ==nmodels:.     
-000106a0: 2020 2069 6620 6e6f 7420 2854 6720 2020     if not (Tg   
-000106b0: 2020 2020 2020 2069 7320 4e6f 6e65 293a         is None):
-000106c0: 0a20 2020 2020 2020 2020 2020 2054 675f  .            Tg_
-000106d0: 6c69 7374 2a3d 5467 0a20 2020 2020 2020  list*=Tg.       
-000106e0: 2023 2065 6c73 653a 0a20 2020 2020 2020   # else:.       
-000106f0: 2023 2020 2020 2054 675f 6c69 7374 2a3d   #     Tg_list*=
-00010700: 3130 300a 2020 2020 6966 206e 702e 7375  100.    if np.su
-00010710: 6d28 6e48 706c 7573 5f6c 6973 7429 3d3d  m(nHplus_list)==
-00010720: 6e6d 6f64 656c 733a 0a20 2020 2020 2020  nmodels:.       
-00010730: 2069 6620 6e6f 7420 286e 4870 6c75 7320   if not (nHplus 
-00010740: 2020 2020 2069 7320 4e6f 6e65 293a 0a20       is None):. 
-00010750: 2020 2020 2020 2020 2020 206e 4870 6c75             nHplu
-00010760: 735f 6c69 7374 2a3d 6e48 706c 7573 0a20  s_list*=nHplus. 
-00010770: 2020 2020 2020 2023 2065 6c73 653a 0a20         # else:. 
-00010780: 2020 2020 2020 2023 2020 2020 206e 4870         #     nHp
-00010790: 6c75 735f 6c69 7374 2a3d 3165 310a 2020  lus_list*=1e1.  
-000107a0: 2020 6966 206e 702e 7375 6d28 6e48 315f    if np.sum(nH1_
-000107b0: 6c69 7374 293d 3d6e 6d6f 6465 6c73 3a0a  list)==nmodels:.
-000107c0: 2020 2020 2020 2020 6966 206e 6f74 2028          if not (
-000107d0: 6e48 3120 2020 2020 2020 2020 6973 204e  nH1         is N
-000107e0: 6f6e 6529 3a0a 2020 2020 2020 2020 2020  one):.          
-000107f0: 2020 6e48 315f 6c69 7374 2a3d 6e48 310a    nH1_list*=nH1.
-00010800: 2020 2020 2020 2020 2320 656c 7365 3a0a          # else:.
-00010810: 2020 2020 2020 2020 2320 2020 2020 6e48          #     nH
-00010820: 315f 6c69 7374 2a3d 3165 3132 0a20 2020  1_list*=1e12.   
-00010830: 2069 6620 6e70 2e73 756d 286e 4832 5f6c   if np.sum(nH2_l
-00010840: 6973 7429 3d3d 6e6d 6f64 656c 733a 0a20  ist)==nmodels:. 
-00010850: 2020 2020 2020 2069 6620 6e6f 7420 286e         if not (n
-00010860: 4832 2020 2020 2020 2020 2069 7320 4e6f  H2         is No
-00010870: 6e65 293a 0a20 2020 2020 2020 2020 2020  ne):.           
-00010880: 206e 4832 5f6c 6973 742a 3d6e 4832 0a20   nH2_list*=nH2. 
-00010890: 2020 2020 2020 2023 2065 6c73 653a 0a20         # else:. 
-000108a0: 2020 2020 2020 2023 2020 2020 206e 4832         #     nH2
-000108b0: 5f6c 6973 742a 3d31 6531 320a 2020 2020  _list*=1e12.    
-000108c0: 6966 206e 702e 7375 6d28 6e48 655f 6c69  if np.sum(nHe_li
-000108d0: 7374 293d 3d6e 6d6f 6465 6c73 3a0a 2020  st)==nmodels:.  
-000108e0: 2020 2020 2020 6966 206e 6f74 2028 6e48        if not (nH
-000108f0: 6520 2020 2020 2020 2020 6973 204e 6f6e  e         is Non
-00010900: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
-00010910: 6e48 655f 6c69 7374 2a3d 6e48 650a 2020  nHe_list*=nHe.  
-00010920: 2020 2020 2020 2320 656c 7365 3a0a 2020        # else:.  
-00010930: 2020 2020 2020 2320 2020 2020 6e48 655f        #     nHe_
-00010940: 6c69 7374 2a3d 3165 3131 0a20 2020 2069  list*=1e11.    i
-00010950: 6620 6e70 2e73 756d 286e 656c 6563 5f6c  f np.sum(nelec_l
-00010960: 6973 7429 3d3d 6e6d 6f64 656c 733a 0a20  ist)==nmodels:. 
-00010970: 2020 2020 2020 2069 6620 6e6f 7420 286e         if not (n
-00010980: 656c 6563 2020 2020 2020 2069 7320 4e6f  elec       is No
-00010990: 6e65 293a 0a20 2020 2020 2020 2020 2020  ne):.           
-000109a0: 206e 656c 6563 5f6c 6973 742a 3d6e 656c   nelec_list*=nel
-000109b0: 6563 0a20 2020 2020 2020 2023 2065 6c73  ec.        # els
-000109c0: 653a 0a20 2020 2020 2020 2023 2020 2020  e:.        #    
-000109d0: 206e 656c 6563 5f6c 6973 742a 3d31 6538   nelec_list*=1e8
-000109e0: 0a20 2020 2069 6620 6e70 2e73 756d 2854  .    if np.sum(T
-000109f0: 645f 6c69 7374 293d 3d6e 6d6f 6465 6c73  d_list)==nmodels
-00010a00: 3a0a 2020 2020 2020 2020 6966 206e 6f74  :.        if not
-00010a10: 2028 5464 2020 2020 2020 2020 2020 6973   (Td          is
-00010a20: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
-00010a30: 2020 2020 5464 5f6c 6973 742a 3d54 640a      Td_list*=Td.
-00010a40: 2020 2020 2020 2020 2320 656c 7365 3a0a          # else:.
-00010a50: 2020 2020 2020 2020 2320 2020 2020 5464          #     Td
-00010a60: 5f6c 6973 742a 3d31 300a 2020 2020 6966  _list*=10.    if
-00010a70: 206e 702e 7375 6d28 7674 7572 625f 6c69   np.sum(vturb_li
-00010a80: 7374 293d 3d6e 6d6f 6465 6c73 3a0a 2020  st)==nmodels:.  
-00010a90: 2020 2020 2020 6966 206e 6f74 2028 7674        if not (vt
-00010aa0: 7572 6220 2020 2020 2020 6973 204e 6f6e  urb       is Non
-00010ab0: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
-00010ac0: 7674 7572 625f 6c69 7374 2a3d 7674 7572  vturb_list*=vtur
-00010ad0: 620a 2020 2020 2020 2020 2320 656c 7365  b.        # else
-00010ae0: 3a0a 2020 2020 2020 2020 2320 2020 2020  :.        #     
-00010af0: 7674 7572 625f 6c69 7374 2a3d 312e 340a  vturb_list*=1.4.
-00010b00: 2020 2020 6966 206e 702e 7375 6d28 6475      if np.sum(du
-00010b10: 7374 5f74 6f5f 6761 735f 6c69 7374 293d  st_to_gas_list)=
-00010b20: 3d6e 6d6f 6465 6c73 3a0a 2020 2020 2020  =nmodels:.      
-00010b30: 2020 6966 206e 6f74 2028 6475 7374 5f74    if not (dust_t
-00010b40: 6f5f 6761 7320 6973 204e 6f6e 6529 3a0a  o_gas is None):.
-00010b50: 2020 2020 2020 2020 2020 2020 6475 7374              dust
-00010b60: 5f74 6f5f 6761 735f 6c69 7374 2a3d 6475  _to_gas_list*=du
-00010b70: 7374 5f74 6f5f 6761 730a 2020 2020 2020  st_to_gas.      
-00010b80: 2020 2320 656c 7365 3a0a 2020 2020 2020    # else:.      
-00010b90: 2020 2320 2020 2020 6475 7374 5f74 6f5f    #     dust_to_
-00010ba0: 6761 735f 6c69 7374 2a3d 3165 2d32 310a  gas_list*=1e-21.
-00010bb0: 2020 2020 6966 206e 702e 7375 6d28 525f      if np.sum(R_
-00010bc0: 6f76 6572 6c61 705f 6c69 7374 293d 3d6e  overlap_list)==n
-00010bd0: 6d6f 6465 6c73 3a0a 2020 2020 2020 2020  models:.        
-00010be0: 6966 206e 6f74 2028 525f 6f76 6572 6c61  if not (R_overla
-00010bf0: 7020 6973 204e 6f6e 6529 3a0a 2020 2020  p is None):.    
-00010c00: 2020 2020 2020 2020 525f 6f76 6572 6c61          R_overla
-00010c10: 705f 6c69 7374 2a3d 525f 6f76 6572 6c61  p_list*=R_overla
-00010c20: 700a 2020 2020 2020 2020 2320 656c 7365  p.        # else
-00010c30: 3a0a 2020 2020 2020 2020 2320 2020 2020  :.        #     
-00010c40: 525f 6f76 6572 6c61 705f 6c69 7374 2a3d  R_overlap_list*=
-00010c50: 3165 350a 2020 2020 6966 206e 702e 7375  1e5.    if np.su
-00010c60: 6d28 6c69 6e65 5f6f 7665 726c 6170 5f6c  m(line_overlap_l
-00010c70: 6973 7429 3d3d 322a 6e6d 6f64 656c 733a  ist)==2*nmodels:
-00010c80: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00010c90: 286c 696e 655f 6f76 6572 6c61 7020 6973  (line_overlap is
-00010ca0: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
-00010cb0: 2020 2020 6c69 6e65 5f6f 7665 726c 6170      line_overlap
-00010cc0: 5f6c 6973 742a 3d6e 702e 6172 7261 7928  _list*=np.array(
-00010cd0: 6c69 6e65 5f6f 7665 726c 6170 290a 2020  line_overlap).  
-00010ce0: 2020 2020 2020 2320 656c 7365 3a0a 2020        # else:.  
-00010cf0: 2020 2020 2020 2320 2020 2020 6c69 6e65        #     line
-00010d00: 5f6f 7665 726c 6170 5f6c 6973 742a 3d6e  _overlap_list*=n
-00010d10: 702e 6172 7261 7928 2834 2c33 3029 290a  p.array((4,30)).
-00010d20: 0a20 2020 206f 732e 7379 7374 656d 2866  .    os.system(f
-00010d30: 2774 6f75 6368 207b 6469 7265 6374 6f72  'touch {director
-00010d40: 792b 222f 536c 6162 496e 7075 742e 696e  y+"/SlabInput.in
-00010d50: 227d 2729 0a20 2020 2066 3d6f 7065 6e28  "}').    f=open(
-00010d60: 6469 7265 6374 6f72 792b 272f 536c 6162  directory+'/Slab
-00010d70: 496e 7075 742e 696e 272c 2777 2729 0a20  Input.in','w'). 
-00010d80: 2020 2066 2e77 7269 7465 2822 2a2a 2a2a     f.write("****
-00010d90: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00010da0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00010db0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00010dc0: 2a2a 2a2a 2a2a 2a5c 6e22 290a 2020 2020  *******\n").    
-00010dd0: 662e 7772 6974 6528 222a 2a2a 2049 6e70  f.write("*** Inp
-00010de0: 7574 2066 696c 6520 666f 7220 736c 6162  ut file for slab
-00010df0: 2065 7363 6170 6520 7072 6f62 6162 696c   escape probabil
-00010e00: 6974 7920 7769 7468 2050 726f 4469 4d6f  ity with ProDiMo
-00010e10: 202a 2a2a 5c6e 2229 0a20 2020 2066 2e77   ***\n").    f.w
-00010e20: 7269 7465 2822 2a2a 2a2a 2a2a 2a2a 2a2a  rite("**********
-00010e30: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00010e40: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00010e50: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00010e60: 2a5c 6e22 290a 2020 2020 662e 7772 6974  *\n").    f.writ
-00010e70: 6528 222a 2a2a 206e 6d6f 6465 6c73 2073  e("*** nmodels s
-00010e80: 686f 756c 6420 666f 6c6c 6f77 206f 7574  hould follow out
-00010e90: 7075 745f 6669 6c65 6e61 6d65 202a 2a2a  put_filename ***
-00010ea0: 5c6e 2229 0a20 2020 2066 2e77 7269 7465  \n").    f.write
-00010eb0: 2866 277b 6f75 7470 7574 5f66 696c 656e  (f'{output_filen
-00010ec0: 616d 657d 2021 206f 7574 7075 745f 6669  ame} ! output_fi
-00010ed0: 6c65 6e61 6d65 5c6e 2729 0a20 2020 2066  lename\n').    f
-00010ee0: 2e77 7269 7465 2866 277b 6f76 6572 6c61  .write(f'{overla
-00010ef0: 705f 6669 6c65 6e61 6d65 7d20 2120 6f76  p_filename} ! ov
-00010f00: 6572 6c61 705f 6669 6c65 6e61 6d65 5c6e  erlap_filename\n
-00010f10: 2729 0a20 2020 2069 6620 7365 7061 7261  ').    if separa
-00010f20: 7465 5f6f 705f 6669 6c65 733a 0a20 2020  te_op_files:.   
-00010f30: 2020 2020 2066 2e77 7269 7465 2827 2e74       f.write('.t
-00010f40: 7275 652e 2020 2020 2120 7365 7061 7261  rue.    ! separa
-00010f50: 7465 5f6f 705f 6669 6c65 735c 6e27 290a  te_op_files\n').
-00010f60: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00010f70: 2020 662e 7772 6974 6528 272e 6661 6c73    f.write('.fals
-00010f80: 652e 2020 2021 2073 6570 6172 6174 655f  e.   ! separate_
-00010f90: 6f70 5f66 696c 6573 5c6e 2729 0a20 2020  op_files\n').   
-00010fa0: 2069 6620 6669 7473 5f6f 705f 6669 6c65   if fits_op_file
-00010fb0: 733a 0a20 2020 2020 2020 2066 2e77 7269  s:.        f.wri
-00010fc0: 7465 2827 2e74 7275 652e 2020 2020 2120  te('.true.    ! 
-00010fd0: 6669 7473 5f6f 705f 6669 6c65 735c 6e27  fits_op_files\n'
-00010fe0: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
-00010ff0: 2020 2020 662e 7772 6974 6528 272e 6661      f.write('.fa
-00011000: 6c73 652e 2020 2021 2066 6974 735f 6f70  lse.   ! fits_op
-00011010: 5f66 696c 6573 5c6e 2729 0a20 2020 2069  _files\n').    i
-00011020: 6620 6e6f 5f69 6e64 6976 6964 7561 6c5f  f no_individual_
-00011030: 6c69 6e65 733a 0a20 2020 2020 2020 2066  lines:.        f
-00011040: 2e77 7269 7465 2827 2e74 7275 652e 2020  .write('.true.  
-00011050: 2020 2120 6e6f 5f69 6e64 6976 6964 7561    ! no_individua
-00011060: 6c5f 6c69 6e65 735c 6e27 290a 2020 2020  l_lines\n').    
-00011070: 656c 7365 3a0a 2020 2020 2020 2020 662e  else:.        f.
-00011080: 7772 6974 6528 272e 6661 6c73 652e 2020  write('.false.  
-00011090: 2021 206e 6f5f 696e 6469 7669 6475 616c   ! no_individual
-000110a0: 5f6c 696e 6573 5c6e 2729 0a20 2020 2069  _lines\n').    i
-000110b0: 6620 736c 6162 5f52 543a 0a20 2020 2020  f slab_RT:.     
-000110c0: 2020 2066 2e77 7269 7465 2827 2e74 7275     f.write('.tru
-000110d0: 652e 2020 2020 2120 736c 6162 5f52 5420  e.    ! slab_RT 
-000110e0: 5c6e 2729 0a20 2020 2065 6c73 653a 0a20  \n').    else:. 
-000110f0: 2020 2020 2020 2066 2e77 7269 7465 2827         f.write('
-00011100: 2e66 616c 7365 2e20 2020 2120 736c 6162  .false.   ! slab
-00011110: 5f52 5420 5c6e 2729 0a20 2020 2069 6620  _RT \n').    if 
-00011120: 7368 6f72 745f 666f 726d 6174 3a0a 2020  short_format:.  
-00011130: 2020 2020 2020 662e 7772 6974 6528 272e        f.write('.
-00011140: 7472 7565 2e20 2020 2021 2073 686f 7274  true.    ! short
-00011150: 5f66 6f72 6d61 745c 6e27 290a 2020 2020  _format\n').    
-00011160: 656c 7365 3a0a 2020 2020 2020 2020 662e  else:.        f.
-00011170: 7772 6974 6528 272e 6661 6c73 652e 2020  write('.false.  
-00011180: 2021 2073 686f 7274 5f66 6f72 6d61 745c   ! short_format\
-00011190: 6e27 290a 2020 2020 662e 7772 6974 6528  n').    f.write(
-000111a0: 6627 7b6e 6d6f 6465 6c73 7d20 2020 2020  f'{nmodels}     
-000111b0: 2020 2020 2020 2020 2120 6e6d 6f64 656c          ! nmodel
-000111c0: 735c 6e27 290a 2020 2020 662e 7772 6974  s\n').    f.writ
-000111d0: 6528 272d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  e('-------------
-000111e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000111f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00011200: 2d2d 2d2d 2d2d 2d2d 2d2d 2729 0a20 2020  ----------').   
-00011210: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-00011220: 6e6d 6f64 656c 7329 3a0a 2020 2020 2020  nmodels):.      
-00011230: 2020 662e 7772 6974 6528 6627 5c6e 2a2a    f.write(f'\n**
-00011240: 2a20 6d6f 6465 6c20 7b69 2b31 7d20 2a2a  * model {i+1} **
-00011250: 2a5c 6e27 290a 2020 2020 2020 2020 6966  *\n').        if
-00011260: 206e 702e 7375 6d28 4e74 6f74 5f6c 6973   np.sum(Ntot_lis
-00011270: 7429 213d 6e6d 6f64 656c 733a 0a20 2020  t)!=nmodels:.   
-00011280: 2020 2020 2020 2020 2066 2e77 7269 7465           f.write
-00011290: 2866 6d74 2e66 6f72 6d61 7428 277b 3a2e  (fmt.format('{:.
-000112a0: 336d 7d27 2c4e 746f 745f 6c69 7374 5b69  3m}',Ntot_list[i
-000112b0: 5d29 290a 2020 2020 2020 2020 2020 2020  ])).            
-000112c0: 662e 7772 6974 6528 2709 2020 2021 204e  f.write('.   ! N
-000112d0: 4874 6f74 2020 5b63 6d5e 2d32 5d20 746f  Htot  [cm^-2] to
-000112e0: 7461 6c20 6761 7320 636f 6c75 6d6e 2064  tal gas column d
-000112f0: 656e 7369 7479 5c6e 2729 0a20 2020 2020  ensity\n').     
-00011300: 2020 2069 6620 6e70 2e73 756d 286e 4870     if np.sum(nHp
-00011310: 6c75 735f 6c69 7374 2921 3d6e 6d6f 6465  lus_list)!=nmode
-00011320: 6c73 3a0a 2020 2020 2020 2020 2020 2020  ls:.            
-00011330: 662e 7772 6974 6528 666d 742e 666f 726d  f.write(fmt.form
-00011340: 6174 2827 7b3a 2e33 6d7d 272c 6e48 706c  at('{:.3m}',nHpl
-00011350: 7573 5f6c 6973 745b 695d 2929 0a20 2020  us_list[i])).   
-00011360: 2020 2020 2020 2020 2066 2e77 7269 7465           f.write
-00011370: 2827 0920 2020 2120 6e48 2b20 2020 205b  ('.   ! nH+    [
-00011380: 636d 5e2d 335d 2020 7072 6f74 6f6e 206e  cm^-3]  proton n
-00011390: 756d 6265 7220 6465 6e73 6974 795c 6e27  umber density\n'
-000113a0: 290a 2020 2020 2020 2020 6966 206e 702e  ).        if np.
-000113b0: 7375 6d28 6e48 315f 6c69 7374 2921 3d6e  sum(nH1_list)!=n
-000113c0: 6d6f 6465 6c73 3a0a 2020 2020 2020 2020  models:.        
-000113d0: 2020 2020 662e 7772 6974 6528 666d 742e      f.write(fmt.
-000113e0: 666f 726d 6174 2827 7b3a 2e33 6d7d 272c  format('{:.3m}',
-000113f0: 6e48 315f 6c69 7374 5b69 5d29 290a 2020  nH1_list[i])).  
-00011400: 2020 2020 2020 2020 2020 662e 7772 6974            f.writ
-00011410: 6528 2709 2020 2021 206e 4849 0920 5b63  e('.   ! nHI. [c
-00011420: 6d5e 2d33 5d20 6174 6f6d 6963 2068 7964  m^-3] atomic hyd
-00011430: 726f 6765 6e5c 6e27 290a 2020 2020 2020  rogen\n').      
-00011440: 2020 6966 206e 702e 7375 6d28 6e48 325f    if np.sum(nH2_
-00011450: 6c69 7374 2921 3d6e 6d6f 6465 6c73 3a0a  list)!=nmodels:.
-00011460: 2020 2020 2020 2020 2020 2020 662e 7772              f.wr
-00011470: 6974 6528 666d 742e 666f 726d 6174 2827  ite(fmt.format('
-00011480: 7b3a 2e33 6d7d 272c 6e48 325f 6c69 7374  {:.3m}',nH2_list
-00011490: 5b69 5d29 290a 2020 2020 2020 2020 2020  [i])).          
-000114a0: 2020 662e 7772 6974 6528 2709 2020 2021    f.write('.   !
-000114b0: 206e 4832 2020 2020 5b63 6d5e 2d33 5d20   nH2    [cm^-3] 
-000114c0: 2020 6d6f 6c65 6375 6c61 7220 6879 6472    molecular hydr
-000114d0: 6f67 656e 5c6e 2729 0a20 2020 2020 2020  ogen\n').       
-000114e0: 2069 6620 6e70 2e73 756d 286e 4865 5f6c   if np.sum(nHe_l
-000114f0: 6973 7429 213d 6e6d 6f64 656c 733a 0a20  ist)!=nmodels:. 
-00011500: 2020 2020 2020 2020 2020 2066 2e77 7269             f.wri
-00011510: 7465 2866 6d74 2e66 6f72 6d61 7428 277b  te(fmt.format('{
-00011520: 3a2e 336d 7d27 2c6e 4865 5f6c 6973 745b  :.3m}',nHe_list[
-00011530: 695d 2929 0a20 2020 2020 2020 2020 2020  i])).           
-00011540: 2066 2e77 7269 7465 2827 0920 2020 2120   f.write('.   ! 
-00011550: 6e48 6520 2020 205b 636d 5e2d 335d 2020  nHe    [cm^-3]  
-00011560: 2048 656c 6975 6d5c 6e27 290a 2020 2020   Helium\n').    
-00011570: 2020 2020 6966 206e 702e 7375 6d28 6e65      if np.sum(ne
-00011580: 6c65 635f 6c69 7374 2921 3d6e 6d6f 6465  lec_list)!=nmode
-00011590: 6c73 3a0a 2020 2020 2020 2020 2020 2020  ls:.            
-000115a0: 662e 7772 6974 6528 666d 742e 666f 726d  f.write(fmt.form
-000115b0: 6174 2827 7b3a 2e33 6d7d 272c 6e65 6c65  at('{:.3m}',nele
-000115c0: 635f 6c69 7374 5b69 5d29 290a 2020 2020  c_list[i])).    
-000115d0: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
-000115e0: 2709 2020 2021 206e 656c 6563 2020 5b63  '.   ! nelec  [c
-000115f0: 6d5e 2d33 5d20 2020 656c 6563 7472 6f6e  m^-3]   electron
-00011600: 206e 756d 6265 7220 6465 6e73 6974 795c   number density\
-00011610: 6e27 290a 2020 2020 2020 2020 6966 206e  n').        if n
-00011620: 702e 7375 6d28 5467 5f6c 6973 7429 213d  p.sum(Tg_list)!=
-00011630: 6e6d 6f64 656c 733a 0a20 2020 2020 2020  nmodels:.       
-00011640: 2020 2020 2066 2e77 7269 7465 2866 6d74       f.write(fmt
-00011650: 2e66 6f72 6d61 7428 277b 3a2e 336d 7d27  .format('{:.3m}'
-00011660: 2c54 675f 6c69 7374 5b69 5d29 290a 2020  ,Tg_list[i])).  
-00011670: 2020 2020 2020 2020 2020 662e 7772 6974            f.writ
-00011680: 6528 2709 2020 2021 2054 6761 7320 5b4b  e('.   ! Tgas [K
-00011690: 5d20 2020 2020 2020 2020 2020 6761 7320  ]           gas 
-000116a0: 7465 6d70 6572 6174 7572 655c 6e27 290a  temperature\n').
-000116b0: 2020 2020 2020 2020 6966 206e 702e 7375          if np.su
-000116c0: 6d28 5464 5f6c 6973 7429 213d 6e6d 6f64  m(Td_list)!=nmod
-000116d0: 656c 733a 0a20 2020 2020 2020 2020 2020  els:.           
-000116e0: 2066 2e77 7269 7465 2866 6d74 2e66 6f72   f.write(fmt.for
-000116f0: 6d61 7428 277b 3a2e 336d 7d27 2c54 645f  mat('{:.3m}',Td_
-00011700: 6c69 7374 5b69 5d29 290a 2020 2020 2020  list[i])).      
-00011710: 2020 2020 2020 662e 7772 6974 6528 2709        f.write('.
-00011720: 2020 2021 2054 6475 7374 205b 4b5d 2020     ! Tdust [K]  
-00011730: 2020 2020 2020 2020 2064 7573 7420 7465           dust te
-00011740: 6d70 6572 6174 7572 655c 6e27 290a 2020  mperature\n').  
-00011750: 2020 2020 2020 6966 206e 702e 7375 6d28        if np.sum(
-00011760: 7674 7572 625f 6c69 7374 2921 3d6e 6d6f  vturb_list)!=nmo
-00011770: 6465 6c73 3a0a 2020 2020 2020 2020 2020  dels:.          
-00011780: 2020 662e 7772 6974 6528 666d 742e 666f    f.write(fmt.fo
-00011790: 726d 6174 2827 7b3a 2e33 6d7d 272c 7674  rmat('{:.3m}',vt
-000117a0: 7572 625f 6c69 7374 5b69 5d29 290a 2020  urb_list[i])).  
-000117b0: 2020 2020 2020 2020 2020 662e 7772 6974            f.writ
-000117c0: 6528 2709 2020 2021 2076 7475 7262 2020  e('.   ! vturb  
-000117d0: 5b6b 6d73 2f73 5d20 2020 2074 7572 6275  [kms/s]    turbu
-000117e0: 6c65 6e74 2076 656c 6f63 6974 795c 6e27  lent velocity\n'
-000117f0: 290a 2020 2020 2020 2020 6966 206e 702e  ).        if np.
-00011800: 7375 6d28 6475 7374 5f74 6f5f 6761 735f  sum(dust_to_gas_
-00011810: 6c69 7374 2921 3d6e 6d6f 6465 6c73 3a0a  list)!=nmodels:.
-00011820: 2020 2020 2020 2020 2020 2020 662e 7772              f.wr
-00011830: 6974 6528 666d 742e 666f 726d 6174 2827  ite(fmt.format('
-00011840: 7b3a 2e33 6d7d 272c 6475 7374 5f74 6f5f  {:.3m}',dust_to_
-00011850: 6761 735f 6c69 7374 5b69 5d29 290a 2020  gas_list[i])).  
-00011860: 2020 2020 2020 2020 2020 662e 7772 6974            f.writ
-00011870: 6528 2709 2020 2021 2064 7573 745f 746f  e('.   ! dust_to
-00011880: 5f67 6173 5c6e 2729 0a20 2020 2020 2020  _gas\n').       
-00011890: 2069 6620 6e70 2e73 756d 286c 696e 655f   if np.sum(line_
-000118a0: 6f76 6572 6c61 705f 6c69 7374 2921 3d32  overlap_list)!=2
-000118b0: 2a6e 6d6f 6465 6c73 3a0a 2020 2020 2020  *nmodels:.      
-000118c0: 2020 2020 2020 662e 7772 6974 6528 666d        f.write(fm
-000118d0: 742e 666f 726d 6174 2827 7b3a 2e33 667d  t.format('{:.3f}
-000118e0: 272c 6c69 6e65 5f6f 7665 726c 6170 5f6c  ',line_overlap_l
-000118f0: 6973 745b 692c 305d 292b 2720 272b 666d  ist[i,0])+' '+fm
-00011900: 742e 666f 726d 6174 2827 7b3a 2e33 667d  t.format('{:.3f}
-00011910: 272c 6c69 6e65 5f6f 7665 726c 6170 5f6c  ',line_overlap_l
-00011920: 6973 745b 692c 315d 2929 0a20 2020 2020  ist[i,1])).     
-00011930: 2020 2020 2020 2066 2e77 7269 7465 2827         f.write('
-00011940: 0920 2020 2120 6c69 6e65 5f6f 7665 726c  .   ! line_overl
-00011950: 6170 2020 5b6d 6963 726f 6e73 5d20 206d  ap  [microns]  m
-00011960: 696e 696d 756d 2061 6e64 206d 6178 696d  inimum and maxim
-00011970: 756d 2077 6176 656c 656e 6774 6873 2066  um wavelengths f
-00011980: 6f72 206c 696e 6520 6f76 6572 6c61 705c  or line overlap\
-00011990: 6e27 290a 2020 2020 2020 2020 6966 206e  n').        if n
-000119a0: 702e 7375 6d28 525f 6f76 6572 6c61 705f  p.sum(R_overlap_
-000119b0: 6c69 7374 2921 3d6e 6d6f 6465 6c73 3a0a  list)!=nmodels:.
-000119c0: 2020 2020 2020 2020 2020 2020 662e 7772              f.wr
-000119d0: 6974 6528 666d 742e 666f 726d 6174 2827  ite(fmt.format('
-000119e0: 7b3a 2e33 6d7d 272c 525f 6f76 6572 6c61  {:.3m}',R_overla
-000119f0: 705f 6c69 7374 5b69 5d29 290a 2020 2020  p_list[i])).    
-00011a00: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
-00011a10: 2709 2020 2021 2052 5f6f 7665 726c 6170  '.   ! R_overlap
-00011a20: 2020 7361 6d70 6c69 6e67 2067 7269 6420    sampling grid 
-00011a30: 7265 736f 6c75 7469 6f6e 2066 6f72 206c  resolution for l
-00011a40: 696e 6520 6f76 6572 6c61 705c 6e27 290a  ine overlap\n').
-00011a50: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
-00011a60: 6627 7b6c 656e 2873 7065 6369 6573 5f6c  f'{len(species_l
-00011a70: 6973 7429 7d09 2020 2021 204e 7370 6563  ist)}.   ! Nspec
-00011a80: 6965 7320 2020 2020 2020 2020 2020 206e  ies            n
-00011a90: 756d 6265 7220 6f66 2073 7065 6369 6573  umber of species
-00011aa0: 2066 6f72 2074 6861 7420 6d6f 6465 6c5c   for that model\
-00011ab0: 6e27 290a 2020 2020 2020 2020 666f 7220  n').        for 
-00011ac0: 6a20 696e 2072 616e 6765 286c 656e 2873  j in range(len(s
-00011ad0: 7065 6369 6573 5f6c 6973 7429 293a 0a20  pecies_list)):. 
-00011ae0: 2020 2020 2020 2020 2020 2066 2e77 7269             f.wri
-00011af0: 7465 2866 277b 6c69 7374 2873 7065 6369  te(f'{list(speci
-00011b00: 6573 5f6c 6973 742e 6b65 7973 2829 295b  es_list.keys())[
-00011b10: 6a5d 7d20 2020 2020 207b 7370 6563 6965  j]}      {specie
-00011b20: 735f 6c69 7374 5b6c 6973 7428 7370 6563  s_list[list(spec
-00011b30: 6965 735f 6c69 7374 2e6b 6579 7328 2929  ies_list.keys())
-00011b40: 5b6a 5d5d 7d5c 6e27 290a 2020 2020 2020  [j]]}\n').      
-00011b50: 2020 662e 7772 6974 6528 2720 2020 2020    f.write('     
-00011b60: 2020 2020 2020 2120 656e 645c 6e27 290a        ! end\n').
-00011b70: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
-00011b80: 272d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  '---------------
-00011b90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00011ba0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00011bb0: 2d2d 2d2d 2d2d 2d2d 2729 0a20 2020 2066  --------').    f
-00011bc0: 2e63 6c6f 7365 2829 0a20 2020 2072 6574  .close().    ret
-00011bd0: 7572 6e0a 0a0a 6465 6620 6765 6e65 7261  urn...def genera
-00011be0: 7465 5f31 445f 7374 7275 6374 7572 6528  te_1D_structure(
-00011bf0: 647a 2c73 7065 6369 6573 5f6c 6973 742c  dz,species_list,
-00011c00: 7674 7572 622c 6e64 2c54 642c 6e5f 7370  vturb,nd,Td,n_sp
-00011c10: 6563 6965 732c 545f 7370 6563 6965 732c  ecies,T_species,
-00011c20: 6e48 323d 302c 6e48 493d 302c 6e48 4949  nH2=0,nHI=0,nHII
-00011c30: 3d30 2c6e 4865 3d30 2c6e 656c 6563 3d30  =0,nHe=0,nelec=0
-00011c40: 2c66 696c 656e 616d 653d 2731 445f 7374  ,filename='1D_st
-00011c50: 7275 6374 7572 6527 293a 0a20 2020 2022  ructure'):.    "
-00011c60: 2222 0a20 2020 2047 656e 6572 6174 6573  "".    Generates
-00011c70: 2031 4420 7374 7275 6374 7572 6520 6669   1D structure fi
-00011c80: 6c65 2072 6571 7569 7265 6420 666f 7220  le required for 
-00011c90: 3144 2073 6c61 6220 6d6f 6465 6c73 0a20  1D slab models. 
-00011ca0: 2020 2022 2222 0a20 2020 2069 6620 6973     """.    if is
-00011cb0: 696e 7374 616e 6365 2864 7a2c 666c 6f61  instance(dz,floa
-00011cc0: 7429 206f 7220 6973 696e 7374 616e 6365  t) or isinstance
-00011cd0: 2864 7a2c 696e 7429 3a20 647a 3d6e 702e  (dz,int): dz=np.
-00011ce0: 6172 7261 7928 5b64 7a5d 290a 2020 2020  array([dz]).    
-00011cf0: 6966 2069 7369 6e73 7461 6e63 6528 647a  if isinstance(dz
-00011d00: 2c6c 6973 7429 3a20 647a 3d6e 702e 6172  ,list): dz=np.ar
-00011d10: 7261 7928 647a 290a 2020 2020 6966 2069  ray(dz).    if i
-00011d20: 7369 6e73 7461 6e63 6528 7370 6563 6965  sinstance(specie
-00011d30: 735f 6c69 7374 2c73 7472 293a 2073 7065  s_list,str): spe
-00011d40: 6369 6573 5f6c 6973 743d 5b73 7065 6369  cies_list=[speci
-00011d50: 6573 5f6c 6973 745d 0a20 2020 2069 6620  es_list].    if 
-00011d60: 6973 696e 7374 616e 6365 2876 7475 7262  isinstance(vturb
-00011d70: 2c66 6c6f 6174 2920 6f72 2069 7369 6e73  ,float) or isins
-00011d80: 7461 6e63 6528 7674 7572 622c 696e 7429  tance(vturb,int)
-00011d90: 3a20 7674 7572 623d 6e70 2e6f 6e65 735f  : vturb=np.ones_
-00011da0: 6c69 6b65 2864 7a29 2a76 7475 7262 0a20  like(dz)*vturb. 
-00011db0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-00011dc0: 286e 642c 666c 6f61 7429 206f 7220 6973  (nd,float) or is
-00011dd0: 696e 7374 616e 6365 286e 642c 696e 7429  instance(nd,int)
-00011de0: 3a20 6e64 3d6e 702e 6f6e 6573 5f6c 696b  : nd=np.ones_lik
-00011df0: 6528 647a 292a 6e64 0a20 2020 2069 6620  e(dz)*nd.    if 
-00011e00: 6973 696e 7374 616e 6365 2854 642c 666c  isinstance(Td,fl
-00011e10: 6f61 7429 206f 7220 6973 696e 7374 616e  oat) or isinstan
-00011e20: 6365 2854 642c 696e 7429 3a20 5464 3d6e  ce(Td,int): Td=n
-00011e30: 702e 6f6e 6573 5f6c 696b 6528 647a 292a  p.ones_like(dz)*
-00011e40: 5464 0a20 2020 2069 6620 6973 696e 7374  Td.    if isinst
-00011e50: 616e 6365 286e 4832 2c66 6c6f 6174 2920  ance(nH2,float) 
-00011e60: 6f72 2069 7369 6e73 7461 6e63 6528 6e48  or isinstance(nH
-00011e70: 322c 696e 7429 3a20 6e48 323d 6e70 2e6f  2,int): nH2=np.o
-00011e80: 6e65 735f 6c69 6b65 2864 7a29 2a6e 4832  nes_like(dz)*nH2
-00011e90: 0a20 2020 2069 6620 6973 696e 7374 616e  .    if isinstan
-00011ea0: 6365 286e 4849 2c66 6c6f 6174 2920 6f72  ce(nHI,float) or
-00011eb0: 2069 7369 6e73 7461 6e63 6528 6e48 492c   isinstance(nHI,
-00011ec0: 696e 7429 3a20 6e48 493d 6e70 2e6f 6e65  int): nHI=np.one
-00011ed0: 735f 6c69 6b65 2864 7a29 2a6e 4849 0a20  s_like(dz)*nHI. 
-00011ee0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-00011ef0: 286e 4849 492c 666c 6f61 7429 206f 7220  (nHII,float) or 
-00011f00: 6973 696e 7374 616e 6365 286e 4849 492c  isinstance(nHII,
-00011f10: 696e 7429 3a20 6e48 4949 3d6e 702e 6f6e  int): nHII=np.on
-00011f20: 6573 5f6c 696b 6528 647a 292a 6e48 4949  es_like(dz)*nHII
-00011f30: 0a20 2020 2069 6620 6973 696e 7374 616e  .    if isinstan
-00011f40: 6365 286e 4865 2c66 6c6f 6174 2920 6f72  ce(nHe,float) or
-00011f50: 2069 7369 6e73 7461 6e63 6528 6e48 652c   isinstance(nHe,
-00011f60: 696e 7429 3a20 6e48 653d 6e70 2e6f 6e65  int): nHe=np.one
-00011f70: 735f 6c69 6b65 2864 7a29 2a6e 4865 0a20  s_like(dz)*nHe. 
-00011f80: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-00011f90: 286e 656c 6563 2c66 6c6f 6174 2920 6f72  (nelec,float) or
-00011fa0: 2069 7369 6e73 7461 6e63 6528 6e65 6c65   isinstance(nele
-00011fb0: 632c 696e 7429 3a20 6e65 6c65 633d 6e70  c,int): nelec=np
-00011fc0: 2e6f 6e65 735f 6c69 6b65 2864 7a29 2a6e  .ones_like(dz)*n
-00011fd0: 656c 6563 0a20 2020 2069 6620 6973 696e  elec.    if isin
-00011fe0: 7374 616e 6365 286e 5f73 7065 6369 6573  stance(n_species
-00011ff0: 2c66 6c6f 6174 2920 6f72 2069 7369 6e73  ,float) or isins
-00012000: 7461 6e63 6528 6e5f 7370 6563 6965 732c  tance(n_species,
-00012010: 696e 7429 3a20 6e5f 7370 6563 6965 733d  int): n_species=
-00012020: 6e70 2e6f 6e65 7328 2864 7a2e 7368 6170  np.ones((dz.shap
-00012030: 655b 305d 2c6c 656e 2873 7065 6369 6573  e[0],len(species
-00012040: 5f6c 6973 7429 2929 2a6e 5f73 7065 6369  _list)))*n_speci
-00012050: 6573 0a20 2020 2069 6620 6973 696e 7374  es.    if isinst
-00012060: 616e 6365 2854 5f73 7065 6369 6573 2c66  ance(T_species,f
-00012070: 6c6f 6174 2920 6f72 2069 7369 6e73 7461  loat) or isinsta
-00012080: 6e63 6528 545f 7370 6563 6965 732c 696e  nce(T_species,in
-00012090: 7429 3a20 545f 7370 6563 6965 733d 6e70  t): T_species=np
-000120a0: 2e6f 6e65 7328 2864 7a2e 7368 6170 655b  .ones((dz.shape[
-000120b0: 305d 2c6c 656e 2873 7065 6369 6573 5f6c  0],len(species_l
-000120c0: 6973 7429 2929 2a54 5f73 7065 6369 6573  ist)))*T_species
-000120d0: 0a20 2020 2069 6620 6973 696e 7374 616e  .    if isinstan
-000120e0: 6365 2854 5f73 7065 6369 6573 2c6c 6973  ce(T_species,lis
-000120f0: 7429 3a20 545f 7370 6563 6965 733d 6e70  t): T_species=np
-00012100: 2e61 7272 6179 2854 5f73 7065 6369 6573  .array(T_species
-00012110: 290a 2020 2020 6966 2069 7369 6e73 7461  ).    if isinsta
-00012120: 6e63 6528 6e5f 7370 6563 6965 732c 6c69  nce(n_species,li
-00012130: 7374 293a 206e 5f73 7065 6369 6573 3d6e  st): n_species=n
-00012140: 702e 6172 7261 7928 6e5f 7370 6563 6965  p.array(n_specie
-00012150: 7329 0a20 2020 2069 6620 6e70 2e61 7272  s).    if np.arr
-00012160: 6179 2854 5f73 7065 6369 6573 292e 7369  ay(T_species).si
-00012170: 7a65 3d3d 6c65 6e28 7370 6563 6965 735f  ze==len(species_
-00012180: 6c69 7374 293a 0a20 2020 2020 2020 2054  list):.        T
-00012190: 5f73 7065 6369 6573 5f74 656d 703d 6e70  _species_temp=np
-000121a0: 2e6f 6e65 7328 2864 7a2e 7368 6170 655b  .ones((dz.shape[
-000121b0: 305d 2c6c 656e 2873 7065 6369 6573 5f6c  0],len(species_l
-000121c0: 6973 7429 2929 0a20 2020 2020 2020 2066  ist))).        f
-000121d0: 6f72 2069 2069 6e20 7261 6e67 6528 6c65  or i in range(le
-000121e0: 6e28 7370 6563 6965 735f 6c69 7374 2929  n(species_list))
-000121f0: 3a0a 2020 2020 2020 2020 2020 2020 545f  :.            T_
-00012200: 7370 6563 6965 735f 7465 6d70 5b3a 2c69  species_temp[:,i
-00012210: 5d3d 545f 7370 6563 6965 735b 695d 0a20  ]=T_species[i]. 
-00012220: 2020 2020 2020 2054 5f73 7065 6369 6573         T_species
-00012230: 3d54 5f73 7065 6369 6573 5f74 656d 702a  =T_species_temp*
-00012240: 312e 3030 0a20 2020 2069 6620 6e70 2e61  1.00.    if np.a
-00012250: 7272 6179 286e 5f73 7065 6369 6573 292e  rray(n_species).
-00012260: 7369 7a65 3d3d 6c65 6e28 7370 6563 6965  size==len(specie
-00012270: 735f 6c69 7374 293a 0a20 2020 2020 2020  s_list):.       
-00012280: 206e 5f73 7065 6369 6573 5f74 656d 703d   n_species_temp=
-00012290: 6e70 2e6f 6e65 7328 2864 7a2e 7368 6170  np.ones((dz.shap
-000122a0: 655b 305d 2c6c 656e 2873 7065 6369 6573  e[0],len(species
-000122b0: 5f6c 6973 7429 2929 0a20 2020 2020 2020  _list))).       
-000122c0: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-000122d0: 6c65 6e28 7370 6563 6965 735f 6c69 7374  len(species_list
-000122e0: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
-000122f0: 6e5f 7370 6563 6965 735f 7465 6d70 5b3a  n_species_temp[:
-00012300: 2c69 5d3d 6e5f 7370 6563 6965 735b 695d  ,i]=n_species[i]
-00012310: 0a20 2020 2020 2020 206e 5f73 7065 6369  .        n_speci
-00012320: 6573 3d6e 5f73 7065 6369 6573 5f74 656d  es=n_species_tem
-00012330: 702a 312e 3030 0a0a 2020 2020 7769 7468  p*1.00..    with
-00012340: 206f 7065 6e28 6669 6c65 6e61 6d65 2c27   open(filename,'
-00012350: 7727 2920 6173 2066 3a0a 2020 2020 2020  w') as f:.      
-00012360: 2020 662e 7772 6974 6528 6627 7b6c 656e    f.write(f'{len
-00012370: 2864 7a29 3a64 7d5c 6e27 290a 2020 2020  (dz):d}\n').    
-00012380: 2020 2020 662e 7772 6974 6528 6627 7b6c      f.write(f'{l
-00012390: 656e 2873 7065 6369 6573 5f6c 6973 7429  en(species_list)
-000123a0: 3a64 7d5c 6e27 290a 2020 2020 2020 2020  :d}\n').        
-000123b0: 666f 7220 6920 696e 2072 616e 6765 286c  for i in range(l
-000123c0: 656e 2873 7065 6369 6573 5f6c 6973 7429  en(species_list)
-000123d0: 293a 0a20 2020 2020 2020 2020 2020 2066  ):.            f
-000123e0: 2e77 7269 7465 2873 7065 6369 6573 5f6c  .write(species_l
-000123f0: 6973 745b 695d 2b27 5c6e 2729 0a20 2020  ist[i]+'\n').   
-00012400: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
-00012410: 6e67 6528 6c65 6e28 647a 2929 3a0a 2020  nge(len(dz)):.  
-00012420: 2020 2020 2020 2020 2020 7374 7269 6e67            string
-00012430: 3d27 270a 2020 2020 2020 2020 2020 2020  =''.            
-00012440: 7374 7269 6e67 2b3d 6627 7b69 2b31 3a64  string+=f'{i+1:d
-00012450: 7d20 2027 0a20 2020 2020 2020 2020 2020  }  '.           
-00012460: 2073 7472 696e 672b 3d66 277b 647a 5b69   string+=f'{dz[i
-00012470: 5d3a 2e33 657d 2020 270a 2020 2020 2020  ]:.3e}  '.      
-00012480: 2020 2020 2020 7374 7269 6e67 2b3d 6627        string+=f'
-00012490: 7b76 7475 7262 5b69 5d3a 2e33 667d 2020  {vturb[i]:.3f}  
-000124a0: 270a 2020 2020 2020 2020 2020 2020 7374  '.            st
-000124b0: 7269 6e67 2b3d 6627 7b6e 645b 695d 3a2e  ring+=f'{nd[i]:.
-000124c0: 3365 7d20 2027 0a20 2020 2020 2020 2020  3e}  '.         
-000124d0: 2020 2073 7472 696e 672b 3d66 277b 5464     string+=f'{Td
-000124e0: 5b69 5d3a 2e33 667d 2020 270a 2020 2020  [i]:.3f}  '.    
-000124f0: 2020 2020 2020 2020 666f 7220 6a20 696e          for j in
-00012500: 2072 616e 6765 286c 656e 2873 7065 6369   range(len(speci
-00012510: 6573 5f6c 6973 7429 293a 0a20 2020 2020  es_list)):.     
-00012520: 2020 2020 2020 2020 2020 2073 7472 696e             strin
-00012530: 672b 3d66 277b 6e5f 7370 6563 6965 735b  g+=f'{n_species[
-00012540: 692c 6a5d 3a2e 3365 7d20 2027 0a20 2020  i,j]:.3e}  '.   
-00012550: 2020 2020 2020 2020 2066 6f72 206a 2069           for j i
-00012560: 6e20 7261 6e67 6528 6c65 6e28 7370 6563  n range(len(spec
-00012570: 6965 735f 6c69 7374 2929 3a0a 2020 2020  ies_list)):.    
-00012580: 2020 2020 2020 2020 2020 2020 7374 7269              stri
-00012590: 6e67 2b3d 6627 7b54 5f73 7065 6369 6573  ng+=f'{T_species
-000125a0: 5b69 2c6a 5d3a 2e33 667d 2020 270a 2020  [i,j]:.3f}  '.  
-000125b0: 2020 2020 2020 2020 2020 7374 7269 6e67            string
-000125c0: 2b3d 6627 7b6e 4832 5b69 5d3a 2e33 657d  +=f'{nH2[i]:.3e}
-000125d0: 2020 270a 2020 2020 2020 2020 2020 2020    '.            
-000125e0: 7374 7269 6e67 2b3d 6627 7b6e 4849 5b69  string+=f'{nHI[i
-000125f0: 5d3a 2e33 657d 2020 270a 2020 2020 2020  ]:.3e}  '.      
-00012600: 2020 2020 2020 7374 7269 6e67 2b3d 6627        string+=f'
-00012610: 7b6e 4849 495b 695d 3a2e 3365 7d20 2027  {nHII[i]:.3e}  '
-00012620: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
-00012630: 696e 672b 3d66 277b 6e48 655b 695d 3a2e  ing+=f'{nHe[i]:.
-00012640: 3365 7d20 2027 0a20 2020 2020 2020 2020  3e}  '.         
-00012650: 2020 2073 7472 696e 672b 3d66 277b 6e65     string+=f'{ne
-00012660: 6c65 635b 695d 3a2e 3365 7d20 2027 0a20  lec[i]:.3e}  '. 
-00012670: 2020 2020 2020 2020 2020 2066 2e77 7269             f.wri
-00012680: 7465 2873 7472 696e 672b 275c 6e27 290a  te(string+'\n').
-00012690: 2020 2020 2020 2020 662e 636c 6f73 6528          f.close(
-000126a0: 290a 0a0a 636c 6173 7320 4d79 466f 726d  )...class MyForm
-000126b0: 6174 7465 7228 7374 7269 6e67 2e46 6f72  atter(string.For
-000126c0: 6d61 7474 6572 293a 0a20 2020 2022 2222  matter):.    """
-000126d0: 0a20 2020 2053 7472 696e 6720 666f 726d  .    String form
-000126e0: 6174 7465 7220 666f 7220 7072 6f64 7563  atter for produc
-000126f0: 696e 6720 696e 7075 7420 6669 6c65 730a  ing input files.
-00012700: 2020 2020 2222 220a 0a20 2020 2064 6566      """..    def
-00012710: 2066 6f72 6d61 745f 6669 656c 6428 7365   format_field(se
-00012720: 6c66 2c76 616c 7565 2c66 6f72 6d61 745f  lf,value,format_
-00012730: 7370 6563 293a 0a20 2020 2020 2020 2069  spec):.        i
-00012740: 6620 666f 726d 6174 5f73 7065 635b 2d31  f format_spec[-1
-00012750: 5d3d 3d27 6d27 3a0a 2020 2020 2020 2020  ]=='m':.        
-00012760: 2020 2020 7265 7475 726e 2073 7570 6572      return super
-00012770: 2829 2e66 6f72 6d61 745f 6669 656c 6428  ().format_field(
-00012780: 7661 6c75 652c 666f 726d 6174 5f73 7065  value,format_spe
-00012790: 635b 3a2d 315d 2b27 6527 292e 7265 706c  c[:-1]+'e').repl
-000127a0: 6163 6528 2765 2b27 2c27 6527 290a 2020  ace('e+','e').  
-000127b0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-000127c0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000127d0: 7570 6572 2829 2e66 6f72 6d61 745f 6669  uper().format_fi
-000127e0: 656c 6428 7661 6c75 652c 666f 726d 6174  eld(value,format
-000127f0: 5f73 7065 6329 0a0a 0a66 6d74 3d4d 7946  _spec)...fmt=MyF
-00012800: 6f72 6d61 7474 6572 2829 0a0a 0a64 6566  ormatter()...def
-00012810: 206c 696e 655f 666c 7578 286c 312c 6c32   line_flux(l1,l2
-00012820: 2c77 6176 656c 656e 6774 682c 666c 7578  ,wavelength,flux
-00012830: 293a 0a20 2020 2027 2727 0a20 2020 2055  ):.    '''.    U
-00012840: 6e69 7473 3a20 5265 7475 726e 2069 7320  nits: Return is 
-00012850: 696e 2074 6865 2073 616d 6520 756e 6974  in the same unit
-00012860: 2061 7320 696e 7075 742e 205b 4173 7375   as input. [Assu
-00012870: 6d65 6420 746f 2062 6520 696e 2065 7267  med to be in erg
-00012880: 2f73 2f63 6d32 2f73 725d 206c 3120 616e  /s/cm2/sr] l1 an
-00012890: 6420 6c32 2073 616d 6520 756e 6974 2061  d l2 same unit a
-000128a0: 7320 7761 7665 6c65 6e67 7468 0a0a 2020  s wavelength..  
-000128b0: 2020 5265 7475 726e 730a 2020 2020 2d2d    Returns.    --
-000128c0: 2d2d 2d2d 2d0a 2020 2020 666c 6f61 743a  -----.    float:
-000128d0: 0a20 2020 2020 2053 756d 206f 6620 696e  .      Sum of in
-000128e0: 7465 6772 6174 6564 206c 696e 6520 666c  tegrated line fl
-000128f0: 7578 2062 6574 7765 656e 2077 6176 656c  ux between wavel
-00012900: 656e 6774 6873 206c 3120 616e 6420 6c32  engths l1 and l2
-00012910: 2e0a 0a20 2020 2027 2727 0a20 2020 206d  ...    '''.    m
-00012920: 6173 6b3d 2877 6176 656c 656e 6774 683e  ask=(wavelength>
-00012930: 6c31 2926 2877 6176 656c 656e 6774 683c  l1)&(wavelength<
-00012940: 3d6c 3229 0a20 2020 2072 6574 7572 6e20  =l2).    return 
-00012950: 6e70 2e73 756d 2866 6c75 785b 6d61 736b  np.sum(flux[mask
-00012960: 5d29 0a0a 0a64 6566 206c 696e 655f 666c  ])...def line_fl
-00012970: 7578 6573 2877 696e 646f 7773 2c77 6176  uxes(windows,wav
-00012980: 656c 656e 6774 682c 666c 7578 293a 0a20  elength,flux):. 
-00012990: 2020 2027 2727 0a20 2020 2052 6574 7572     '''.    Retur
-000129a0: 6e3a 2061 7272 6179 206f 6620 7375 6d20  n: array of sum 
-000129b0: 6f66 2069 6e74 6567 7261 7465 6420 6c69  of integrated li
-000129c0: 6e65 2066 6c75 7820 696e 2077 6176 656c  ne flux in wavel
-000129d0: 656e 6774 6820 7769 6e64 6f77 732e 0a0a  ength windows...
-000129e0: 2020 2020 556e 6974 733a 2052 6574 7572      Units: Retur
-000129f0: 6e20 6973 2069 6e20 7468 6520 7361 6d65  n is in the same
-00012a00: 2075 6e69 7420 6173 2069 6e70 7574 2e20   unit as input. 
-00012a10: 5b41 7373 756d 6564 2074 6f20 6265 2069  [Assumed to be i
-00012a20: 6e20 6572 672f 732f 636d 322f 7372 5d0a  n erg/s/cm2/sr].
-00012a30: 0a20 2020 2077 696e 646f 7773 3a20 6c69  .    windows: li
-00012a40: 7374 206f 6620 7761 7665 6c65 6e67 7468  st of wavelength
-00012a50: 206c 696d 6974 7320 6f66 2077 696e 646f   limits of windo
-00012a60: 7773 2e20 4578 616d 706c 653a 205b 5b31  ws. Example: [[1
-00012a70: 342c 3134 2e35 5d2c 5b31 352c 3136 2e32  4,14.5],[15,16.2
-00012a80: 5d2c 5b31 322e 352c 3134 2e31 5d5d 0a20  ],[12.5,14.1]]. 
-00012a90: 2020 2027 2727 0a20 2020 2046 3d5b 5d0a     '''.    F=[].
-00012aa0: 2020 2020 666f 7220 5720 696e 2077 696e      for W in win
-00012ab0: 646f 7773 3a0a 2020 2020 2020 2020 462e  dows:.        F.
-00012ac0: 6170 7065 6e64 286c 696e 655f 666c 7578  append(line_flux
-00012ad0: 2857 5b30 5d2c 575b 315d 2c77 6176 656c  (W[0],W[1],wavel
-00012ae0: 656e 6774 682c 666c 7578 2929 0a20 2020  ength,flux)).   
-00012af0: 2072 6574 7572 6e28 6e70 2e61 7272 6179   return(np.array
-00012b00: 2846 2929 0a0a 0a64 6566 206c 696e 655f  (F))...def line_
-00012b10: 666c 7578 5f72 6174 696f 7328 7261 7469  flux_ratios(rati
-00012b20: 6f5f 7769 6e64 6f77 732c 7761 7665 6c65  o_windows,wavele
-00012b30: 6e67 7468 2c66 6c75 7829 3a0a 2020 2020  ngth,flux):.    
-00012b40: 2727 270a 2020 2020 5265 7475 726e 3a20  '''.    Return: 
-00012b50: 496e 7465 6772 6174 6564 206c 696e 6520  Integrated line 
-00012b60: 666c 7578 2072 6174 696f 7320 6265 7477  flux ratios betw
-00012b70: 6565 6e20 7761 7665 6c65 6e67 7468 7320  een wavelengths 
-00012b80: 6c31 2061 6e64 206c 322e 0a0a 2020 2020  l1 and l2...    
-00012b90: 556e 6974 3a20 5265 7475 726e 2068 6173  Unit: Return has
-00012ba0: 206e 6f20 756e 6974 2e20 5b49 6e70 7574   no unit. [Input
-00012bb0: 2069 7320 6173 7375 6d65 6420 746f 2062   is assumed to b
-00012bc0: 6520 696e 2065 7267 2f73 2f63 6d32 2f73  e in erg/s/cm2/s
-00012bd0: 725d 0a0a 2020 2020 7261 7469 6f5f 7769  r]..    ratio_wi
-00012be0: 6e64 6f77 733a 206c 6973 7420 6f66 2077  ndows: list of w
-00012bf0: 6176 656c 656e 6774 6820 7769 6e64 6f77  avelength window
-00012c00: 732e 2045 7861 6d70 6c65 3a20 5b5b 5b31  s. Example: [[[1
-00012c10: 342c 3134 2e35 5d2c 5b31 352c 3136 2e32  4,14.5],[15,16.2
-00012c20: 5d5d 2c5b 5b31 322e 352c 3134 2e31 5d2c  ]],[[12.5,14.1],
-00012c30: 5b31 332e 342c 3133 2e38 5d5d 5d0a 2020  [13.4,13.8]]].  
-00012c40: 2020 2727 270a 2020 2020 523d 5b5d 0a20    '''.    R=[]. 
-00012c50: 2020 2066 6f72 2077 696e 646f 7720 696e     for window in
-00012c60: 2072 6174 696f 5f77 696e 646f 7773 3a0a   ratio_windows:.
-00012c70: 2020 2020 2020 2020 463d 6c69 6e65 5f66          F=line_f
-00012c80: 6c75 7865 7328 5b77 696e 646f 775b 305d  luxes([window[0]
-00012c90: 2c77 696e 646f 775b 315d 5d2c 7761 7665  ,window[1]],wave
-00012ca0: 6c65 6e67 7468 2c66 6c75 7829 0a20 2020  length,flux).   
-00012cb0: 2020 2020 2052 2e61 7070 656e 6428 465b       R.append(F[
-00012cc0: 315d 2f46 5b30 5d29 0a20 2020 2072 6574  1]/F[0]).    ret
-00012cd0: 7572 6e28 6e70 2e61 7272 6179 2852 2929  urn(np.array(R))
-00012ce0: 0a0a 0a64 6566 206c 696e 655f 666c 7578  ...def line_flux
-00012cf0: 5f70 726f 6475 6374 7328 7072 6f64 7563  _products(produc
-00012d00: 745f 7769 6e64 6f77 732c 7761 7665 6c65  t_windows,wavele
-00012d10: 6e67 7468 2c66 6c75 7829 3a0a 2020 2020  ngth,flux):.    
-00012d20: 2727 270a 2020 2020 5265 7475 726e 3a20  '''.    Return: 
-00012d30: 496e 7465 6772 6174 6564 206c 696e 6520  Integrated line 
-00012d40: 666c 7578 2070 726f 6475 6374 7320 6265  flux products be
-00012d50: 7477 6565 6e20 7761 7665 6c65 6e67 7468  tween wavelength
-00012d60: 7320 6c31 2061 6e64 206c 322e 0a0a 2020  s l1 and l2...  
-00012d70: 2020 556e 6974 3a20 5265 7475 726e 2075    Unit: Return u
-00012d80: 6e69 7420 6973 206f 7574 7075 7420 756e  nit is output un
-00012d90: 6974 7320 7371 7561 7265 642e 205b 496e  its squared. [In
-00012da0: 7075 7420 6973 2061 7373 756d 6564 2074  put is assumed t
-00012db0: 6f20 6265 2069 6e20 6572 672f 732f 636d  o be in erg/s/cm
-00012dc0: 322f 7372 5d0a 0a20 2020 2070 726f 6475  2/sr]..    produ
-00012dd0: 6374 5f77 696e 646f 7773 3a20 6c69 7374  ct_windows: list
-00012de0: 206f 6620 7761 7665 6c65 6e67 7468 2077   of wavelength w
-00012df0: 696e 646f 7773 2e20 4578 616d 706c 653a  indows. Example:
-00012e00: 205b 5b5b 3134 2c31 342e 355d 2c5b 3135   [[[14,14.5],[15
-00012e10: 2c31 362e 325d 5d2c 5b5b 3132 2e35 2c31  ,16.2]],[[12.5,1
-00012e20: 342e 315d 2c5b 3133 2e34 2c31 332e 385d  4.1],[13.4,13.8]
-00012e30: 5d5d 0a20 2020 2027 2727 0a20 2020 2052  ]].    '''.    R
-00012e40: 3d5b 5d0a 2020 2020 666f 7220 7769 6e64  =[].    for wind
-00012e50: 6f77 2069 6e20 7072 6f64 7563 745f 7769  ow in product_wi
-00012e60: 6e64 6f77 733a 0a20 2020 2020 2020 2046  ndows:.        F
-00012e70: 3d6c 696e 655f 666c 7578 6573 285b 7769  =line_fluxes([wi
-00012e80: 6e64 6f77 5b30 5d2c 7769 6e64 6f77 5b31  ndow[0],window[1
-00012e90: 5d5d 2c77 6176 656c 656e 6774 682c 666c  ]],wavelength,fl
-00012ea0: 7578 290a 2020 2020 2020 2020 522e 6170  ux).        R.ap
-00012eb0: 7065 6e64 2846 5b31 5d2a 465b 305d 290a  pend(F[1]*F[0]).
-00012ec0: 2020 2020 7265 7475 726e 286e 702e 6172      return(np.ar
-00012ed0: 7261 7928 5229 290a 0a0a 6465 6620 7370  ray(R))...def sp
-00012ee0: 6563 7472 616c 5f66 6c75 7828 6c31 2c6c  ectral_flux(l1,l
-00012ef0: 322c 7761 7665 6c65 6e67 7468 2c66 6c75  2,wavelength,flu
-00012f00: 7829 3a0a 2020 2020 2727 270a 2020 2020  x):.    '''.    
-00012f10: 556e 6974 3a20 5265 7475 726e 2069 6e20  Unit: Return in 
-00012f20: 5b65 7267 2f73 2f63 6d32 5d20 616e 6420  [erg/s/cm2] and 
-00012f30: 696e 7075 7420 6973 2069 6e20 5b4a 795d  input is in [Jy]
-00012f40: 206c 312c 206c 322c 2061 6e64 2077 6176   l1, l2, and wav
-00012f50: 656c 656e 6774 6820 696e 206d 6963 726f  elength in micro
-00012f60: 6e73 0a0a 2020 2020 5265 7475 726e 730a  ns..    Returns.
-00012f70: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-00012f80: 666c 6f61 743a 0a20 2020 2020 2053 756d  float:.      Sum
-00012f90: 206f 6620 696e 7465 6772 6174 6564 206c   of integrated l
-00012fa0: 696e 6520 666c 7578 2062 6574 7765 656e  ine flux between
-00012fb0: 2077 6176 656c 656e 6774 6873 206c 3120   wavelengths l1 
-00012fc0: 616e 6420 6c32 2e0a 0a20 2020 2027 2727  and l2...    '''
-00012fd0: 0a20 2020 2066 6c75 783d 666c 7578 2a31  .    flux=flux*1
-00012fe0: 652d 3233 2020 2320 436f 6e76 6572 7469  e-23  # Converti
-00012ff0: 6e67 204a 7920 746f 2065 7267 2e73 e288  ng Jy to erg.s..
-00013000: 9231 2e63 6de2 8892 322e 487a e288 9231  .1.cm...2.Hz...1
-00013010: 0a20 2020 2077 6176 656c 656e 6774 683d  .    wavelength=
-00013020: 7761 7665 6c65 6e67 7468 2a31 652d 3420  wavelength*1e-4 
-00013030: 2023 2043 6f6e 7665 7274 696e 6720 6d69   # Converting mi
-00013040: 6372 6f6e 7320 746f 2063 6d0a 2020 2020  crons to cm.    
-00013050: 666c 7578 3d66 6c75 785b 6e70 2e61 7267  flux=flux[np.arg
-00013060: 736f 7274 2877 6176 656c 656e 6774 6829  sort(wavelength)
-00013070: 5d0a 2020 2020 7761 7665 6c65 6e67 7468  ].    wavelength
-00013080: 3d77 6176 656c 656e 6774 685b 6e70 2e61  =wavelength[np.a
-00013090: 7267 736f 7274 2877 6176 656c 656e 6774  rgsort(wavelengt
-000130a0: 6829 5d0a 2020 2020 6c31 3d6c 312a 3165  h)].    l1=l1*1e
-000130b0: 2d34 2020 2320 436f 6e76 6572 7469 6e67  -4  # Converting
-000130c0: 206d 6963 726f 6e73 2074 6f20 636d 0a20   microns to cm. 
-000130d0: 2020 206c 323d 6c32 2a31 652d 3420 2023     l2=l2*1e-4  #
-000130e0: 2043 6f6e 7665 7274 696e 6720 6d69 6372   Converting micr
-000130f0: 6f6e 7320 746f 2063 6d0a 2020 2020 635f  ons to cm.    c_
-00013100: 636d 733d 632a 3165 3220 2023 2043 6f6e  cms=c*1e2  # Con
-00013110: 7665 7274 696e 6720 6d2f 7320 746f 2063  verting m/s to c
-00013120: 6d2f 730a 2020 2020 6d61 736b 3d28 7761  m/s.    mask=(wa
-00013130: 7665 6c65 6e67 7468 3e6c 3129 2628 7761  velength>l1)&(wa
-00013140: 7665 6c65 6e67 7468 3c3d 6c32 290a 2020  velength<=l2).  
-00013150: 2020 7761 7665 3d77 6176 656c 656e 6774    wave=wavelengt
-00013160: 685b 6d61 736b 5d0a 2020 2020 2320 7761  h[mask].    # wa
-00013170: 7665 3120 2020 2020 203d 206e 702e 726f  ve1      = np.ro
-00013180: 6c6c 2877 6176 656c 656e 6774 682c 3129  ll(wavelength,1)
-00013190: 5b6d 6173 6b5d 0a20 2020 2023 2077 6176  [mask].    # wav
-000131a0: 6531 2020 2020 2020 3d20 3130 2a2a 2828  e1      = 10**((
-000131b0: 6e70 2e6c 6f67 3130 2877 6176 6529 2b6e  np.log10(wave)+n
-000131c0: 702e 6c6f 6731 3028 7761 7665 3129 292f  p.log10(wave1))/
-000131d0: 3229 0a20 2020 2023 2077 6176 6532 2020  2).    # wave2  
-000131e0: 2020 2020 3d20 6e70 2e72 6f6c 6c28 7761      = np.roll(wa
-000131f0: 7665 6c65 6e67 7468 2c2d 3129 5b6d 6173  velength,-1)[mas
-00013200: 6b5d 0a20 2020 2023 2077 6176 6532 2020  k].    # wave2  
-00013210: 2020 2020 3d20 3130 2a2a 2828 6e70 2e6c      = 10**((np.l
-00013220: 6f67 3130 2877 6176 6529 2b6e 702e 6c6f  og10(wave)+np.lo
-00013230: 6731 3028 7761 7665 3229 292f 3229 0a20  g10(wave2))/2). 
-00013240: 2020 2023 2064 6e75 2020 2020 2020 2020     # dnu        
-00013250: 3d20 632a 2877 6176 6532 2d77 6176 6531  = c*(wave2-wave1
-00013260: 292f 7761 7665 2a2a 322a 3165 320a 2020  )/wave**2*1e2.  
-00013270: 2020 7761 7665 313d 6e70 2e72 6f6c 6c28    wave1=np.roll(
-00013280: 7761 7665 6c65 6e67 7468 2c31 295b 6d61  wavelength,1)[ma
-00013290: 736b 5d0a 2020 2020 7761 7665 323d 6e70  sk].    wave2=np
-000132a0: 2e72 6f6c 6c28 7761 7665 6c65 6e67 7468  .roll(wavelength
-000132b0: 2c2d 3129 5b6d 6173 6b5d 0a20 2020 2064  ,-1)[mask].    d
-000132c0: 6e75 3d28 635f 636d 732a 2831 2f77 6176  nu=(c_cms*(1/wav
-000132d0: 6531 2d31 2f77 6176 6532 292f 3229 0a20  e1-1/wave2)/2). 
-000132e0: 2020 2072 6574 7572 6e28 6e70 2e73 756d     return(np.sum
-000132f0: 2866 6c75 785b 6d61 736b 5d2a 646e 7529  (flux[mask]*dnu)
-00013300: 290a 0a0a 6465 6620 7370 6563 7472 616c  )...def spectral
-00013310: 5f66 6c75 7865 7328 7769 6e64 6f77 732c  _fluxes(windows,
-00013320: 7761 7665 6c65 6e67 7468 2c66 6c75 7829  wavelength,flux)
-00013330: 3a0a 2020 2020 2727 270a 2020 2020 5265  :.    '''.    Re
-00013340: 7475 726e 3a20 5375 6d20 6f66 2069 6e74  turn: Sum of int
-00013350: 6567 7261 7465 6420 6c69 6e65 2066 6c75  egrated line flu
-00013360: 7820 6265 7477 6565 6e20 7761 7665 6c65  x between wavele
-00013370: 6e67 7468 2077 696e 646f 7773 2e0a 0a20  ngth windows... 
-00013380: 2020 2055 6e69 743a 2072 6574 7572 6e20     Unit: return 
-00013390: 6973 2069 6e20 5b65 7267 2f73 2f63 6d32  is in [erg/s/cm2
-000133a0: 5d20 616e 6420 696e 7075 7420 6973 2069  ] and input is i
-000133b0: 6e20 5b4a 795d 0a0a 2020 2020 7769 6e64  n [Jy]..    wind
-000133c0: 6f77 733a 206c 6973 7420 6f66 2077 6176  ows: list of wav
-000133d0: 656c 656e 6774 6820 6c69 6d69 7473 2028  elength limits (
-000133e0: 6d69 6372 6f6e 7329 206f 6620 7769 6e64  microns) of wind
-000133f0: 6f77 732e 2045 7861 6d70 6c65 3a20 5b5b  ows. Example: [[
-00013400: 3134 2c31 342e 355d 2c5b 3135 2c31 362e  14,14.5],[15,16.
-00013410: 325d 2c5b 3132 2e35 2c31 342e 315d 5d0a  2],[12.5,14.1]].
-00013420: 2020 2020 2727 270a 2020 2020 463d 5b5d      '''.    F=[]
-00013430: 0a20 2020 2066 6f72 2057 2069 6e20 7769  .    for W in wi
-00013440: 6e64 6f77 733a 0a20 2020 2020 2020 2046  ndows:.        F
-00013450: 2e61 7070 656e 6428 7370 6563 7472 616c  .append(spectral
-00013460: 5f66 6c75 7828 575b 305d 2c57 5b31 5d2c  _flux(W[0],W[1],
-00013470: 7761 7665 6c65 6e67 7468 2c66 6c75 7829  wavelength,flux)
-00013480: 290a 2020 2020 7265 7475 726e 286e 702e  ).    return(np.
-00013490: 6172 7261 7928 4629 290a 0a0a 6465 6620  array(F))...def 
-000134a0: 7370 6563 7472 616c 5f66 6c75 785f 7261  spectral_flux_ra
-000134b0: 7469 6f73 2872 6174 696f 5f77 696e 646f  tios(ratio_windo
-000134c0: 7773 2c77 6176 656c 656e 6774 682c 666c  ws,wavelength,fl
-000134d0: 7578 293a 0a20 2020 2027 2727 0a20 2020  ux):.    '''.   
-000134e0: 2052 6574 7572 6e3a 2053 7065 6374 7261   Return: Spectra
-000134f0: 6c20 696e 7465 6772 6174 6564 2066 6c75  l integrated flu
-00013500: 7820 7261 7469 6f73 2062 6574 7765 656e  x ratios between
-00013510: 2077 6176 656c 656e 6774 6820 7769 6e64   wavelength wind
-00013520: 6f77 732e 0a0a 2020 2020 556e 6974 733a  ows...    Units:
-00013530: 2052 6574 7572 6e20 6973 2077 6974 686f   Return is witho
-00013540: 7574 2075 6e69 7473 2061 6e64 2069 6e70  ut units and inp
-00013550: 7574 2069 7320 696e 205b 4a79 5d0a 0a20  ut is in [Jy].. 
-00013560: 2020 2072 6174 696f 5f77 696e 646f 7773     ratio_windows
-00013570: 3a20 6c69 7374 206f 6620 7761 7665 6c65  : list of wavele
-00013580: 6e67 7468 2028 6d69 6372 6f6e 7329 2077  ngth (microns) w
-00013590: 696e 646f 7773 2e20 4578 616d 706c 653a  indows. Example:
-000135a0: 205b 5b5b 3134 2c31 342e 355d 2c5b 3135   [[[14,14.5],[15
-000135b0: 2c31 362e 325d 5d2c 5b5b 3132 2e35 2c31  ,16.2]],[[12.5,1
-000135c0: 342e 315d 2c5b 3133 2e34 2c31 332e 385d  4.1],[13.4,13.8]
-000135d0: 5d5d 0a20 2020 2027 2727 0a20 2020 2052  ]].    '''.    R
-000135e0: 3d5b 5d0a 2020 2020 666f 7220 7769 6e64  =[].    for wind
-000135f0: 6f77 2069 6e20 7261 7469 6f5f 7769 6e64  ow in ratio_wind
-00013600: 6f77 733a 0a20 2020 2020 2020 2046 3d73  ows:.        F=s
-00013610: 7065 6374 7261 6c5f 666c 7578 6573 285b  pectral_fluxes([
-00013620: 7769 6e64 6f77 5b30 5d2c 7769 6e64 6f77  window[0],window
-00013630: 5b31 5d5d 2c77 6176 656c 656e 6774 682c  [1]],wavelength,
-00013640: 666c 7578 290a 2020 2020 2020 2020 522e  flux).        R.
-00013650: 6170 7065 6e64 2846 5b31 5d2f 465b 305d  append(F[1]/F[0]
-00013660: 290a 2020 2020 7265 7475 726e 286e 702e  ).    return(np.
-00013670: 6172 7261 7928 5229 290a 0a0a 6465 6620  array(R))...def 
-00013680: 7370 6563 7472 616c 5f66 6c75 785f 7072  spectral_flux_pr
-00013690: 6f64 7563 7473 2870 726f 6475 6374 5f77  oducts(product_w
-000136a0: 696e 646f 7773 2c77 6176 656c 656e 6774  indows,wavelengt
-000136b0: 682c 666c 7578 293a 0a20 2020 2027 2727  h,flux):.    '''
-000136c0: 0a20 2020 2052 6574 7572 6e3a 2050 726f  .    Return: Pro
-000136d0: 6475 6374 7320 6f66 2073 7065 6374 7261  ducts of spectra
-000136e0: 6c20 696e 7465 6772 6174 6564 2066 6c75  l integrated flu
-000136f0: 7865 7320 6265 7477 6565 6e20 7761 7665  xes between wave
-00013700: 6c65 6e67 7468 2077 696e 646f 7773 2e0a  length windows..
-00013710: 0a20 2020 2055 6e69 7473 3a20 5265 7475  .    Units: Retu
-00013720: 726e 2075 6e69 7420 6973 206f 7574 7075  rn unit is outpu
-00013730: 7420 756e 6974 7320 7371 7561 7265 6420  t units squared 
-00013740: 616e 6420 696e 7075 7420 6973 2069 6e20  and input is in 
-00013750: 5b4a 795d 0a0a 2020 2020 7072 6f64 7563  [Jy]..    produc
-00013760: 745f 7769 6e64 6f77 733a 206c 6973 7420  t_windows: list 
-00013770: 6f66 2077 6176 656c 656e 6774 6820 286d  of wavelength (m
-00013780: 6963 726f 6e73 2920 7769 6e64 6f77 732e  icrons) windows.
-00013790: 2045 7861 6d70 6c65 3a20 5b5b 5b31 342c   Example: [[[14,
-000137a0: 3134 2e35 5d2c 5b31 352c 3136 2e32 5d5d  14.5],[15,16.2]]
-000137b0: 2c5b 5b31 322e 352c 3134 2e31 5d2c 5b31  ,[[12.5,14.1],[1
-000137c0: 332e 342c 3133 2e38 5d5d 5d0a 2020 2020  3.4,13.8]]].    
-000137d0: 2727 270a 2020 2020 523d 5b5d 0a20 2020  '''.    R=[].   
-000137e0: 2066 6f72 2077 696e 646f 7720 696e 2070   for window in p
-000137f0: 726f 6475 6374 5f77 696e 646f 7773 3a0a  roduct_windows:.
-00013800: 2020 2020 2020 2020 463d 7370 6563 7472          F=spectr
-00013810: 616c 5f66 6c75 7865 7328 5b77 696e 646f  al_fluxes([windo
-00013820: 775b 305d 2c77 696e 646f 775b 315d 5d2c  w[0],window[1]],
-00013830: 7761 7665 6c65 6e67 7468 2c66 6c75 7829  wavelength,flux)
-00013840: 0a20 2020 2020 2020 2052 2e61 7070 656e  .        R.appen
-00013850: 6428 465b 315d 2a46 5b30 5d29 0a20 2020  d(F[1]*F[0]).   
-00013860: 2072 6574 7572 6e28 6e70 2e61 7272 6179   return(np.array
-00013870: 2852 2929 0a0a 0a64 6566 2063 6869 325f  (R))...def chi2_
-00013880: 736c 6162 2873 6c61 625f 6461 7461 2c73  slab(slab_data,s
-00013890: 7065 6374 7261 2c77 696e 646f 7773 3d5b  pectra,windows=[
-000138a0: 5d2c 7261 7469 6f5f 7769 6e64 6f77 733d  ],ratio_windows=
-000138b0: 5b5d 2c70 726f 6475 6374 5f77 696e 646f  [],product_windo
-000138c0: 7773 3d5b 5d2c 5264 6973 6b3d 6e70 2e6c  ws=[],Rdisk=np.l
-000138d0: 6f67 7370 6163 6528 2d32 2c32 2c31 3029  ogspace(-2,2,10)
-000138e0: 2c64 6973 7461 6e63 653d 3132 302c 636f  ,distance=120,co
-000138f0: 6e76 6f6c 7665 3d46 616c 7365 2c4e 4c54  nvolve=False,NLT
-00013900: 453d 4661 6c73 652c 7368 6f72 745f 666f  E=False,short_fo
-00013910: 726d 6174 3d46 616c 7365 293a 0a20 2020  rmat=False):.   
-00013920: 2027 2727 0a20 2020 2052 6574 7572 6e73   '''.    Returns
-00013930: 2063 6869 3220 6261 7365 6420 6f6e 2073   chi2 based on s
-00013940: 656c 6563 7465 6420 7370 6563 7472 616c  elected spectral
-00013950: 2077 696e 646f 7773 2061 6372 6f73 7320   windows across 
-00013960: 6469 6666 6572 656e 7420 656d 6974 7469  different emitti
-00013970: 6e67 2064 6973 6b20 7261 6469 7573 0a0a  ng disk radius..
-00013980: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-00013990: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-000139a0: 2020 736c 6162 5f64 6174 6120 3a20 7374    slab_data : st
-000139b0: 7269 6e67 206f 7220 736c 6162 5f6d 6f64  ring or slab_mod
-000139c0: 656c 2069 6e73 7461 6e63 650a 2020 2020  el instance.    
-000139d0: 2020 7061 7468 2063 6f72 7265 7370 6f6e    path correspon
-000139e0: 6469 6e67 2074 6f20 6120 7369 6e67 6c65  ding to a single
-000139f0: 2073 6c61 6220 6d6f 6465 6c20 6f72 2061   slab model or a
-00013a00: 2073 696e 676c 6520 736c 6162 5f6d 6f64   single slab_mod
-00013a10: 656c 2069 6e73 7461 6e63 650a 0a20 2020  el instance..   
-00013a20: 2073 7065 6374 7261 203a 206e 756d 7079   spectra : numpy
-00013a30: 2e61 7272 6179 0a20 2020 2020 206e 756d  .array.      num
-00013a40: 7079 2061 7272 6179 2077 6974 6820 6669  py array with fi
-00013a50: 7273 7420 636f 6c75 6d6e 2074 6865 2077  rst column the w
-00013a60: 6176 656c 656e 6774 6820 696e 205b 6d69  avelength in [mi
-00013a70: 6372 6f6e 735d 2061 6e64 2073 6563 6f6e  crons] and secon
-00013a80: 6420 636f 6c75 6d6e 2066 6c75 7820 696e  d column flux in
-00013a90: 205b 4a79 5d0a 0a20 2020 2077 696e 646f   [Jy]..    windo
-00013aa0: 7773 203a 2061 7272 6179 5f6c 696b 650a  ws : array_like.
-00013ab0: 2020 2020 2020 4c69 7374 206f 6620 7370        List of sp
-00013ac0: 6563 7472 616c 2077 696e 646f 7773 2066  ectral windows f
-00013ad0: 6f72 2063 6869 3220 6361 6c63 756c 6174  or chi2 calculat
-00013ae0: 696f 6e20 2877 6569 6768 7473 206f 7074  ion (weights opt
-00013af0: 696f 6e61 6c29 2e20 466f 726d 6174 203a  ional). Format :
-00013b00: 205b 7769 6e64 6f77 312c 7769 6e64 6f77   [window1,window
-00013b10: 322c 2e2e 2e2e 5d0a 2020 2020 2020 5769  2,....].      Wi
-00013b20: 6e64 6f77 2066 6f72 6d61 743a 205b 6c61  ndow format: [la
-00013b30: 6d62 6461 5f30 2c20 6c61 6d62 6461 5f31  mbda_0, lambda_1
-00013b40: 2c20 7765 6967 6874 5d20 7765 6967 6874  , weight] weight
-00013b50: 2069 7320 6f70 7469 6f6e 616c 2c20 7573   is optional, us
-00013b60: 6564 2066 6f72 2077 6569 6768 7465 6420  ed for weighted 
-00013b70: 6368 6932 0a20 2020 2020 2045 7861 6d70  chi2.      Examp
-00013b80: 6c65 2077 6974 686f 7574 2077 6569 6768  le without weigh
-00013b90: 743a 205b 5b31 342c 3134 2e35 5d2c 5b31  t: [[14,14.5],[1
-00013ba0: 352c 3136 2e32 5d2c 5b31 322e 352c 3134  5,16.2],[12.5,14
-00013bb0: 2e31 5d5d 0a20 2020 2020 2045 7861 6d70  .1]].      Examp
-00013bc0: 6c65 2077 6974 6820 7765 6967 6874 3a20  le with weight: 
-00013bd0: 5b5b 3134 2c31 342e 352c 325d 2c5b 3135  [[14,14.5,2],[15
-00013be0: 2c31 362e 322c 355d 2c5b 3132 2e35 2c31  ,16.2,5],[12.5,1
-00013bf0: 342e 312c 315d 5d0a 2020 2020 2020 5765  4.1,1]].      We
-00013c00: 6967 6874 7320 6172 6520 6175 746f 6d61  ights are automa
-00013c10: 7469 6361 6c6c 7920 6e6f 726d 616c 6973  tically normalis
-00013c20: 6564 2c20 736f 2073 756d 206f 6620 7765  ed, so sum of we
-00013c30: 6967 6874 7320 6e65 6564 206e 6f74 2062  ights need not b
-00013c40: 6520 310a 0a20 2020 2052 6469 736b 203a  e 1..    Rdisk :
-00013c50: 2061 7272 6179 5f6c 696b 650a 2020 2020   array_like.    
-00013c60: 2020 5261 6469 7573 2063 6f72 7265 7370    Radius corresp
-00013c70: 6f6e 6469 6e67 2074 6f20 656d 6974 7469  onding to emitti
-00013c80: 6e67 2061 7265 6120 696e 2061 7374 726f  ng area in astro
-00013c90: 6e6f 6d69 6361 6c20 756e 6974 730a 0a20  nomical units.. 
-00013ca0: 2020 2064 6973 7461 6e63 6520 3a20 666c     distance : fl
-00013cb0: 6f61 740a 2020 2020 2020 6469 7374 616e  oat.      distan
-00013cc0: 6365 206f 6620 6469 736b 2069 6e20 7061  ce of disk in pa
-00013cd0: 7273 6563 0a0a 2020 2020 636f 6e76 6f6c  rsec..    convol
-00013ce0: 7665 203a 2062 6f6f 6c65 616e 0a20 2020  ve : boolean.   
-00013cf0: 2020 2049 6620 5472 7565 2c20 7468 6520     If True, the 
-00013d00: 6368 6932 2069 7320 7065 7266 6f72 6d65  chi2 is performe
-00013d10: 6420 6f6e 2063 6f6e 766f 6c76 6564 2073  d on convolved s
-00013d20: 7065 6374 7261 2061 6e64 206e 6f74 206f  pectra and not o
-00013d30: 6e20 696e 6469 7669 6475 616c 206c 696e  n individual lin
-00013d40: 6573 0a0a 2020 2020 4e4c 5445 203a 2062  es..    NLTE : b
-00013d50: 6f6f 6c65 616e 0a20 2020 2020 2069 6620  oolean.      if 
-00013d60: 5472 7565 2c20 4e4c 5445 2066 6c75 7820  True, NLTE flux 
-00013d70: 6973 2074 616b 656e 2066 726f 6d20 7468  is taken from th
-00013d80: 6520 736c 6162 206d 6f64 656c 2e0a 2020  e slab model..  
-00013d90: 2020 2727 270a 2020 2020 6172 6561 3d6e    '''.    area=n
-00013da0: 702e 7069 2a28 5264 6973 6b2a 6175 2f64  p.pi*(Rdisk*au/d
-00013db0: 6973 7461 6e63 652f 7063 292a 2a32 0a20  istance/pc)**2. 
-00013dc0: 2020 2063 6869 5f61 7265 613d 6e70 2e7a     chi_area=np.z
-00013dd0: 6572 6f73 2828 6c65 6e28 6172 6561 2929  eros((len(area))
-00013de0: 290a 2020 2020 6966 2069 7369 6e73 7461  ).    if isinsta
-00013df0: 6e63 6528 736c 6162 5f64 6174 612c 7374  nce(slab_data,st
-00013e00: 7229 3a20 736c 6162 5f64 6174 613d 7265  r): slab_data=re
-00013e10: 6164 5f73 6c61 6228 736c 6162 5f64 6174  ad_slab(slab_dat
-00013e20: 612c 7665 7262 6f73 653d 4661 6c73 652c  a,verbose=False,
-00013e30: 7368 6f72 745f 666f 726d 6174 3d73 686f  short_format=sho
-00013e40: 7274 5f66 6f72 6d61 7429 0a20 2020 2069  rt_format).    i
-00013e50: 6620 6c65 6e28 7769 6e64 6f77 7329 3c30  f len(windows)<0
-00013e60: 2061 6e64 206c 656e 2872 6174 696f 5f77   and len(ratio_w
-00013e70: 696e 646f 7773 293c 3020 616e 6420 6c65  indows)<0 and le
-00013e80: 6e28 7072 6f64 7563 745f 7769 6e64 6f77  n(product_window
-00013e90: 7329 3c30 3a20 7265 7475 726e 2063 6869  s)<0: return chi
-00013ea0: 5f61 7265 610a 2020 2020 6966 2063 6f6e  _area.    if con
-00013eb0: 766f 6c76 653a 2020 2320 746f 2065 7374  volve:  # to est
-00013ec0: 696d 6174 6520 666c 7578 2066 726f 6d20  imate flux from 
-00013ed0: 636f 6e76 6f6c 7665 6420 7370 6563 7472  convolved spectr
-00013ee0: 610a 2020 2020 2020 2020 6c6d 696e 2c6c  a.        lmin,l
-00013ef0: 6d61 783d 5b5d 2c5b 5d0a 2020 2020 2020  max=[],[].      
-00013f00: 2020 6966 206c 656e 2877 696e 646f 7773    if len(windows
-00013f10: 293e 303a 0a20 2020 2020 2020 2020 2020  )>0:.           
-00013f20: 206c 6d69 6e2e 6170 7065 6e64 286e 702e   lmin.append(np.
-00013f30: 616d 696e 286e 702e 6172 7261 7928 5b5b  amin(np.array([[
-00013f40: 695b 305d 2c69 5b31 5d5d 2066 6f72 2069  i[0],i[1]] for i
-00013f50: 2069 6e20 7769 6e64 6f77 735d 292e 666c   in windows]).fl
-00013f60: 6174 7465 6e28 2929 290a 2020 2020 2020  atten())).      
-00013f70: 2020 2020 2020 6c6d 6178 2e61 7070 656e        lmax.appen
-00013f80: 6428 6e70 2e61 6d61 7828 6e70 2e61 7272  d(np.amax(np.arr
-00013f90: 6179 285b 5b69 5b30 5d2c 695b 315d 5d20  ay([[i[0],i[1]] 
-00013fa0: 666f 7220 6920 696e 2077 696e 646f 7773  for i in windows
-00013fb0: 5d29 2e66 6c61 7474 656e 2829 2929 0a20  ]).flatten())). 
-00013fc0: 2020 2020 2020 2069 6620 6c65 6e28 7261         if len(ra
-00013fd0: 7469 6f5f 7769 6e64 6f77 7329 3e30 3a0a  tio_windows)>0:.
-00013fe0: 2020 2020 2020 2020 2020 2020 6c6d 696e              lmin
-00013ff0: 2e61 7070 656e 6428 6e70 2e61 6d69 6e28  .append(np.amin(
-00014000: 6e70 2e61 7272 6179 285b 5b69 5b30 5d2c  np.array([[i[0],
-00014010: 695b 315d 5d20 666f 7220 6920 696e 2072  i[1]] for i in r
-00014020: 6174 696f 5f77 696e 646f 7773 5d29 2e66  atio_windows]).f
-00014030: 6c61 7474 656e 2829 2929 0a20 2020 2020  latten())).     
-00014040: 2020 2020 2020 206c 6d61 782e 6170 7065         lmax.appe
-00014050: 6e64 286e 702e 616d 6178 286e 702e 6172  nd(np.amax(np.ar
-00014060: 7261 7928 5b5b 695b 305d 2c69 5b31 5d5d  ray([[i[0],i[1]]
-00014070: 2066 6f72 2069 2069 6e20 7261 7469 6f5f   for i in ratio_
-00014080: 7769 6e64 6f77 735d 292e 666c 6174 7465  windows]).flatte
-00014090: 6e28 2929 290a 2020 2020 2020 2020 6966  n())).        if
-000140a0: 206c 656e 2870 726f 6475 6374 5f77 696e   len(product_win
-000140b0: 646f 7773 293e 303a 0a20 2020 2020 2020  dows)>0:.       
-000140c0: 2020 2020 206c 6d69 6e2e 6170 7065 6e64       lmin.append
-000140d0: 286e 702e 616d 696e 286e 702e 6172 7261  (np.amin(np.arra
-000140e0: 7928 5b5b 695b 305d 2c69 5b31 5d5d 2066  y([[i[0],i[1]] f
-000140f0: 6f72 2069 2069 6e20 7072 6f64 7563 745f  or i in product_
-00014100: 7769 6e64 6f77 735d 292e 666c 6174 7465  windows]).flatte
-00014110: 6e28 2929 290a 2020 2020 2020 2020 2020  n())).          
-00014120: 2020 6c6d 6178 2e61 7070 656e 6428 6e70    lmax.append(np
-00014130: 2e61 6d61 7828 6e70 2e61 7272 6179 285b  .amax(np.array([
-00014140: 5b69 5b30 5d2c 695b 315d 5d20 666f 7220  [i[0],i[1]] for 
-00014150: 6920 696e 2070 726f 6475 6374 5f77 696e  i in product_win
-00014160: 646f 7773 5d29 2e66 6c61 7474 656e 2829  dows]).flatten()
-00014170: 2929 0a20 2020 2020 2020 206c 6d69 6e3d  )).        lmin=
-00014180: 6e70 2e61 6d69 6e28 6c6d 696e 290a 2020  np.amin(lmin).  
-00014190: 2020 2020 2020 6c6d 6178 3d6e 702e 616d        lmax=np.am
-000141a0: 6178 286c 6d61 7829 0a20 2020 2020 2020  ax(lmax).       
-000141b0: 2073 6c61 625f 6461 7461 2e63 6f6e 766f   slab_data.convo
-000141c0: 6c76 6528 523d 3230 3030 2c6c 616d 6264  lve(R=2000,lambd
-000141d0: 615f 303d 6c6d 696e 2a30 2e39 2c6c 616d  a_0=lmin*0.9,lam
-000141e0: 6264 615f 6e3d 6c6d 6178 2a31 2e31 2c4e  bda_n=lmax*1.1,N
-000141f0: 4c54 453d 4e4c 5445 2c76 6572 626f 7365  LTE=NLTE,verbose
-00014200: 3d46 616c 7365 290a 2020 2020 2020 2020  =False).        
-00014210: 6966 204e 4c54 453a 0a20 2020 2020 2020  if NLTE:.       
-00014220: 2020 2020 2046 6d6f 6465 6c3d 7370 6563       Fmodel=spec
-00014230: 7472 616c 5f66 6c75 7865 7328 7769 6e64  tral_fluxes(wind
-00014240: 6f77 732c 736c 6162 5f64 6174 612e 636f  ows,slab_data.co
-00014250: 6e76 5761 7665 6c65 6e67 7468 2c73 6c61  nvWavelength,sla
-00014260: 625f 6461 7461 2e63 6f6e 764e 4c54 4566  b_data.convNLTEf
-00014270: 6c75 782a 3165 3233 290a 2020 2020 2020  lux*1e23).      
-00014280: 2020 2020 2020 526d 6f64 656c 3d73 7065        Rmodel=spe
-00014290: 6374 7261 6c5f 666c 7578 5f72 6174 696f  ctral_flux_ratio
-000142a0: 7328 7261 7469 6f5f 7769 6e64 6f77 732c  s(ratio_windows,
-000142b0: 736c 6162 5f64 6174 612e 636f 6e76 5761  slab_data.convWa
-000142c0: 7665 6c65 6e67 7468 2c73 6c61 625f 6461  velength,slab_da
-000142d0: 7461 2e63 6f6e 764e 4c54 4566 6c75 782a  ta.convNLTEflux*
-000142e0: 3165 3233 290a 2020 2020 2020 2020 2020  1e23).          
-000142f0: 2020 506d 6f64 656c 3d73 7065 6374 7261    Pmodel=spectra
-00014300: 6c5f 666c 7578 5f70 726f 6475 6374 7328  l_flux_products(
-00014310: 7072 6f64 7563 745f 7769 6e64 6f77 732c  product_windows,
-00014320: 736c 6162 5f64 6174 612e 636f 6e76 5761  slab_data.convWa
-00014330: 7665 6c65 6e67 7468 2c73 6c61 625f 6461  velength,slab_da
-00014340: 7461 2e63 6f6e 764e 4c54 4566 6c75 782a  ta.convNLTEflux*
-00014350: 3165 3233 290a 2020 2020 2020 2020 656c  1e23).        el
-00014360: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00014370: 466d 6f64 656c 3d73 7065 6374 7261 6c5f  Fmodel=spectral_
-00014380: 666c 7578 6573 2877 696e 646f 7773 2c73  fluxes(windows,s
-00014390: 6c61 625f 6461 7461 2e63 6f6e 7657 6176  lab_data.convWav
-000143a0: 656c 656e 6774 682c 736c 6162 5f64 6174  elength,slab_dat
-000143b0: 612e 636f 6e76 4c54 4566 6c75 782a 3165  a.convLTEflux*1e
-000143c0: 3233 290a 2020 2020 2020 2020 2020 2020  23).            
-000143d0: 526d 6f64 656c 3d73 7065 6374 7261 6c5f  Rmodel=spectral_
-000143e0: 666c 7578 5f72 6174 696f 7328 7261 7469  flux_ratios(rati
-000143f0: 6f5f 7769 6e64 6f77 732c 736c 6162 5f64  o_windows,slab_d
-00014400: 6174 612e 636f 6e76 5761 7665 6c65 6e67  ata.convWaveleng
-00014410: 7468 2c73 6c61 625f 6461 7461 2e63 6f6e  th,slab_data.con
-00014420: 764c 5445 666c 7578 2a31 6532 3329 0a20  vLTEflux*1e23). 
-00014430: 2020 2020 2020 2020 2020 2050 6d6f 6465             Pmode
-00014440: 6c3d 7370 6563 7472 616c 5f66 6c75 785f  l=spectral_flux_
-00014450: 7072 6f64 7563 7473 2870 726f 6475 6374  products(product
-00014460: 5f77 696e 646f 7773 2c73 6c61 625f 6461  _windows,slab_da
-00014470: 7461 2e63 6f6e 7657 6176 656c 656e 6774  ta.convWavelengt
-00014480: 682c 736c 6162 5f64 6174 612e 636f 6e76  h,slab_data.conv
-00014490: 4c54 4566 6c75 782a 3165 3233 290a 2020  LTEflux*1e23).  
-000144a0: 2020 656c 7365 3a20 2023 2074 6f20 6573    else:  # to es
-000144b0: 7469 6d61 7465 2066 6c75 7820 6672 6f6d  timate flux from
-000144c0: 206c 696e 6520 6c69 7374 0a20 2020 2020   line list.     
-000144d0: 2020 2069 6620 4e4c 5445 3a0a 2020 2020     if NLTE:.    
-000144e0: 2020 2020 2020 2020 743d 2746 4e4c 5445          t='FNLTE
-000144f0: 270a 2020 2020 2020 2020 656c 7365 3a0a  '.        else:.
-00014500: 2020 2020 2020 2020 2020 2020 743d 2746              t='F
-00014510: 4c54 4527 0a20 2020 2020 2020 206c 696e  LTE'.        lin
-00014520: 6564 6174 613d 736c 6162 5f64 6174 612e  edata=slab_data.
-00014530: 6c69 6e65 6461 7461 0a20 2020 2020 2020  linedata.       
-00014540: 206c 696e 6564 6174 612e 736f 7274 5f76   linedata.sort_v
-00014550: 616c 7565 7328 6279 3d5b 2747 487a 275d  alues(by=['GHz']
-00014560: 2c61 7363 656e 6469 6e67 3d46 616c 7365  ,ascending=False
-00014570: 2c69 6e70 6c61 6365 3d54 7275 652c 6967  ,inplace=True,ig
-00014580: 6e6f 7265 5f69 6e64 6578 3d54 7275 6529  nore_index=True)
-00014590: 0a20 2020 2020 2020 2046 6d6f 6465 6c3d  .        Fmodel=
-000145a0: 6c69 6e65 5f66 6c75 7865 7328 7769 6e64  line_fluxes(wind
-000145b0: 6f77 732c 632f 6c69 6e65 6461 7461 5b27  ows,c/linedata['
-000145c0: 4748 7a27 5d2a 3165 2d33 2c6c 696e 6564  GHz']*1e-3,lined
-000145d0: 6174 615b 745d 290a 2020 2020 2020 2020  ata[t]).        
-000145e0: 526d 6f64 656c 3d6c 696e 655f 666c 7578  Rmodel=line_flux
-000145f0: 5f72 6174 696f 7328 7261 7469 6f5f 7769  _ratios(ratio_wi
-00014600: 6e64 6f77 732c 632f 6c69 6e65 6461 7461  ndows,c/linedata
-00014610: 5b27 4748 7a27 5d2a 3165 2d33 2c6c 696e  ['GHz']*1e-3,lin
-00014620: 6564 6174 615b 745d 290a 2020 2020 2020  edata[t]).      
-00014630: 2020 506d 6f64 656c 3d6c 696e 655f 666c    Pmodel=line_fl
-00014640: 7578 5f72 6174 696f 7328 7072 6f64 7563  ux_ratios(produc
-00014650: 745f 7769 6e64 6f77 732c 632f 6c69 6e65  t_windows,c/line
-00014660: 6461 7461 5b27 4748 7a27 5d2a 3165 2d33  data['GHz']*1e-3
-00014670: 2c6c 696e 6564 6174 615b 745d 290a 2020  ,linedata[t]).  
-00014680: 2020 466f 6273 6572 7665 643d 7370 6563    Fobserved=spec
-00014690: 7472 616c 5f66 6c75 7865 7328 7769 6e64  tral_fluxes(wind
-000146a0: 6f77 732c 7370 6563 7472 615b 3a2c 305d  ows,spectra[:,0]
-000146b0: 2c73 7065 6374 7261 5b3a 2c31 5d29 0a20  ,spectra[:,1]). 
-000146c0: 2020 2052 6f62 7365 7276 6564 3d73 7065     Robserved=spe
-000146d0: 6374 7261 6c5f 666c 7578 5f72 6174 696f  ctral_flux_ratio
-000146e0: 7328 7261 7469 6f5f 7769 6e64 6f77 732c  s(ratio_windows,
-000146f0: 7370 6563 7472 615b 3a2c 305d 2c73 7065  spectra[:,0],spe
-00014700: 6374 7261 5b3a 2c31 5d29 0a20 2020 2050  ctra[:,1]).    P
-00014710: 6f62 7365 7276 6564 3d73 7065 6374 7261  observed=spectra
-00014720: 6c5f 666c 7578 5f70 726f 6475 6374 7328  l_flux_products(
-00014730: 7072 6f64 7563 745f 7769 6e64 6f77 732c  product_windows,
-00014740: 7370 6563 7472 615b 3a2c 305d 2c73 7065  spectra[:,0],spe
-00014750: 6374 7261 5b3a 2c31 5d29 0a20 2020 206e  ctra[:,1]).    n
-00014760: 6f72 6d5f 6661 6374 6f72 3d30 0a20 2020  orm_factor=0.   
-00014770: 2069 6620 6c65 6e28 7769 6e64 6f77 7329   if len(windows)
-00014780: 3e30 3a0a 2020 2020 2020 2020 6172 6561  >0:.        area
-00014790: 5f32 643d 6e70 2e64 7374 6163 6b28 5b61  _2d=np.dstack([a
-000147a0: 7265 6120 666f 7220 6920 696e 2072 616e  rea for i in ran
-000147b0: 6765 286c 656e 2877 696e 646f 7773 2929  ge(len(windows))
-000147c0: 5d29 2e73 7175 6565 7a65 2829 2e72 6573  ]).squeeze().res
-000147d0: 6861 7065 2828 6c65 6e28 6172 6561 292c  hape((len(area),
-000147e0: 6c65 6e28 7769 6e64 6f77 7329 2929 0a20  len(windows))). 
-000147f0: 2020 2020 2020 2046 6d6f 6465 6c5f 3264         Fmodel_2d
-00014800: 3d6e 702e 6473 7461 636b 285b 466d 6f64  =np.dstack([Fmod
-00014810: 656c 2066 6f72 2069 2069 6e20 7261 6e67  el for i in rang
-00014820: 6528 6c65 6e28 6172 6561 2929 5d29 2e73  e(len(area))]).s
-00014830: 7175 6565 7a65 2829 2e54 2e72 6573 6861  queeze().T.resha
-00014840: 7065 2828 6c65 6e28 6172 6561 292c 6c65  pe((len(area),le
-00014850: 6e28 7769 6e64 6f77 7329 2929 0a20 2020  n(windows))).   
-00014860: 2020 2020 2046 6f62 7365 7276 6564 5f32       Fobserved_2
-00014870: 643d 6e70 2e64 7374 6163 6b28 5b46 6f62  d=np.dstack([Fob
-00014880: 7365 7276 6564 2066 6f72 2069 2069 6e20  served for i in 
-00014890: 7261 6e67 6528 6c65 6e28 6172 6561 2929  range(len(area))
-000148a0: 5d29 2e73 7175 6565 7a65 2829 2e54 2e72  ]).squeeze().T.r
-000148b0: 6573 6861 7065 2828 6c65 6e28 6172 6561  eshape((len(area
-000148c0: 292c 6c65 6e28 7769 6e64 6f77 7329 2929  ),len(windows)))
-000148d0: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
-000148e0: 7769 6e64 6f77 735b 305d 293d 3d33 3a20  windows[0])==3: 
-000148f0: 2023 2077 6569 6768 7465 6420 6368 6932   # weighted chi2
-00014900: 0a20 2020 2020 2020 2020 2020 2077 696e  .            win
-00014910: 646f 7773 5f77 6569 6768 7473 3d6e 702e  dows_weights=np.
-00014920: 6172 7261 7928 5b77 696e 646f 7773 5b6b  array([windows[k
-00014930: 5d5b 325d 2066 6f72 206b 2069 6e20 7261  ][2] for k in ra
-00014940: 6e67 6528 6c65 6e28 7769 6e64 6f77 7329  nge(len(windows)
-00014950: 295d 290a 2020 2020 2020 2020 2020 2020  )]).            
-00014960: 7769 6e64 6f77 735f 7765 6967 6874 735f  windows_weights_
-00014970: 3264 3d6e 702e 6473 7461 636b 285b 7769  2d=np.dstack([wi
-00014980: 6e64 6f77 735f 7765 6967 6874 7320 666f  ndows_weights fo
-00014990: 7220 6920 696e 2072 616e 6765 286c 656e  r i in range(len
-000149a0: 2861 7265 6129 295d 292e 7371 7565 657a  (area))]).squeez
-000149b0: 6528 292e 542e 7265 7368 6170 6528 286c  e().T.reshape((l
-000149c0: 656e 2861 7265 6129 2c6c 656e 2877 696e  en(area),len(win
-000149d0: 646f 7773 5f77 6569 6768 7473 2929 290a  dows_weights))).
-000149e0: 2020 2020 2020 2020 2020 2020 6368 695f              chi_
-000149f0: 6172 6561 2b3d 6e70 2e73 756d 2828 2846  area+=np.sum(((F
-00014a00: 6d6f 6465 6c5f 3264 2a61 7265 615f 3264  model_2d*area_2d
-00014a10: 2d46 6f62 7365 7276 6564 5f32 6429 2f46  -Fobserved_2d)/F
-00014a20: 6f62 7365 7276 6564 5f32 6429 2a2a 322a  observed_2d)**2*
-00014a30: 7769 6e64 6f77 735f 7765 6967 6874 735f  windows_weights_
-00014a40: 3264 2c61 7869 733d 3129 0a20 2020 2020  2d,axis=1).     
-00014a50: 2020 2020 2020 206e 6f72 6d5f 6661 6374         norm_fact
-00014a60: 6f72 2b3d 6e70 2e73 756d 2877 696e 646f  or+=np.sum(windo
-00014a70: 7773 5f77 6569 6768 7473 290a 2020 2020  ws_weights).    
-00014a80: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00014a90: 2020 2020 2020 6368 695f 6172 6561 2b3d        chi_area+=
-00014aa0: 6e70 2e73 756d 2828 2846 6d6f 6465 6c5f  np.sum(((Fmodel_
-00014ab0: 3264 2a61 7265 615f 3264 2d46 6f62 7365  2d*area_2d-Fobse
-00014ac0: 7276 6564 5f32 6429 2f46 6f62 7365 7276  rved_2d)/Fobserv
-00014ad0: 6564 5f32 6429 2a2a 322c 6178 6973 3d31  ed_2d)**2,axis=1
-00014ae0: 290a 2020 2020 2020 2020 2020 2020 6e6f  ).            no
-00014af0: 726d 5f66 6163 746f 722b 3d6c 656e 2877  rm_factor+=len(w
-00014b00: 696e 646f 7773 290a 2020 2020 6966 206c  indows).    if l
-00014b10: 656e 2872 6174 696f 5f77 696e 646f 7773  en(ratio_windows
-00014b20: 293e 303a 0a20 2020 2020 2020 2052 6d6f  )>0:.        Rmo
-00014b30: 6465 6c5f 3264 3d6e 702e 6473 7461 636b  del_2d=np.dstack
-00014b40: 285b 526d 6f64 656c 2066 6f72 2069 2069  ([Rmodel for i i
-00014b50: 6e20 7261 6e67 6528 6c65 6e28 6172 6561  n range(len(area
-00014b60: 2929 5d29 2e73 7175 6565 7a65 2829 2e54  ))]).squeeze().T
-00014b70: 2e72 6573 6861 7065 2828 6c65 6e28 6172  .reshape((len(ar
-00014b80: 6561 292c 6c65 6e28 7261 7469 6f5f 7769  ea),len(ratio_wi
-00014b90: 6e64 6f77 7329 2929 0a20 2020 2020 2020  ndows))).       
-00014ba0: 2052 6f62 7365 7276 6564 5f32 643d 6e70   Robserved_2d=np
-00014bb0: 2e64 7374 6163 6b28 5b52 6f62 7365 7276  .dstack([Robserv
-00014bc0: 6564 2066 6f72 2069 2069 6e20 7261 6e67  ed for i in rang
-00014bd0: 6528 6c65 6e28 6172 6561 2929 5d29 2e73  e(len(area))]).s
-00014be0: 7175 6565 7a65 2829 2e54 2e72 6573 6861  queeze().T.resha
-00014bf0: 7065 2828 6c65 6e28 6172 6561 292c 6c65  pe((len(area),le
-00014c00: 6e28 7261 7469 6f5f 7769 6e64 6f77 7329  n(ratio_windows)
-00014c10: 2929 0a20 2020 2020 2020 2069 6620 286c  )).        if (l
-00014c20: 656e 2872 6174 696f 5f77 696e 646f 7773  en(ratio_windows
-00014c30: 5b30 5d29 3d3d 3329 3a20 2023 2077 6569  [0])==3):  # wei
-00014c40: 6768 7465 6420 6368 6932 0a20 2020 2020  ghted chi2.     
-00014c50: 2020 2020 2020 2072 6174 696f 5f77 696e         ratio_win
-00014c60: 646f 7773 5f77 6569 6768 7473 3d6e 702e  dows_weights=np.
-00014c70: 6172 7261 7928 5b72 6174 696f 5f77 696e  array([ratio_win
-00014c80: 646f 7773 5b6b 5d5b 325d 2066 6f72 206b  dows[k][2] for k
-00014c90: 2069 6e20 7261 6e67 6528 6c65 6e28 7261   in range(len(ra
-00014ca0: 7469 6f5f 7769 6e64 6f77 7329 295d 290a  tio_windows))]).
-00014cb0: 2020 2020 2020 2020 2020 2020 7261 7469              rati
-00014cc0: 6f5f 7769 6e64 6f77 735f 7765 6967 6874  o_windows_weight
-00014cd0: 735f 3264 3d6e 702e 6473 7461 636b 285b  s_2d=np.dstack([
-00014ce0: 7261 7469 6f5f 7769 6e64 6f77 735f 7765  ratio_windows_we
-00014cf0: 6967 6874 7320 666f 7220 6920 696e 2072  ights for i in r
-00014d00: 616e 6765 286c 656e 2861 7265 6129 295d  ange(len(area))]
-00014d10: 292e 7371 7565 657a 6528 292e 542e 7265  ).squeeze().T.re
-00014d20: 7368 6170 6528 286c 656e 2861 7265 6129  shape((len(area)
-00014d30: 2c6c 656e 2872 6174 696f 5f77 696e 646f  ,len(ratio_windo
-00014d40: 7773 5f77 6569 6768 7473 2929 290a 2020  ws_weights))).  
-00014d50: 2020 2020 2020 2020 2020 6368 695f 6172            chi_ar
-00014d60: 6561 2b3d 6e70 2e73 756d 2828 2852 6d6f  ea+=np.sum(((Rmo
-00014d70: 6465 6c5f 3264 2d52 6f62 7365 7276 6564  del_2d-Robserved
-00014d80: 5f32 6429 2f52 6f62 7365 7276 6564 5f32  _2d)/Robserved_2
-00014d90: 6429 2a2a 322a 7261 7469 6f5f 7769 6e64  d)**2*ratio_wind
-00014da0: 6f77 735f 7765 6967 6874 735f 3264 2c61  ows_weights_2d,a
-00014db0: 7869 733d 3129 0a20 2020 2020 2020 2020  xis=1).         
-00014dc0: 2020 206e 6f72 6d5f 6661 6374 6f72 2b3d     norm_factor+=
-00014dd0: 6e70 2e73 756d 2872 6174 696f 5f77 696e  np.sum(ratio_win
-00014de0: 646f 7773 5f77 6569 6768 7473 290a 2020  dows_weights).  
-00014df0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00014e00: 2020 2020 2020 2020 6368 695f 6172 6561          chi_area
-00014e10: 2b3d 6e70 2e73 756d 2828 2852 6d6f 6465  +=np.sum(((Rmode
-00014e20: 6c5f 3264 2d52 6f62 7365 7276 6564 5f32  l_2d-Robserved_2
-00014e30: 6429 2f52 6f62 7365 7276 6564 5f32 6429  d)/Robserved_2d)
-00014e40: 2a2a 322c 6178 6973 3d31 290a 2020 2020  **2,axis=1).    
-00014e50: 2020 2020 2020 2020 6e6f 726d 5f66 6163          norm_fac
-00014e60: 746f 722b 3d6c 656e 2872 6174 696f 5f77  tor+=len(ratio_w
-00014e70: 696e 646f 7773 290a 2020 2020 6966 206c  indows).    if l
-00014e80: 656e 2870 726f 6475 6374 5f77 696e 646f  en(product_windo
-00014e90: 7773 293e 303a 0a20 2020 2020 2020 2061  ws)>0:.        a
-00014ea0: 7265 615f 3264 3d6e 702e 6473 7461 636b  rea_2d=np.dstack
-00014eb0: 285b 6172 6561 2066 6f72 2069 2069 6e20  ([area for i in 
-00014ec0: 7261 6e67 6528 6c65 6e28 7072 6f64 7563  range(len(produc
-00014ed0: 745f 7769 6e64 6f77 7329 295d 292e 7371  t_windows))]).sq
-00014ee0: 7565 657a 6528 292e 7265 7368 6170 6528  ueeze().reshape(
-00014ef0: 286c 656e 2861 7265 6129 2c6c 656e 2870  (len(area),len(p
-00014f00: 726f 6475 6374 5f77 696e 646f 7773 2929  roduct_windows))
-00014f10: 290a 2020 2020 2020 2020 506d 6f64 656c  ).        Pmodel
-00014f20: 5f32 643d 6e70 2e64 7374 6163 6b28 5b50  _2d=np.dstack([P
-00014f30: 6d6f 6465 6c20 666f 7220 6920 696e 2072  model for i in r
-00014f40: 616e 6765 286c 656e 2861 7265 6129 295d  ange(len(area))]
-00014f50: 292e 7371 7565 657a 6528 292e 542e 7265  ).squeeze().T.re
-00014f60: 7368 6170 6528 286c 656e 2861 7265 6129  shape((len(area)
-00014f70: 2c6c 656e 2870 726f 6475 6374 5f77 696e  ,len(product_win
-00014f80: 646f 7773 2929 290a 2020 2020 2020 2020  dows))).        
-00014f90: 506f 6273 6572 7665 645f 3264 3d6e 702e  Pobserved_2d=np.
-00014fa0: 6473 7461 636b 285b 506f 6273 6572 7665  dstack([Pobserve
-00014fb0: 6420 666f 7220 6920 696e 2072 616e 6765  d for i in range
-00014fc0: 286c 656e 2861 7265 6129 295d 292e 7371  (len(area))]).sq
-00014fd0: 7565 657a 6528 292e 542e 7265 7368 6170  ueeze().T.reshap
-00014fe0: 6528 286c 656e 2861 7265 6129 2c6c 656e  e((len(area),len
-00014ff0: 2870 726f 6475 6374 5f77 696e 646f 7773  (product_windows
-00015000: 2929 290a 2020 2020 2020 2020 6966 2028  ))).        if (
-00015010: 6c65 6e28 7072 6f64 7563 745f 7769 6e64  len(product_wind
-00015020: 6f77 735b 305d 293d 3d33 293a 2020 2320  ows[0])==3):  # 
-00015030: 7765 6967 6874 6564 2063 6869 320a 2020  weighted chi2.  
-00015040: 2020 2020 2020 2020 2020 7072 6f64 7563            produc
-00015050: 745f 7769 6e64 6f77 735f 7765 6967 6874  t_windows_weight
-00015060: 733d 6e70 2e61 7272 6179 285b 7072 6f64  s=np.array([prod
-00015070: 7563 745f 7769 6e64 6f77 735b 6b5d 5b32  uct_windows[k][2
-00015080: 5d20 666f 7220 6b20 696e 2072 616e 6765  ] for k in range
-00015090: 286c 656e 2870 726f 6475 6374 5f77 696e  (len(product_win
-000150a0: 646f 7773 2929 5d29 0a20 2020 2020 2020  dows))]).       
-000150b0: 2020 2020 2070 726f 6475 6374 5f77 696e       product_win
-000150c0: 646f 7773 5f77 6569 6768 7473 5f32 643d  dows_weights_2d=
-000150d0: 6e70 2e64 7374 6163 6b28 5b70 726f 6475  np.dstack([produ
-000150e0: 6374 5f77 696e 646f 7773 5f77 6569 6768  ct_windows_weigh
-000150f0: 7473 2066 6f72 2069 2069 6e20 7261 6e67  ts for i in rang
-00015100: 6528 6c65 6e28 6172 6561 2929 5d29 2e73  e(len(area))]).s
-00015110: 7175 6565 7a65 2829 2e54 2e72 6573 6861  queeze().T.resha
-00015120: 7065 2828 6c65 6e28 6172 6561 292c 6c65  pe((len(area),le
-00015130: 6e28 7072 6f64 7563 745f 7769 6e64 6f77  n(product_window
-00015140: 735f 7765 6967 6874 7329 2929 0a20 2020  s_weights))).   
-00015150: 2020 2020 2020 2020 2063 6869 5f61 7265           chi_are
-00015160: 612b 3d6e 702e 7375 6d28 2828 2850 6d6f  a+=np.sum((((Pmo
-00015170: 6465 6c5f 3264 2a61 7265 615f 3264 2a2a  del_2d*area_2d**
-00015180: 3229 2a2a 302e 352d 2850 6f62 7365 7276  2)**0.5-(Pobserv
-00015190: 6564 5f32 6429 2a2a 302e 3529 2f28 506f  ed_2d)**0.5)/(Po
-000151a0: 6273 6572 7665 645f 3264 292a 2a30 2e35  bserved_2d)**0.5
-000151b0: 292a 2a32 2a70 726f 6475 6374 5f77 696e  )**2*product_win
-000151c0: 646f 7773 5f77 6569 6768 7473 5f32 642c  dows_weights_2d,
-000151d0: 6178 6973 3d31 290a 2020 2020 2020 2020  axis=1).        
-000151e0: 2020 2020 6e6f 726d 5f66 6163 746f 722b      norm_factor+
-000151f0: 3d6e 702e 7375 6d28 7072 6f64 7563 745f  =np.sum(product_
-00015200: 7769 6e64 6f77 735f 7765 6967 6874 7329  windows_weights)
-00015210: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00015220: 2020 2020 2020 2020 2020 2063 6869 5f61             chi_a
-00015230: 7265 612b 3d6e 702e 7375 6d28 2828 2850  rea+=np.sum((((P
-00015240: 6d6f 6465 6c5f 3264 2a61 7265 615f 3264  model_2d*area_2d
-00015250: 2a2a 3229 2a2a 302e 352d 2850 6f62 7365  **2)**0.5-(Pobse
-00015260: 7276 6564 5f32 6429 2a2a 302e 3529 2f28  rved_2d)**0.5)/(
-00015270: 506f 6273 6572 7665 645f 3264 292a 2a30  Pobserved_2d)**0
-00015280: 2e35 292a 2a32 2c61 7869 733d 3129 0a20  .5)**2,axis=1). 
-00015290: 2020 2020 2020 2020 2020 206e 6f72 6d5f             norm_
-000152a0: 6661 6374 6f72 2b3d 6c65 6e28 7072 6f64  factor+=len(prod
-000152b0: 7563 745f 7769 6e64 6f77 7329 0a20 2020  uct_windows).   
-000152c0: 2069 6620 6e6f 726d 5f66 6163 746f 723e   if norm_factor>
-000152d0: 303a 2063 6869 5f61 7265 612f 3d6e 6f72  0: chi_area/=nor
-000152e0: 6d5f 6661 6374 6f72 0a20 2020 2072 6574  m_factor.    ret
-000152f0: 7572 6e28 6368 695f 6172 6561 290a 0a0a  urn(chi_area)...
-00015300: 6465 6620 7265 645f 6368 6932 5f73 6c61  def red_chi2_sla
-00015310: 6228 736c 6162 5f64 6174 612c 7370 6563  b(slab_data,spec
-00015320: 7472 612c 6d61 736b 2c52 6469 736b 3d6e  tra,mask,Rdisk=n
-00015330: 702e 6c6f 6773 7061 6365 282d 322c 322c  p.logspace(-2,2,
-00015340: 3130 292c 6469 7374 616e 6365 3d31 3230  10),distance=120
-00015350: 2c4e 4c54 453d 4661 6c73 652c 523d 3330  ,NLTE=False,R=30
-00015360: 3030 2c73 686f 7274 5f66 6f72 6d61 743d  00,short_format=
-00015370: 4661 6c73 652c 6f76 6572 6c61 703d 4661  False,overlap=Fa
-00015380: 6c73 652c 6e6f 6973 655f 6c65 7665 6c3d  lse,noise_level=
-00015390: 3129 3a0a 2020 2020 2727 270a 2020 2020  1):.    '''.    
-000153a0: 5265 7475 726e 7320 7265 6475 6365 6420  Returns reduced 
-000153b0: 6368 6932 2062 6173 6564 206f 6e20 7365  chi2 based on se
-000153c0: 6c65 6374 6564 2073 7065 6374 7261 6c20  lected spectral 
-000153d0: 7769 6e64 6f77 7320 6163 726f 7373 2064  windows across d
-000153e0: 6966 6665 7265 6e74 2065 6d69 7474 696e  ifferent emittin
-000153f0: 6720 6469 736b 2072 6164 6975 730a 0a20  g disk radius.. 
-00015400: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-00015410: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-00015420: 2073 6c61 625f 6461 7461 203a 2073 7472   slab_data : str
-00015430: 696e 6720 6f72 2073 6c61 625f 6d6f 6465  ing or slab_mode
-00015440: 6c20 696e 7374 616e 6365 0a20 2020 2020  l instance.     
-00015450: 2070 6174 6820 636f 7272 6573 706f 6e64   path correspond
-00015460: 696e 6720 746f 2061 2073 696e 676c 6520  ing to a single 
-00015470: 736c 6162 206d 6f64 656c 206f 7220 6120  slab model or a 
-00015480: 7369 6e67 6c65 2073 6c61 625f 6d6f 6465  single slab_mode
-00015490: 6c20 696e 7374 616e 6365 0a20 2020 200a  l instance.    .
-000154a0: 2020 2020 7370 6563 7472 6120 3a20 6e75      spectra : nu
-000154b0: 6d70 792e 6172 7261 790a 2020 2020 2020  mpy.array.      
-000154c0: 6e75 6d70 7920 6172 7261 7920 7769 7468  numpy array with
-000154d0: 2066 6972 7374 2063 6f6c 756d 6e20 7468   first column th
-000154e0: 6520 7761 7665 6c65 6e67 7468 2069 6e20  e wavelength in 
-000154f0: 5b6d 6963 726f 6e73 5d20 616e 6420 7365  [microns] and se
-00015500: 636f 6e64 2063 6f6c 756d 6e20 666c 7578  cond column flux
-00015510: 2069 6e20 5b4a 795d 0a20 2020 200a 2020   in [Jy].    .  
-00015520: 2020 5264 6973 6b20 3a20 666c 6f61 740a    Rdisk : float.
-00015530: 2020 2020 2020 5261 6469 7573 2063 6f72        Radius cor
-00015540: 7265 7370 6f6e 6469 6e67 2074 6f20 656d  responding to em
-00015550: 6974 7469 6e67 2061 7265 6120 696e 2061  itting area in a
-00015560: 7374 726f 6e6f 6d69 6361 6c20 756e 6974  stronomical unit
-00015570: 730a 2020 2020 0a20 2020 2064 6973 7461  s.    .    dista
-00015580: 6e63 6520 3a20 666c 6f61 740a 2020 2020  nce : float.    
-00015590: 2020 6469 7374 616e 6365 206f 6620 6469    distance of di
-000155a0: 736b 2069 6e20 7061 7273 6563 0a20 2020  sk in parsec.   
-000155b0: 200a 2020 2020 4e4c 5445 203a 2062 6f6f   .    NLTE : boo
-000155c0: 6c65 616e 0a20 2020 2020 2069 6620 5472  lean.      if Tr
-000155d0: 7565 2c20 4e4c 5445 2066 6c75 7820 6973  ue, NLTE flux is
-000155e0: 2074 616b 656e 2066 726f 6d20 7468 6520   taken from the 
-000155f0: 736c 6162 206d 6f64 656c 2069 6e20 6361  slab model in ca
-00015600: 7365 206f 6620 6f76 6572 6c61 703d 4661  se of overlap=Fa
-00015610: 6c73 652e 0a20 2020 2027 2727 0a20 2020  lse..    '''.   
-00015620: 2061 7265 613d 286e 702e 7069 2a28 5264   area=(np.pi*(Rd
-00015630: 6973 6b2a 6175 2f64 6973 7461 6e63 652f  isk*au/distance/
-00015640: 7063 292a 2a32 292e 7265 7368 6170 6528  pc)**2).reshape(
-00015650: 5264 6973 6b2e 7368 6170 655b 305d 2c31  Rdisk.shape[0],1
-00015660: 290a 0a20 2020 2069 6620 6e6f 7420 6f76  )..    if not ov
-00015670: 6572 6c61 703a 0a20 2020 2020 2020 2069  erlap:.        i
-00015680: 6620 6973 696e 7374 616e 6365 2873 6c61  f isinstance(sla
-00015690: 625f 6461 7461 2c73 7472 293a 2073 6c61  b_data,str): sla
-000156a0: 625f 6461 7461 3d72 6561 645f 736c 6162  b_data=read_slab
-000156b0: 2873 6c61 625f 6461 7461 2c76 6572 626f  (slab_data,verbo
-000156c0: 7365 3d46 616c 7365 2c73 686f 7274 5f66  se=False,short_f
-000156d0: 6f72 6d61 743d 7368 6f72 745f 666f 726d  ormat=short_form
-000156e0: 6174 290a 2020 2020 2020 2020 6c6d 696e  at).        lmin
-000156f0: 3d6e 702e 616d 696e 2873 7065 6374 7261  =np.amin(spectra
-00015700: 5b3a 2c30 5d29 0a20 2020 2020 2020 206c  [:,0]).        l
-00015710: 6d61 783d 6e70 2e61 6d61 7828 7370 6563  max=np.amax(spec
-00015720: 7472 615b 3a2c 305d 290a 2020 2020 2020  tra[:,0]).      
-00015730: 2020 736c 6162 5f64 6174 612e 636f 6e76    slab_data.conv
-00015740: 6f6c 7665 2852 3d52 2c6c 616d 6264 615f  olve(R=R,lambda_
-00015750: 303d 6c6d 696e 2a30 2e39 2c6c 616d 6264  0=lmin*0.9,lambd
-00015760: 615f 6e3d 6c6d 6178 2a31 2e31 2c4e 4c54  a_n=lmax*1.1,NLT
-00015770: 453d 4e4c 5445 2c76 6572 626f 7365 3d46  E=NLTE,verbose=F
-00015780: 616c 7365 290a 2020 2020 2020 2020 6966  alse).        if
-00015790: 204e 4c54 453a 0a20 2020 2020 2020 2020   NLTE:.         
-000157a0: 2020 206d 6f64 656c 5370 6563 3d73 7065     modelSpec=spe
-000157b0: 6374 7265 732e 7370 6563 7472 6573 2873  ctres.spectres(s
-000157c0: 7065 6374 7261 5b3a 2c30 5d2c 736c 6162  pectra[:,0],slab
-000157d0: 5f64 6174 612e 636f 6e76 5761 7665 6c65  _data.convWavele
-000157e0: 6e67 7468 2c73 6c61 625f 6461 7461 2e63  ngth,slab_data.c
-000157f0: 6f6e 764e 4c54 4566 6c75 782a 3165 3233  onvNLTEflux*1e23
-00015800: 2c76 6572 626f 7365 3d46 616c 7365 2c66  ,verbose=False,f
-00015810: 696c 6c3d 302e 3029 0a20 2020 2020 2020  ill=0.0).       
-00015820: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00015830: 2020 206d 6f64 656c 5370 6563 3d73 7065     modelSpec=spe
-00015840: 6374 7265 732e 7370 6563 7472 6573 2873  ctres.spectres(s
-00015850: 7065 6374 7261 5b3a 2c30 5d2c 736c 6162  pectra[:,0],slab
-00015860: 5f64 6174 612e 636f 6e76 5761 7665 6c65  _data.convWavele
-00015870: 6e67 7468 2c73 6c61 625f 6461 7461 2e63  ngth,slab_data.c
-00015880: 6f6e 764c 5445 666c 7578 2a31 6532 332c  onvLTEflux*1e23,
-00015890: 7665 7262 6f73 653d 4661 6c73 652c 6669  verbose=False,fi
-000158a0: 6c6c 3d30 2e30 290a 2020 2020 656c 7365  ll=0.0).    else
-000158b0: 3a0a 2020 2020 2020 2020 6966 2069 7369  :.        if isi
-000158c0: 6e73 7461 6e63 6528 736c 6162 5f64 6174  nstance(slab_dat
-000158d0: 612c 7374 7229 3a20 736c 6162 5f64 6174  a,str): slab_dat
-000158e0: 613d 7265 6164 5f6f 7665 726c 6170 5f73  a=read_overlap_s
-000158f0: 7065 6374 7261 2873 6c61 625f 6461 7461  pectra(slab_data
-00015900: 2c76 6572 626f 7365 3d46 616c 7365 290a  ,verbose=False).
-00015910: 2020 2020 2020 2020 6c6d 696e 3d6e 702e          lmin=np.
-00015920: 616d 696e 2873 7065 6374 7261 5b3a 2c30  amin(spectra[:,0
-00015930: 5d29 0a20 2020 2020 2020 206c 6d61 783d  ]).        lmax=
-00015940: 6e70 2e61 6d61 7828 7370 6563 7472 615b  np.amax(spectra[
-00015950: 3a2c 305d 290a 2020 2020 2020 2020 736c  :,0]).        sl
-00015960: 6162 5f64 6174 612e 636f 6e76 6f6c 7665  ab_data.convolve
-00015970: 5f6f 7665 726c 6170 2852 3d52 2c6c 616d  _overlap(R=R,lam
-00015980: 6264 615f 303d 6c6d 696e 2a30 2e39 2c6c  bda_0=lmin*0.9,l
-00015990: 616d 6264 615f 6e3d 6c6d 6178 2a31 2e31  ambda_n=lmax*1.1
-000159a0: 2c76 6572 626f 7365 3d46 616c 7365 290a  ,verbose=False).
-000159b0: 2020 2020 2020 2020 6d6f 6465 6c53 7065          modelSpe
-000159c0: 633d 7370 6563 7472 6573 2e73 7065 6374  c=spectres.spect
-000159d0: 7265 7328 7370 6563 7472 615b 3a2c 305d  res(spectra[:,0]
-000159e0: 2c63 2f73 6c61 625f 6461 7461 2e63 6f6e  ,c/slab_data.con
-000159f0: 764f 7665 726c 6170 4672 6571 5b3a 3a2d  vOverlapFreq[::-
-00015a00: 315d 2a31 652d 332c 736c 6162 5f64 6174  1]*1e-3,slab_dat
-00015a10: 612e 636f 6e76 4f76 6572 6c61 704c 5445  a.convOverlapLTE
-00015a20: 5b3a 3a2d 315d 2a31 6532 332c 7665 7262  [::-1]*1e23,verb
-00015a30: 6f73 653d 4661 6c73 652c 6669 6c6c 3d30  ose=False,fill=0
-00015a40: 2e30 290a 2020 2020 7370 6563 7472 615f  .0).    spectra_
-00015a50: 3264 3d73 7065 6374 7261 5b6d 6173 6b2c  2d=spectra[mask,
-00015a60: 315d 2e72 6573 6861 7065 2831 2c73 7065  1].reshape(1,spe
-00015a70: 6374 7261 5b6d 6173 6b2c 2d31 5d2e 7368  ctra[mask,-1].sh
-00015a80: 6170 655b 305d 292a 6e70 2e6f 6e65 735f  ape[0])*np.ones_
-00015a90: 6c69 6b65 2861 7265 6129 0a20 2020 206d  like(area).    m
-00015aa0: 6f64 656c 5370 6563 5f32 643d 6d6f 6465  odelSpec_2d=mode
-00015ab0: 6c53 7065 635b 6d61 736b 5d2e 7265 7368  lSpec[mask].resh
-00015ac0: 6170 6528 312c 6d6f 6465 6c53 7065 635b  ape(1,modelSpec[
-00015ad0: 6d61 736b 5d2e 7368 6170 655b 305d 292a  mask].shape[0])*
-00015ae0: 6e70 2e6f 6e65 735f 6c69 6b65 2861 7265  np.ones_like(are
-00015af0: 6129 0a20 2020 2061 7265 615f 3264 3d61  a).    area_2d=a
-00015b00: 7265 612e 7265 7368 6170 6528 6172 6561  rea.reshape(area
-00015b10: 2e73 6861 7065 5b30 5d2c 3129 0a20 2020  .shape[0],1).   
-00015b20: 2063 6869 5f61 7265 613d 6e70 2e73 756d   chi_area=np.sum
-00015b30: 2828 7370 6563 7472 615f 3264 2d6d 6f64  ((spectra_2d-mod
-00015b40: 656c 5370 6563 5f32 642a 6172 6561 5f32  elSpec_2d*area_2
-00015b50: 6429 2a2a 322c 6178 6973 3d31 292f 6c65  d)**2,axis=1)/le
-00015b60: 6e28 7370 6563 7472 615b 6d61 736b 2c30  n(spectra[mask,0
-00015b70: 5d29 2f6e 6f69 7365 5f6c 6576 656c 2a2a  ])/noise_level**
-00015b80: 320a 0a20 2020 2072 6574 7572 6e28 6368  2..    return(ch
-00015b90: 695f 6172 6561 290a                      i_area).
+0000fed0: 0a20 2020 206e 4831 5f6c 6973 743d 6e70  .    nH1_list=np
+0000fee0: 2e6f 6e65 7328 286e 6d6f 6465 6c73 2929  .ones((nmodels))
+0000fef0: 0a20 2020 206e 4832 5f6c 6973 743d 6e70  .    nH2_list=np
+0000ff00: 2e6f 6e65 7328 286e 6d6f 6465 6c73 2929  .ones((nmodels))
+0000ff10: 0a20 2020 206e 4865 5f6c 6973 743d 6e70  .    nHe_list=np
+0000ff20: 2e6f 6e65 7328 286e 6d6f 6465 6c73 2929  .ones((nmodels))
+0000ff30: 0a20 2020 206e 656c 6563 5f6c 6973 743d  .    nelec_list=
+0000ff40: 6e70 2e6f 6e65 7328 286e 6d6f 6465 6c73  np.ones((nmodels
+0000ff50: 2929 0a20 2020 2054 645f 6c69 7374 3d6e  )).    Td_list=n
+0000ff60: 702e 6f6e 6573 2828 6e6d 6f64 656c 7329  p.ones((nmodels)
+0000ff70: 290a 2020 2020 7674 7572 625f 6c69 7374  ).    vturb_list
+0000ff80: 3d6e 702e 6f6e 6573 2828 6e6d 6f64 656c  =np.ones((nmodel
+0000ff90: 7329 290a 2020 2020 6475 7374 5f74 6f5f  s)).    dust_to_
+0000ffa0: 6761 735f 6c69 7374 3d6e 702e 6f6e 6573  gas_list=np.ones
+0000ffb0: 2828 6e6d 6f64 656c 7329 290a 2020 2020  ((nmodels)).    
+0000ffc0: 525f 6f76 6572 6c61 705f 6c69 7374 3d6e  R_overlap_list=n
+0000ffd0: 702e 6f6e 6573 2828 6e6d 6f64 656c 7329  p.ones((nmodels)
+0000ffe0: 290a 2020 2020 6c69 6e65 5f6f 7665 726c  ).    line_overl
+0000fff0: 6170 5f6c 6973 743d 6e70 2e6f 6e65 7328  ap_list=np.ones(
+00010000: 286e 6d6f 6465 6c73 2c32 2929 0a20 2020  (nmodels,2)).   
+00010010: 2069 6620 6c65 6e28 7370 6563 6965 735f   if len(species_
+00010020: 6c69 7374 293c 313a 2072 6169 7365 2056  list)<1: raise V
+00010030: 616c 7565 4572 726f 7228 2754 6865 2073  alueError('The s
+00010040: 7065 6369 6573 5f6c 6973 7420 6361 6e6e  pecies_list cann
+00010050: 6f74 2062 6520 656d 7074 7927 290a 0a20  ot be empty').. 
+00010060: 2020 2069 6620 6e6f 7420 636f 6d62 696e     if not combin
+00010070: 6174 696f 6e3a 0a20 2020 2020 2020 2066  ation:.        f
+00010080: 6f72 2069 2069 6e20 7261 6e67 6528 6c65  or i in range(le
+00010090: 6e28 6772 6964 5f70 6172 616d 6574 6572  n(grid_parameter
+000100a0: 7329 293a 0a20 2020 2020 2020 2020 2020  s)):.           
+000100b0: 2069 6620 6c69 7374 2867 7269 645f 7061   if list(grid_pa
+000100c0: 7261 6d65 7465 7273 2e6b 6579 7328 2929  rameters.keys())
+000100d0: 5b69 5d3d 3d27 4e74 6f74 273a 0a20 2020  [i]=='Ntot':.   
+000100e0: 2020 2020 2020 2020 2020 2020 204e 746f               Nto
+000100f0: 745f 6c69 7374 2a3d 6772 6964 5f70 6172  t_list*=grid_par
+00010100: 616d 6574 6572 735b 274e 746f 7427 5d0a  ameters['Ntot'].
+00010110: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00010120: 206c 6973 7428 6772 6964 5f70 6172 616d   list(grid_param
+00010130: 6574 6572 732e 6b65 7973 2829 295b 695d  eters.keys())[i]
+00010140: 3d3d 2754 6727 3a0a 2020 2020 2020 2020  =='Tg':.        
+00010150: 2020 2020 2020 2020 5467 5f6c 6973 742a          Tg_list*
+00010160: 3d67 7269 645f 7061 7261 6d65 7465 7273  =grid_parameters
+00010170: 5b27 5467 275d 0a20 2020 2020 2020 2020  ['Tg'].         
+00010180: 2020 2065 6c69 6620 6c69 7374 2867 7269     elif list(gri
+00010190: 645f 7061 7261 6d65 7465 7273 2e6b 6579  d_parameters.key
+000101a0: 7328 2929 5b69 5d3d 3d27 6e48 706c 7573  s())[i]=='nHplus
+000101b0: 273a 0a20 2020 2020 2020 2020 2020 2020  ':.             
+000101c0: 2020 206e 4870 6c75 735f 6c69 7374 2a3d     nHplus_list*=
+000101d0: 6772 6964 5f70 6172 616d 6574 6572 735b  grid_parameters[
+000101e0: 276e 4870 6c75 7327 5d0a 2020 2020 2020  'nHplus'].      
+000101f0: 2020 2020 2020 656c 6966 206c 6973 7428        elif list(
+00010200: 6772 6964 5f70 6172 616d 6574 6572 732e  grid_parameters.
+00010210: 6b65 7973 2829 295b 695d 3d3d 276e 4831  keys())[i]=='nH1
+00010220: 273a 0a20 2020 2020 2020 2020 2020 2020  ':.             
+00010230: 2020 206e 4831 5f6c 6973 742a 3d67 7269     nH1_list*=gri
+00010240: 645f 7061 7261 6d65 7465 7273 5b27 6e48  d_parameters['nH
+00010250: 3127 5d0a 2020 2020 2020 2020 2020 2020  1'].            
+00010260: 656c 6966 206c 6973 7428 6772 6964 5f70  elif list(grid_p
+00010270: 6172 616d 6574 6572 732e 6b65 7973 2829  arameters.keys()
+00010280: 295b 695d 3d3d 276e 4832 273a 0a20 2020  )[i]=='nH2':.   
+00010290: 2020 2020 2020 2020 2020 2020 206e 4832               nH2
+000102a0: 5f6c 6973 742a 3d67 7269 645f 7061 7261  _list*=grid_para
+000102b0: 6d65 7465 7273 5b27 6e48 3227 5d0a 2020  meters['nH2'].  
+000102c0: 2020 2020 2020 2020 2020 656c 6966 206c            elif l
+000102d0: 6973 7428 6772 6964 5f70 6172 616d 6574  ist(grid_paramet
+000102e0: 6572 732e 6b65 7973 2829 295b 695d 3d3d  ers.keys())[i]==
+000102f0: 276e 4865 273a 0a20 2020 2020 2020 2020  'nHe':.         
+00010300: 2020 2020 2020 206e 4865 5f6c 6973 742a         nHe_list*
+00010310: 3d67 7269 645f 7061 7261 6d65 7465 7273  =grid_parameters
+00010320: 5b27 6e48 6527 5d0a 2020 2020 2020 2020  ['nHe'].        
+00010330: 2020 2020 656c 6966 206c 6973 7428 6772      elif list(gr
+00010340: 6964 5f70 6172 616d 6574 6572 732e 6b65  id_parameters.ke
+00010350: 7973 2829 295b 695d 3d3d 276e 656c 6563  ys())[i]=='nelec
+00010360: 273a 0a20 2020 2020 2020 2020 2020 2020  ':.             
+00010370: 2020 206e 656c 6563 5f6c 6973 742a 3d67     nelec_list*=g
+00010380: 7269 645f 7061 7261 6d65 7465 7273 5b27  rid_parameters['
+00010390: 6e65 6c65 6327 5d0a 2020 2020 2020 2020  nelec'].        
+000103a0: 2020 2020 656c 6966 206c 6973 7428 6772      elif list(gr
+000103b0: 6964 5f70 6172 616d 6574 6572 732e 6b65  id_parameters.ke
+000103c0: 7973 2829 295b 695d 3d3d 2754 6427 3a0a  ys())[i]=='Td':.
+000103d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000103e0: 5464 5f6c 6973 742a 3d67 7269 645f 7061  Td_list*=grid_pa
+000103f0: 7261 6d65 7465 7273 5b27 5464 275d 0a20  rameters['Td']. 
+00010400: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00010410: 6c69 7374 2867 7269 645f 7061 7261 6d65  list(grid_parame
+00010420: 7465 7273 2e6b 6579 7328 2929 5b69 5d3d  ters.keys())[i]=
+00010430: 3d27 7674 7572 6227 3a0a 2020 2020 2020  ='vturb':.      
+00010440: 2020 2020 2020 2020 2020 7674 7572 625f            vturb_
+00010450: 6c69 7374 2a3d 6772 6964 5f70 6172 616d  list*=grid_param
+00010460: 6574 6572 735b 2776 7475 7262 275d 0a20  eters['vturb']. 
+00010470: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00010480: 6c69 7374 2867 7269 645f 7061 7261 6d65  list(grid_parame
+00010490: 7465 7273 2e6b 6579 7328 2929 5b69 5d3d  ters.keys())[i]=
+000104a0: 3d27 6475 7374 5f74 6f5f 6761 7327 3a0a  ='dust_to_gas':.
+000104b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000104c0: 6475 7374 5f74 6f5f 6761 735f 6c69 7374  dust_to_gas_list
+000104d0: 2a3d 6772 6964 5f70 6172 616d 6574 6572  *=grid_parameter
+000104e0: 735b 2764 7573 745f 746f 5f67 6173 275d  s['dust_to_gas']
+000104f0: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+00010500: 6620 6c69 7374 2867 7269 645f 7061 7261  f list(grid_para
+00010510: 6d65 7465 7273 2e6b 6579 7328 2929 5b69  meters.keys())[i
+00010520: 5d3d 3d27 525f 6f76 6572 6c61 7027 3a0a  ]=='R_overlap':.
+00010530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010540: 525f 6f76 6572 6c61 705f 6c69 7374 2a3d  R_overlap_list*=
+00010550: 6772 6964 5f70 6172 616d 6574 6572 735b  grid_parameters[
+00010560: 2752 5f6f 7665 726c 6170 275d 0a20 2020  'R_overlap'].   
+00010570: 2020 2020 2020 2020 2065 6c69 6620 6c69           elif li
+00010580: 7374 2867 7269 645f 7061 7261 6d65 7465  st(grid_paramete
+00010590: 7273 2e6b 6579 7328 2929 5b69 5d3d 3d27  rs.keys())[i]=='
+000105a0: 6c69 6e65 5f6f 7665 726c 6170 273a 0a20  line_overlap':. 
+000105b0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000105c0: 6f72 206a 2069 6e20 7261 6e67 6528 6c65  or j in range(le
+000105d0: 6e28 6772 6964 5f70 6172 616d 6574 6572  n(grid_parameter
+000105e0: 735b 276c 696e 655f 6f76 6572 6c61 7027  s['line_overlap'
+000105f0: 5d29 293a 0a20 2020 2020 2020 2020 2020  ])):.           
+00010600: 2020 2020 2020 2020 206c 696e 655f 6f76           line_ov
+00010610: 6572 6c61 705f 6c69 7374 5b6a 2c3a 5d3d  erlap_list[j,:]=
+00010620: 6e70 2e61 7272 6179 2867 7269 645f 7061  np.array(grid_pa
+00010630: 7261 6d65 7465 7273 5b27 6c69 6e65 5f6f  rameters['line_o
+00010640: 7665 726c 6170 275d 5b6a 5d29 0a20 2020  verlap'][j]).   
+00010650: 2020 2020 2020 2020 2065 6c73 653a 2072           else: r
+00010660: 6169 7365 204b 6579 4572 726f 7228 6627  aise KeyError(f'
+00010670: 556e 6964 656e 7469 6669 6564 2067 7269  Unidentified gri
+00010680: 6420 7061 7261 6d65 7465 7220 7b6c 6973  d parameter {lis
+00010690: 7428 6772 6964 5f70 6172 616d 6574 6572  t(grid_parameter
+000106a0: 732e 6b65 7973 2829 295b 695d 7d27 290a  s.keys())[i]}').
+000106b0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+000106c0: 2020 7261 6973 6520 4b65 7945 7272 6f72    raise KeyError
+000106d0: 2827 436f 6d62 696e 6174 696f 6e20 6973  ('Combination is
+000106e0: 2073 7469 6c6c 206e 6f74 2073 7570 706f   still not suppo
+000106f0: 7274 6564 2729 0a0a 2020 2020 6966 206e  rted')..    if n
+00010700: 702e 7375 6d28 4e74 6f74 5f6c 6973 7429  p.sum(Ntot_list)
+00010710: 3d3d 6e6d 6f64 656c 733a 0a20 2020 2020  ==nmodels:.     
+00010720: 2020 2069 6620 6e6f 7420 284e 746f 7420     if not (Ntot 
+00010730: 2020 2020 2020 2069 7320 4e6f 6e65 293a         is None):
+00010740: 0a20 2020 2020 2020 2020 2020 204e 746f  .            Nto
+00010750: 745f 6c69 7374 2a3d 4e74 6f74 0a20 2020  t_list*=Ntot.   
+00010760: 2020 2020 2023 2065 6c73 653a 0a20 2020       # else:.   
+00010770: 2020 2020 2023 2020 2020 204e 746f 745f       #     Ntot_
+00010780: 6c69 7374 2a3d 3165 3135 0a20 2020 2069  list*=1e15.    i
+00010790: 6620 6e70 2e73 756d 2854 675f 6c69 7374  f np.sum(Tg_list
+000107a0: 293d 3d6e 6d6f 6465 6c73 3a0a 2020 2020  )==nmodels:.    
+000107b0: 2020 2020 6966 206e 6f74 2028 5467 2020      if not (Tg  
+000107c0: 2020 2020 2020 2020 6973 204e 6f6e 6529          is None)
+000107d0: 3a0a 2020 2020 2020 2020 2020 2020 5467  :.            Tg
+000107e0: 5f6c 6973 742a 3d54 670a 2020 2020 2020  _list*=Tg.      
+000107f0: 2020 2320 656c 7365 3a0a 2020 2020 2020    # else:.      
+00010800: 2020 2320 2020 2020 5467 5f6c 6973 742a    #     Tg_list*
+00010810: 3d31 3030 0a20 2020 2069 6620 6e70 2e73  =100.    if np.s
+00010820: 756d 286e 4870 6c75 735f 6c69 7374 293d  um(nHplus_list)=
+00010830: 3d6e 6d6f 6465 6c73 3a0a 2020 2020 2020  =nmodels:.      
+00010840: 2020 6966 206e 6f74 2028 6e48 706c 7573    if not (nHplus
+00010850: 2020 2020 2020 6973 204e 6f6e 6529 3a0a        is None):.
+00010860: 2020 2020 2020 2020 2020 2020 6e48 706c              nHpl
+00010870: 7573 5f6c 6973 742a 3d6e 4870 6c75 730a  us_list*=nHplus.
+00010880: 2020 2020 2020 2020 2320 656c 7365 3a0a          # else:.
+00010890: 2020 2020 2020 2020 2320 2020 2020 6e48          #     nH
+000108a0: 706c 7573 5f6c 6973 742a 3d31 6531 0a20  plus_list*=1e1. 
+000108b0: 2020 2069 6620 6e70 2e73 756d 286e 4831     if np.sum(nH1
+000108c0: 5f6c 6973 7429 3d3d 6e6d 6f64 656c 733a  _list)==nmodels:
+000108d0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+000108e0: 286e 4831 2020 2020 2020 2020 2069 7320  (nH1         is 
+000108f0: 4e6f 6e65 293a 0a20 2020 2020 2020 2020  None):.         
+00010900: 2020 206e 4831 5f6c 6973 742a 3d6e 4831     nH1_list*=nH1
+00010910: 0a20 2020 2020 2020 2023 2065 6c73 653a  .        # else:
+00010920: 0a20 2020 2020 2020 2023 2020 2020 206e  .        #     n
+00010930: 4831 5f6c 6973 742a 3d31 6531 320a 2020  H1_list*=1e12.  
+00010940: 2020 6966 206e 702e 7375 6d28 6e48 325f    if np.sum(nH2_
+00010950: 6c69 7374 293d 3d6e 6d6f 6465 6c73 3a0a  list)==nmodels:.
+00010960: 2020 2020 2020 2020 6966 206e 6f74 2028          if not (
+00010970: 6e48 3220 2020 2020 2020 2020 6973 204e  nH2         is N
+00010980: 6f6e 6529 3a0a 2020 2020 2020 2020 2020  one):.          
+00010990: 2020 6e48 325f 6c69 7374 2a3d 6e48 320a    nH2_list*=nH2.
+000109a0: 2020 2020 2020 2020 2320 656c 7365 3a0a          # else:.
+000109b0: 2020 2020 2020 2020 2320 2020 2020 6e48          #     nH
+000109c0: 325f 6c69 7374 2a3d 3165 3132 0a20 2020  2_list*=1e12.   
+000109d0: 2069 6620 6e70 2e73 756d 286e 4865 5f6c   if np.sum(nHe_l
+000109e0: 6973 7429 3d3d 6e6d 6f64 656c 733a 0a20  ist)==nmodels:. 
+000109f0: 2020 2020 2020 2069 6620 6e6f 7420 286e         if not (n
+00010a00: 4865 2020 2020 2020 2020 2069 7320 4e6f  He         is No
+00010a10: 6e65 293a 0a20 2020 2020 2020 2020 2020  ne):.           
+00010a20: 206e 4865 5f6c 6973 742a 3d6e 4865 0a20   nHe_list*=nHe. 
+00010a30: 2020 2020 2020 2023 2065 6c73 653a 0a20         # else:. 
+00010a40: 2020 2020 2020 2023 2020 2020 206e 4865         #     nHe
+00010a50: 5f6c 6973 742a 3d31 6531 310a 2020 2020  _list*=1e11.    
+00010a60: 6966 206e 702e 7375 6d28 6e65 6c65 635f  if np.sum(nelec_
+00010a70: 6c69 7374 293d 3d6e 6d6f 6465 6c73 3a0a  list)==nmodels:.
+00010a80: 2020 2020 2020 2020 6966 206e 6f74 2028          if not (
+00010a90: 6e65 6c65 6320 2020 2020 2020 6973 204e  nelec       is N
+00010aa0: 6f6e 6529 3a0a 2020 2020 2020 2020 2020  one):.          
+00010ab0: 2020 6e65 6c65 635f 6c69 7374 2a3d 6e65    nelec_list*=ne
+00010ac0: 6c65 630a 2020 2020 2020 2020 2320 656c  lec.        # el
+00010ad0: 7365 3a0a 2020 2020 2020 2020 2320 2020  se:.        #   
+00010ae0: 2020 6e65 6c65 635f 6c69 7374 2a3d 3165    nelec_list*=1e
+00010af0: 380a 2020 2020 6966 206e 702e 7375 6d28  8.    if np.sum(
+00010b00: 5464 5f6c 6973 7429 3d3d 6e6d 6f64 656c  Td_list)==nmodel
+00010b10: 733a 0a20 2020 2020 2020 2069 6620 6e6f  s:.        if no
+00010b20: 7420 2854 6420 2020 2020 2020 2020 2069  t (Td          i
+00010b30: 7320 4e6f 6e65 293a 0a20 2020 2020 2020  s None):.       
+00010b40: 2020 2020 2054 645f 6c69 7374 2a3d 5464       Td_list*=Td
+00010b50: 0a20 2020 2020 2020 2023 2065 6c73 653a  .        # else:
+00010b60: 0a20 2020 2020 2020 2023 2020 2020 2054  .        #     T
+00010b70: 645f 6c69 7374 2a3d 3130 0a20 2020 2069  d_list*=10.    i
+00010b80: 6620 6e70 2e73 756d 2876 7475 7262 5f6c  f np.sum(vturb_l
+00010b90: 6973 7429 3d3d 6e6d 6f64 656c 733a 0a20  ist)==nmodels:. 
+00010ba0: 2020 2020 2020 2069 6620 6e6f 7420 2876         if not (v
+00010bb0: 7475 7262 2020 2020 2020 2069 7320 4e6f  turb       is No
+00010bc0: 6e65 293a 0a20 2020 2020 2020 2020 2020  ne):.           
+00010bd0: 2076 7475 7262 5f6c 6973 742a 3d76 7475   vturb_list*=vtu
+00010be0: 7262 0a20 2020 2020 2020 2023 2065 6c73  rb.        # els
+00010bf0: 653a 0a20 2020 2020 2020 2023 2020 2020  e:.        #    
+00010c00: 2076 7475 7262 5f6c 6973 742a 3d31 2e34   vturb_list*=1.4
+00010c10: 0a20 2020 2069 6620 6e70 2e73 756d 2864  .    if np.sum(d
+00010c20: 7573 745f 746f 5f67 6173 5f6c 6973 7429  ust_to_gas_list)
+00010c30: 3d3d 6e6d 6f64 656c 733a 0a20 2020 2020  ==nmodels:.     
+00010c40: 2020 2069 6620 6e6f 7420 2864 7573 745f     if not (dust_
+00010c50: 746f 5f67 6173 2069 7320 4e6f 6e65 293a  to_gas is None):
+00010c60: 0a20 2020 2020 2020 2020 2020 2064 7573  .            dus
+00010c70: 745f 746f 5f67 6173 5f6c 6973 742a 3d64  t_to_gas_list*=d
+00010c80: 7573 745f 746f 5f67 6173 0a20 2020 2020  ust_to_gas.     
+00010c90: 2020 2023 2065 6c73 653a 0a20 2020 2020     # else:.     
+00010ca0: 2020 2023 2020 2020 2064 7573 745f 746f     #     dust_to
+00010cb0: 5f67 6173 5f6c 6973 742a 3d31 652d 3231  _gas_list*=1e-21
+00010cc0: 0a20 2020 2069 6620 6e70 2e73 756d 2852  .    if np.sum(R
+00010cd0: 5f6f 7665 726c 6170 5f6c 6973 7429 3d3d  _overlap_list)==
+00010ce0: 6e6d 6f64 656c 733a 0a20 2020 2020 2020  nmodels:.       
+00010cf0: 2069 6620 6e6f 7420 2852 5f6f 7665 726c   if not (R_overl
+00010d00: 6170 2069 7320 4e6f 6e65 293a 0a20 2020  ap is None):.   
+00010d10: 2020 2020 2020 2020 2052 5f6f 7665 726c           R_overl
+00010d20: 6170 5f6c 6973 742a 3d52 5f6f 7665 726c  ap_list*=R_overl
+00010d30: 6170 0a20 2020 2020 2020 2023 2065 6c73  ap.        # els
+00010d40: 653a 0a20 2020 2020 2020 2023 2020 2020  e:.        #    
+00010d50: 2052 5f6f 7665 726c 6170 5f6c 6973 742a   R_overlap_list*
+00010d60: 3d31 6535 0a20 2020 2069 6620 6e70 2e73  =1e5.    if np.s
+00010d70: 756d 286c 696e 655f 6f76 6572 6c61 705f  um(line_overlap_
+00010d80: 6c69 7374 293d 3d32 2a6e 6d6f 6465 6c73  list)==2*nmodels
+00010d90: 3a0a 2020 2020 2020 2020 6966 206e 6f74  :.        if not
+00010da0: 2028 6c69 6e65 5f6f 7665 726c 6170 2069   (line_overlap i
+00010db0: 7320 4e6f 6e65 293a 0a20 2020 2020 2020  s None):.       
+00010dc0: 2020 2020 206c 696e 655f 6f76 6572 6c61       line_overla
+00010dd0: 705f 6c69 7374 2a3d 6e70 2e61 7272 6179  p_list*=np.array
+00010de0: 286c 696e 655f 6f76 6572 6c61 7029 0a20  (line_overlap). 
+00010df0: 2020 2020 2020 2023 2065 6c73 653a 0a20         # else:. 
+00010e00: 2020 2020 2020 2023 2020 2020 206c 696e         #     lin
+00010e10: 655f 6f76 6572 6c61 705f 6c69 7374 2a3d  e_overlap_list*=
+00010e20: 6e70 2e61 7272 6179 2828 342c 3330 2929  np.array((4,30))
+00010e30: 0a0a 2020 2020 6f73 2e73 7973 7465 6d28  ..    os.system(
+00010e40: 6627 746f 7563 6820 7b64 6972 6563 746f  f'touch {directo
+00010e50: 7279 2b22 2f53 6c61 6249 6e70 7574 2e69  ry+"/SlabInput.i
+00010e60: 6e22 7d27 290a 2020 2020 663d 6f70 656e  n"}').    f=open
+00010e70: 2864 6972 6563 746f 7279 2b27 2f53 6c61  (directory+'/Sla
+00010e80: 6249 6e70 7574 2e69 6e27 2c27 7727 290a  bInput.in','w').
+00010e90: 2020 2020 662e 7772 6974 6528 222a 2a2a      f.write("***
+00010ea0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00010eb0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00010ec0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00010ed0: 2a2a 2a2a 2a2a 2a2a 5c6e 2229 0a20 2020  ********\n").   
+00010ee0: 2066 2e77 7269 7465 2822 2a2a 2a20 496e   f.write("*** In
+00010ef0: 7075 7420 6669 6c65 2066 6f72 2073 6c61  put file for sla
+00010f00: 6220 6573 6361 7065 2070 726f 6261 6269  b escape probabi
+00010f10: 6c69 7479 2077 6974 6820 5072 6f44 694d  lity with ProDiM
+00010f20: 6f20 2a2a 2a5c 6e22 290a 2020 2020 662e  o ***\n").    f.
+00010f30: 7772 6974 6528 222a 2a2a 2a2a 2a2a 2a2a  write("*********
+00010f40: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00010f50: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00010f60: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00010f70: 2a2a 5c6e 2229 0a20 2020 2066 2e77 7269  **\n").    f.wri
+00010f80: 7465 2822 2a2a 2a20 6e6d 6f64 656c 7320  te("*** nmodels 
+00010f90: 7368 6f75 6c64 2066 6f6c 6c6f 7720 6f75  should follow ou
+00010fa0: 7470 7574 5f66 696c 656e 616d 6520 2a2a  tput_filename **
+00010fb0: 2a5c 6e22 290a 2020 2020 662e 7772 6974  *\n").    f.writ
+00010fc0: 6528 6627 7b6f 7574 7075 745f 6669 6c65  e(f'{output_file
+00010fd0: 6e61 6d65 7d20 2120 6f75 7470 7574 5f66  name} ! output_f
+00010fe0: 696c 656e 616d 655c 6e27 290a 2020 2020  ilename\n').    
+00010ff0: 662e 7772 6974 6528 6627 7b6f 7665 726c  f.write(f'{overl
+00011000: 6170 5f66 696c 656e 616d 657d 2021 206f  ap_filename} ! o
+00011010: 7665 726c 6170 5f66 696c 656e 616d 655c  verlap_filename\
+00011020: 6e27 290a 2020 2020 6966 2073 6570 6172  n').    if separ
+00011030: 6174 655f 6f70 5f66 696c 6573 3a0a 2020  ate_op_files:.  
+00011040: 2020 2020 2020 662e 7772 6974 6528 272e        f.write('.
+00011050: 7472 7565 2e20 2020 2021 2073 6570 6172  true.    ! separ
+00011060: 6174 655f 6f70 5f66 696c 6573 5c6e 2729  ate_op_files\n')
+00011070: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+00011080: 2020 2066 2e77 7269 7465 2827 2e66 616c     f.write('.fal
+00011090: 7365 2e20 2020 2120 7365 7061 7261 7465  se.   ! separate
+000110a0: 5f6f 705f 6669 6c65 735c 6e27 290a 2020  _op_files\n').  
+000110b0: 2020 6966 2066 6974 735f 6f70 5f66 696c    if fits_op_fil
+000110c0: 6573 3a0a 2020 2020 2020 2020 662e 7772  es:.        f.wr
+000110d0: 6974 6528 272e 7472 7565 2e20 2020 2021  ite('.true.    !
+000110e0: 2066 6974 735f 6f70 5f66 696c 6573 5c6e   fits_op_files\n
+000110f0: 2729 0a20 2020 2065 6c73 653a 0a20 2020  ').    else:.   
+00011100: 2020 2020 2066 2e77 7269 7465 2827 2e66       f.write('.f
+00011110: 616c 7365 2e20 2020 2120 6669 7473 5f6f  alse.   ! fits_o
+00011120: 705f 6669 6c65 735c 6e27 290a 2020 2020  p_files\n').    
+00011130: 6966 206e 6f5f 696e 6469 7669 6475 616c  if no_individual
+00011140: 5f6c 696e 6573 3a0a 2020 2020 2020 2020  _lines:.        
+00011150: 662e 7772 6974 6528 272e 7472 7565 2e20  f.write('.true. 
+00011160: 2020 2021 206e 6f5f 696e 6469 7669 6475     ! no_individu
+00011170: 616c 5f6c 696e 6573 5c6e 2729 0a20 2020  al_lines\n').   
+00011180: 2065 6c73 653a 0a20 2020 2020 2020 2066   else:.        f
+00011190: 2e77 7269 7465 2827 2e66 616c 7365 2e20  .write('.false. 
+000111a0: 2020 2120 6e6f 5f69 6e64 6976 6964 7561    ! no_individua
+000111b0: 6c5f 6c69 6e65 735c 6e27 290a 2020 2020  l_lines\n').    
+000111c0: 6966 2073 6c61 625f 5254 3a0a 2020 2020  if slab_RT:.    
+000111d0: 2020 2020 662e 7772 6974 6528 272e 7472      f.write('.tr
+000111e0: 7565 2e20 2020 2021 2073 6c61 625f 5254  ue.    ! slab_RT
+000111f0: 205c 6e27 290a 2020 2020 656c 7365 3a0a   \n').    else:.
+00011200: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
+00011210: 272e 6661 6c73 652e 2020 2021 2073 6c61  '.false.   ! sla
+00011220: 625f 5254 205c 6e27 290a 2020 2020 6966  b_RT \n').    if
+00011230: 2073 686f 7274 5f66 6f72 6d61 743a 0a20   short_format:. 
+00011240: 2020 2020 2020 2066 2e77 7269 7465 2827         f.write('
+00011250: 2e74 7275 652e 2020 2020 2120 7368 6f72  .true.    ! shor
+00011260: 745f 666f 726d 6174 5c6e 2729 0a20 2020  t_format\n').   
+00011270: 2065 6c73 653a 0a20 2020 2020 2020 2066   else:.        f
+00011280: 2e77 7269 7465 2827 2e66 616c 7365 2e20  .write('.false. 
+00011290: 2020 2120 7368 6f72 745f 666f 726d 6174    ! short_format
+000112a0: 5c6e 2729 0a20 2020 2066 2e77 7269 7465  \n').    f.write
+000112b0: 2866 277b 6e6d 6f64 656c 737d 2020 2020  (f'{nmodels}    
+000112c0: 2020 2020 2020 2020 2021 206e 6d6f 6465           ! nmode
+000112d0: 6c73 5c6e 2729 0a20 2020 2066 2e77 7269  ls\n').    f.wri
+000112e0: 7465 2827 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  te('------------
+000112f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00011300: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00011310: 2d2d 2d2d 2d2d 2d2d 2d2d 2d27 290a 2020  -----------').  
+00011320: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
+00011330: 286e 6d6f 6465 6c73 293a 0a20 2020 2020  (nmodels):.     
+00011340: 2020 2066 2e77 7269 7465 2866 275c 6e2a     f.write(f'\n*
+00011350: 2a2a 206d 6f64 656c 207b 692b 317d 202a  ** model {i+1} *
+00011360: 2a2a 5c6e 2729 0a20 2020 2020 2020 2069  **\n').        i
+00011370: 6620 6e70 2e73 756d 284e 746f 745f 6c69  f np.sum(Ntot_li
+00011380: 7374 2921 3d6e 6d6f 6465 6c73 3a0a 2020  st)!=nmodels:.  
+00011390: 2020 2020 2020 2020 2020 662e 7772 6974            f.writ
+000113a0: 6528 666d 742e 666f 726d 6174 2827 7b3a  e(fmt.format('{:
+000113b0: 2e33 6d7d 272c 4e74 6f74 5f6c 6973 745b  .3m}',Ntot_list[
+000113c0: 695d 2929 0a20 2020 2020 2020 2020 2020  i])).           
+000113d0: 2066 2e77 7269 7465 2827 0920 2020 2120   f.write('.   ! 
+000113e0: 4e48 746f 7420 205b 636d 5e2d 325d 2074  NHtot  [cm^-2] t
+000113f0: 6f74 616c 2067 6173 2063 6f6c 756d 6e20  otal gas column 
+00011400: 6465 6e73 6974 795c 6e27 290a 2020 2020  density\n').    
+00011410: 2020 2020 6966 206e 702e 7375 6d28 6e48      if np.sum(nH
+00011420: 706c 7573 5f6c 6973 7429 213d 6e6d 6f64  plus_list)!=nmod
+00011430: 656c 733a 0a20 2020 2020 2020 2020 2020  els:.           
+00011440: 2066 2e77 7269 7465 2866 6d74 2e66 6f72   f.write(fmt.for
+00011450: 6d61 7428 277b 3a2e 336d 7d27 2c6e 4870  mat('{:.3m}',nHp
+00011460: 6c75 735f 6c69 7374 5b69 5d29 290a 2020  lus_list[i])).  
+00011470: 2020 2020 2020 2020 2020 662e 7772 6974            f.writ
+00011480: 6528 2709 2020 2021 206e 482b 2020 2020  e('.   ! nH+    
+00011490: 5b63 6d5e 2d33 5d20 2070 726f 746f 6e20  [cm^-3]  proton 
+000114a0: 6e75 6d62 6572 2064 656e 7369 7479 5c6e  number density\n
+000114b0: 2729 0a20 2020 2020 2020 2069 6620 6e70  ').        if np
+000114c0: 2e73 756d 286e 4831 5f6c 6973 7429 213d  .sum(nH1_list)!=
+000114d0: 6e6d 6f64 656c 733a 0a20 2020 2020 2020  nmodels:.       
+000114e0: 2020 2020 2066 2e77 7269 7465 2866 6d74       f.write(fmt
+000114f0: 2e66 6f72 6d61 7428 277b 3a2e 336d 7d27  .format('{:.3m}'
+00011500: 2c6e 4831 5f6c 6973 745b 695d 2929 0a20  ,nH1_list[i])). 
+00011510: 2020 2020 2020 2020 2020 2066 2e77 7269             f.wri
+00011520: 7465 2827 0920 2020 2120 6e48 4909 205b  te('.   ! nHI. [
+00011530: 636d 5e2d 335d 2061 746f 6d69 6320 6879  cm^-3] atomic hy
+00011540: 6472 6f67 656e 5c6e 2729 0a20 2020 2020  drogen\n').     
+00011550: 2020 2069 6620 6e70 2e73 756d 286e 4832     if np.sum(nH2
+00011560: 5f6c 6973 7429 213d 6e6d 6f64 656c 733a  _list)!=nmodels:
+00011570: 0a20 2020 2020 2020 2020 2020 2066 2e77  .            f.w
+00011580: 7269 7465 2866 6d74 2e66 6f72 6d61 7428  rite(fmt.format(
+00011590: 277b 3a2e 336d 7d27 2c6e 4832 5f6c 6973  '{:.3m}',nH2_lis
+000115a0: 745b 695d 2929 0a20 2020 2020 2020 2020  t[i])).         
+000115b0: 2020 2066 2e77 7269 7465 2827 0920 2020     f.write('.   
+000115c0: 2120 6e48 3220 2020 205b 636d 5e2d 335d  ! nH2    [cm^-3]
+000115d0: 2020 206d 6f6c 6563 756c 6172 2068 7964     molecular hyd
+000115e0: 726f 6765 6e5c 6e27 290a 2020 2020 2020  rogen\n').      
+000115f0: 2020 6966 206e 702e 7375 6d28 6e48 655f    if np.sum(nHe_
+00011600: 6c69 7374 2921 3d6e 6d6f 6465 6c73 3a0a  list)!=nmodels:.
+00011610: 2020 2020 2020 2020 2020 2020 662e 7772              f.wr
+00011620: 6974 6528 666d 742e 666f 726d 6174 2827  ite(fmt.format('
+00011630: 7b3a 2e33 6d7d 272c 6e48 655f 6c69 7374  {:.3m}',nHe_list
+00011640: 5b69 5d29 290a 2020 2020 2020 2020 2020  [i])).          
+00011650: 2020 662e 7772 6974 6528 2709 2020 2021    f.write('.   !
+00011660: 206e 4865 2020 2020 5b63 6d5e 2d33 5d20   nHe    [cm^-3] 
+00011670: 2020 4865 6c69 756d 5c6e 2729 0a20 2020    Helium\n').   
+00011680: 2020 2020 2069 6620 6e70 2e73 756d 286e       if np.sum(n
+00011690: 656c 6563 5f6c 6973 7429 213d 6e6d 6f64  elec_list)!=nmod
+000116a0: 656c 733a 0a20 2020 2020 2020 2020 2020  els:.           
+000116b0: 2066 2e77 7269 7465 2866 6d74 2e66 6f72   f.write(fmt.for
+000116c0: 6d61 7428 277b 3a2e 336d 7d27 2c6e 656c  mat('{:.3m}',nel
+000116d0: 6563 5f6c 6973 745b 695d 2929 0a20 2020  ec_list[i])).   
+000116e0: 2020 2020 2020 2020 2066 2e77 7269 7465           f.write
+000116f0: 2827 0920 2020 2120 6e65 6c65 6320 205b  ('.   ! nelec  [
+00011700: 636d 5e2d 335d 2020 2065 6c65 6374 726f  cm^-3]   electro
+00011710: 6e20 6e75 6d62 6572 2064 656e 7369 7479  n number density
+00011720: 5c6e 2729 0a20 2020 2020 2020 2069 6620  \n').        if 
+00011730: 6e70 2e73 756d 2854 675f 6c69 7374 2921  np.sum(Tg_list)!
+00011740: 3d6e 6d6f 6465 6c73 3a0a 2020 2020 2020  =nmodels:.      
+00011750: 2020 2020 2020 662e 7772 6974 6528 666d        f.write(fm
+00011760: 742e 666f 726d 6174 2827 7b3a 2e33 6d7d  t.format('{:.3m}
+00011770: 272c 5467 5f6c 6973 745b 695d 2929 0a20  ',Tg_list[i])). 
+00011780: 2020 2020 2020 2020 2020 2066 2e77 7269             f.wri
+00011790: 7465 2827 0920 2020 2120 5467 6173 205b  te('.   ! Tgas [
+000117a0: 4b5d 2020 2020 2020 2020 2020 2067 6173  K]           gas
+000117b0: 2074 656d 7065 7261 7475 7265 5c6e 2729   temperature\n')
+000117c0: 0a20 2020 2020 2020 2069 6620 6e70 2e73  .        if np.s
+000117d0: 756d 2854 645f 6c69 7374 2921 3d6e 6d6f  um(Td_list)!=nmo
+000117e0: 6465 6c73 3a0a 2020 2020 2020 2020 2020  dels:.          
+000117f0: 2020 662e 7772 6974 6528 666d 742e 666f    f.write(fmt.fo
+00011800: 726d 6174 2827 7b3a 2e33 6d7d 272c 5464  rmat('{:.3m}',Td
+00011810: 5f6c 6973 745b 695d 2929 0a20 2020 2020  _list[i])).     
+00011820: 2020 2020 2020 2066 2e77 7269 7465 2827         f.write('
+00011830: 0920 2020 2120 5464 7573 7420 5b4b 5d20  .   ! Tdust [K] 
+00011840: 2020 2020 2020 2020 2020 6475 7374 2074            dust t
+00011850: 656d 7065 7261 7475 7265 5c6e 2729 0a20  emperature\n'). 
+00011860: 2020 2020 2020 2069 6620 6e70 2e73 756d         if np.sum
+00011870: 2876 7475 7262 5f6c 6973 7429 213d 6e6d  (vturb_list)!=nm
+00011880: 6f64 656c 733a 0a20 2020 2020 2020 2020  odels:.         
+00011890: 2020 2066 2e77 7269 7465 2866 6d74 2e66     f.write(fmt.f
+000118a0: 6f72 6d61 7428 277b 3a2e 336d 7d27 2c76  ormat('{:.3m}',v
+000118b0: 7475 7262 5f6c 6973 745b 695d 2929 0a20  turb_list[i])). 
+000118c0: 2020 2020 2020 2020 2020 2066 2e77 7269             f.wri
+000118d0: 7465 2827 0920 2020 2120 7674 7572 6220  te('.   ! vturb 
+000118e0: 205b 6b6d 732f 735d 2020 2020 7475 7262   [kms/s]    turb
+000118f0: 756c 656e 7420 7665 6c6f 6369 7479 5c6e  ulent velocity\n
+00011900: 2729 0a20 2020 2020 2020 2069 6620 6e70  ').        if np
+00011910: 2e73 756d 2864 7573 745f 746f 5f67 6173  .sum(dust_to_gas
+00011920: 5f6c 6973 7429 213d 6e6d 6f64 656c 733a  _list)!=nmodels:
+00011930: 0a20 2020 2020 2020 2020 2020 2066 2e77  .            f.w
+00011940: 7269 7465 2866 6d74 2e66 6f72 6d61 7428  rite(fmt.format(
+00011950: 277b 3a2e 336d 7d27 2c64 7573 745f 746f  '{:.3m}',dust_to
+00011960: 5f67 6173 5f6c 6973 745b 695d 2929 0a20  _gas_list[i])). 
+00011970: 2020 2020 2020 2020 2020 2066 2e77 7269             f.wri
+00011980: 7465 2827 0920 2020 2120 6475 7374 5f74  te('.   ! dust_t
+00011990: 6f5f 6761 735c 6e27 290a 2020 2020 2020  o_gas\n').      
+000119a0: 2020 6966 206e 702e 7375 6d28 6c69 6e65    if np.sum(line
+000119b0: 5f6f 7665 726c 6170 5f6c 6973 7429 213d  _overlap_list)!=
+000119c0: 322a 6e6d 6f64 656c 733a 0a20 2020 2020  2*nmodels:.     
+000119d0: 2020 2020 2020 2066 2e77 7269 7465 2866         f.write(f
+000119e0: 6d74 2e66 6f72 6d61 7428 277b 3a2e 3366  mt.format('{:.3f
+000119f0: 7d27 2c6c 696e 655f 6f76 6572 6c61 705f  }',line_overlap_
+00011a00: 6c69 7374 5b69 2c30 5d29 2b27 2027 2b66  list[i,0])+' '+f
+00011a10: 6d74 2e66 6f72 6d61 7428 277b 3a2e 3366  mt.format('{:.3f
+00011a20: 7d27 2c6c 696e 655f 6f76 6572 6c61 705f  }',line_overlap_
+00011a30: 6c69 7374 5b69 2c31 5d29 290a 2020 2020  list[i,1])).    
+00011a40: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
+00011a50: 2709 2020 2021 206c 696e 655f 6f76 6572  '.   ! line_over
+00011a60: 6c61 7020 205b 6d69 6372 6f6e 735d 2020  lap  [microns]  
+00011a70: 6d69 6e69 6d75 6d20 616e 6420 6d61 7869  minimum and maxi
+00011a80: 6d75 6d20 7761 7665 6c65 6e67 7468 7320  mum wavelengths 
+00011a90: 666f 7220 6c69 6e65 206f 7665 726c 6170  for line overlap
+00011aa0: 5c6e 2729 0a20 2020 2020 2020 2069 6620  \n').        if 
+00011ab0: 6e70 2e73 756d 2852 5f6f 7665 726c 6170  np.sum(R_overlap
+00011ac0: 5f6c 6973 7429 213d 6e6d 6f64 656c 733a  _list)!=nmodels:
+00011ad0: 0a20 2020 2020 2020 2020 2020 2066 2e77  .            f.w
+00011ae0: 7269 7465 2866 6d74 2e66 6f72 6d61 7428  rite(fmt.format(
+00011af0: 277b 3a2e 336d 7d27 2c52 5f6f 7665 726c  '{:.3m}',R_overl
+00011b00: 6170 5f6c 6973 745b 695d 2929 0a20 2020  ap_list[i])).   
+00011b10: 2020 2020 2020 2020 2066 2e77 7269 7465           f.write
+00011b20: 2827 0920 2020 2120 525f 6f76 6572 6c61  ('.   ! R_overla
+00011b30: 7020 2073 616d 706c 696e 6720 6772 6964  p  sampling grid
+00011b40: 2072 6573 6f6c 7574 696f 6e20 666f 7220   resolution for 
+00011b50: 6c69 6e65 206f 7665 726c 6170 5c6e 2729  line overlap\n')
+00011b60: 0a20 2020 2020 2020 2066 2e77 7269 7465  .        f.write
+00011b70: 2866 277b 6c65 6e28 7370 6563 6965 735f  (f'{len(species_
+00011b80: 6c69 7374 297d 0920 2020 2120 4e73 7065  list)}.   ! Nspe
+00011b90: 6369 6573 2020 2020 2020 2020 2020 2020  cies            
+00011ba0: 6e75 6d62 6572 206f 6620 7370 6563 6965  number of specie
+00011bb0: 7320 666f 7220 7468 6174 206d 6f64 656c  s for that model
+00011bc0: 5c6e 2729 0a20 2020 2020 2020 2066 6f72  \n').        for
+00011bd0: 206a 2069 6e20 7261 6e67 6528 6c65 6e28   j in range(len(
+00011be0: 7370 6563 6965 735f 6c69 7374 2929 3a0a  species_list)):.
+00011bf0: 2020 2020 2020 2020 2020 2020 662e 7772              f.wr
+00011c00: 6974 6528 6627 7b6c 6973 7428 7370 6563  ite(f'{list(spec
+00011c10: 6965 735f 6c69 7374 2e6b 6579 7328 2929  ies_list.keys())
+00011c20: 5b6a 5d7d 2020 2020 2020 7b73 7065 6369  [j]}      {speci
+00011c30: 6573 5f6c 6973 745b 6c69 7374 2873 7065  es_list[list(spe
+00011c40: 6369 6573 5f6c 6973 742e 6b65 7973 2829  cies_list.keys()
+00011c50: 295b 6a5d 5d7d 5c6e 2729 0a20 2020 2020  )[j]]}\n').     
+00011c60: 2020 2066 2e77 7269 7465 2827 2020 2020     f.write('    
+00011c70: 2020 2020 2020 2021 2065 6e64 5c6e 2729         ! end\n')
+00011c80: 0a20 2020 2020 2020 2066 2e77 7269 7465  .        f.write
+00011c90: 2827 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ('--------------
+00011ca0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00011cb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00011cc0: 2d2d 2d2d 2d2d 2d2d 2d27 290a 2020 2020  ---------').    
+00011cd0: 662e 636c 6f73 6528 290a 2020 2020 7265  f.close().    re
+00011ce0: 7475 726e 0a0a 0a64 6566 2067 656e 6572  turn...def gener
+00011cf0: 6174 655f 3144 5f73 7472 7563 7475 7265  ate_1D_structure
+00011d00: 2864 7a2c 7370 6563 6965 735f 6c69 7374  (dz,species_list
+00011d10: 2c76 7475 7262 2c6e 642c 5464 2c6e 5f73  ,vturb,nd,Td,n_s
+00011d20: 7065 6369 6573 2c54 5f73 7065 6369 6573  pecies,T_species
+00011d30: 2c6e 4832 3d30 2c6e 4849 3d30 2c6e 4849  ,nH2=0,nHI=0,nHI
+00011d40: 493d 302c 6e48 653d 302c 6e65 6c65 633d  I=0,nHe=0,nelec=
+00011d50: 302c 6669 6c65 6e61 6d65 3d27 3144 5f73  0,filename='1D_s
+00011d60: 7472 7563 7475 7265 2729 3a0a 2020 2020  tructure'):.    
+00011d70: 2222 220a 2020 2020 4765 6e65 7261 7465  """.    Generate
+00011d80: 7320 3144 2073 7472 7563 7475 7265 2066  s 1D structure f
+00011d90: 696c 6520 7265 7175 6972 6564 2066 6f72  ile required for
+00011da0: 2031 4420 736c 6162 206d 6f64 656c 730a   1D slab models.
+00011db0: 2020 2020 2222 220a 2020 2020 6966 2069      """.    if i
+00011dc0: 7369 6e73 7461 6e63 6528 647a 2c66 6c6f  sinstance(dz,flo
+00011dd0: 6174 2920 6f72 2069 7369 6e73 7461 6e63  at) or isinstanc
+00011de0: 6528 647a 2c69 6e74 293a 2064 7a3d 6e70  e(dz,int): dz=np
+00011df0: 2e61 7272 6179 285b 647a 5d29 0a20 2020  .array([dz]).   
+00011e00: 2069 6620 6973 696e 7374 616e 6365 2864   if isinstance(d
+00011e10: 7a2c 6c69 7374 293a 2064 7a3d 6e70 2e61  z,list): dz=np.a
+00011e20: 7272 6179 2864 7a29 0a20 2020 2069 6620  rray(dz).    if 
+00011e30: 6973 696e 7374 616e 6365 2873 7065 6369  isinstance(speci
+00011e40: 6573 5f6c 6973 742c 7374 7229 3a20 7370  es_list,str): sp
+00011e50: 6563 6965 735f 6c69 7374 3d5b 7370 6563  ecies_list=[spec
+00011e60: 6965 735f 6c69 7374 5d0a 2020 2020 6966  ies_list].    if
+00011e70: 2069 7369 6e73 7461 6e63 6528 7674 7572   isinstance(vtur
+00011e80: 622c 666c 6f61 7429 206f 7220 6973 696e  b,float) or isin
+00011e90: 7374 616e 6365 2876 7475 7262 2c69 6e74  stance(vturb,int
+00011ea0: 293a 2076 7475 7262 3d6e 702e 6f6e 6573  ): vturb=np.ones
+00011eb0: 5f6c 696b 6528 647a 292a 7674 7572 620a  _like(dz)*vturb.
+00011ec0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+00011ed0: 6528 6e64 2c66 6c6f 6174 2920 6f72 2069  e(nd,float) or i
+00011ee0: 7369 6e73 7461 6e63 6528 6e64 2c69 6e74  sinstance(nd,int
+00011ef0: 293a 206e 643d 6e70 2e6f 6e65 735f 6c69  ): nd=np.ones_li
+00011f00: 6b65 2864 7a29 2a6e 640a 2020 2020 6966  ke(dz)*nd.    if
+00011f10: 2069 7369 6e73 7461 6e63 6528 5464 2c66   isinstance(Td,f
+00011f20: 6c6f 6174 2920 6f72 2069 7369 6e73 7461  loat) or isinsta
+00011f30: 6e63 6528 5464 2c69 6e74 293a 2054 643d  nce(Td,int): Td=
+00011f40: 6e70 2e6f 6e65 735f 6c69 6b65 2864 7a29  np.ones_like(dz)
+00011f50: 2a54 640a 2020 2020 6966 2069 7369 6e73  *Td.    if isins
+00011f60: 7461 6e63 6528 6e48 322c 666c 6f61 7429  tance(nH2,float)
+00011f70: 206f 7220 6973 696e 7374 616e 6365 286e   or isinstance(n
+00011f80: 4832 2c69 6e74 293a 206e 4832 3d6e 702e  H2,int): nH2=np.
+00011f90: 6f6e 6573 5f6c 696b 6528 647a 292a 6e48  ones_like(dz)*nH
+00011fa0: 320a 2020 2020 6966 2069 7369 6e73 7461  2.    if isinsta
+00011fb0: 6e63 6528 6e48 492c 666c 6f61 7429 206f  nce(nHI,float) o
+00011fc0: 7220 6973 696e 7374 616e 6365 286e 4849  r isinstance(nHI
+00011fd0: 2c69 6e74 293a 206e 4849 3d6e 702e 6f6e  ,int): nHI=np.on
+00011fe0: 6573 5f6c 696b 6528 647a 292a 6e48 490a  es_like(dz)*nHI.
+00011ff0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+00012000: 6528 6e48 4949 2c66 6c6f 6174 2920 6f72  e(nHII,float) or
+00012010: 2069 7369 6e73 7461 6e63 6528 6e48 4949   isinstance(nHII
+00012020: 2c69 6e74 293a 206e 4849 493d 6e70 2e6f  ,int): nHII=np.o
+00012030: 6e65 735f 6c69 6b65 2864 7a29 2a6e 4849  nes_like(dz)*nHI
+00012040: 490a 2020 2020 6966 2069 7369 6e73 7461  I.    if isinsta
+00012050: 6e63 6528 6e48 652c 666c 6f61 7429 206f  nce(nHe,float) o
+00012060: 7220 6973 696e 7374 616e 6365 286e 4865  r isinstance(nHe
+00012070: 2c69 6e74 293a 206e 4865 3d6e 702e 6f6e  ,int): nHe=np.on
+00012080: 6573 5f6c 696b 6528 647a 292a 6e48 650a  es_like(dz)*nHe.
+00012090: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+000120a0: 6528 6e65 6c65 632c 666c 6f61 7429 206f  e(nelec,float) o
+000120b0: 7220 6973 696e 7374 616e 6365 286e 656c  r isinstance(nel
+000120c0: 6563 2c69 6e74 293a 206e 656c 6563 3d6e  ec,int): nelec=n
+000120d0: 702e 6f6e 6573 5f6c 696b 6528 647a 292a  p.ones_like(dz)*
+000120e0: 6e65 6c65 630a 2020 2020 6966 2069 7369  nelec.    if isi
+000120f0: 6e73 7461 6e63 6528 6e5f 7370 6563 6965  nstance(n_specie
+00012100: 732c 666c 6f61 7429 206f 7220 6973 696e  s,float) or isin
+00012110: 7374 616e 6365 286e 5f73 7065 6369 6573  stance(n_species
+00012120: 2c69 6e74 293a 206e 5f73 7065 6369 6573  ,int): n_species
+00012130: 3d6e 702e 6f6e 6573 2828 647a 2e73 6861  =np.ones((dz.sha
+00012140: 7065 5b30 5d2c 6c65 6e28 7370 6563 6965  pe[0],len(specie
+00012150: 735f 6c69 7374 2929 292a 6e5f 7370 6563  s_list)))*n_spec
+00012160: 6965 730a 2020 2020 6966 2069 7369 6e73  ies.    if isins
+00012170: 7461 6e63 6528 545f 7370 6563 6965 732c  tance(T_species,
+00012180: 666c 6f61 7429 206f 7220 6973 696e 7374  float) or isinst
+00012190: 616e 6365 2854 5f73 7065 6369 6573 2c69  ance(T_species,i
+000121a0: 6e74 293a 2054 5f73 7065 6369 6573 3d6e  nt): T_species=n
+000121b0: 702e 6f6e 6573 2828 647a 2e73 6861 7065  p.ones((dz.shape
+000121c0: 5b30 5d2c 6c65 6e28 7370 6563 6965 735f  [0],len(species_
+000121d0: 6c69 7374 2929 292a 545f 7370 6563 6965  list)))*T_specie
+000121e0: 730a 2020 2020 6966 2069 7369 6e73 7461  s.    if isinsta
+000121f0: 6e63 6528 545f 7370 6563 6965 732c 6c69  nce(T_species,li
+00012200: 7374 293a 2054 5f73 7065 6369 6573 3d6e  st): T_species=n
+00012210: 702e 6172 7261 7928 545f 7370 6563 6965  p.array(T_specie
+00012220: 7329 0a20 2020 2069 6620 6973 696e 7374  s).    if isinst
+00012230: 616e 6365 286e 5f73 7065 6369 6573 2c6c  ance(n_species,l
+00012240: 6973 7429 3a20 6e5f 7370 6563 6965 733d  ist): n_species=
+00012250: 6e70 2e61 7272 6179 286e 5f73 7065 6369  np.array(n_speci
+00012260: 6573 290a 2020 2020 6966 206e 702e 6172  es).    if np.ar
+00012270: 7261 7928 545f 7370 6563 6965 7329 2e73  ray(T_species).s
+00012280: 697a 653d 3d6c 656e 2873 7065 6369 6573  ize==len(species
+00012290: 5f6c 6973 7429 3a0a 2020 2020 2020 2020  _list):.        
+000122a0: 545f 7370 6563 6965 735f 7465 6d70 3d6e  T_species_temp=n
+000122b0: 702e 6f6e 6573 2828 647a 2e73 6861 7065  p.ones((dz.shape
+000122c0: 5b30 5d2c 6c65 6e28 7370 6563 6965 735f  [0],len(species_
+000122d0: 6c69 7374 2929 290a 2020 2020 2020 2020  list))).        
+000122e0: 666f 7220 6920 696e 2072 616e 6765 286c  for i in range(l
+000122f0: 656e 2873 7065 6369 6573 5f6c 6973 7429  en(species_list)
+00012300: 293a 0a20 2020 2020 2020 2020 2020 2054  ):.            T
+00012310: 5f73 7065 6369 6573 5f74 656d 705b 3a2c  _species_temp[:,
+00012320: 695d 3d54 5f73 7065 6369 6573 5b69 5d0a  i]=T_species[i].
+00012330: 2020 2020 2020 2020 545f 7370 6563 6965          T_specie
+00012340: 733d 545f 7370 6563 6965 735f 7465 6d70  s=T_species_temp
+00012350: 2a31 2e30 300a 2020 2020 6966 206e 702e  *1.00.    if np.
+00012360: 6172 7261 7928 6e5f 7370 6563 6965 7329  array(n_species)
+00012370: 2e73 697a 653d 3d6c 656e 2873 7065 6369  .size==len(speci
+00012380: 6573 5f6c 6973 7429 3a0a 2020 2020 2020  es_list):.      
+00012390: 2020 6e5f 7370 6563 6965 735f 7465 6d70    n_species_temp
+000123a0: 3d6e 702e 6f6e 6573 2828 647a 2e73 6861  =np.ones((dz.sha
+000123b0: 7065 5b30 5d2c 6c65 6e28 7370 6563 6965  pe[0],len(specie
+000123c0: 735f 6c69 7374 2929 290a 2020 2020 2020  s_list))).      
+000123d0: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
+000123e0: 286c 656e 2873 7065 6369 6573 5f6c 6973  (len(species_lis
+000123f0: 7429 293a 0a20 2020 2020 2020 2020 2020  t)):.           
+00012400: 206e 5f73 7065 6369 6573 5f74 656d 705b   n_species_temp[
+00012410: 3a2c 695d 3d6e 5f73 7065 6369 6573 5b69  :,i]=n_species[i
+00012420: 5d0a 2020 2020 2020 2020 6e5f 7370 6563  ].        n_spec
+00012430: 6965 733d 6e5f 7370 6563 6965 735f 7465  ies=n_species_te
+00012440: 6d70 2a31 2e30 300a 0a20 2020 2077 6974  mp*1.00..    wit
+00012450: 6820 6f70 656e 2866 696c 656e 616d 652c  h open(filename,
+00012460: 2777 2729 2061 7320 663a 0a20 2020 2020  'w') as f:.     
+00012470: 2020 2066 2e77 7269 7465 2866 277b 6c65     f.write(f'{le
+00012480: 6e28 647a 293a 647d 5c6e 2729 0a20 2020  n(dz):d}\n').   
+00012490: 2020 2020 2066 2e77 7269 7465 2866 277b       f.write(f'{
+000124a0: 6c65 6e28 7370 6563 6965 735f 6c69 7374  len(species_list
+000124b0: 293a 647d 5c6e 2729 0a20 2020 2020 2020  ):d}\n').       
+000124c0: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+000124d0: 6c65 6e28 7370 6563 6965 735f 6c69 7374  len(species_list
+000124e0: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
+000124f0: 662e 7772 6974 6528 7370 6563 6965 735f  f.write(species_
+00012500: 6c69 7374 5b69 5d2b 275c 6e27 290a 2020  list[i]+'\n').  
+00012510: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
+00012520: 616e 6765 286c 656e 2864 7a29 293a 0a20  ange(len(dz)):. 
+00012530: 2020 2020 2020 2020 2020 2073 7472 696e             strin
+00012540: 673d 2727 0a20 2020 2020 2020 2020 2020  g=''.           
+00012550: 2073 7472 696e 672b 3d66 277b 692b 313a   string+=f'{i+1:
+00012560: 647d 2020 270a 2020 2020 2020 2020 2020  d}  '.          
+00012570: 2020 7374 7269 6e67 2b3d 6627 7b64 7a5b    string+=f'{dz[
+00012580: 695d 3a2e 3365 7d20 2027 0a20 2020 2020  i]:.3e}  '.     
+00012590: 2020 2020 2020 2073 7472 696e 672b 3d66         string+=f
+000125a0: 277b 7674 7572 625b 695d 3a2e 3366 7d20  '{vturb[i]:.3f} 
+000125b0: 2027 0a20 2020 2020 2020 2020 2020 2073   '.            s
+000125c0: 7472 696e 672b 3d66 277b 6e64 5b69 5d3a  tring+=f'{nd[i]:
+000125d0: 2e33 657d 2020 270a 2020 2020 2020 2020  .3e}  '.        
+000125e0: 2020 2020 7374 7269 6e67 2b3d 6627 7b54      string+=f'{T
+000125f0: 645b 695d 3a2e 3366 7d20 2027 0a20 2020  d[i]:.3f}  '.   
+00012600: 2020 2020 2020 2020 2066 6f72 206a 2069           for j i
+00012610: 6e20 7261 6e67 6528 6c65 6e28 7370 6563  n range(len(spec
+00012620: 6965 735f 6c69 7374 2929 3a0a 2020 2020  ies_list)):.    
+00012630: 2020 2020 2020 2020 2020 2020 7374 7269              stri
+00012640: 6e67 2b3d 6627 7b6e 5f73 7065 6369 6573  ng+=f'{n_species
+00012650: 5b69 2c6a 5d3a 2e33 657d 2020 270a 2020  [i,j]:.3e}  '.  
+00012660: 2020 2020 2020 2020 2020 666f 7220 6a20            for j 
+00012670: 696e 2072 616e 6765 286c 656e 2873 7065  in range(len(spe
+00012680: 6369 6573 5f6c 6973 7429 293a 0a20 2020  cies_list)):.   
+00012690: 2020 2020 2020 2020 2020 2020 2073 7472               str
+000126a0: 696e 672b 3d66 277b 545f 7370 6563 6965  ing+=f'{T_specie
+000126b0: 735b 692c 6a5d 3a2e 3366 7d20 2027 0a20  s[i,j]:.3f}  '. 
+000126c0: 2020 2020 2020 2020 2020 2073 7472 696e             strin
+000126d0: 672b 3d66 277b 6e48 325b 695d 3a2e 3365  g+=f'{nH2[i]:.3e
+000126e0: 7d20 2027 0a20 2020 2020 2020 2020 2020  }  '.           
+000126f0: 2073 7472 696e 672b 3d66 277b 6e48 495b   string+=f'{nHI[
+00012700: 695d 3a2e 3365 7d20 2027 0a20 2020 2020  i]:.3e}  '.     
+00012710: 2020 2020 2020 2073 7472 696e 672b 3d66         string+=f
+00012720: 277b 6e48 4949 5b69 5d3a 2e33 657d 2020  '{nHII[i]:.3e}  
+00012730: 270a 2020 2020 2020 2020 2020 2020 7374  '.            st
+00012740: 7269 6e67 2b3d 6627 7b6e 4865 5b69 5d3a  ring+=f'{nHe[i]:
+00012750: 2e33 657d 2020 270a 2020 2020 2020 2020  .3e}  '.        
+00012760: 2020 2020 7374 7269 6e67 2b3d 6627 7b6e      string+=f'{n
+00012770: 656c 6563 5b69 5d3a 2e33 657d 2020 270a  elec[i]:.3e}  '.
+00012780: 2020 2020 2020 2020 2020 2020 662e 7772              f.wr
+00012790: 6974 6528 7374 7269 6e67 2b27 5c6e 2729  ite(string+'\n')
+000127a0: 0a20 2020 2020 2020 2066 2e63 6c6f 7365  .        f.close
+000127b0: 2829 0a0a 0a63 6c61 7373 204d 7946 6f72  ()...class MyFor
+000127c0: 6d61 7474 6572 2873 7472 696e 672e 466f  matter(string.Fo
+000127d0: 726d 6174 7465 7229 3a0a 2020 2020 2222  rmatter):.    ""
+000127e0: 220a 2020 2020 5374 7269 6e67 2066 6f72  ".    String for
+000127f0: 6d61 7474 6572 2066 6f72 2070 726f 6475  matter for produ
+00012800: 6369 6e67 2069 6e70 7574 2066 696c 6573  cing input files
+00012810: 0a20 2020 2022 2222 0a0a 2020 2020 6465  .    """..    de
+00012820: 6620 666f 726d 6174 5f66 6965 6c64 2873  f format_field(s
+00012830: 656c 662c 7661 6c75 652c 666f 726d 6174  elf,value,format
+00012840: 5f73 7065 6329 3a0a 2020 2020 2020 2020  _spec):.        
+00012850: 6966 2066 6f72 6d61 745f 7370 6563 5b2d  if format_spec[-
+00012860: 315d 3d3d 276d 273a 0a20 2020 2020 2020  1]=='m':.       
+00012870: 2020 2020 2072 6574 7572 6e20 7375 7065       return supe
+00012880: 7228 292e 666f 726d 6174 5f66 6965 6c64  r().format_field
+00012890: 2876 616c 7565 2c66 6f72 6d61 745f 7370  (value,format_sp
+000128a0: 6563 5b3a 2d31 5d2b 2765 2729 2e72 6570  ec[:-1]+'e').rep
+000128b0: 6c61 6365 2827 652b 272c 2765 2729 0a20  lace('e+','e'). 
+000128c0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+000128d0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000128e0: 7375 7065 7228 292e 666f 726d 6174 5f66  super().format_f
+000128f0: 6965 6c64 2876 616c 7565 2c66 6f72 6d61  ield(value,forma
+00012900: 745f 7370 6563 290a 0a0a 666d 743d 4d79  t_spec)...fmt=My
+00012910: 466f 726d 6174 7465 7228 290a 0a0a 6465  Formatter()...de
+00012920: 6620 6c69 6e65 5f66 6c75 7828 6c31 2c6c  f line_flux(l1,l
+00012930: 322c 7761 7665 6c65 6e67 7468 2c66 6c75  2,wavelength,flu
+00012940: 7829 3a0a 2020 2020 2727 270a 2020 2020  x):.    '''.    
+00012950: 556e 6974 733a 2052 6574 7572 6e20 6973  Units: Return is
+00012960: 2069 6e20 7468 6520 7361 6d65 2075 6e69   in the same uni
+00012970: 7420 6173 2069 6e70 7574 2e20 5b41 7373  t as input. [Ass
+00012980: 756d 6564 2074 6f20 6265 2069 6e20 6572  umed to be in er
+00012990: 672f 732f 636d 322f 7372 5d20 6c31 2061  g/s/cm2/sr] l1 a
+000129a0: 6e64 206c 3220 7361 6d65 2075 6e69 7420  nd l2 same unit 
+000129b0: 6173 2077 6176 656c 656e 6774 680a 0a20  as wavelength.. 
+000129c0: 2020 2052 6574 7572 6e73 0a20 2020 202d     Returns.    -
+000129d0: 2d2d 2d2d 2d2d 0a20 2020 2066 6c6f 6174  ------.    float
+000129e0: 3a0a 2020 2020 2020 5375 6d20 6f66 2069  :.      Sum of i
+000129f0: 6e74 6567 7261 7465 6420 6c69 6e65 2066  ntegrated line f
+00012a00: 6c75 7820 6265 7477 6565 6e20 7761 7665  lux between wave
+00012a10: 6c65 6e67 7468 7320 6c31 2061 6e64 206c  lengths l1 and l
+00012a20: 322e 0a0a 2020 2020 2727 270a 2020 2020  2...    '''.    
+00012a30: 6d61 736b 3d28 7761 7665 6c65 6e67 7468  mask=(wavelength
+00012a40: 3e6c 3129 2628 7761 7665 6c65 6e67 7468  >l1)&(wavelength
+00012a50: 3c3d 6c32 290a 2020 2020 7265 7475 726e  <=l2).    return
+00012a60: 206e 702e 7375 6d28 666c 7578 5b6d 6173   np.sum(flux[mas
+00012a70: 6b5d 290a 0a0a 6465 6620 6c69 6e65 5f66  k])...def line_f
+00012a80: 6c75 7865 7328 7769 6e64 6f77 732c 7761  luxes(windows,wa
+00012a90: 7665 6c65 6e67 7468 2c66 6c75 7829 3a0a  velength,flux):.
+00012aa0: 2020 2020 2727 270a 2020 2020 5265 7475      '''.    Retu
+00012ab0: 726e 3a20 6172 7261 7920 6f66 2073 756d  rn: array of sum
+00012ac0: 206f 6620 696e 7465 6772 6174 6564 206c   of integrated l
+00012ad0: 696e 6520 666c 7578 2069 6e20 7761 7665  ine flux in wave
+00012ae0: 6c65 6e67 7468 2077 696e 646f 7773 2e0a  length windows..
+00012af0: 0a20 2020 2055 6e69 7473 3a20 5265 7475  .    Units: Retu
+00012b00: 726e 2069 7320 696e 2074 6865 2073 616d  rn is in the sam
+00012b10: 6520 756e 6974 2061 7320 696e 7075 742e  e unit as input.
+00012b20: 205b 4173 7375 6d65 6420 746f 2062 6520   [Assumed to be 
+00012b30: 696e 2065 7267 2f73 2f63 6d32 2f73 725d  in erg/s/cm2/sr]
+00012b40: 0a0a 2020 2020 7769 6e64 6f77 733a 206c  ..    windows: l
+00012b50: 6973 7420 6f66 2077 6176 656c 656e 6774  ist of wavelengt
+00012b60: 6820 6c69 6d69 7473 206f 6620 7769 6e64  h limits of wind
+00012b70: 6f77 732e 2045 7861 6d70 6c65 3a20 5b5b  ows. Example: [[
+00012b80: 3134 2c31 342e 355d 2c5b 3135 2c31 362e  14,14.5],[15,16.
+00012b90: 325d 2c5b 3132 2e35 2c31 342e 315d 5d0a  2],[12.5,14.1]].
+00012ba0: 2020 2020 2727 270a 2020 2020 463d 5b5d      '''.    F=[]
+00012bb0: 0a20 2020 2066 6f72 2057 2069 6e20 7769  .    for W in wi
+00012bc0: 6e64 6f77 733a 0a20 2020 2020 2020 2046  ndows:.        F
+00012bd0: 2e61 7070 656e 6428 6c69 6e65 5f66 6c75  .append(line_flu
+00012be0: 7828 575b 305d 2c57 5b31 5d2c 7761 7665  x(W[0],W[1],wave
+00012bf0: 6c65 6e67 7468 2c66 6c75 7829 290a 2020  length,flux)).  
+00012c00: 2020 7265 7475 726e 286e 702e 6172 7261    return(np.arra
+00012c10: 7928 4629 290a 0a0a 6465 6620 6c69 6e65  y(F))...def line
+00012c20: 5f66 6c75 785f 7261 7469 6f73 2872 6174  _flux_ratios(rat
+00012c30: 696f 5f77 696e 646f 7773 2c77 6176 656c  io_windows,wavel
+00012c40: 656e 6774 682c 666c 7578 293a 0a20 2020  ength,flux):.   
+00012c50: 2027 2727 0a20 2020 2052 6574 7572 6e3a   '''.    Return:
+00012c60: 2049 6e74 6567 7261 7465 6420 6c69 6e65   Integrated line
+00012c70: 2066 6c75 7820 7261 7469 6f73 2062 6574   flux ratios bet
+00012c80: 7765 656e 2077 6176 656c 656e 6774 6873  ween wavelengths
+00012c90: 206c 3120 616e 6420 6c32 2e0a 0a20 2020   l1 and l2...   
+00012ca0: 2055 6e69 743a 2052 6574 7572 6e20 6861   Unit: Return ha
+00012cb0: 7320 6e6f 2075 6e69 742e 205b 496e 7075  s no unit. [Inpu
+00012cc0: 7420 6973 2061 7373 756d 6564 2074 6f20  t is assumed to 
+00012cd0: 6265 2069 6e20 6572 672f 732f 636d 322f  be in erg/s/cm2/
+00012ce0: 7372 5d0a 0a20 2020 2072 6174 696f 5f77  sr]..    ratio_w
+00012cf0: 696e 646f 7773 3a20 6c69 7374 206f 6620  indows: list of 
+00012d00: 7761 7665 6c65 6e67 7468 2077 696e 646f  wavelength windo
+00012d10: 7773 2e20 4578 616d 706c 653a 205b 5b5b  ws. Example: [[[
+00012d20: 3134 2c31 342e 355d 2c5b 3135 2c31 362e  14,14.5],[15,16.
+00012d30: 325d 5d2c 5b5b 3132 2e35 2c31 342e 315d  2]],[[12.5,14.1]
+00012d40: 2c5b 3133 2e34 2c31 332e 385d 5d5d 0a20  ,[13.4,13.8]]]. 
+00012d50: 2020 2027 2727 0a20 2020 2052 3d5b 5d0a     '''.    R=[].
+00012d60: 2020 2020 666f 7220 7769 6e64 6f77 2069      for window i
+00012d70: 6e20 7261 7469 6f5f 7769 6e64 6f77 733a  n ratio_windows:
+00012d80: 0a20 2020 2020 2020 2046 3d6c 696e 655f  .        F=line_
+00012d90: 666c 7578 6573 285b 7769 6e64 6f77 5b30  fluxes([window[0
+00012da0: 5d2c 7769 6e64 6f77 5b31 5d5d 2c77 6176  ],window[1]],wav
+00012db0: 656c 656e 6774 682c 666c 7578 290a 2020  elength,flux).  
+00012dc0: 2020 2020 2020 522e 6170 7065 6e64 2846        R.append(F
+00012dd0: 5b31 5d2f 465b 305d 290a 2020 2020 7265  [1]/F[0]).    re
+00012de0: 7475 726e 286e 702e 6172 7261 7928 5229  turn(np.array(R)
+00012df0: 290a 0a0a 6465 6620 6c69 6e65 5f66 6c75  )...def line_flu
+00012e00: 785f 7072 6f64 7563 7473 2870 726f 6475  x_products(produ
+00012e10: 6374 5f77 696e 646f 7773 2c77 6176 656c  ct_windows,wavel
+00012e20: 656e 6774 682c 666c 7578 293a 0a20 2020  ength,flux):.   
+00012e30: 2027 2727 0a20 2020 2052 6574 7572 6e3a   '''.    Return:
+00012e40: 2049 6e74 6567 7261 7465 6420 6c69 6e65   Integrated line
+00012e50: 2066 6c75 7820 7072 6f64 7563 7473 2062   flux products b
+00012e60: 6574 7765 656e 2077 6176 656c 656e 6774  etween wavelengt
+00012e70: 6873 206c 3120 616e 6420 6c32 2e0a 0a20  hs l1 and l2... 
+00012e80: 2020 2055 6e69 743a 2052 6574 7572 6e20     Unit: Return 
+00012e90: 756e 6974 2069 7320 6f75 7470 7574 2075  unit is output u
+00012ea0: 6e69 7473 2073 7175 6172 6564 2e20 5b49  nits squared. [I
+00012eb0: 6e70 7574 2069 7320 6173 7375 6d65 6420  nput is assumed 
+00012ec0: 746f 2062 6520 696e 2065 7267 2f73 2f63  to be in erg/s/c
+00012ed0: 6d32 2f73 725d 0a0a 2020 2020 7072 6f64  m2/sr]..    prod
+00012ee0: 7563 745f 7769 6e64 6f77 733a 206c 6973  uct_windows: lis
+00012ef0: 7420 6f66 2077 6176 656c 656e 6774 6820  t of wavelength 
+00012f00: 7769 6e64 6f77 732e 2045 7861 6d70 6c65  windows. Example
+00012f10: 3a20 5b5b 5b31 342c 3134 2e35 5d2c 5b31  : [[[14,14.5],[1
+00012f20: 352c 3136 2e32 5d5d 2c5b 5b31 322e 352c  5,16.2]],[[12.5,
+00012f30: 3134 2e31 5d2c 5b31 332e 342c 3133 2e38  14.1],[13.4,13.8
+00012f40: 5d5d 5d0a 2020 2020 2727 270a 2020 2020  ]]].    '''.    
+00012f50: 523d 5b5d 0a20 2020 2066 6f72 2077 696e  R=[].    for win
+00012f60: 646f 7720 696e 2070 726f 6475 6374 5f77  dow in product_w
+00012f70: 696e 646f 7773 3a0a 2020 2020 2020 2020  indows:.        
+00012f80: 463d 6c69 6e65 5f66 6c75 7865 7328 5b77  F=line_fluxes([w
+00012f90: 696e 646f 775b 305d 2c77 696e 646f 775b  indow[0],window[
+00012fa0: 315d 5d2c 7761 7665 6c65 6e67 7468 2c66  1]],wavelength,f
+00012fb0: 6c75 7829 0a20 2020 2020 2020 2052 2e61  lux).        R.a
+00012fc0: 7070 656e 6428 465b 315d 2a46 5b30 5d29  ppend(F[1]*F[0])
+00012fd0: 0a20 2020 2072 6574 7572 6e28 6e70 2e61  .    return(np.a
+00012fe0: 7272 6179 2852 2929 0a0a 0a64 6566 2073  rray(R))...def s
+00012ff0: 7065 6374 7261 6c5f 666c 7578 286c 312c  pectral_flux(l1,
+00013000: 6c32 2c77 6176 656c 656e 6774 682c 666c  l2,wavelength,fl
+00013010: 7578 293a 0a20 2020 2027 2727 0a20 2020  ux):.    '''.   
+00013020: 2055 6e69 743a 2052 6574 7572 6e20 696e   Unit: Return in
+00013030: 205b 6572 672f 732f 636d 325d 2061 6e64   [erg/s/cm2] and
+00013040: 2069 6e70 7574 2069 7320 696e 205b 4a79   input is in [Jy
+00013050: 5d20 6c31 2c20 6c32 2c20 616e 6420 7761  ] l1, l2, and wa
+00013060: 7665 6c65 6e67 7468 2069 6e20 6d69 6372  velength in micr
+00013070: 6f6e 730a 0a20 2020 2052 6574 7572 6e73  ons..    Returns
+00013080: 0a20 2020 202d 2d2d 2d2d 2d2d 0a20 2020  .    -------.   
+00013090: 2066 6c6f 6174 3a0a 2020 2020 2020 5375   float:.      Su
+000130a0: 6d20 6f66 2069 6e74 6567 7261 7465 6420  m of integrated 
+000130b0: 6c69 6e65 2066 6c75 7820 6265 7477 6565  line flux betwee
+000130c0: 6e20 7761 7665 6c65 6e67 7468 7320 6c31  n wavelengths l1
+000130d0: 2061 6e64 206c 322e 0a0a 2020 2020 2727   and l2...    ''
+000130e0: 270a 2020 2020 666c 7578 3d66 6c75 782a  '.    flux=flux*
+000130f0: 3165 2d32 3320 2023 2043 6f6e 7665 7274  1e-23  # Convert
+00013100: 696e 6720 4a79 2074 6f20 6572 672e 73e2  ing Jy to erg.s.
+00013110: 8892 312e 636d e288 9232 2e48 7ae2 8892  ..1.cm...2.Hz...
+00013120: 310a 2020 2020 7761 7665 6c65 6e67 7468  1.    wavelength
+00013130: 3d77 6176 656c 656e 6774 682a 3165 2d34  =wavelength*1e-4
+00013140: 2020 2320 436f 6e76 6572 7469 6e67 206d    # Converting m
+00013150: 6963 726f 6e73 2074 6f20 636d 0a20 2020  icrons to cm.   
+00013160: 2066 6c75 783d 666c 7578 5b6e 702e 6172   flux=flux[np.ar
+00013170: 6773 6f72 7428 7761 7665 6c65 6e67 7468  gsort(wavelength
+00013180: 295d 0a20 2020 2077 6176 656c 656e 6774  )].    wavelengt
+00013190: 683d 7761 7665 6c65 6e67 7468 5b6e 702e  h=wavelength[np.
+000131a0: 6172 6773 6f72 7428 7761 7665 6c65 6e67  argsort(waveleng
+000131b0: 7468 295d 0a20 2020 206c 313d 6c31 2a31  th)].    l1=l1*1
+000131c0: 652d 3420 2023 2043 6f6e 7665 7274 696e  e-4  # Convertin
+000131d0: 6720 6d69 6372 6f6e 7320 746f 2063 6d0a  g microns to cm.
+000131e0: 2020 2020 6c32 3d6c 322a 3165 2d34 2020      l2=l2*1e-4  
+000131f0: 2320 436f 6e76 6572 7469 6e67 206d 6963  # Converting mic
+00013200: 726f 6e73 2074 6f20 636d 0a20 2020 2063  rons to cm.    c
+00013210: 5f63 6d73 3d63 2a31 6532 2020 2320 436f  _cms=c*1e2  # Co
+00013220: 6e76 6572 7469 6e67 206d 2f73 2074 6f20  nverting m/s to 
+00013230: 636d 2f73 0a20 2020 206d 6173 6b3d 2877  cm/s.    mask=(w
+00013240: 6176 656c 656e 6774 683e 6c31 2926 2877  avelength>l1)&(w
+00013250: 6176 656c 656e 6774 683c 3d6c 3229 0a20  avelength<=l2). 
+00013260: 2020 2077 6176 653d 7761 7665 6c65 6e67     wave=waveleng
+00013270: 7468 5b6d 6173 6b5d 0a20 2020 2023 2077  th[mask].    # w
+00013280: 6176 6531 2020 2020 2020 3d20 6e70 2e72  ave1      = np.r
+00013290: 6f6c 6c28 7761 7665 6c65 6e67 7468 2c31  oll(wavelength,1
+000132a0: 295b 6d61 736b 5d0a 2020 2020 2320 7761  )[mask].    # wa
+000132b0: 7665 3120 2020 2020 203d 2031 302a 2a28  ve1      = 10**(
+000132c0: 286e 702e 6c6f 6731 3028 7761 7665 292b  (np.log10(wave)+
+000132d0: 6e70 2e6c 6f67 3130 2877 6176 6531 2929  np.log10(wave1))
+000132e0: 2f32 290a 2020 2020 2320 7761 7665 3220  /2).    # wave2 
+000132f0: 2020 2020 203d 206e 702e 726f 6c6c 2877       = np.roll(w
+00013300: 6176 656c 656e 6774 682c 2d31 295b 6d61  avelength,-1)[ma
+00013310: 736b 5d0a 2020 2020 2320 7761 7665 3220  sk].    # wave2 
+00013320: 2020 2020 203d 2031 302a 2a28 286e 702e       = 10**((np.
+00013330: 6c6f 6731 3028 7761 7665 292b 6e70 2e6c  log10(wave)+np.l
+00013340: 6f67 3130 2877 6176 6532 2929 2f32 290a  og10(wave2))/2).
+00013350: 2020 2020 2320 646e 7520 2020 2020 2020      # dnu       
+00013360: 203d 2063 2a28 7761 7665 322d 7761 7665   = c*(wave2-wave
+00013370: 3129 2f77 6176 652a 2a32 2a31 6532 0a20  1)/wave**2*1e2. 
+00013380: 2020 2077 6176 6531 3d6e 702e 726f 6c6c     wave1=np.roll
+00013390: 2877 6176 656c 656e 6774 682c 3129 5b6d  (wavelength,1)[m
+000133a0: 6173 6b5d 0a20 2020 2077 6176 6532 3d6e  ask].    wave2=n
+000133b0: 702e 726f 6c6c 2877 6176 656c 656e 6774  p.roll(wavelengt
+000133c0: 682c 2d31 295b 6d61 736b 5d0a 2020 2020  h,-1)[mask].    
+000133d0: 646e 753d 2863 5f63 6d73 2a28 312f 7761  dnu=(c_cms*(1/wa
+000133e0: 7665 312d 312f 7761 7665 3229 2f32 290a  ve1-1/wave2)/2).
+000133f0: 2020 2020 7265 7475 726e 286e 702e 7375      return(np.su
+00013400: 6d28 666c 7578 5b6d 6173 6b5d 2a64 6e75  m(flux[mask]*dnu
+00013410: 2929 0a0a 0a64 6566 2073 7065 6374 7261  ))...def spectra
+00013420: 6c5f 666c 7578 6573 2877 696e 646f 7773  l_fluxes(windows
+00013430: 2c77 6176 656c 656e 6774 682c 666c 7578  ,wavelength,flux
+00013440: 293a 0a20 2020 2027 2727 0a20 2020 2052  ):.    '''.    R
+00013450: 6574 7572 6e3a 2053 756d 206f 6620 696e  eturn: Sum of in
+00013460: 7465 6772 6174 6564 206c 696e 6520 666c  tegrated line fl
+00013470: 7578 2062 6574 7765 656e 2077 6176 656c  ux between wavel
+00013480: 656e 6774 6820 7769 6e64 6f77 732e 0a0a  ength windows...
+00013490: 2020 2020 556e 6974 3a20 7265 7475 726e      Unit: return
+000134a0: 2069 7320 696e 205b 6572 672f 732f 636d   is in [erg/s/cm
+000134b0: 325d 2061 6e64 2069 6e70 7574 2069 7320  2] and input is 
+000134c0: 696e 205b 4a79 5d0a 0a20 2020 2077 696e  in [Jy]..    win
+000134d0: 646f 7773 3a20 6c69 7374 206f 6620 7761  dows: list of wa
+000134e0: 7665 6c65 6e67 7468 206c 696d 6974 7320  velength limits 
+000134f0: 286d 6963 726f 6e73 2920 6f66 2077 696e  (microns) of win
+00013500: 646f 7773 2e20 4578 616d 706c 653a 205b  dows. Example: [
+00013510: 5b31 342c 3134 2e35 5d2c 5b31 352c 3136  [14,14.5],[15,16
+00013520: 2e32 5d2c 5b31 322e 352c 3134 2e31 5d5d  .2],[12.5,14.1]]
+00013530: 0a20 2020 2027 2727 0a20 2020 2046 3d5b  .    '''.    F=[
+00013540: 5d0a 2020 2020 666f 7220 5720 696e 2077  ].    for W in w
+00013550: 696e 646f 7773 3a0a 2020 2020 2020 2020  indows:.        
+00013560: 462e 6170 7065 6e64 2873 7065 6374 7261  F.append(spectra
+00013570: 6c5f 666c 7578 2857 5b30 5d2c 575b 315d  l_flux(W[0],W[1]
+00013580: 2c77 6176 656c 656e 6774 682c 666c 7578  ,wavelength,flux
+00013590: 2929 0a20 2020 2072 6574 7572 6e28 6e70  )).    return(np
+000135a0: 2e61 7272 6179 2846 2929 0a0a 0a64 6566  .array(F))...def
+000135b0: 2073 7065 6374 7261 6c5f 666c 7578 5f72   spectral_flux_r
+000135c0: 6174 696f 7328 7261 7469 6f5f 7769 6e64  atios(ratio_wind
+000135d0: 6f77 732c 7761 7665 6c65 6e67 7468 2c66  ows,wavelength,f
+000135e0: 6c75 7829 3a0a 2020 2020 2727 270a 2020  lux):.    '''.  
+000135f0: 2020 5265 7475 726e 3a20 5370 6563 7472    Return: Spectr
+00013600: 616c 2069 6e74 6567 7261 7465 6420 666c  al integrated fl
+00013610: 7578 2072 6174 696f 7320 6265 7477 6565  ux ratios betwee
+00013620: 6e20 7761 7665 6c65 6e67 7468 2077 696e  n wavelength win
+00013630: 646f 7773 2e0a 0a20 2020 2055 6e69 7473  dows...    Units
+00013640: 3a20 5265 7475 726e 2069 7320 7769 7468  : Return is with
+00013650: 6f75 7420 756e 6974 7320 616e 6420 696e  out units and in
+00013660: 7075 7420 6973 2069 6e20 5b4a 795d 0a0a  put is in [Jy]..
+00013670: 2020 2020 7261 7469 6f5f 7769 6e64 6f77      ratio_window
+00013680: 733a 206c 6973 7420 6f66 2077 6176 656c  s: list of wavel
+00013690: 656e 6774 6820 286d 6963 726f 6e73 2920  ength (microns) 
+000136a0: 7769 6e64 6f77 732e 2045 7861 6d70 6c65  windows. Example
+000136b0: 3a20 5b5b 5b31 342c 3134 2e35 5d2c 5b31  : [[[14,14.5],[1
+000136c0: 352c 3136 2e32 5d5d 2c5b 5b31 322e 352c  5,16.2]],[[12.5,
+000136d0: 3134 2e31 5d2c 5b31 332e 342c 3133 2e38  14.1],[13.4,13.8
+000136e0: 5d5d 5d0a 2020 2020 2727 270a 2020 2020  ]]].    '''.    
+000136f0: 523d 5b5d 0a20 2020 2066 6f72 2077 696e  R=[].    for win
+00013700: 646f 7720 696e 2072 6174 696f 5f77 696e  dow in ratio_win
+00013710: 646f 7773 3a0a 2020 2020 2020 2020 463d  dows:.        F=
+00013720: 7370 6563 7472 616c 5f66 6c75 7865 7328  spectral_fluxes(
+00013730: 5b77 696e 646f 775b 305d 2c77 696e 646f  [window[0],windo
+00013740: 775b 315d 5d2c 7761 7665 6c65 6e67 7468  w[1]],wavelength
+00013750: 2c66 6c75 7829 0a20 2020 2020 2020 2052  ,flux).        R
+00013760: 2e61 7070 656e 6428 465b 315d 2f46 5b30  .append(F[1]/F[0
+00013770: 5d29 0a20 2020 2072 6574 7572 6e28 6e70  ]).    return(np
+00013780: 2e61 7272 6179 2852 2929 0a0a 0a64 6566  .array(R))...def
+00013790: 2073 7065 6374 7261 6c5f 666c 7578 5f70   spectral_flux_p
+000137a0: 726f 6475 6374 7328 7072 6f64 7563 745f  roducts(product_
+000137b0: 7769 6e64 6f77 732c 7761 7665 6c65 6e67  windows,waveleng
+000137c0: 7468 2c66 6c75 7829 3a0a 2020 2020 2727  th,flux):.    ''
+000137d0: 270a 2020 2020 5265 7475 726e 3a20 5072  '.    Return: Pr
+000137e0: 6f64 7563 7473 206f 6620 7370 6563 7472  oducts of spectr
+000137f0: 616c 2069 6e74 6567 7261 7465 6420 666c  al integrated fl
+00013800: 7578 6573 2062 6574 7765 656e 2077 6176  uxes between wav
+00013810: 656c 656e 6774 6820 7769 6e64 6f77 732e  elength windows.
+00013820: 0a0a 2020 2020 556e 6974 733a 2052 6574  ..    Units: Ret
+00013830: 7572 6e20 756e 6974 2069 7320 6f75 7470  urn unit is outp
+00013840: 7574 2075 6e69 7473 2073 7175 6172 6564  ut units squared
+00013850: 2061 6e64 2069 6e70 7574 2069 7320 696e   and input is in
+00013860: 205b 4a79 5d0a 0a20 2020 2070 726f 6475   [Jy]..    produ
+00013870: 6374 5f77 696e 646f 7773 3a20 6c69 7374  ct_windows: list
+00013880: 206f 6620 7761 7665 6c65 6e67 7468 2028   of wavelength (
+00013890: 6d69 6372 6f6e 7329 2077 696e 646f 7773  microns) windows
+000138a0: 2e20 4578 616d 706c 653a 205b 5b5b 3134  . Example: [[[14
+000138b0: 2c31 342e 355d 2c5b 3135 2c31 362e 325d  ,14.5],[15,16.2]
+000138c0: 5d2c 5b5b 3132 2e35 2c31 342e 315d 2c5b  ],[[12.5,14.1],[
+000138d0: 3133 2e34 2c31 332e 385d 5d5d 0a20 2020  13.4,13.8]]].   
+000138e0: 2027 2727 0a20 2020 2052 3d5b 5d0a 2020   '''.    R=[].  
+000138f0: 2020 666f 7220 7769 6e64 6f77 2069 6e20    for window in 
+00013900: 7072 6f64 7563 745f 7769 6e64 6f77 733a  product_windows:
+00013910: 0a20 2020 2020 2020 2046 3d73 7065 6374  .        F=spect
+00013920: 7261 6c5f 666c 7578 6573 285b 7769 6e64  ral_fluxes([wind
+00013930: 6f77 5b30 5d2c 7769 6e64 6f77 5b31 5d5d  ow[0],window[1]]
+00013940: 2c77 6176 656c 656e 6774 682c 666c 7578  ,wavelength,flux
+00013950: 290a 2020 2020 2020 2020 522e 6170 7065  ).        R.appe
+00013960: 6e64 2846 5b31 5d2a 465b 305d 290a 2020  nd(F[1]*F[0]).  
+00013970: 2020 7265 7475 726e 286e 702e 6172 7261    return(np.arra
+00013980: 7928 5229 290a 0a0a 6465 6620 6368 6932  y(R))...def chi2
+00013990: 5f73 6c61 6228 736c 6162 5f64 6174 612c  _slab(slab_data,
+000139a0: 7370 6563 7472 612c 7769 6e64 6f77 733d  spectra,windows=
+000139b0: 5b5d 2c72 6174 696f 5f77 696e 646f 7773  [],ratio_windows
+000139c0: 3d5b 5d2c 7072 6f64 7563 745f 7769 6e64  =[],product_wind
+000139d0: 6f77 733d 5b5d 2c52 6469 736b 3d6e 702e  ows=[],Rdisk=np.
+000139e0: 6c6f 6773 7061 6365 282d 322c 322c 3130  logspace(-2,2,10
+000139f0: 292c 6469 7374 616e 6365 3d31 3230 2c63  ),distance=120,c
+00013a00: 6f6e 766f 6c76 653d 4661 6c73 652c 4e4c  onvolve=False,NL
+00013a10: 5445 3d46 616c 7365 2c73 686f 7274 5f66  TE=False,short_f
+00013a20: 6f72 6d61 743d 4661 6c73 6529 3a0a 2020  ormat=False):.  
+00013a30: 2020 2727 270a 2020 2020 5265 7475 726e    '''.    Return
+00013a40: 7320 6368 6932 2062 6173 6564 206f 6e20  s chi2 based on 
+00013a50: 7365 6c65 6374 6564 2073 7065 6374 7261  selected spectra
+00013a60: 6c20 7769 6e64 6f77 7320 6163 726f 7373  l windows across
+00013a70: 2064 6966 6665 7265 6e74 2065 6d69 7474   different emitt
+00013a80: 696e 6720 6469 736b 2072 6164 6975 730a  ing disk radius.
+00013a90: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
+00013aa0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+00013ab0: 2020 2073 6c61 625f 6461 7461 203a 2073     slab_data : s
+00013ac0: 7472 696e 6720 6f72 2073 6c61 625f 6d6f  tring or slab_mo
+00013ad0: 6465 6c20 696e 7374 616e 6365 0a20 2020  del instance.   
+00013ae0: 2020 2070 6174 6820 636f 7272 6573 706f     path correspo
+00013af0: 6e64 696e 6720 746f 2061 2073 696e 676c  nding to a singl
+00013b00: 6520 736c 6162 206d 6f64 656c 206f 7220  e slab model or 
+00013b10: 6120 7369 6e67 6c65 2073 6c61 625f 6d6f  a single slab_mo
+00013b20: 6465 6c20 696e 7374 616e 6365 0a0a 2020  del instance..  
+00013b30: 2020 7370 6563 7472 6120 3a20 6e75 6d70    spectra : nump
+00013b40: 792e 6172 7261 790a 2020 2020 2020 6e75  y.array.      nu
+00013b50: 6d70 7920 6172 7261 7920 7769 7468 2066  mpy array with f
+00013b60: 6972 7374 2063 6f6c 756d 6e20 7468 6520  irst column the 
+00013b70: 7761 7665 6c65 6e67 7468 2069 6e20 5b6d  wavelength in [m
+00013b80: 6963 726f 6e73 5d20 616e 6420 7365 636f  icrons] and seco
+00013b90: 6e64 2063 6f6c 756d 6e20 666c 7578 2069  nd column flux i
+00013ba0: 6e20 5b4a 795d 0a0a 2020 2020 7769 6e64  n [Jy]..    wind
+00013bb0: 6f77 7320 3a20 6172 7261 795f 6c69 6b65  ows : array_like
+00013bc0: 0a20 2020 2020 204c 6973 7420 6f66 2073  .      List of s
+00013bd0: 7065 6374 7261 6c20 7769 6e64 6f77 7320  pectral windows 
+00013be0: 666f 7220 6368 6932 2063 616c 6375 6c61  for chi2 calcula
+00013bf0: 7469 6f6e 2028 7765 6967 6874 7320 6f70  tion (weights op
+00013c00: 7469 6f6e 616c 292e 2046 6f72 6d61 7420  tional). Format 
+00013c10: 3a20 5b77 696e 646f 7731 2c77 696e 646f  : [window1,windo
+00013c20: 7732 2c2e 2e2e 2e5d 0a20 2020 2020 2057  w2,....].      W
+00013c30: 696e 646f 7720 666f 726d 6174 3a20 5b6c  indow format: [l
+00013c40: 616d 6264 615f 302c 206c 616d 6264 615f  ambda_0, lambda_
+00013c50: 312c 2077 6569 6768 745d 2077 6569 6768  1, weight] weigh
+00013c60: 7420 6973 206f 7074 696f 6e61 6c2c 2075  t is optional, u
+00013c70: 7365 6420 666f 7220 7765 6967 6874 6564  sed for weighted
+00013c80: 2063 6869 320a 2020 2020 2020 4578 616d   chi2.      Exam
+00013c90: 706c 6520 7769 7468 6f75 7420 7765 6967  ple without weig
+00013ca0: 6874 3a20 5b5b 3134 2c31 342e 355d 2c5b  ht: [[14,14.5],[
+00013cb0: 3135 2c31 362e 325d 2c5b 3132 2e35 2c31  15,16.2],[12.5,1
+00013cc0: 342e 315d 5d0a 2020 2020 2020 4578 616d  4.1]].      Exam
+00013cd0: 706c 6520 7769 7468 2077 6569 6768 743a  ple with weight:
+00013ce0: 205b 5b31 342c 3134 2e35 2c32 5d2c 5b31   [[14,14.5,2],[1
+00013cf0: 352c 3136 2e32 2c35 5d2c 5b31 322e 352c  5,16.2,5],[12.5,
+00013d00: 3134 2e31 2c31 5d5d 0a20 2020 2020 2057  14.1,1]].      W
+00013d10: 6569 6768 7473 2061 7265 2061 7574 6f6d  eights are autom
+00013d20: 6174 6963 616c 6c79 206e 6f72 6d61 6c69  atically normali
+00013d30: 7365 642c 2073 6f20 7375 6d20 6f66 2077  sed, so sum of w
+00013d40: 6569 6768 7473 206e 6565 6420 6e6f 7420  eights need not 
+00013d50: 6265 2031 0a0a 2020 2020 5264 6973 6b20  be 1..    Rdisk 
+00013d60: 3a20 6172 7261 795f 6c69 6b65 0a20 2020  : array_like.   
+00013d70: 2020 2052 6164 6975 7320 636f 7272 6573     Radius corres
+00013d80: 706f 6e64 696e 6720 746f 2065 6d69 7474  ponding to emitt
+00013d90: 696e 6720 6172 6561 2069 6e20 6173 7472  ing area in astr
+00013da0: 6f6e 6f6d 6963 616c 2075 6e69 7473 0a0a  onomical units..
+00013db0: 2020 2020 6469 7374 616e 6365 203a 2066      distance : f
+00013dc0: 6c6f 6174 0a20 2020 2020 2064 6973 7461  loat.      dista
+00013dd0: 6e63 6520 6f66 2064 6973 6b20 696e 2070  nce of disk in p
+00013de0: 6172 7365 630a 0a20 2020 2063 6f6e 766f  arsec..    convo
+00013df0: 6c76 6520 3a20 626f 6f6c 6561 6e0a 2020  lve : boolean.  
+00013e00: 2020 2020 4966 2054 7275 652c 2074 6865      If True, the
+00013e10: 2063 6869 3220 6973 2070 6572 666f 726d   chi2 is perform
+00013e20: 6564 206f 6e20 636f 6e76 6f6c 7665 6420  ed on convolved 
+00013e30: 7370 6563 7472 6120 616e 6420 6e6f 7420  spectra and not 
+00013e40: 6f6e 2069 6e64 6976 6964 7561 6c20 6c69  on individual li
+00013e50: 6e65 730a 0a20 2020 204e 4c54 4520 3a20  nes..    NLTE : 
+00013e60: 626f 6f6c 6561 6e0a 2020 2020 2020 6966  boolean.      if
+00013e70: 2054 7275 652c 204e 4c54 4520 666c 7578   True, NLTE flux
+00013e80: 2069 7320 7461 6b65 6e20 6672 6f6d 2074   is taken from t
+00013e90: 6865 2073 6c61 6220 6d6f 6465 6c2e 0a20  he slab model.. 
+00013ea0: 2020 2027 2727 0a20 2020 2061 7265 613d     '''.    area=
+00013eb0: 6e70 2e70 692a 2852 6469 736b 2a61 752f  np.pi*(Rdisk*au/
+00013ec0: 6469 7374 616e 6365 2f70 6329 2a2a 320a  distance/pc)**2.
+00013ed0: 2020 2020 6368 695f 6172 6561 3d6e 702e      chi_area=np.
+00013ee0: 7a65 726f 7328 286c 656e 2861 7265 6129  zeros((len(area)
+00013ef0: 2929 0a20 2020 2069 6620 6973 696e 7374  )).    if isinst
+00013f00: 616e 6365 2873 6c61 625f 6461 7461 2c73  ance(slab_data,s
+00013f10: 7472 293a 2073 6c61 625f 6461 7461 3d72  tr): slab_data=r
+00013f20: 6561 645f 736c 6162 2873 6c61 625f 6461  ead_slab(slab_da
+00013f30: 7461 2c76 6572 626f 7365 3d46 616c 7365  ta,verbose=False
+00013f40: 2c73 686f 7274 5f66 6f72 6d61 743d 7368  ,short_format=sh
+00013f50: 6f72 745f 666f 726d 6174 290a 2020 2020  ort_format).    
+00013f60: 6966 206c 656e 2877 696e 646f 7773 293c  if len(windows)<
+00013f70: 3020 616e 6420 6c65 6e28 7261 7469 6f5f  0 and len(ratio_
+00013f80: 7769 6e64 6f77 7329 3c30 2061 6e64 206c  windows)<0 and l
+00013f90: 656e 2870 726f 6475 6374 5f77 696e 646f  en(product_windo
+00013fa0: 7773 293c 303a 2072 6574 7572 6e20 6368  ws)<0: return ch
+00013fb0: 695f 6172 6561 0a20 2020 2069 6620 636f  i_area.    if co
+00013fc0: 6e76 6f6c 7665 3a20 2023 2074 6f20 6573  nvolve:  # to es
+00013fd0: 7469 6d61 7465 2066 6c75 7820 6672 6f6d  timate flux from
+00013fe0: 2063 6f6e 766f 6c76 6564 2073 7065 6374   convolved spect
+00013ff0: 7261 0a20 2020 2020 2020 206c 6d69 6e2c  ra.        lmin,
+00014000: 6c6d 6178 3d5b 5d2c 5b5d 0a20 2020 2020  lmax=[],[].     
+00014010: 2020 2069 6620 6c65 6e28 7769 6e64 6f77     if len(window
+00014020: 7329 3e30 3a0a 2020 2020 2020 2020 2020  s)>0:.          
+00014030: 2020 6c6d 696e 2e61 7070 656e 6428 6e70    lmin.append(np
+00014040: 2e61 6d69 6e28 6e70 2e61 7272 6179 285b  .amin(np.array([
+00014050: 5b69 5b30 5d2c 695b 315d 5d20 666f 7220  [i[0],i[1]] for 
+00014060: 6920 696e 2077 696e 646f 7773 5d29 2e66  i in windows]).f
+00014070: 6c61 7474 656e 2829 2929 0a20 2020 2020  latten())).     
+00014080: 2020 2020 2020 206c 6d61 782e 6170 7065         lmax.appe
+00014090: 6e64 286e 702e 616d 6178 286e 702e 6172  nd(np.amax(np.ar
+000140a0: 7261 7928 5b5b 695b 305d 2c69 5b31 5d5d  ray([[i[0],i[1]]
+000140b0: 2066 6f72 2069 2069 6e20 7769 6e64 6f77   for i in window
+000140c0: 735d 292e 666c 6174 7465 6e28 2929 290a  s]).flatten())).
+000140d0: 2020 2020 2020 2020 6966 206c 656e 2872          if len(r
+000140e0: 6174 696f 5f77 696e 646f 7773 293e 303a  atio_windows)>0:
+000140f0: 0a20 2020 2020 2020 2020 2020 206c 6d69  .            lmi
+00014100: 6e2e 6170 7065 6e64 286e 702e 616d 696e  n.append(np.amin
+00014110: 286e 702e 6172 7261 7928 5b5b 695b 305d  (np.array([[i[0]
+00014120: 2c69 5b31 5d5d 2066 6f72 2069 2069 6e20  ,i[1]] for i in 
+00014130: 7261 7469 6f5f 7769 6e64 6f77 735d 292e  ratio_windows]).
+00014140: 666c 6174 7465 6e28 2929 290a 2020 2020  flatten())).    
+00014150: 2020 2020 2020 2020 6c6d 6178 2e61 7070          lmax.app
+00014160: 656e 6428 6e70 2e61 6d61 7828 6e70 2e61  end(np.amax(np.a
+00014170: 7272 6179 285b 5b69 5b30 5d2c 695b 315d  rray([[i[0],i[1]
+00014180: 5d20 666f 7220 6920 696e 2072 6174 696f  ] for i in ratio
+00014190: 5f77 696e 646f 7773 5d29 2e66 6c61 7474  _windows]).flatt
+000141a0: 656e 2829 2929 0a20 2020 2020 2020 2069  en())).        i
+000141b0: 6620 6c65 6e28 7072 6f64 7563 745f 7769  f len(product_wi
+000141c0: 6e64 6f77 7329 3e30 3a0a 2020 2020 2020  ndows)>0:.      
+000141d0: 2020 2020 2020 6c6d 696e 2e61 7070 656e        lmin.appen
+000141e0: 6428 6e70 2e61 6d69 6e28 6e70 2e61 7272  d(np.amin(np.arr
+000141f0: 6179 285b 5b69 5b30 5d2c 695b 315d 5d20  ay([[i[0],i[1]] 
+00014200: 666f 7220 6920 696e 2070 726f 6475 6374  for i in product
+00014210: 5f77 696e 646f 7773 5d29 2e66 6c61 7474  _windows]).flatt
+00014220: 656e 2829 2929 0a20 2020 2020 2020 2020  en())).         
+00014230: 2020 206c 6d61 782e 6170 7065 6e64 286e     lmax.append(n
+00014240: 702e 616d 6178 286e 702e 6172 7261 7928  p.amax(np.array(
+00014250: 5b5b 695b 305d 2c69 5b31 5d5d 2066 6f72  [[i[0],i[1]] for
+00014260: 2069 2069 6e20 7072 6f64 7563 745f 7769   i in product_wi
+00014270: 6e64 6f77 735d 292e 666c 6174 7465 6e28  ndows]).flatten(
+00014280: 2929 290a 2020 2020 2020 2020 6c6d 696e  ))).        lmin
+00014290: 3d6e 702e 616d 696e 286c 6d69 6e29 0a20  =np.amin(lmin). 
+000142a0: 2020 2020 2020 206c 6d61 783d 6e70 2e61         lmax=np.a
+000142b0: 6d61 7828 6c6d 6178 290a 2020 2020 2020  max(lmax).      
+000142c0: 2020 736c 6162 5f64 6174 612e 636f 6e76    slab_data.conv
+000142d0: 6f6c 7665 2852 3d32 3030 302c 6c61 6d62  olve(R=2000,lamb
+000142e0: 6461 5f30 3d6c 6d69 6e2a 302e 392c 6c61  da_0=lmin*0.9,la
+000142f0: 6d62 6461 5f6e 3d6c 6d61 782a 312e 312c  mbda_n=lmax*1.1,
+00014300: 4e4c 5445 3d4e 4c54 452c 7665 7262 6f73  NLTE=NLTE,verbos
+00014310: 653d 4661 6c73 6529 0a20 2020 2020 2020  e=False).       
+00014320: 2069 6620 4e4c 5445 3a0a 2020 2020 2020   if NLTE:.      
+00014330: 2020 2020 2020 466d 6f64 656c 3d73 7065        Fmodel=spe
+00014340: 6374 7261 6c5f 666c 7578 6573 2877 696e  ctral_fluxes(win
+00014350: 646f 7773 2c73 6c61 625f 6461 7461 2e63  dows,slab_data.c
+00014360: 6f6e 7657 6176 656c 656e 6774 682c 736c  onvWavelength,sl
+00014370: 6162 5f64 6174 612e 636f 6e76 4e4c 5445  ab_data.convNLTE
+00014380: 666c 7578 2a31 6532 3329 0a20 2020 2020  flux*1e23).     
+00014390: 2020 2020 2020 2052 6d6f 6465 6c3d 7370         Rmodel=sp
+000143a0: 6563 7472 616c 5f66 6c75 785f 7261 7469  ectral_flux_rati
+000143b0: 6f73 2872 6174 696f 5f77 696e 646f 7773  os(ratio_windows
+000143c0: 2c73 6c61 625f 6461 7461 2e63 6f6e 7657  ,slab_data.convW
+000143d0: 6176 656c 656e 6774 682c 736c 6162 5f64  avelength,slab_d
+000143e0: 6174 612e 636f 6e76 4e4c 5445 666c 7578  ata.convNLTEflux
+000143f0: 2a31 6532 3329 0a20 2020 2020 2020 2020  *1e23).         
+00014400: 2020 2050 6d6f 6465 6c3d 7370 6563 7472     Pmodel=spectr
+00014410: 616c 5f66 6c75 785f 7072 6f64 7563 7473  al_flux_products
+00014420: 2870 726f 6475 6374 5f77 696e 646f 7773  (product_windows
+00014430: 2c73 6c61 625f 6461 7461 2e63 6f6e 7657  ,slab_data.convW
+00014440: 6176 656c 656e 6774 682c 736c 6162 5f64  avelength,slab_d
+00014450: 6174 612e 636f 6e76 4e4c 5445 666c 7578  ata.convNLTEflux
+00014460: 2a31 6532 3329 0a20 2020 2020 2020 2065  *1e23).        e
+00014470: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00014480: 2046 6d6f 6465 6c3d 7370 6563 7472 616c   Fmodel=spectral
+00014490: 5f66 6c75 7865 7328 7769 6e64 6f77 732c  _fluxes(windows,
+000144a0: 736c 6162 5f64 6174 612e 636f 6e76 5761  slab_data.convWa
+000144b0: 7665 6c65 6e67 7468 2c73 6c61 625f 6461  velength,slab_da
+000144c0: 7461 2e63 6f6e 764c 5445 666c 7578 2a31  ta.convLTEflux*1
+000144d0: 6532 3329 0a20 2020 2020 2020 2020 2020  e23).           
+000144e0: 2052 6d6f 6465 6c3d 7370 6563 7472 616c   Rmodel=spectral
+000144f0: 5f66 6c75 785f 7261 7469 6f73 2872 6174  _flux_ratios(rat
+00014500: 696f 5f77 696e 646f 7773 2c73 6c61 625f  io_windows,slab_
+00014510: 6461 7461 2e63 6f6e 7657 6176 656c 656e  data.convWavelen
+00014520: 6774 682c 736c 6162 5f64 6174 612e 636f  gth,slab_data.co
+00014530: 6e76 4c54 4566 6c75 782a 3165 3233 290a  nvLTEflux*1e23).
+00014540: 2020 2020 2020 2020 2020 2020 506d 6f64              Pmod
+00014550: 656c 3d73 7065 6374 7261 6c5f 666c 7578  el=spectral_flux
+00014560: 5f70 726f 6475 6374 7328 7072 6f64 7563  _products(produc
+00014570: 745f 7769 6e64 6f77 732c 736c 6162 5f64  t_windows,slab_d
+00014580: 6174 612e 636f 6e76 5761 7665 6c65 6e67  ata.convWaveleng
+00014590: 7468 2c73 6c61 625f 6461 7461 2e63 6f6e  th,slab_data.con
+000145a0: 764c 5445 666c 7578 2a31 6532 3329 0a20  vLTEflux*1e23). 
+000145b0: 2020 2065 6c73 653a 2020 2320 746f 2065     else:  # to e
+000145c0: 7374 696d 6174 6520 666c 7578 2066 726f  stimate flux fro
+000145d0: 6d20 6c69 6e65 206c 6973 740a 2020 2020  m line list.    
+000145e0: 2020 2020 6966 204e 4c54 453a 0a20 2020      if NLTE:.   
+000145f0: 2020 2020 2020 2020 2074 3d27 464e 4c54           t='FNLT
+00014600: 4527 0a20 2020 2020 2020 2065 6c73 653a  E'.        else:
+00014610: 0a20 2020 2020 2020 2020 2020 2074 3d27  .            t='
+00014620: 464c 5445 270a 2020 2020 2020 2020 6c69  FLTE'.        li
+00014630: 6e65 6461 7461 3d73 6c61 625f 6461 7461  nedata=slab_data
+00014640: 2e6c 696e 6564 6174 610a 2020 2020 2020  .linedata.      
+00014650: 2020 6c69 6e65 6461 7461 2e73 6f72 745f    linedata.sort_
+00014660: 7661 6c75 6573 2862 793d 5b27 4748 7a27  values(by=['GHz'
+00014670: 5d2c 6173 6365 6e64 696e 673d 4661 6c73  ],ascending=Fals
+00014680: 652c 696e 706c 6163 653d 5472 7565 2c69  e,inplace=True,i
+00014690: 676e 6f72 655f 696e 6465 783d 5472 7565  gnore_index=True
+000146a0: 290a 2020 2020 2020 2020 466d 6f64 656c  ).        Fmodel
+000146b0: 3d6c 696e 655f 666c 7578 6573 2877 696e  =line_fluxes(win
+000146c0: 646f 7773 2c63 2f6c 696e 6564 6174 615b  dows,c/linedata[
+000146d0: 2747 487a 275d 2a31 652d 332c 6c69 6e65  'GHz']*1e-3,line
+000146e0: 6461 7461 5b74 5d29 0a20 2020 2020 2020  data[t]).       
+000146f0: 2052 6d6f 6465 6c3d 6c69 6e65 5f66 6c75   Rmodel=line_flu
+00014700: 785f 7261 7469 6f73 2872 6174 696f 5f77  x_ratios(ratio_w
+00014710: 696e 646f 7773 2c63 2f6c 696e 6564 6174  indows,c/linedat
+00014720: 615b 2747 487a 275d 2a31 652d 332c 6c69  a['GHz']*1e-3,li
+00014730: 6e65 6461 7461 5b74 5d29 0a20 2020 2020  nedata[t]).     
+00014740: 2020 2050 6d6f 6465 6c3d 6c69 6e65 5f66     Pmodel=line_f
+00014750: 6c75 785f 7261 7469 6f73 2870 726f 6475  lux_ratios(produ
+00014760: 6374 5f77 696e 646f 7773 2c63 2f6c 696e  ct_windows,c/lin
+00014770: 6564 6174 615b 2747 487a 275d 2a31 652d  edata['GHz']*1e-
+00014780: 332c 6c69 6e65 6461 7461 5b74 5d29 0a20  3,linedata[t]). 
+00014790: 2020 2046 6f62 7365 7276 6564 3d73 7065     Fobserved=spe
+000147a0: 6374 7261 6c5f 666c 7578 6573 2877 696e  ctral_fluxes(win
+000147b0: 646f 7773 2c73 7065 6374 7261 5b3a 2c30  dows,spectra[:,0
+000147c0: 5d2c 7370 6563 7472 615b 3a2c 315d 290a  ],spectra[:,1]).
+000147d0: 2020 2020 526f 6273 6572 7665 643d 7370      Robserved=sp
+000147e0: 6563 7472 616c 5f66 6c75 785f 7261 7469  ectral_flux_rati
+000147f0: 6f73 2872 6174 696f 5f77 696e 646f 7773  os(ratio_windows
+00014800: 2c73 7065 6374 7261 5b3a 2c30 5d2c 7370  ,spectra[:,0],sp
+00014810: 6563 7472 615b 3a2c 315d 290a 2020 2020  ectra[:,1]).    
+00014820: 506f 6273 6572 7665 643d 7370 6563 7472  Pobserved=spectr
+00014830: 616c 5f66 6c75 785f 7072 6f64 7563 7473  al_flux_products
+00014840: 2870 726f 6475 6374 5f77 696e 646f 7773  (product_windows
+00014850: 2c73 7065 6374 7261 5b3a 2c30 5d2c 7370  ,spectra[:,0],sp
+00014860: 6563 7472 615b 3a2c 315d 290a 2020 2020  ectra[:,1]).    
+00014870: 6e6f 726d 5f66 6163 746f 723d 300a 2020  norm_factor=0.  
+00014880: 2020 6966 206c 656e 2877 696e 646f 7773    if len(windows
+00014890: 293e 303a 0a20 2020 2020 2020 2061 7265  )>0:.        are
+000148a0: 615f 3264 3d6e 702e 6473 7461 636b 285b  a_2d=np.dstack([
+000148b0: 6172 6561 2066 6f72 2069 2069 6e20 7261  area for i in ra
+000148c0: 6e67 6528 6c65 6e28 7769 6e64 6f77 7329  nge(len(windows)
+000148d0: 295d 292e 7371 7565 657a 6528 292e 7265  )]).squeeze().re
+000148e0: 7368 6170 6528 286c 656e 2861 7265 6129  shape((len(area)
+000148f0: 2c6c 656e 2877 696e 646f 7773 2929 290a  ,len(windows))).
+00014900: 2020 2020 2020 2020 466d 6f64 656c 5f32          Fmodel_2
+00014910: 643d 6e70 2e64 7374 6163 6b28 5b46 6d6f  d=np.dstack([Fmo
+00014920: 6465 6c20 666f 7220 6920 696e 2072 616e  del for i in ran
+00014930: 6765 286c 656e 2861 7265 6129 295d 292e  ge(len(area))]).
+00014940: 7371 7565 657a 6528 292e 542e 7265 7368  squeeze().T.resh
+00014950: 6170 6528 286c 656e 2861 7265 6129 2c6c  ape((len(area),l
+00014960: 656e 2877 696e 646f 7773 2929 290a 2020  en(windows))).  
+00014970: 2020 2020 2020 466f 6273 6572 7665 645f        Fobserved_
+00014980: 3264 3d6e 702e 6473 7461 636b 285b 466f  2d=np.dstack([Fo
+00014990: 6273 6572 7665 6420 666f 7220 6920 696e  bserved for i in
+000149a0: 2072 616e 6765 286c 656e 2861 7265 6129   range(len(area)
+000149b0: 295d 292e 7371 7565 657a 6528 292e 542e  )]).squeeze().T.
+000149c0: 7265 7368 6170 6528 286c 656e 2861 7265  reshape((len(are
+000149d0: 6129 2c6c 656e 2877 696e 646f 7773 2929  a),len(windows))
+000149e0: 290a 2020 2020 2020 2020 6966 206c 656e  ).        if len
+000149f0: 2877 696e 646f 7773 5b30 5d29 3d3d 333a  (windows[0])==3:
+00014a00: 2020 2320 7765 6967 6874 6564 2063 6869    # weighted chi
+00014a10: 320a 2020 2020 2020 2020 2020 2020 7769  2.            wi
+00014a20: 6e64 6f77 735f 7765 6967 6874 733d 6e70  ndows_weights=np
+00014a30: 2e61 7272 6179 285b 7769 6e64 6f77 735b  .array([windows[
+00014a40: 6b5d 5b32 5d20 666f 7220 6b20 696e 2072  k][2] for k in r
+00014a50: 616e 6765 286c 656e 2877 696e 646f 7773  ange(len(windows
+00014a60: 2929 5d29 0a20 2020 2020 2020 2020 2020  ))]).           
+00014a70: 2077 696e 646f 7773 5f77 6569 6768 7473   windows_weights
+00014a80: 5f32 643d 6e70 2e64 7374 6163 6b28 5b77  _2d=np.dstack([w
+00014a90: 696e 646f 7773 5f77 6569 6768 7473 2066  indows_weights f
+00014aa0: 6f72 2069 2069 6e20 7261 6e67 6528 6c65  or i in range(le
+00014ab0: 6e28 6172 6561 2929 5d29 2e73 7175 6565  n(area))]).squee
+00014ac0: 7a65 2829 2e54 2e72 6573 6861 7065 2828  ze().T.reshape((
+00014ad0: 6c65 6e28 6172 6561 292c 6c65 6e28 7769  len(area),len(wi
+00014ae0: 6e64 6f77 735f 7765 6967 6874 7329 2929  ndows_weights)))
+00014af0: 0a20 2020 2020 2020 2020 2020 2063 6869  .            chi
+00014b00: 5f61 7265 612b 3d6e 702e 7375 6d28 2828  _area+=np.sum(((
+00014b10: 466d 6f64 656c 5f32 642a 6172 6561 5f32  Fmodel_2d*area_2
+00014b20: 642d 466f 6273 6572 7665 645f 3264 292f  d-Fobserved_2d)/
+00014b30: 466f 6273 6572 7665 645f 3264 292a 2a32  Fobserved_2d)**2
+00014b40: 2a77 696e 646f 7773 5f77 6569 6768 7473  *windows_weights
+00014b50: 5f32 642c 6178 6973 3d31 290a 2020 2020  _2d,axis=1).    
+00014b60: 2020 2020 2020 2020 6e6f 726d 5f66 6163          norm_fac
+00014b70: 746f 722b 3d6e 702e 7375 6d28 7769 6e64  tor+=np.sum(wind
+00014b80: 6f77 735f 7765 6967 6874 7329 0a20 2020  ows_weights).   
+00014b90: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00014ba0: 2020 2020 2020 2063 6869 5f61 7265 612b         chi_area+
+00014bb0: 3d6e 702e 7375 6d28 2828 466d 6f64 656c  =np.sum(((Fmodel
+00014bc0: 5f32 642a 6172 6561 5f32 642d 466f 6273  _2d*area_2d-Fobs
+00014bd0: 6572 7665 645f 3264 292f 466f 6273 6572  erved_2d)/Fobser
+00014be0: 7665 645f 3264 292a 2a32 2c61 7869 733d  ved_2d)**2,axis=
+00014bf0: 3129 0a20 2020 2020 2020 2020 2020 206e  1).            n
+00014c00: 6f72 6d5f 6661 6374 6f72 2b3d 6c65 6e28  orm_factor+=len(
+00014c10: 7769 6e64 6f77 7329 0a20 2020 2069 6620  windows).    if 
+00014c20: 6c65 6e28 7261 7469 6f5f 7769 6e64 6f77  len(ratio_window
+00014c30: 7329 3e30 3a0a 2020 2020 2020 2020 526d  s)>0:.        Rm
+00014c40: 6f64 656c 5f32 643d 6e70 2e64 7374 6163  odel_2d=np.dstac
+00014c50: 6b28 5b52 6d6f 6465 6c20 666f 7220 6920  k([Rmodel for i 
+00014c60: 696e 2072 616e 6765 286c 656e 2861 7265  in range(len(are
+00014c70: 6129 295d 292e 7371 7565 657a 6528 292e  a))]).squeeze().
+00014c80: 542e 7265 7368 6170 6528 286c 656e 2861  T.reshape((len(a
+00014c90: 7265 6129 2c6c 656e 2872 6174 696f 5f77  rea),len(ratio_w
+00014ca0: 696e 646f 7773 2929 290a 2020 2020 2020  indows))).      
+00014cb0: 2020 526f 6273 6572 7665 645f 3264 3d6e    Robserved_2d=n
+00014cc0: 702e 6473 7461 636b 285b 526f 6273 6572  p.dstack([Robser
+00014cd0: 7665 6420 666f 7220 6920 696e 2072 616e  ved for i in ran
+00014ce0: 6765 286c 656e 2861 7265 6129 295d 292e  ge(len(area))]).
+00014cf0: 7371 7565 657a 6528 292e 542e 7265 7368  squeeze().T.resh
+00014d00: 6170 6528 286c 656e 2861 7265 6129 2c6c  ape((len(area),l
+00014d10: 656e 2872 6174 696f 5f77 696e 646f 7773  en(ratio_windows
+00014d20: 2929 290a 2020 2020 2020 2020 6966 2028  ))).        if (
+00014d30: 6c65 6e28 7261 7469 6f5f 7769 6e64 6f77  len(ratio_window
+00014d40: 735b 305d 293d 3d33 293a 2020 2320 7765  s[0])==3):  # we
+00014d50: 6967 6874 6564 2063 6869 320a 2020 2020  ighted chi2.    
+00014d60: 2020 2020 2020 2020 7261 7469 6f5f 7769          ratio_wi
+00014d70: 6e64 6f77 735f 7765 6967 6874 733d 6e70  ndows_weights=np
+00014d80: 2e61 7272 6179 285b 7261 7469 6f5f 7769  .array([ratio_wi
+00014d90: 6e64 6f77 735b 6b5d 5b32 5d20 666f 7220  ndows[k][2] for 
+00014da0: 6b20 696e 2072 616e 6765 286c 656e 2872  k in range(len(r
+00014db0: 6174 696f 5f77 696e 646f 7773 2929 5d29  atio_windows))])
+00014dc0: 0a20 2020 2020 2020 2020 2020 2072 6174  .            rat
+00014dd0: 696f 5f77 696e 646f 7773 5f77 6569 6768  io_windows_weigh
+00014de0: 7473 5f32 643d 6e70 2e64 7374 6163 6b28  ts_2d=np.dstack(
+00014df0: 5b72 6174 696f 5f77 696e 646f 7773 5f77  [ratio_windows_w
+00014e00: 6569 6768 7473 2066 6f72 2069 2069 6e20  eights for i in 
+00014e10: 7261 6e67 6528 6c65 6e28 6172 6561 2929  range(len(area))
+00014e20: 5d29 2e73 7175 6565 7a65 2829 2e54 2e72  ]).squeeze().T.r
+00014e30: 6573 6861 7065 2828 6c65 6e28 6172 6561  eshape((len(area
+00014e40: 292c 6c65 6e28 7261 7469 6f5f 7769 6e64  ),len(ratio_wind
+00014e50: 6f77 735f 7765 6967 6874 7329 2929 0a20  ows_weights))). 
+00014e60: 2020 2020 2020 2020 2020 2063 6869 5f61             chi_a
+00014e70: 7265 612b 3d6e 702e 7375 6d28 2828 526d  rea+=np.sum(((Rm
+00014e80: 6f64 656c 5f32 642d 526f 6273 6572 7665  odel_2d-Robserve
+00014e90: 645f 3264 292f 526f 6273 6572 7665 645f  d_2d)/Robserved_
+00014ea0: 3264 292a 2a32 2a72 6174 696f 5f77 696e  2d)**2*ratio_win
+00014eb0: 646f 7773 5f77 6569 6768 7473 5f32 642c  dows_weights_2d,
+00014ec0: 6178 6973 3d31 290a 2020 2020 2020 2020  axis=1).        
+00014ed0: 2020 2020 6e6f 726d 5f66 6163 746f 722b      norm_factor+
+00014ee0: 3d6e 702e 7375 6d28 7261 7469 6f5f 7769  =np.sum(ratio_wi
+00014ef0: 6e64 6f77 735f 7765 6967 6874 7329 0a20  ndows_weights). 
+00014f00: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00014f10: 2020 2020 2020 2020 2063 6869 5f61 7265           chi_are
+00014f20: 612b 3d6e 702e 7375 6d28 2828 526d 6f64  a+=np.sum(((Rmod
+00014f30: 656c 5f32 642d 526f 6273 6572 7665 645f  el_2d-Robserved_
+00014f40: 3264 292f 526f 6273 6572 7665 645f 3264  2d)/Robserved_2d
+00014f50: 292a 2a32 2c61 7869 733d 3129 0a20 2020  )**2,axis=1).   
+00014f60: 2020 2020 2020 2020 206e 6f72 6d5f 6661           norm_fa
+00014f70: 6374 6f72 2b3d 6c65 6e28 7261 7469 6f5f  ctor+=len(ratio_
+00014f80: 7769 6e64 6f77 7329 0a20 2020 2069 6620  windows).    if 
+00014f90: 6c65 6e28 7072 6f64 7563 745f 7769 6e64  len(product_wind
+00014fa0: 6f77 7329 3e30 3a0a 2020 2020 2020 2020  ows)>0:.        
+00014fb0: 6172 6561 5f32 643d 6e70 2e64 7374 6163  area_2d=np.dstac
+00014fc0: 6b28 5b61 7265 6120 666f 7220 6920 696e  k([area for i in
+00014fd0: 2072 616e 6765 286c 656e 2870 726f 6475   range(len(produ
+00014fe0: 6374 5f77 696e 646f 7773 2929 5d29 2e73  ct_windows))]).s
+00014ff0: 7175 6565 7a65 2829 2e72 6573 6861 7065  queeze().reshape
+00015000: 2828 6c65 6e28 6172 6561 292c 6c65 6e28  ((len(area),len(
+00015010: 7072 6f64 7563 745f 7769 6e64 6f77 7329  product_windows)
+00015020: 2929 0a20 2020 2020 2020 2050 6d6f 6465  )).        Pmode
+00015030: 6c5f 3264 3d6e 702e 6473 7461 636b 285b  l_2d=np.dstack([
+00015040: 506d 6f64 656c 2066 6f72 2069 2069 6e20  Pmodel for i in 
+00015050: 7261 6e67 6528 6c65 6e28 6172 6561 2929  range(len(area))
+00015060: 5d29 2e73 7175 6565 7a65 2829 2e54 2e72  ]).squeeze().T.r
+00015070: 6573 6861 7065 2828 6c65 6e28 6172 6561  eshape((len(area
+00015080: 292c 6c65 6e28 7072 6f64 7563 745f 7769  ),len(product_wi
+00015090: 6e64 6f77 7329 2929 0a20 2020 2020 2020  ndows))).       
+000150a0: 2050 6f62 7365 7276 6564 5f32 643d 6e70   Pobserved_2d=np
+000150b0: 2e64 7374 6163 6b28 5b50 6f62 7365 7276  .dstack([Pobserv
+000150c0: 6564 2066 6f72 2069 2069 6e20 7261 6e67  ed for i in rang
+000150d0: 6528 6c65 6e28 6172 6561 2929 5d29 2e73  e(len(area))]).s
+000150e0: 7175 6565 7a65 2829 2e54 2e72 6573 6861  queeze().T.resha
+000150f0: 7065 2828 6c65 6e28 6172 6561 292c 6c65  pe((len(area),le
+00015100: 6e28 7072 6f64 7563 745f 7769 6e64 6f77  n(product_window
+00015110: 7329 2929 0a20 2020 2020 2020 2069 6620  s))).        if 
+00015120: 286c 656e 2870 726f 6475 6374 5f77 696e  (len(product_win
+00015130: 646f 7773 5b30 5d29 3d3d 3329 3a20 2023  dows[0])==3):  #
+00015140: 2077 6569 6768 7465 6420 6368 6932 0a20   weighted chi2. 
+00015150: 2020 2020 2020 2020 2020 2070 726f 6475             produ
+00015160: 6374 5f77 696e 646f 7773 5f77 6569 6768  ct_windows_weigh
+00015170: 7473 3d6e 702e 6172 7261 7928 5b70 726f  ts=np.array([pro
+00015180: 6475 6374 5f77 696e 646f 7773 5b6b 5d5b  duct_windows[k][
+00015190: 325d 2066 6f72 206b 2069 6e20 7261 6e67  2] for k in rang
+000151a0: 6528 6c65 6e28 7072 6f64 7563 745f 7769  e(len(product_wi
+000151b0: 6e64 6f77 7329 295d 290a 2020 2020 2020  ndows))]).      
+000151c0: 2020 2020 2020 7072 6f64 7563 745f 7769        product_wi
+000151d0: 6e64 6f77 735f 7765 6967 6874 735f 3264  ndows_weights_2d
+000151e0: 3d6e 702e 6473 7461 636b 285b 7072 6f64  =np.dstack([prod
+000151f0: 7563 745f 7769 6e64 6f77 735f 7765 6967  uct_windows_weig
+00015200: 6874 7320 666f 7220 6920 696e 2072 616e  hts for i in ran
+00015210: 6765 286c 656e 2861 7265 6129 295d 292e  ge(len(area))]).
+00015220: 7371 7565 657a 6528 292e 542e 7265 7368  squeeze().T.resh
+00015230: 6170 6528 286c 656e 2861 7265 6129 2c6c  ape((len(area),l
+00015240: 656e 2870 726f 6475 6374 5f77 696e 646f  en(product_windo
+00015250: 7773 5f77 6569 6768 7473 2929 290a 2020  ws_weights))).  
+00015260: 2020 2020 2020 2020 2020 6368 695f 6172            chi_ar
+00015270: 6561 2b3d 6e70 2e73 756d 2828 2828 506d  ea+=np.sum((((Pm
+00015280: 6f64 656c 5f32 642a 6172 6561 5f32 642a  odel_2d*area_2d*
+00015290: 2a32 292a 2a30 2e35 2d28 506f 6273 6572  *2)**0.5-(Pobser
+000152a0: 7665 645f 3264 292a 2a30 2e35 292f 2850  ved_2d)**0.5)/(P
+000152b0: 6f62 7365 7276 6564 5f32 6429 2a2a 302e  observed_2d)**0.
+000152c0: 3529 2a2a 322a 7072 6f64 7563 745f 7769  5)**2*product_wi
+000152d0: 6e64 6f77 735f 7765 6967 6874 735f 3264  ndows_weights_2d
+000152e0: 2c61 7869 733d 3129 0a20 2020 2020 2020  ,axis=1).       
+000152f0: 2020 2020 206e 6f72 6d5f 6661 6374 6f72       norm_factor
+00015300: 2b3d 6e70 2e73 756d 2870 726f 6475 6374  +=np.sum(product
+00015310: 5f77 696e 646f 7773 5f77 6569 6768 7473  _windows_weights
+00015320: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+00015330: 2020 2020 2020 2020 2020 2020 6368 695f              chi_
+00015340: 6172 6561 2b3d 6e70 2e73 756d 2828 2828  area+=np.sum((((
+00015350: 506d 6f64 656c 5f32 642a 6172 6561 5f32  Pmodel_2d*area_2
+00015360: 642a 2a32 292a 2a30 2e35 2d28 506f 6273  d**2)**0.5-(Pobs
+00015370: 6572 7665 645f 3264 292a 2a30 2e35 292f  erved_2d)**0.5)/
+00015380: 2850 6f62 7365 7276 6564 5f32 6429 2a2a  (Pobserved_2d)**
+00015390: 302e 3529 2a2a 322c 6178 6973 3d31 290a  0.5)**2,axis=1).
+000153a0: 2020 2020 2020 2020 2020 2020 6e6f 726d              norm
+000153b0: 5f66 6163 746f 722b 3d6c 656e 2870 726f  _factor+=len(pro
+000153c0: 6475 6374 5f77 696e 646f 7773 290a 2020  duct_windows).  
+000153d0: 2020 6966 206e 6f72 6d5f 6661 6374 6f72    if norm_factor
+000153e0: 3e30 3a20 6368 695f 6172 6561 2f3d 6e6f  >0: chi_area/=no
+000153f0: 726d 5f66 6163 746f 720a 2020 2020 7265  rm_factor.    re
+00015400: 7475 726e 2863 6869 5f61 7265 6129 0a0a  turn(chi_area)..
+00015410: 0a64 6566 2072 6564 5f63 6869 325f 736c  .def red_chi2_sl
+00015420: 6162 2873 6c61 625f 6461 7461 2c73 7065  ab(slab_data,spe
+00015430: 6374 7261 2c6d 6173 6b2c 5264 6973 6b3d  ctra,mask,Rdisk=
+00015440: 6e70 2e6c 6f67 7370 6163 6528 2d32 2c32  np.logspace(-2,2
+00015450: 2c31 3029 2c64 6973 7461 6e63 653d 3132  ,10),distance=12
+00015460: 302c 4e4c 5445 3d46 616c 7365 2c52 3d33  0,NLTE=False,R=3
+00015470: 3030 302c 7368 6f72 745f 666f 726d 6174  000,short_format
+00015480: 3d46 616c 7365 2c6f 7665 726c 6170 3d46  =False,overlap=F
+00015490: 616c 7365 2c6e 6f69 7365 5f6c 6576 656c  alse,noise_level
+000154a0: 3d31 293a 0a20 2020 2027 2727 0a20 2020  =1):.    '''.   
+000154b0: 2052 6574 7572 6e73 2072 6564 7563 6564   Returns reduced
+000154c0: 2063 6869 3220 6261 7365 6420 6f6e 2073   chi2 based on s
+000154d0: 656c 6563 7465 6420 7370 6563 7472 616c  elected spectral
+000154e0: 2077 696e 646f 7773 2061 6372 6f73 7320   windows across 
+000154f0: 6469 6666 6572 656e 7420 656d 6974 7469  different emitti
+00015500: 6e67 2064 6973 6b20 7261 6469 7573 0a0a  ng disk radius..
+00015510: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+00015520: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+00015530: 2020 736c 6162 5f64 6174 6120 3a20 7374    slab_data : st
+00015540: 7269 6e67 206f 7220 736c 6162 5f6d 6f64  ring or slab_mod
+00015550: 656c 2069 6e73 7461 6e63 650a 2020 2020  el instance.    
+00015560: 2020 7061 7468 2063 6f72 7265 7370 6f6e    path correspon
+00015570: 6469 6e67 2074 6f20 6120 7369 6e67 6c65  ding to a single
+00015580: 2073 6c61 6220 6d6f 6465 6c20 6f72 2061   slab model or a
+00015590: 2073 696e 676c 6520 736c 6162 5f6d 6f64   single slab_mod
+000155a0: 656c 2069 6e73 7461 6e63 650a 2020 2020  el instance.    
+000155b0: 0a20 2020 2073 7065 6374 7261 203a 206e  .    spectra : n
+000155c0: 756d 7079 2e61 7272 6179 0a20 2020 2020  umpy.array.     
+000155d0: 206e 756d 7079 2061 7272 6179 2077 6974   numpy array wit
+000155e0: 6820 6669 7273 7420 636f 6c75 6d6e 2074  h first column t
+000155f0: 6865 2077 6176 656c 656e 6774 6820 696e  he wavelength in
+00015600: 205b 6d69 6372 6f6e 735d 2061 6e64 2073   [microns] and s
+00015610: 6563 6f6e 6420 636f 6c75 6d6e 2066 6c75  econd column flu
+00015620: 7820 696e 205b 4a79 5d0a 2020 2020 0a20  x in [Jy].    . 
+00015630: 2020 2052 6469 736b 203a 2066 6c6f 6174     Rdisk : float
+00015640: 0a20 2020 2020 2052 6164 6975 7320 636f  .      Radius co
+00015650: 7272 6573 706f 6e64 696e 6720 746f 2065  rresponding to e
+00015660: 6d69 7474 696e 6720 6172 6561 2069 6e20  mitting area in 
+00015670: 6173 7472 6f6e 6f6d 6963 616c 2075 6e69  astronomical uni
+00015680: 7473 0a20 2020 200a 2020 2020 6469 7374  ts.    .    dist
+00015690: 616e 6365 203a 2066 6c6f 6174 0a20 2020  ance : float.   
+000156a0: 2020 2064 6973 7461 6e63 6520 6f66 2064     distance of d
+000156b0: 6973 6b20 696e 2070 6172 7365 630a 2020  isk in parsec.  
+000156c0: 2020 0a20 2020 204e 4c54 4520 3a20 626f    .    NLTE : bo
+000156d0: 6f6c 6561 6e0a 2020 2020 2020 6966 2054  olean.      if T
+000156e0: 7275 652c 204e 4c54 4520 666c 7578 2069  rue, NLTE flux i
+000156f0: 7320 7461 6b65 6e20 6672 6f6d 2074 6865  s taken from the
+00015700: 2073 6c61 6220 6d6f 6465 6c20 696e 2063   slab model in c
+00015710: 6173 6520 6f66 206f 7665 726c 6170 3d46  ase of overlap=F
+00015720: 616c 7365 2e0a 2020 2020 2727 270a 2020  alse..    '''.  
+00015730: 2020 6172 6561 3d28 6e70 2e70 692a 2852    area=(np.pi*(R
+00015740: 6469 736b 2a61 752f 6469 7374 616e 6365  disk*au/distance
+00015750: 2f70 6329 2a2a 3229 2e72 6573 6861 7065  /pc)**2).reshape
+00015760: 2852 6469 736b 2e73 6861 7065 5b30 5d2c  (Rdisk.shape[0],
+00015770: 3129 0a0a 2020 2020 6966 206e 6f74 206f  1)..    if not o
+00015780: 7665 726c 6170 3a0a 2020 2020 2020 2020  verlap:.        
+00015790: 6966 2069 7369 6e73 7461 6e63 6528 736c  if isinstance(sl
+000157a0: 6162 5f64 6174 612c 7374 7229 3a20 736c  ab_data,str): sl
+000157b0: 6162 5f64 6174 613d 7265 6164 5f73 6c61  ab_data=read_sla
+000157c0: 6228 736c 6162 5f64 6174 612c 7665 7262  b(slab_data,verb
+000157d0: 6f73 653d 4661 6c73 652c 7368 6f72 745f  ose=False,short_
+000157e0: 666f 726d 6174 3d73 686f 7274 5f66 6f72  format=short_for
+000157f0: 6d61 7429 0a20 2020 2020 2020 206c 6d69  mat).        lmi
+00015800: 6e3d 6e70 2e61 6d69 6e28 7370 6563 7472  n=np.amin(spectr
+00015810: 615b 3a2c 305d 290a 2020 2020 2020 2020  a[:,0]).        
+00015820: 6c6d 6178 3d6e 702e 616d 6178 2873 7065  lmax=np.amax(spe
+00015830: 6374 7261 5b3a 2c30 5d29 0a20 2020 2020  ctra[:,0]).     
+00015840: 2020 2073 6c61 625f 6461 7461 2e63 6f6e     slab_data.con
+00015850: 766f 6c76 6528 523d 522c 6c61 6d62 6461  volve(R=R,lambda
+00015860: 5f30 3d6c 6d69 6e2a 302e 392c 6c61 6d62  _0=lmin*0.9,lamb
+00015870: 6461 5f6e 3d6c 6d61 782a 312e 312c 4e4c  da_n=lmax*1.1,NL
+00015880: 5445 3d4e 4c54 452c 7665 7262 6f73 653d  TE=NLTE,verbose=
+00015890: 4661 6c73 6529 0a20 2020 2020 2020 2069  False).        i
+000158a0: 6620 4e4c 5445 3a0a 2020 2020 2020 2020  f NLTE:.        
+000158b0: 2020 2020 6d6f 6465 6c53 7065 633d 7370      modelSpec=sp
+000158c0: 6563 7472 6573 2e73 7065 6374 7265 7328  ectres.spectres(
+000158d0: 7370 6563 7472 615b 3a2c 305d 2c73 6c61  spectra[:,0],sla
+000158e0: 625f 6461 7461 2e63 6f6e 7657 6176 656c  b_data.convWavel
+000158f0: 656e 6774 682c 736c 6162 5f64 6174 612e  ength,slab_data.
+00015900: 636f 6e76 4e4c 5445 666c 7578 2a31 6532  convNLTEflux*1e2
+00015910: 332c 7665 7262 6f73 653d 4661 6c73 652c  3,verbose=False,
+00015920: 6669 6c6c 3d30 2e30 290a 2020 2020 2020  fill=0.0).      
+00015930: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00015940: 2020 2020 6d6f 6465 6c53 7065 633d 7370      modelSpec=sp
+00015950: 6563 7472 6573 2e73 7065 6374 7265 7328  ectres.spectres(
+00015960: 7370 6563 7472 615b 3a2c 305d 2c73 6c61  spectra[:,0],sla
+00015970: 625f 6461 7461 2e63 6f6e 7657 6176 656c  b_data.convWavel
+00015980: 656e 6774 682c 736c 6162 5f64 6174 612e  ength,slab_data.
+00015990: 636f 6e76 4c54 4566 6c75 782a 3165 3233  convLTEflux*1e23
+000159a0: 2c76 6572 626f 7365 3d46 616c 7365 2c66  ,verbose=False,f
+000159b0: 696c 6c3d 302e 3029 0a20 2020 2065 6c73  ill=0.0).    els
+000159c0: 653a 0a20 2020 2020 2020 2069 6620 6973  e:.        if is
+000159d0: 696e 7374 616e 6365 2873 6c61 625f 6461  instance(slab_da
+000159e0: 7461 2c73 7472 293a 2073 6c61 625f 6461  ta,str): slab_da
+000159f0: 7461 3d72 6561 645f 6f76 6572 6c61 705f  ta=read_overlap_
+00015a00: 7370 6563 7472 6128 736c 6162 5f64 6174  spectra(slab_dat
+00015a10: 612c 7665 7262 6f73 653d 4661 6c73 6529  a,verbose=False)
+00015a20: 0a20 2020 2020 2020 206c 6d69 6e3d 6e70  .        lmin=np
+00015a30: 2e61 6d69 6e28 7370 6563 7472 615b 3a2c  .amin(spectra[:,
+00015a40: 305d 290a 2020 2020 2020 2020 6c6d 6178  0]).        lmax
+00015a50: 3d6e 702e 616d 6178 2873 7065 6374 7261  =np.amax(spectra
+00015a60: 5b3a 2c30 5d29 0a20 2020 2020 2020 2073  [:,0]).        s
+00015a70: 6c61 625f 6461 7461 2e63 6f6e 766f 6c76  lab_data.convolv
+00015a80: 655f 6f76 6572 6c61 7028 523d 522c 6c61  e_overlap(R=R,la
+00015a90: 6d62 6461 5f30 3d6c 6d69 6e2a 302e 392c  mbda_0=lmin*0.9,
+00015aa0: 6c61 6d62 6461 5f6e 3d6c 6d61 782a 312e  lambda_n=lmax*1.
+00015ab0: 312c 7665 7262 6f73 653d 4661 6c73 6529  1,verbose=False)
+00015ac0: 0a20 2020 2020 2020 206d 6f64 656c 5370  .        modelSp
+00015ad0: 6563 3d73 7065 6374 7265 732e 7370 6563  ec=spectres.spec
+00015ae0: 7472 6573 2873 7065 6374 7261 5b3a 2c30  tres(spectra[:,0
+00015af0: 5d2c 632f 736c 6162 5f64 6174 612e 636f  ],c/slab_data.co
+00015b00: 6e76 4f76 6572 6c61 7046 7265 715b 3a3a  nvOverlapFreq[::
+00015b10: 2d31 5d2a 3165 2d33 2c73 6c61 625f 6461  -1]*1e-3,slab_da
+00015b20: 7461 2e63 6f6e 764f 7665 726c 6170 4c54  ta.convOverlapLT
+00015b30: 455b 3a3a 2d31 5d2a 3165 3233 2c76 6572  E[::-1]*1e23,ver
+00015b40: 626f 7365 3d46 616c 7365 2c66 696c 6c3d  bose=False,fill=
+00015b50: 302e 3029 0a20 2020 2073 7065 6374 7261  0.0).    spectra
+00015b60: 5f32 643d 7370 6563 7472 615b 6d61 736b  _2d=spectra[mask
+00015b70: 2c31 5d2e 7265 7368 6170 6528 312c 7370  ,1].reshape(1,sp
+00015b80: 6563 7472 615b 6d61 736b 2c2d 315d 2e73  ectra[mask,-1].s
+00015b90: 6861 7065 5b30 5d29 2a6e 702e 6f6e 6573  hape[0])*np.ones
+00015ba0: 5f6c 696b 6528 6172 6561 290a 2020 2020  _like(area).    
+00015bb0: 6d6f 6465 6c53 7065 635f 3264 3d6d 6f64  modelSpec_2d=mod
+00015bc0: 656c 5370 6563 5b6d 6173 6b5d 2e72 6573  elSpec[mask].res
+00015bd0: 6861 7065 2831 2c6d 6f64 656c 5370 6563  hape(1,modelSpec
+00015be0: 5b6d 6173 6b5d 2e73 6861 7065 5b30 5d29  [mask].shape[0])
+00015bf0: 2a6e 702e 6f6e 6573 5f6c 696b 6528 6172  *np.ones_like(ar
+00015c00: 6561 290a 2020 2020 6172 6561 5f32 643d  ea).    area_2d=
+00015c10: 6172 6561 2e72 6573 6861 7065 2861 7265  area.reshape(are
+00015c20: 612e 7368 6170 655b 305d 2c31 290a 2020  a.shape[0],1).  
+00015c30: 2020 6368 695f 6172 6561 3d6e 702e 7375    chi_area=np.su
+00015c40: 6d28 2873 7065 6374 7261 5f32 642d 6d6f  m((spectra_2d-mo
+00015c50: 6465 6c53 7065 635f 3264 2a61 7265 615f  delSpec_2d*area_
+00015c60: 3264 292a 2a32 2c61 7869 733d 3129 2f6c  2d)**2,axis=1)/l
+00015c70: 656e 2873 7065 6374 7261 5b6d 6173 6b2c  en(spectra[mask,
+00015c80: 305d 292f 6e6f 6973 655f 6c65 7665 6c2a  0])/noise_level*
+00015c90: 2a32 0a0a 2020 2020 7265 7475 726e 2863  *2..    return(c
+00015ca0: 6869 5f61 7265 6129 0a                   hi_area).
```

### Comparing `prodimopy-2.1.6/prodimopy/script_compare.py` & `prodimopy-2.2/prodimopy/script_compare.py`

 * *Files identical despite different names*

### Comparing `prodimopy-2.1.6/prodimopy/script_params.py` & `prodimopy-2.2/prodimopy/script_params.py`

 * *Files identical despite different names*

### Comparing `prodimopy-2.1.6/prodimopy/script_plot.py` & `prodimopy-2.2/prodimopy/script_plot.py`

 * *Files identical despite different names*

### Comparing `prodimopy-2.1.6/prodimopy/script_plot_models.py` & `prodimopy-2.2/prodimopy/script_plot_models.py`

 * *Files identical despite different names*

### Comparing `prodimopy-2.1.6/prodimopy/utils.py` & `prodimopy-2.2/prodimopy/utils.py`

 * *Files identical despite different names*

### Comparing `prodimopy-2.1.6/prodimopy/utils_casasim.py` & `prodimopy-2.2/prodimopy/utils_casasim.py`

 * *Files identical despite different names*

### Comparing `prodimopy-2.1.6/prodimopy.egg-info/PKG-INFO` & `prodimopy-2.2/prodimopy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prodimopy
-Version: 2.1.6
+Version: 2.2
 Summary: Python tools for ProDiMo.
 Home-page: https://gitlab.astro.rug.nl/prodimo/prodimopy/
 Author: Christian Rab
 Author-email: rab@astro.rug.nl
 License: MIT License
 Keywords: astronomy astrophysics star-formation protoplanetary-disks
 Classifier: Development Status :: 4 - Beta
```

### Comparing `prodimopy-2.1.6/prodimopy.egg-info/SOURCES.txt` & `prodimopy-2.2/prodimopy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 prodimopy/plot_mc.py
 prodimopy/plot_models.py
 prodimopy/plot_slab.py
 prodimopy/read.py
 prodimopy/read_casasim.py
 prodimopy/read_mc.py
 prodimopy/read_slab.py
+prodimopy/run_slab.py
 prodimopy/script_compare.py
 prodimopy/script_params.py
 prodimopy/script_plot.py
 prodimopy/script_plot_models.py
 prodimopy/utils.py
 prodimopy/utils_casasim.py
 prodimopy.egg-info/PKG-INFO
```

### Comparing `prodimopy-2.1.6/setup.py` & `prodimopy-2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
 setup(
     name='prodimopy',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='2.1.6',
+    version='2.2',
 
     description='Python tools for ProDiMo.',
     long_description=long_description,
     long_description_content_type="text/markdown",
 
     # The project's main homepage.
     url='https://gitlab.astro.rug.nl/prodimo/prodimopy/',
```

