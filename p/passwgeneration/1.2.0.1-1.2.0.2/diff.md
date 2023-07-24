# Comparing `tmp/passwgeneration-1.2.0.1-py3-none-any.whl.zip` & `tmp/passwgeneration-1.2.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 4224 bytes, number of entries: 10
+Zip file size: 4225 bytes, number of entries: 10
 -rw-rw-r--  2.0 unx       67 b- defN 23-Jul-19 05:17 package/__init__.py
 -rw-rw-r--  2.0 unx     1118 b- defN 23-Jul-19 05:07 package/generate_password.py
 -rw-rw-r--  2.0 unx     1086 b- defN 23-Jul-17 08:02 packan/__init__.py
 -rw-rw-r--  2.0 unx       66 b- defN 23-Jul-19 05:32 passwgeneration/__init__.py
 -rw-rw-r--  2.0 unx     1616 b- defN 23-Jul-24 11:08 passwgeneration/generate_password.py
 -rw-rw-r--  2.0 unx      854 b- defN 23-Jul-20 09:51 passwgeneration/test_passw.py
--rw-rw-r--  2.0 unx      736 b- defN 23-Jul-24 11:12 passwgeneration-1.2.0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-24 11:12 passwgeneration-1.2.0.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       16 b- defN 23-Jul-24 11:12 passwgeneration-1.2.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      831 b- defN 23-Jul-24 11:12 passwgeneration-1.2.0.1.dist-info/RECORD
-10 files, 6482 bytes uncompressed, 2792 bytes compressed:  56.9%
+-rw-rw-r--  2.0 unx      736 b- defN 23-Jul-24 17:41 passwgeneration-1.2.0.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-24 17:41 passwgeneration-1.2.0.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       16 b- defN 23-Jul-24 17:41 passwgeneration-1.2.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      831 b- defN 23-Jul-24 17:41 passwgeneration-1.2.0.2.dist-info/RECORD
+10 files, 6482 bytes uncompressed, 2793 bytes compressed:  56.9%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: passwgeneration/generate_password.py
 Comment: 
 
 Filename: passwgeneration/test_passw.py
 Comment: 
 
-Filename: passwgeneration-1.2.0.1.dist-info/METADATA
+Filename: passwgeneration-1.2.0.2.dist-info/METADATA
 Comment: 
 
-Filename: passwgeneration-1.2.0.1.dist-info/WHEEL
+Filename: passwgeneration-1.2.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: passwgeneration-1.2.0.1.dist-info/top_level.txt
+Filename: passwgeneration-1.2.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: passwgeneration-1.2.0.1.dist-info/RECORD
+Filename: passwgeneration-1.2.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `passwgeneration-1.2.0.1.dist-info/METADATA` & `passwgeneration-1.2.0.2.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: passwgeneration
-Version: 1.2.0.1
+Version: 1.2.0.2
 Summary: Python package to generate random passwords of maximum length 12, avoiding names present in specified files.
 Home-page: https://github.com/kanchann23/genUniquePassw
 Author: kanchan
 Author-email: kanchanbora321@gmail.com
 License: MIT
 Keywords: security,password
 Classifier: Development Status :: 5 - Production/Stable
```

## Comparing `passwgeneration-1.2.0.1.dist-info/RECORD` & `passwgeneration-1.2.0.2.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 package/__init__.py,sha256=vc7ytYfEglbNbgRsavY3Fe5foReTO3wh56sRNjcuhc8,67
 package/generate_password.py,sha256=RSKaMTLLoJ1EIRu-93R9qci0apZHysei9PryYaZ4VZ8,1118
 packan/__init__.py,sha256=hZNBvDsiMZ1td5s61ZdkHy-no5B4E3loyNAqFldOiH4,1086
 passwgeneration/__init__.py,sha256=65hh4rKClkH48KbDjFuCFRUIbnJwHn9QjXZzlpoGCSk,66
 passwgeneration/generate_password.py,sha256=BxWJcQzaeoj-LhdZMz1WymwXR7ilaJ1CbsAqCcG1JD4,1616
 passwgeneration/test_passw.py,sha256=xSs8lvQroI09gu2Hzg1j5TPYtenOgspvQwSbaaCT-g0,854
-passwgeneration-1.2.0.1.dist-info/METADATA,sha256=m660HhYguVDBRnKrjXl_rD64bz8eanLeiN1dRs1ifIE,736
-passwgeneration-1.2.0.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-passwgeneration-1.2.0.1.dist-info/top_level.txt,sha256=8EZOdUTGPPD740cZZNDDDz72N1HK10qFfFDAVnRy_tY,16
-passwgeneration-1.2.0.1.dist-info/RECORD,,
+passwgeneration-1.2.0.2.dist-info/METADATA,sha256=vukVJZnh63xwl7BP4z0HrCOM4ieM226Tna-hBnj6lg0,736
+passwgeneration-1.2.0.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+passwgeneration-1.2.0.2.dist-info/top_level.txt,sha256=8EZOdUTGPPD740cZZNDDDz72N1HK10qFfFDAVnRy_tY,16
+passwgeneration-1.2.0.2.dist-info/RECORD,,
```

