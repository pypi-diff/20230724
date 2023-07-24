# Comparing `tmp/dgh-0.0.8.tar.gz` & `tmp/dgh-0.1.0.tar.gz`

## Comparing `dgh-0.0.8.tar` & `dgh-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 dgh-0.0.8/CHANGELOG.md
--rw-r--r--   0        0        0    10507 2020-02-02 00:00:00.000000 dgh-0.0.8/illustration.pdf
--rw-r--r--   0        0        0    13473 2020-02-02 00:00:00.000000 dgh-0.0.8/illustration.png
--rw-r--r--   0        0        0    10989 2020-02-02 00:00:00.000000 dgh-0.0.8/illustration.svg
--rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 dgh-0.0.8/illustration_wide.pdf
--rw-r--r--   0        0        0     4599 2020-02-02 00:00:00.000000 dgh-0.0.8/illustration_wide_tall.pdf
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 dgh-0.0.8/dgh/__init__.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 dgh-0.0.8/dgh/constants.py
--rw-r--r--   0        0        0     7259 2020-02-02 00:00:00.000000 dgh-0.0.8/dgh/dgh.py
--rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 dgh-0.0.8/dgh/fw.py
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 dgh-0.0.8/dgh/mappings.py
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 dgh-0.0.8/dgh/spaces.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 dgh-0.0.8/.gitignore
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 dgh-0.0.8/LICENSE
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 dgh-0.0.8/README.md
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 dgh-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 dgh-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 dgh-0.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0    10558 2020-02-02 00:00:00.000000 dgh-0.1.0/illustration.pdf
+-rw-r--r--   0        0        0    11309 2020-02-02 00:00:00.000000 dgh-0.1.0/illustration.svg
+-rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 dgh-0.1.0/illustration_wide.pdf
+-rw-r--r--   0        0        0     4599 2020-02-02 00:00:00.000000 dgh-0.1.0/illustration_wide_tall.pdf
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 dgh-0.1.0/dgh/__init__.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 dgh-0.1.0/dgh/constants.py
+-rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 dgh-0.1.0/dgh/dgh.py
+-rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 dgh-0.1.0/dgh/fw.py
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 dgh-0.1.0/dgh/mappings.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 dgh-0.1.0/dgh/spaces.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 dgh-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 dgh-0.1.0/LICENSE
+-rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 dgh-0.1.0/README.md
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 dgh-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 dgh-0.1.0/PKG-INFO
```

### Comparing `dgh-0.0.8/CHANGELOG.md` & `dgh-0.1.0/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,27 @@
 # Changelog
 
 <!--next-version-placeholder-->
+## v0.1.0 (Jul 24 2023)
+
+### Feature
+
+- Added searching for best c as default behavior
+- Added function for random generation of a bi-mapping polytope vertex R
+- Added `__version__` variable
+- Python >= 3.8 is now required
+
+### Fix
+
+- Removed convexity-based calculation of c and warm-start sequences of c due to inefficiency
+
+### Documentation
+
+- Created "Advanced" section where the logic behind parameter c is explained
+
 ## v0.0.8 (May 11 2023)
 
 ### Feature
 
 - Added f, g to verbose output if returning them
 
 ### Fix
```

### Comparing `dgh-0.0.8/illustration.pdf` & `dgh-0.1.0/illustration.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 17% similar despite different names*

#### dumppdf -adt {}

 * *error from `dumppdf -adt {}`:*

 * *DEBUG:pdfminer.psparser:seek: 0*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b''*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'%%EOF'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'10186'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'startxref'*

 * *DEBUG:pdfminer.pdfdocument:xref found: pos=b'10186'*

 * *DEBUG:pdfminer.psparser:seek: 10186*

 * *DEBUG:pdfminer.psparser:nexttoken: (10186, 21)*

 * *DEBUG:pdfminer.pdfdocument:read_xref_from: start=10186, token=21*

 * *DEBUG:pdfminer.psparser:seek: 10186*

 * *DEBUG:pdfminer.psparser:nexttoken: (10186, 21)*

 * *DEBUG:pdfminer.psparser:nexttoken: (10189, 0)*

 * *DEBUG:pdfminer.psparser:nexttoken: (10191, /b'obj')*

 * *DEBUG:pdfminer.psparser:nexttoken: (10195, /b'<<')*

 * *DEBUG:pdfminer.psparser:start_type: pos=10195, type='d'*

 * *DEBUG:pdfminer.psparser:nexttoken: (10198, /'Type')*

 * *DEBUG:pdfminer.psparser:nexttoken: (10204, /'XRef')*

 * *DEBUG:pdfminer.psparser:nexttoken: (10210, /'Index')*

 * *DEBUG:pdfminer.psparser:nexttoken: (10217, /b'[')*

 * *DEBUG:pdfminer.psparser:start_type: pos=10217, type='a'*

 * *DEBUG:pdfminer.psparser:nexttoken: (10218, 0)*

 * *DEBUG:pdfminer.psparser:nexttoken: (10220, 22)*

 * *DEBUG:pdfminer.psparser:nexttoken: (10222, /b']')*

 * *DEBUG:pdfminer.psparser:end_type: pos=10217, type='a', objs=[0, 22]*

 * *DEBUG:pdfminer.psparser:nexttoken: (10224, /'Size')*

 * *[ truncated after 25 lines; 714 ignored ]*

