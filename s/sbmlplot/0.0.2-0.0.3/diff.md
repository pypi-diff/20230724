# Comparing `tmp/sbmlplot-0.0.2-py3-none-any.whl.zip` & `tmp/sbmlplot-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 26007 bytes, number of entries: 8
+Zip file size: 26011 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat       25 b- defN 23-Jul-24 17:20 sbmlplot/__init__.py
 -rw-rw-rw-  2.0 fat   179847 b- defN 23-Jul-24 17:20 sbmlplot/sbmlplot.py
--rw-rw-rw-  2.0 fat     2029 b- defN 23-Jul-24 17:20 sbmlplot-0.0.2.data/scripts/test1.py
--rw-rw-rw-  2.0 fat     1104 b- defN 23-Jul-24 17:39 sbmlplot-0.0.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1215 b- defN 23-Jul-24 17:39 sbmlplot-0.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-24 17:39 sbmlplot-0.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-24 17:39 sbmlplot-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      637 b- defN 23-Jul-24 17:39 sbmlplot-0.0.2.dist-info/RECORD
-8 files, 184958 bytes uncompressed, 24897 bytes compressed:  86.5%
+-rw-rw-rw-  2.0 fat     2029 b- defN 23-Jul-24 17:20 sbmlplot-0.0.3.data/scripts/test1.py
+-rw-rw-rw-  2.0 fat     1104 b- defN 23-Jul-24 17:52 sbmlplot-0.0.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1222 b- defN 23-Jul-24 17:52 sbmlplot-0.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-24 17:52 sbmlplot-0.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-24 17:52 sbmlplot-0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      637 b- defN 23-Jul-24 17:52 sbmlplot-0.0.3.dist-info/RECORD
+8 files, 184965 bytes uncompressed, 24901 bytes compressed:  86.5%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: sbmlplot/__init__.py
 Comment: 
 
 Filename: sbmlplot/sbmlplot.py
 Comment: 
 
-Filename: sbmlplot-0.0.2.data/scripts/test1.py
+Filename: sbmlplot-0.0.3.data/scripts/test1.py
 Comment: 
 
-Filename: sbmlplot-0.0.2.dist-info/LICENSE
+Filename: sbmlplot-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: sbmlplot-0.0.2.dist-info/METADATA
+Filename: sbmlplot-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: sbmlplot-0.0.2.dist-info/WHEEL
+Filename: sbmlplot-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: sbmlplot-0.0.2.dist-info/top_level.txt
+Filename: sbmlplot-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: sbmlplot-0.0.2.dist-info/RECORD
+Filename: sbmlplot-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `sbmlplot-0.0.2.data/scripts/test1.py` & `sbmlplot-0.0.3.data/scripts/test1.py`

 * *Files identical despite different names*

## Comparing `sbmlplot-0.0.2.dist-info/LICENSE` & `sbmlplot-0.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sbmlplot-0.0.2.dist-info/METADATA` & `sbmlplot-0.0.3.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: sbmlplot
-Version: 0.0.2
+Version: 0.0.3
 Summary: Visualize the network of SBML models
 Home-page: https://github.com/adelhpour/sbmlplot
 Author: Adel Heydarabadipour
 Author-email: ad.heydarabadi@gmail.com
 License: MIT License
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Requires-Dist: libsbne
 Requires-Dist: matplotlib (>=3.4.0)
 Requires-Dist: numpy
-Requires-Dist: libsbml
+Requires-Dist: python-libsbml
 Requires-Dist: webcolors
 
 Sbmlplot is a python tool built on libSBNE, an API which can read or automatically generate, manipulate, and write SBML Layout and Redner information. Using either the already-included or auto-generated information about Layout and Render extensions of an SBML model, sbmlplot helps you render a static illustration of the biological network of the SBML model through matplotlib and generate a .json file containing the elements and styles information required to render a dynamic illustration of the biological network of the model through cytoscape.js.
```

## Comparing `sbmlplot-0.0.2.dist-info/RECORD` & `sbmlplot-0.0.3.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 sbmlplot/__init__.py,sha256=ILwdZ4hOv4Ac0Y5LZo5JQ7H5voXpSiVQkqIstmdAumg,25
 sbmlplot/sbmlplot.py,sha256=mQXTlLL9yKms1gO6j8TC6ypcRPe_MOBY5hzw0pdAH4c,179847
-sbmlplot-0.0.2.data/scripts/test1.py,sha256=Zb7J9ILJvOG-_SwSZ4E1w2gJ_LjrWcJy3S7-0sgjPJA,2029
-sbmlplot-0.0.2.dist-info/LICENSE,sha256=YFgU2-Gehla18w-vgYNbsnnvK_5y1y0wG2xu4R_uM3c,1104
-sbmlplot-0.0.2.dist-info/METADATA,sha256=nGlmhTuogdJksZAO0hDNYNPsUvdCQ_8HaZYN-Cg1qQs,1215
-sbmlplot-0.0.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-sbmlplot-0.0.2.dist-info/top_level.txt,sha256=2ven7IIRpsIFpIAI6Tjz9FGo7E5a0LF7FY2Pt1Auypg,9
-sbmlplot-0.0.2.dist-info/RECORD,,
+sbmlplot-0.0.3.data/scripts/test1.py,sha256=Zb7J9ILJvOG-_SwSZ4E1w2gJ_LjrWcJy3S7-0sgjPJA,2029
+sbmlplot-0.0.3.dist-info/LICENSE,sha256=YFgU2-Gehla18w-vgYNbsnnvK_5y1y0wG2xu4R_uM3c,1104
+sbmlplot-0.0.3.dist-info/METADATA,sha256=-LgFrfKOiBrnfnfmqc0XahBhjW6eDkeVlb9KHI2Ldm0,1222
+sbmlplot-0.0.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+sbmlplot-0.0.3.dist-info/top_level.txt,sha256=2ven7IIRpsIFpIAI6Tjz9FGo7E5a0LF7FY2Pt1Auypg,9
+sbmlplot-0.0.3.dist-info/RECORD,,
```