```diff
@@ -37,20 +37,20 @@
 <key>Type</key>
 <value><literal>ObjStm</literal></value>
 <key>N</key>
 <value><number>14</number></value>
 <key>First</key>
 <value><number>89</number></value>
 <key>Length</key>
-<value><number>593</number></value>
+<value><number>591</number></value>
 <key>Filter</key>
 <value><literal>FlateDecode</literal></value>
 </dict>
 </props>
-<data size="1018">4 0 6 31 10 129 8 166 1 272 2 277 3 282 13 320 15 334 11 540&#10;12 682 17 724 18 783 19 803&#10;&#60;&#60; /S /GoTo /D [6 0 R /Fit] &#62;&#62;&#10;&#60;&#60;&#10;/Type /Page&#10;/Contents 9 0 R&#10;/Resources 8 0 R&#10;/MediaBox [0 0 196.686 138.994]&#10;/Parent 12 0 R&#10;&#62;&#62;&#10;&#60;&#60;&#10;/D [6 0 R /XYZ 71 67.994 null]&#10;&#62;&#62;&#10;&#60;&#60;&#10; /ColorSpace 3 0 R /Pattern 2 0 R /ExtGState 1 0 R &#10;/Font &#60;&#60; /F66 11 0 R &#62;&#62;&#10;/ProcSet [ /PDF /Text ]&#10;&#62;&#62;&#10;&#60;&#60;&#62;&#62;&#10;&#60;&#60;&#62;&#62;&#10;&#60;&#60;  /pgfprgb [/Pattern /DeviceRGB] &#62;&#62;&#10;[812.6 568.1]&#10;&#60;&#60;&#10;/Type /FontDescriptor&#10;/FontName /ECMUZQ+CMMI12&#10;/Flags 4&#10;/FontBBox [-31 -250 1026 750]&#10;/Ascent 694&#10;/CapHeight 683&#10;/Descent -194&#10;/ItalicAngle -14&#10;/StemV 65&#10;/XHeight 431&#10;/CharSet &#40;/X/Y&#41;&#10;/FontFile 14 0 R&#10;&#62;&#62;&#10;&#60;&#60;&#10;/Type /Font&#10;/Subtype /Type1&#10;/BaseFont /ECMUZQ+CMMI12&#10;/FontDescriptor 15 0 R&#10;/FirstChar 88&#10;/LastChar 89&#10;/Widths 13 0 R&#10;/ToUnicode 16 0 R&#10;&#62;&#62;&#10;&#60;&#60;&#10;/Type /Pages&#10;/Count 1&#10;/Kids [6 0 R]&#10;&#62;&#62;&#10;&#60;&#60;&#10;/Names [&#40;page.2&#41; 10 0 R]&#10;/Limits [&#40;page.2&#41; &#40;page.2&#41;]&#10;&#62;&#62;&#10;&#60;&#60;&#10;/Dests 17 0 R&#10;&#62;&#62;&#10;&#60;&#60;&#10;/Type /Catalog&#10;/Pages 12 0 R&#10;/Names 18 0 R&#10;/PageMode/UseOutlines/PageLabels&#60;&#60;/Nums[0&#60;&#60;/S/D /St 2&#62;&#62;]&#62;&#62;&#10;/OpenAction 4 0 R&#10;&#62;&#62;&#10;</data>
+<data size="1017">4 0 6 31 10 128 8 165 1 271 2 276 3 281 13 319 15 333 11 539&#10;12 681 17 723 18 782 19 802&#10;&#60;&#60; /S /GoTo /D [6 0 R /Fit] &#62;&#62;&#10;&#60;&#60;&#10;/Type /Page&#10;/Contents 9 0 R&#10;/Resources 8 0 R&#10;/MediaBox [0 0 206.98 149.289]&#10;/Parent 12 0 R&#10;&#62;&#62;&#10;&#60;&#60;&#10;/D [6 0 R /XYZ 71 78.289 null]&#10;&#62;&#62;&#10;&#60;&#60;&#10; /ColorSpace 3 0 R /Pattern 2 0 R /ExtGState 1 0 R &#10;/Font &#60;&#60; /F66 11 0 R &#62;&#62;&#10;/ProcSet [ /PDF /Text ]&#10;&#62;&#62;&#10;&#60;&#60;&#62;&#62;&#10;&#60;&#60;&#62;&#62;&#10;&#60;&#60;  /pgfprgb [/Pattern /DeviceRGB] &#62;&#62;&#10;[812.6 568.1]&#10;&#60;&#60;&#10;/Type /FontDescriptor&#10;/FontName /ECMUZQ+CMMI12&#10;/Flags 4&#10;/FontBBox [-31 -250 1026 750]&#10;/Ascent 694&#10;/CapHeight 683&#10;/Descent -194&#10;/ItalicAngle -14&#10;/StemV 65&#10;/XHeight 431&#10;/CharSet &#40;/X/Y&#41;&#10;/FontFile 14 0 R&#10;&#62;&#62;&#10;&#60;&#60;&#10;/Type /Font&#10;/Subtype /Type1&#10;/BaseFont /ECMUZQ+CMMI12&#10;/FontDescriptor 15 0 R&#10;/FirstChar 88&#10;/LastChar 89&#10;/Widths 13 0 R&#10;/ToUnicode 16 0 R&#10;&#62;&#62;&#10;&#60;&#60;&#10;/Type /Pages&#10;/Count 1&#10;/Kids [6 0 R]&#10;&#62;&#62;&#10;&#60;&#60;&#10;/Names [&#40;page.2&#41; 10 0 R]&#10;/Limits [&#40;page.2&#41; &#40;page.2&#41;]&#10;&#62;&#62;&#10;&#60;&#60;&#10;/Dests 17 0 R&#10;&#62;&#62;&#10;&#60;&#60;&#10;/Type /Catalog&#10;/Pages 12 0 R&#10;/Names 18 0 R&#10;/PageMode/UseOutlines/PageLabels&#60;&#60;/Nums[0&#60;&#60;/S/D /St 2&#62;&#62;]&#62;&#62;&#10;/OpenAction 4 0 R&#10;&#62;&#62;&#10;</data>
 </stream>
 </object>
 
 <object id="6">
 <dict size="5">
 <key>Type</key>
 <value><literal>Page</literal></value>
@@ -58,16 +58,16 @@
 <value><ref id="9" /></value>
 <key>Resources</key>
 <value><ref id="8" /></value>
 <key>MediaBox</key>
 <value><list size="4">
 <number>0</number>
 <number>0</number>
-<number>196.686</number>
-<number>138.994</number>
+<number>206.98</number>
+<number>149.289</number>
 </list></value>
 <key>Parent</key>
 <value><ref id="12" /></value>
 </dict>
 </object>
 
 <object id="8">
@@ -92,31 +92,31 @@
 </object>
 
 <object id="9">
 <stream>
 <props>
 <dict size="2">
 <key>Length</key>
-<value><number>828</number></value>
+<value><number>884</number></value>
 <key>Filter</key>
 <value><literal>FlateDecode</literal></value>
 </dict>
 </props>
-<data size="3762">0 g 0 G&#10;1 0 0 1 34.064 119.103 cm&#10;q &#10;0 G &#10;0 g &#10;0.3985 w &#10;q &#10;q &#10;1 0 0 rg &#10;q &#10;1 0 0 rg &#10;5.51819 0.0 m &#10;5.51819 3.04764 3.04764 5.51819 0.0 5.51819 c &#10;-3.04764 5.51819 -5.51819 3.04764 -5.51819 0.0 c &#10;-5.51819 -3.04764 -3.04764 -5.51819 0.0 -5.51819 c &#10;3.04764 -5.51819 5.51819 -3.04764 5.51819 0.0 c &#10;h &#10;0.0 0.0 m &#10;B &#10;Q &#10;q &#10;1.0 0.0 0.0 1.0 0.0 0.0 cm &#10;q &#10;0 G &#10;0 g &#10;Q &#10;Q &#10;Q &#10;q &#10;1 0 0 rg &#10;q &#10;1 0 0 rg &#10;-22.82861 0.0 m &#10;-22.82861 3.04764 -25.29915 5.51819 -28.3468 5.51819 c &#10;-31.39445 5.51819 -33.865 3.04764 -33.865 0.0 c &#10;-33.865 -3.04764 -31.39445 -5.51819 -28.3468 -5.51819 c &#10;-25.29915 -5.51819 -22.82861 -3.04764 -22.82861 0.0 c &#10;h &#10;-28.3468 0.0 m &#10;B &#10;Q &#10;q &#10;1 0 0 1 -28.347 0 cm&#10;1.0 0.0 0.0 1.0 0.0 0.0 cm &#10;q &#10;0 G &#10;0 g &#10;Q &#10;1 0 0 1 28.347 0 cm&#10;Q &#10;Q &#10;q &#10;1 0 0 rg &#10;q &#10;1 0 0 rg &#10;5.51819 -113.38728 m &#10;5.51819 -110.33963 3.04764 -107.86908 0.0 -107.86908 c &#10;-3.04764 -107.86908 -5.51819 -110.33963 -5.51819 -113.38728 c &#10;-5.51819 -116.43492 -3.04764 -118.90547 0.0 -118.90547 c &#10;3.04764 -118.90547 5.51819 -116.43492 5.51819 -113.38728 c &#10;h &#10;0.0 -113.38728 m &#10;B &#10;Q &#10;q &#10;1 0 0 1 0 -113.386 cm&#10;1.0 0.0 0.0 1.0 0.0 0.0 cm &#10;q &#10;0 G &#10;0 g &#10;Q &#10;1 0 0 1 0 113.386 cm&#10;Q &#10;Q &#10;q &#10;1 0 0 rg &#10;q &#10;1 0 0 rg &#10;-22.82861 -113.38728 m &#10;-22.82861 -110.33963 -25.29915 -107.86908 -28.3468 -107.86908 c &#10;-31.39445 -107.86908 -33.865 -110.33963 -33.865 -113.38728 c &#10;-33.865 -116.43492 -31.39445 -118.90547 -28.3468 -118.90547 c &#10;-25.29915 -118.90547 -22.82861 -116.43492 -22.82861 -113.38728 c &#10;h &#10;-28.3468 -113.38728 m &#10;B &#10;Q &#10;q &#10;1 0 0 1 -28.347 -113.386 cm&#10;1.0 0.0 0.0 1.0 0.0 0.0 cm &#10;q &#10;0 G &#10;0 g &#10;Q &#10;1 0 0 1 28.347 113.386 cm&#10;Q &#10;Q &#10;q &#10;q &#10;1 0 0 1 -18.799 -61.667 cm&#10;1.0 0.0 0.0 1.0 0.0 0.0 cm &#10;q &#10;0 G &#10;0 g &#10;1 0 0 1 -15.265 -57.436 cm&#10;BT&#10;/F66 11.9552 Tf 15.265 57.436 Td [&#40;X&#41;]TJ&#10;ET&#10;1 0 0 1 15.265 57.436 cm&#10;Q &#10;1 0 0 1 18.799 61.667 cm&#10;Q &#10;Q &#10;q &#10;0 1 1 rg &#10;q &#10;0 1 1 rg &#10;147.2523 -113.38728 m &#10;147.2523 -110.33963 144.78175 -107.86908 141.7341 -107.86908 c &#10;138.68646 -107.86908 136.21591 -110.33963 136.21591 -113.38728 c &#10;136.21591 -116.43492 138.68646 -118.90547 141.7341 -118.90547 c &#10;144.78175 -118.90547 147.2523 -116.43492 147.2523 -113.38728 c &#10;h &#10;141.7341 -113.38728 m &#10;B &#10;Q &#10;q &#10;1 0 0 1 141.732 -113.386 cm&#10;1.0 0.0 0.0 1.0 0.0 0.0 cm &#10;q &#10;0 G &#10;0 g &#10;Q &#10;1 0 0 1 -141.732 113.386 cm&#10;Q &#10;Q &#10;q &#10;0 1 1 rg &#10;q &#10;0 1 1 rg &#10;132.07993 -13.17442 m &#10;132.07993 -10.12677 129.60938 -7.65622 126.56172 -7.65622 c &#10;123.51407 -7.65622 121.04353 -10.12677 121.04353 -13.17442 c &#10;121.04353 -16.22208 123.51407 -18.69261 126.56172 -18.69261 c &#10;129.60938 -18.69261 132.07993 -16.22208 132.07993 -13.17442 c &#10;h &#10;126.56172 -13.17442 m &#10;B &#10;Q &#10;q &#10;1 0 0 1 126.56 -13.174 cm&#10;1.0 0.0 0.0 1.0 0.0 0.0 cm &#10;q &#10;0 G &#10;0 g &#10;Q &#10;1 0 0 1 -126.56 13.174 cm&#10;Q &#10;Q &#10;q &#10;0 1 1 rg &#10;q &#10;0 1 1 rg &#10;162.42468 -13.17442 m &#10;162.42468 -10.12677 159.95413 -7.65622 156.90648 -7.65622 c &#10;153.85884 -7.65622 151.38829 -10.12677 151.38829 -13.17442 c &#10;151.38829 -16.22208 153.85884 -18.69261 156.90648 -18.69261 c &#10;159.95413 -18.69261 162.42468 -16.22208 162.42468 -13.17442 c &#10;h &#10;156.90648 -13.17442 m &#10;B &#10;Q &#10;q &#10;1 0 0 1 156.904 -13.174 cm&#10;1.0 0.0 0.0 1.0 0.0 0.0 cm &#10;q &#10;0 G &#10;0 g &#10;Q &#10;1 0 0 1 -156.904 13.174 cm&#10;Q &#10;Q &#10;q &#10;0 1 1 rg &#10;q &#10;0 1 1 rg &#10;147.2523 14.1734 m &#10;147.2523 17.22105 144.78175 19.6916 141.7341 19.6916 c &#10;138.68646 19.6916 136.21591 17.22105 136.21591 14.1734 c &#10;136.21591 11.12576 138.68646 8.65521 141.7341 8.65521 c &#10;144.78175 8.65521 147.2523 11.12576 147.2523 14.1734 c &#10;h &#10;141.7341 14.1734 m &#10;B &#10;Q &#10;q &#10;1 0 0 1 141.732 14.173 cm&#10;1.0 0.0 0.0 1.0 0.0 0.0 cm &#10;q &#10;0 G &#10;0 g &#10;Q &#10;1 0 0 1 -141.732 -14.173 cm&#10;Q &#10;Q &#10;q &#10;q &#10;1 0 0 1 138.537 -61.667 cm&#10;1.0 0.0 0.0 1.0 0.0 0.0 cm &#10;q &#10;0 G &#10;0 g &#10;1 0 0 1 -172.601 -57.436 cm&#10;BT&#10;/F66 11.9552 Tf 172.601 57.436 Td [&#40;Y&#41;]TJ&#10;ET&#10;1 0 0 1 172.601 57.436 cm&#10;Q &#10;1 0 0 1 -138.537 61.667 cm&#10;Q &#10;Q &#10;Q &#10;n &#10;Q &#10;</data>
+<data size="3956">0 g 0 G&#10;1 0 0 1 39.211 124.251 cm&#10;q &#10;0 G &#10;0 g &#10;0.3985 w &#10;q &#10;q &#10;0.86667 0.86667 0.86667 rg &#10;-39.21169 -124.25217 m &#10;-39.21169 -124.25217 m &#10;-39.21169 25.03828 l &#10;167.77136 25.03828 l &#10;167.77136 -124.25217 l &#10;h &#10;167.77136 25.03828 m &#10;f &#10;Q &#10;Q &#10;q &#10;q &#10;1 0 0 rg &#10;q &#10;1 0 0 rg &#10;5.51819 0.0 m &#10;5.51819 3.04764 3.04764 5.51819 0.0 5.51819 c &#10;-3.04764 5.51819 -5.51819 3.04764 -5.51819 0.0 c &#10;-5.51819 -3.04764 -3.04764 -5.51819 0.0 -5.51819 c &#10;3.04764 -5.51819 5.51819 -3.04764 5.51819 0.0 c &#10;h &#10;0.0 0.0 m &#10;B &#10;Q &#10;q &#10;1.0 0.0 0.0 1.0 0.0 0.0 cm &#10;q &#10;0 G &#10;0 g &#10;Q &#10;Q &#10;Q &#10;q &#10;1 0 0 rg &#10;q &#10;1 0 0 rg &#10;-22.82861 0.0 m &#10;-22.82861 3.04764 -25.29915 5.51819 -28.3468 5.51819 c &#10;-31.39445 5.51819 -33.865 3.04764 -33.865 0.0 c &#10;-33.865 -3.04764 -31.39445 -5.51819 -28.3468 -5.51819 c &#10;-25.29915 -5.51819 -22.82861 -3.04764 -22.82861 0.0 c &#10;h &#10;-28.3468 0.0 m &#10;B &#10;Q &#10;q &#10;1 0 0 1 -28.346 0 cm&#10;1.0 0.0 0.0 1.0 0.0 0.0 cm &#10;q &#10;0 G &#10;0 g &#10;Q &#10;1 0 0 1 28.346 0 cm&#10;Q &#10;Q &#10;q &#10;1 0 0 rg &#10;q &#10;1 0 0 rg &#10;5.51819 -113.38728 m &#10;5.51819 -110.33963 3.04764 -107.86908 0.0 -107.86908 c &#10;-3.04764 -107.86908 -5.51819 -110.33963 -5.51819 -113.38728 c &#10;-5.51819 -116.43492 -3.04764 -118.90547 0.0 -118.90547 c &#10;3.04764 -118.90547 5.51819 -116.43492 5.51819 -113.38728 c &#10;h &#10;0.0 -113.38728 m &#10;B &#10;Q &#10;q &#10;1 0 0 1 0 -113.386 cm&#10;1.0 0.0 0.0 1.0 0.0 0.0 cm &#10;q &#10;0 G &#10;0 g &#10;Q &#10;1 0 0 1 0 113.386 cm&#10;Q &#10;Q &#10;q &#10;1 0 0 rg &#10;q &#10;1 0 0 rg &#10;-22.82861 -113.38728 m &#10;-22.82861 -110.33963 -25.29915 -107.86908 -28.3468 -107.86908 c &#10;-31.39445 -107.86908 -33.865 -110.33963 -33.865 -113.38728 c &#10;-33.865 -116.43492 -31.39445 -118.90547 -28.3468 -118.90547 c &#10;-25.29915 -118.90547 -22.82861 -116.43492 -22.82861 -113.38728 c &#10;h &#10;-28.3468 -113.38728 m &#10;B &#10;Q &#10;q &#10;1 0 0 1 -28.346 -113.386 cm&#10;1.0 0.0 0.0 1.0 0.0 0.0 cm &#10;q &#10;0 G &#10;0 g &#10;Q &#10;1 0 0 1 28.346 113.386 cm&#10;Q &#10;Q &#10;q &#10;q &#10;1 0 0 1 -18.799 -61.668 cm&#10;1.0 0.0 0.0 1.0 0.0 0.0 cm &#10;q &#10;0 G &#10;0 g &#10;1 0 0 1 -20.412 -62.583 cm&#10;BT&#10;/F66 11.9552 Tf 20.412 62.583 Td [&#40;X&#41;]TJ&#10;ET&#10;1 0 0 1 20.412 62.583 cm&#10;Q &#10;1 0 0 1 18.799 61.668 cm&#10;Q &#10;Q &#10;q &#10;0 1 1 rg &#10;q &#10;0 1 1 rg &#10;147.2523 -113.38728 m &#10;147.2523 -110.33963 144.78175 -107.86908 141.7341 -107.86908 c &#10;138.68646 -107.86908 136.21591 -110.33963 136.21591 -113.38728 c &#10;136.21591 -116.43492 138.68646 -118.90547 141.7341 -118.90547 c &#10;144.78175 -118.90547 147.2523 -116.43492 147.2523 -113.38728 c &#10;h &#10;141.7341 -113.38728 m &#10;B &#10;Q &#10;q &#10;1 0 0 1 141.732 -113.386 cm&#10;1.0 0.0 0.0 1.0 0.0 0.0 cm &#10;q &#10;0 G &#10;0 g &#10;Q &#10;1 0 0 1 -141.732 113.386 cm&#10;Q &#10;Q &#10;q &#10;0 1 1 rg &#10;q &#10;0 1 1 rg &#10;132.07993 -13.17442 m &#10;132.07993 -10.12677 129.60938 -7.65622 126.56172 -7.65622 c &#10;123.51407 -7.65622 121.04353 -10.12677 121.04353 -13.17442 c &#10;121.04353 -16.22208 123.51407 -18.69261 126.56172 -18.69261 c &#10;129.60938 -18.69261 132.07993 -16.22208 132.07993 -13.17442 c &#10;h &#10;126.56172 -13.17442 m &#10;B &#10;Q &#10;q &#10;1 0 0 1 126.56 -13.175 cm&#10;1.0 0.0 0.0 1.0 0.0 0.0 cm &#10;q &#10;0 G &#10;0 g &#10;Q &#10;1 0 0 1 -126.56 13.175 cm&#10;Q &#10;Q &#10;q &#10;0 1 1 rg &#10;q &#10;0 1 1 rg &#10;162.42468 -13.17442 m &#10;162.42468 -10.12677 159.95413 -7.65622 156.90648 -7.65622 c &#10;153.85884 -7.65622 151.38829 -10.12677 151.38829 -13.17442 c &#10;151.38829 -16.22208 153.85884 -18.69261 156.90648 -18.69261 c &#10;159.95413 -18.69261 162.42468 -16.22208 162.42468 -13.17442 c &#10;h &#10;156.90648 -13.17442 m &#10;B &#10;Q &#10;q &#10;1 0 0 1 156.905 -13.175 cm&#10;1.0 0.0 0.0 1.0 0.0 0.0 cm &#10;q &#10;0 G &#10;0 g &#10;Q &#10;1 0 0 1 -156.905 13.175 cm&#10;Q &#10;Q &#10;q &#10;0 1 1 rg &#10;q &#10;0 1 1 rg &#10;147.2523 14.1734 m &#10;147.2523 17.22105 144.78175 19.6916 141.7341 19.6916 c &#10;138.68646 19.6916 136.21591 17.22105 136.21591 14.1734 c &#10;136.21591 11.12576 138.68646 8.65521 141.7341 8.65521 c &#10;144.78175 8.65521 147.2523 11.12576 147.2523 14.1734 c &#10;h &#10;141.7341 14.1734 m &#10;B &#10;Q &#10;q &#10;1 0 0 1 141.732 14.173 cm&#10;1.0 0.0 0.0 1.0 0.0 0.0 cm &#10;q &#10;0 G &#10;0 g &#10;Q &#10;1 0 0 1 -141.732 -14.173 cm&#10;Q &#10;Q &#10;q &#10;q &#10;1 0 0 1 138.538 -61.668 cm&#10;1.0 0.0 0.0 1.0 0.0 0.0 cm &#10;q &#10;0 G &#10;0 g &#10;1 0 0 1 -177.749 -62.583 cm&#10;BT&#10;/F66 11.9552 Tf 177.749 62.583 Td [&#40;Y&#41;]TJ&#10;ET&#10;1 0 0 1 177.749 62.583 cm&#10;Q &#10;1 0 0 1 -138.538 61.668 cm&#10;Q &#10;Q &#10;0.3985 w &#10;Q &#10;n &#10;Q &#10;</data>
 </stream>
 </object>
 
 <object id="10">
 <dict size="1">
 <key>D</key>
 <value><list size="5">
 <ref id="6" />
 <literal>XYZ</literal>
 <number>71</number>
-<number>67.994</number>
+<number>78.289</number>
 <keyword>b'null'</keyword>
 </list></value>
 </dict>
 </object>
 
 <object id="11">
 <dict size="8">
@@ -288,17 +288,17 @@
 <key>Subject</key>
 <value><string size="0"></string></value>
 <key>Creator</key>
 <value><string size="19">LaTeX with hyperref</string></value>
 <key>Keywords</key>
 <value><string size="0"></string></value>
 <key>CreationDate</key>
-<value><string size="17">D:20230510142517Z</string></value>
+<value><string size="17">D:20230519192644Z</string></value>
 <key>ModDate</key>
-<value><string size="17">D:20230510142517Z</string></value>
+<value><string size="17">D:20230519192644Z</string></value>
 <key>Trapped</key>
 <value><literal>False</literal></value>
 <key>PTEX.Fullbanner</key>
 <value><string size="86">This is pdfTeX, Version 3.141592653-2.6-1.40.24 &#40;TeX Live 2022&#41; kpathsea version 6.3.4</string></value>
 </dict>
 </object>
 
@@ -323,24 +323,24 @@
 </list></value>
 <key>Root</key>
 <value><ref id="19" /></value>
 <key>Info</key>
 <value><ref id="20" /></value>
 <key>ID</key>
 <value><list size="2">
-<string size="16">6MW&#187;oP&#29;lu]&#210;Q&#168;&#62;&#178;&#196;</string>
-<string size="16">6MW&#187;oP&#29;lu]&#210;Q&#168;&#62;&#178;&#196;</string>
+<string size="16">$&#156;sP&#135;&#150;&#143;_&#252;:&#153;&#9;&#22;;8e</string>
+<string size="16">$&#156;sP&#135;&#150;&#143;_&#252;:&#153;&#9;&#22;;8e</string>
 </list></value>
 <key>Length</key>
-<value><number>71</number></value>
+<value><number>68</number></value>
 <key>Filter</key>
 <value><literal>FlateDecode</literal></value>
 </dict>
 </props>
-<data size="88">&#0;&#0;&#7;&#255;&#2;&#0;&#5;&#4;&#2;&#0;&#5;&#5;&#2;&#0;&#5;&#6;&#2;&#0;&#5;&#0;&#1;%&#12;&#0;&#2;&#0;&#5;&#1;&#0;&#0;&#0;&#255;&#2;&#0;&#5;&#3;&#1;&#0;&#15;&#0;&#2;&#0;&#5;&#2;&#2;&#0;&#5;&#9;&#2;&#0;&#5;&#10;&#2;&#0;&#5;&#7;&#1;&#3;&#154;&#0;&#2;&#0;&#5;&#8;&#1; &#214;&#0;&#2;&#0;&#5;&#11;&#2;&#0;&#5;&#12;&#2;&#0;&#5;&#13;&#1;#&#222;&#0;&#1;&#39;&#202;&#0;</data>
+<data size="88">&#0;&#0;&#7;&#255;&#2;&#0;&#5;&#4;&#2;&#0;&#5;&#5;&#2;&#0;&#5;&#6;&#2;&#0;&#5;&#0;&#1;%D&#0;&#2;&#0;&#5;&#1;&#0;&#0;&#0;&#255;&#2;&#0;&#5;&#3;&#1;&#0;&#15;&#0;&#2;&#0;&#5;&#2;&#2;&#0;&#5;&#9;&#2;&#0;&#5;&#10;&#2;&#0;&#5;&#7;&#1;&#3;&#210;&#0;&#2;&#0;&#5;&#8;&#1;!&#14;&#0;&#2;&#0;&#5;&#11;&#2;&#0;&#5;&#12;&#2;&#0;&#5;&#13;&#1;$&#22;&#0;&#1;&#40;&#0;&#0;</data>
 </stream>
 </object>
 
 <trailer>
 <dict size="9">
 <key>Type</key>
 <value><literal>XRef</literal></value>
@@ -359,18 +359,18 @@
 </list></value>
 <key>Root</key>
 <value><ref id="19" /></value>
 <key>Info</key>
 <value><ref id="20" /></value>
 <key>ID</key>
 <value><list size="2">
-<string size="16">6MW&#187;oP&#29;lu]&#210;Q&#168;&#62;&#178;&#196;</string>
-<string size="16">6MW&#187;oP&#29;lu]&#210;Q&#168;&#62;&#178;&#196;</string>
+<string size="16">$&#156;sP&#135;&#150;&#143;_&#252;:&#153;&#9;&#22;;8e</string>
+<string size="16">$&#156;sP&#135;&#150;&#143;_&#252;:&#153;&#9;&#22;;8e</string>
 </list></value>
 <key>Length</key>
-<value><number>71</number></value>
+<value><number>68</number></value>
 <key>Filter</key>
 <value><literal>FlateDecode</literal></value>
 </dict>
 </trailer>
 
 </pdf>
```

### Comparing `dgh-0.0.8/illustration_wide.pdf` & `dgh-0.1.0/illustration_wide.pdf`

 * *Files identical despite different names*

### Comparing `dgh-0.0.8/illustration_wide_tall.pdf` & `dgh-0.1.0/illustration_wide_tall.pdf`

 * *Files identical despite different names*

### Comparing `dgh-0.0.8/dgh/fw.py` & `dgh-0.1.0/dgh/fw.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 from functools import partial
 
 from .mappings import fg_to_R
 from .spaces import arrange_distances
 
 
 def solve_frank_wolfe(obj, grad, find_descent_direction, minimize_obj_wrt_gamma, S0,
-                      tol=1e-8, max_iter=10, verbose=0):
+                      tol=1e-8, max_iter=np.inf, verbose=0):
     """
     Minimize smoothed distortion over the bi-mapping polytope 𝓢.
 
     :param obj: smoothed distortion
     :param grad: ∇obj:𝓢🠒𝓢 (function)
     :param find_descent_direction: R:ℝ^(n+m)×(n+m)🠒𝓢 (function)
     :param minimize_obj_wrt_gamma: γ*:𝓢×𝓢🠒ℝ (function)
     :param S0: starting point in 𝓢 (2d-array)
     :param tol: tolerance for measuring rate of descent (float)
-    :param max_iter: maximum number of iterations (int)
+    :param max_iter: maximum number of iterations (int or infinity)
     :param verbose: no output if ≤2, iterations if >2
     :return: solution, number of iterations performed
     """
     S = S0.copy()
     iter = 0
     while iter < max_iter:
         # Find the Frank-Wolfe direction.
@@ -32,15 +32,15 @@
         global_gamma = minimize_obj_wrt_gamma(S, D)
         critical_gammas = {0, 1}
         if 0 < global_gamma < 1:
             critical_gammas.add(global_gamma)
         gamma = min(critical_gammas, key=lambda x: obj(S + x*D))
 
         if verbose > 2:
-            print(f'  iter {iter}: obj(S)={obj(S):.4f}, γ={gamma:.5f}')
+            print(f'  iter {iter}: σ(S)={obj(S):.4f}, γ={gamma:.5f}')
 
         # Stop if the rate of descent is too small or if the line search stalls.
         if np.sum(-grad_at_S * D) < tol or np.isclose(gamma, 0):
             break
 
         # Move S by γ towards R, i.e. to (1-γ)S + γR.
         S += gamma * D
@@ -56,49 +56,48 @@
     """
     Create Frank-Wolfe solver for minimizing c-smoothed distortion over
     the bi-mapping polytope 𝓢.
 
     :param X: distance matrix of X (2d-array)
     :param Y: distance matrix of Y (2d-array)
     :param c: exponentiation base ∈ (1, ∞) for smoothing the distortion (float)
-    :param kwargs:
     :return: solver
     """
     n, m = len(X), len(Y)
 
     # Define auxiliary function that is a component in the objective and its gradient.
-    def aux_sum(S):
+    def dot_multiplicand(S):
         X__Y, Y__X, _Y_X = arrange_distances(X, Y)
         c_Y_X, c__Y_X = c**_Y_X,  c**-_Y_X
 
         return (c__Y_X @ S @ c_Y_X + c_Y_X @ S @ c__Y_X).T + \
             c**-X__Y @ S @ c**Y__X + c**X__Y @ S @ c**-Y__X
 
-    # Smooth distortion as the objective.
+    # Smooth distortion σ as the objective.
     def obj(S):
-        return np.sum(S * aux_sum(S)) - 2 * (n + m)**2  # redundant subtraction
+        return np.sum(S * dot_multiplicand(S))
 
-    # ∇obj.
+    # ∇σ.
     def grad(S):
-        return 2 * aux_sum(S)
+        return 2 * dot_multiplicand(S)
 
-    # To minimize〈R, ∇obj(S)〉over 𝓢 given S ∈ 𝓢, R must be a vertex of 𝓢.
+    # To minimize〈R, ∇σ(S)〉over 𝓢 given S ∈ 𝓢, R must be a vertex of 𝓢.
     def find_descent_direction(grad_at_S):
         f = np.argmin(grad_at_S[:n, :m], axis=1)
         g = np.argmin(grad_at_S[n:, m:], axis=1)
 
         return fg_to_R(f, g)
 
-    # To minimize obj(γ) = obj(S + γD), for line search.
+    # To minimize σ(γ) = σ(S + γD), for line search.
     def minimize_obj_wrt_gamma(S, D):
-        # Leverage that the objective is quadratic in γ, obj(γ) = aγ² + bγ + c.
-        a = np.sum(D * aux_sum(D))
-        b = np.sum(D * aux_sum(S)) + np.sum(S * aux_sum(D))
+        # Leverage that the objective is quadratic in γ, σ(γ) = aγ² + bγ + c.
+        a = np.sum(D * dot_multiplicand(D))
+        b = np.sum(D * dot_multiplicand(S)) + np.sum(S * dot_multiplicand(D))
         with np.errstate(divide='ignore', invalid='ignore'):
-            global_gamma = -b / (2*a)
+            global_gamma = np.divide(-b, 2*a)
 
         return global_gamma
 
     fw = partial(solve_frank_wolfe, obj, grad, find_descent_direction,
                  minimize_obj_wrt_gamma, **kwargs)
 
     return fw
```

### Comparing `dgh-0.0.8/dgh/mappings.py` & `dgh-0.1.0/dgh/mappings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,30 @@
 import numpy as np
 
 from .constants import DEFAULT_SEED
 
 
+def rnd_R(n, m, rnd=None):
+    """
+    Generates random vertex of bi-mapping polytope 𝓢.
+
+    :param n: cardinality of X (int)
+    :param m: cardinality of Y (int)
+    :param rnd: NumPy random state
+    :return: mapping pair R ∈ 𝓡  (2d-array)
+    """
+    rnd = rnd or np.random.RandomState(DEFAULT_SEED)
+
+    R = np.zeros(n+m, n+m)
+    R[np.arange(n), rnd.choice(m, n)] = 1
+    R[n + np.arange(m), m + rnd.choice(n, m)] = 1
+
+    return R
+
+
 def rnd_S(n, m, rnd=None):
     """
     Generates random soft mapping in X🠖Y as a point in the bi-mapping polytope 𝓢.
 
     :param n: cardinality of X (int)
     :param m: cardinality of Y (int)
     :param rnd: NumPy random state
```

### Comparing `dgh-0.0.8/dgh/spaces.py` & `dgh-0.1.0/dgh/spaces.py`

 * *Files identical despite different names*

### Comparing `dgh-0.0.8/LICENSE` & `dgh-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dgh-0.0.8/README.md` & `dgh-0.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # dGH
 
-Computes the Gromov–Hausdorff distance $$d_\text{GH}(X, Y) = \frac{1}{2}\inf_{f:X\to Y, g:Y\to X} \text{dis}\Big(\\{(x, f(x)): x \in X\\} \cup \\{(g(y), y): y \in Y\\}\Big),$$ where $\text{dis}(R) = \sup_{(x, y), (x', y') \in R} |d_X(x, x') - d_Y(y, y')|$ for $R \subseteq X \times Y,$ by solving (a parametric family of) indefinite quadratic minimizations with affine constraints, whose solutions are guaranteed to deliver $d_\text{GH}(X, Y)$ for sufficiently large value of the parameter $c$. The minimizations are solved using the Frank-Wolfe algorithm in $O(n^3)$ time per its iteration, where $n = |X| + |Y|$ is the total number of points. Even when the algorithm fails to find a global minimum, the resulting solution provides an upper bound for $d_\text{GH}(X, Y)$.
+Computes the Gromov–Hausdorff distance $$d_\text{GH}(X, Y) = \frac{1}{2}\inf_{f:X\to Y, g:Y\to X} \text{dis}\Big(\\{(x, f(x)): x \in X\\} \cup \\{(g(y), y): y \in Y\\}\Big),$$ where $\text{dis}(R) = \sup_{(x, y), (x', y') \in R} |d_X(x, x') - d_Y(y, y')|$ for $R \subseteq X \times Y,$ by solving its parametric relaxation whose solutions are guaranteed to deliver $d_\text{GH}(X, Y)$ for sufficiently large value of the parameter $c$. The quadratic relaxation with affine constraints is solved using the Frank–Wolfe algorithm in $O(n^3)$ time per its iteration, where $n = |X| + |Y|$ is the total number of points. Even when the algorithm fails to find a global minimum, the resulting solution provides an upper bound for $d_\text{GH}(X, Y)$.
 
 A manuscript describing the underlying theory is currently in preparation.
 
 ## Quickstart
 
 Installing the package from Python Package Index:
 
 ```$ pip install dgh```
 
 Computing $d_\text{GH}(X, Y)$ where $X$ is the vertices of a tall narrow rectangle and $Y$ is the vertices of a small equilateral triangle together with a remote point from it (see illustration):
 
 <p align="center">
-    <img src="https://github.com/vlad-oles/dgh/blob/main/illustration.png" alt="Illustration of the example" width="400"/>
+    <img src="https://github.com/vlad-oles/dgh/blob/main/illustration.svg" alt="Illustration of the example" width="300"/>
 </p>
 
 ```
 import numpy as np
 import dgh
 
 # Set distance matrix for the rectangle.
@@ -30,24 +30,36 @@
 # Set distance matrix for the triangle and a remote point.
 Y = np.array([[0, 1, 1, 10],
               [0, 0, 1, 10],
               [0, 0, 0, 10],
               [0, 0, 0, 0]])
 Y += Y.T
 
-# Find an upper bound of the Gromov–Hausdorff distance.
-dgh.ub(X, Y)
+# Find an upper bound of the Gromov–Hausdorff distance. In this case, dGH(X, Y) = 0.5.
+dGH = dgh.ub(X, Y)
 ```
 
-Increasing the budget of Frank-Wolfe iterations, and thus the number of restarts, allocated for the search (the default budget is 100):
+Increasing the budget of Frank–Wolfe iterations, and thus the number of restarts, allocated for the search (the default budget is 100):
 
-```d = dgh.ub(X, Y, iter_budget=1000)```
+```dGH = dgh.ub(X, Y, iter_budget=1000)```
 
 Obtaining the mappings $f:X\to Y, g:Y\to X$ (as arrays s.t. $f_i = j \Leftrightarrow f(x_i) = y_j$) that deliver the found minimum:
 
-```d, f, g = dgh.ub(X, Y, return_fg=True)```
+```dGH, f, g = dgh.ub(X, Y, return_fg=True)```
+
+## Advanced
+The performance can be improved by explicitly specifying the relaxation parameter $c \in (1, \infty)$. Small $c$ makes the relaxation easier to solve, but its solutions are more likely to deliver the Gromov–Hausdorff distance when $c$ is large.
+
+By default, the method allocates half of the iteration budget to select the best value of $c$ for $(X, Y)$ from $1+10^{-4}, 1+10^{-2},\ldots,1+10^8$, and then spends the remaining half on refining the Gromov–Hausdorff distance using this $c$. Revealing the value of $c$ selected after the search:
+
+```dgh.ub(X, Y, verbose=1)```
+
+Explicitly providing $c$ to the method (to avoid search and/or to test for better accuracy):
+
+```dGH = dgh.ub(X, Y, c=my_c)```
+
 
 ## Contributing
 If you found a bug or want to suggest an enhancement, you can create a [GitHub Issue](https://docs.github.com/en/issues/tracking-your-work-with-issues/creating-an-issue). Alternatively, you can email vlad.oles (at) proton (dot) me.
 
 ## License
 dGH is released under the MIT license.
```

### Comparing `dgh-0.0.8/pyproject.toml` & `dgh-0.1.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dgh"
-version = "0.0.8"
+version = "0.1.0"
 authors = [
   {name="Vladyslav Oles", email="vlad.oles@proton.me"},
 ]
 description = "Computing the Gromov–Hausdorff distance"
 readme = "README.md"
-requires-python = ">=3.5"
+requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `dgh-0.0.8/PKG-INFO` & `dgh-0.1.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: dgh
-Version: 0.0.8
+Version: 0.1.0
 Summary: Computing the Gromov–Hausdorff distance
 Project-URL: Homepage, https://github.com/vlad-oles/dgh
 Project-URL: Bug Tracker, https://github.com/vlad-oles/dgh/issues
 Author-email: Vladyslav Oles <vlad.oles@proton.me>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.5
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # dGH
 
-Computes the Gromov–Hausdorff distance $$d_\text{GH}(X, Y) = \frac{1}{2}\inf_{f:X\to Y, g:Y\to X} \text{dis}\Big(\\{(x, f(x)): x \in X\\} \cup \\{(g(y), y): y \in Y\\}\Big),$$ where $\text{dis}(R) = \sup_{(x, y), (x', y') \in R} |d_X(x, x') - d_Y(y, y')|$ for $R \subseteq X \times Y,$ by solving (a parametric family of) indefinite quadratic minimizations with affine constraints, whose solutions are guaranteed to deliver $d_\text{GH}(X, Y)$ for sufficiently large value of the parameter $c$. The minimizations are solved using the Frank-Wolfe algorithm in $O(n^3)$ time per its iteration, where $n = |X| + |Y|$ is the total number of points. Even when the algorithm fails to find a global minimum, the resulting solution provides an upper bound for $d_\text{GH}(X, Y)$.
+Computes the Gromov–Hausdorff distance $$d_\text{GH}(X, Y) = \frac{1}{2}\inf_{f:X\to Y, g:Y\to X} \text{dis}\Big(\\{(x, f(x)): x \in X\\} \cup \\{(g(y), y): y \in Y\\}\Big),$$ where $\text{dis}(R) = \sup_{(x, y), (x', y') \in R} |d_X(x, x') - d_Y(y, y')|$ for $R \subseteq X \times Y,$ by solving its parametric relaxation whose solutions are guaranteed to deliver $d_\text{GH}(X, Y)$ for sufficiently large value of the parameter $c$. The quadratic relaxation with affine constraints is solved using the Frank–Wolfe algorithm in $O(n^3)$ time per its iteration, where $n = |X| + |Y|$ is the total number of points. Even when the algorithm fails to find a global minimum, the resulting solution provides an upper bound for $d_\text{GH}(X, Y)$.
 
 A manuscript describing the underlying theory is currently in preparation.
 
 ## Quickstart
 
 Installing the package from Python Package Index:
 
 ```$ pip install dgh```
 
 Computing $d_\text{GH}(X, Y)$ where $X$ is the vertices of a tall narrow rectangle and $Y$ is the vertices of a small equilateral triangle together with a remote point from it (see illustration):
 
 <p align="center">
-    <img src="https://github.com/vlad-oles/dgh/blob/main/illustration.png" alt="Illustration of the example" width="400"/>
+    <img src="https://github.com/vlad-oles/dgh/blob/main/illustration.svg" alt="Illustration of the example" width="300"/>
 </p>
 
 ```
 import numpy as np
 import dgh
 
 # Set distance matrix for the rectangle.
@@ -44,24 +44,36 @@
 # Set distance matrix for the triangle and a remote point.
 Y = np.array([[0, 1, 1, 10],
               [0, 0, 1, 10],
               [0, 0, 0, 10],
               [0, 0, 0, 0]])
 Y += Y.T
 
-# Find an upper bound of the Gromov–Hausdorff distance.
-dgh.ub(X, Y)
+# Find an upper bound of the Gromov–Hausdorff distance. In this case, dGH(X, Y) = 0.5.
+dGH = dgh.ub(X, Y)
 ```
 
-Increasing the budget of Frank-Wolfe iterations, and thus the number of restarts, allocated for the search (the default budget is 100):
+Increasing the budget of Frank–Wolfe iterations, and thus the number of restarts, allocated for the search (the default budget is 100):
 
-```d = dgh.ub(X, Y, iter_budget=1000)```
+```dGH = dgh.ub(X, Y, iter_budget=1000)```
 
 Obtaining the mappings $f:X\to Y, g:Y\to X$ (as arrays s.t. $f_i = j \Leftrightarrow f(x_i) = y_j$) that deliver the found minimum:
 
-```d, f, g = dgh.ub(X, Y, return_fg=True)```
+```dGH, f, g = dgh.ub(X, Y, return_fg=True)```
+
+## Advanced
+The performance can be improved by explicitly specifying the relaxation parameter $c \in (1, \infty)$. Small $c$ makes the relaxation easier to solve, but its solutions are more likely to deliver the Gromov–Hausdorff distance when $c$ is large.
+
+By default, the method allocates half of the iteration budget to select the best value of $c$ for $(X, Y)$ from $1+10^{-4}, 1+10^{-2},\ldots,1+10^8$, and then spends the remaining half on refining the Gromov–Hausdorff distance using this $c$. Revealing the value of $c$ selected after the search:
+
+```dgh.ub(X, Y, verbose=1)```
+
+Explicitly providing $c$ to the method (to avoid search and/or to test for better accuracy):
+
+```dGH = dgh.ub(X, Y, c=my_c)```
+
 
 ## Contributing
 If you found a bug or want to suggest an enhancement, you can create a [GitHub Issue](https://docs.github.com/en/issues/tracking-your-work-with-issues/creating-an-issue). Alternatively, you can email vlad.oles (at) proton (dot) me.
 
 ## License
 dGH is released under the MIT license.
```

