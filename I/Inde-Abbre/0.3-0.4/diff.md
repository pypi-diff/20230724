# Comparing `tmp/Inde_Abbre-0.3-py3-none-any.whl.zip` & `tmp/Inde_Abbre-0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 7607 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat     1456 b- defN 23-Jul-17 05:43 Inde_Abbre/__init__.py
+Zip file size: 7608 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat     1469 b- defN 23-Jul-24 12:24 Inde_Abbre/__init__.py
 -rw-rw-rw-  2.0 fat    12822 b- defN 23-Jul-05 13:11 Inde_Abbre/output_2.json
--rw-rw-rw-  2.0 fat     1094 b- defN 23-Jul-17 07:26 Inde_Abbre-0.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      940 b- defN 23-Jul-17 07:26 Inde_Abbre-0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-17 07:26 Inde_Abbre-0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Jul-17 07:26 Inde_Abbre-0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      551 b- defN 23-Jul-17 07:26 Inde_Abbre-0.3.dist-info/RECORD
-7 files, 16966 bytes uncompressed, 6633 bytes compressed:  60.9%
+-rw-rw-rw-  2.0 fat     1094 b- defN 23-Jul-24 12:27 Inde_Abbre-0.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      940 b- defN 23-Jul-24 12:27 Inde_Abbre-0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-24 12:27 Inde_Abbre-0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Jul-24 12:27 Inde_Abbre-0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      551 b- defN 23-Jul-24 12:27 Inde_Abbre-0.4.dist-info/RECORD
+7 files, 16979 bytes uncompressed, 6634 bytes compressed:  60.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: Inde_Abbre/__init__.py
 Comment: 
 
 Filename: Inde_Abbre/output_2.json
 Comment: 
 
-Filename: Inde_Abbre-0.3.dist-info/LICENSE
+Filename: Inde_Abbre-0.4.dist-info/LICENSE
 Comment: 
 
-Filename: Inde_Abbre-0.3.dist-info/METADATA
+Filename: Inde_Abbre-0.4.dist-info/METADATA
 Comment: 
 
-Filename: Inde_Abbre-0.3.dist-info/WHEEL
+Filename: Inde_Abbre-0.4.dist-info/WHEEL
 Comment: 
 
-Filename: Inde_Abbre-0.3.dist-info/top_level.txt
+Filename: Inde_Abbre-0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: Inde_Abbre-0.3.dist-info/RECORD
+Filename: Inde_Abbre-0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Inde_Abbre/__init__.py

```diff
@@ -14,25 +14,24 @@
 #     abb_dict[j['Unnamed: 0']] = j['List of Abbreviations ']
 
 # now save your dict to JSON
 # with open("output_2.json", 'w') as fp:
 #     json.dump(abb_dict, fp)
 
 # now sload the same json as use it
-
 try:
     
     def Abbreviation(arr):
         """The passing argument should be given in string characters within quotes
         Abbreviation: "lic"
         will give an output of list Life Insurance of corporation
         """
         # package_dir = os.path.dirname(os.path.abspath('Inde_Abbre\\'))
         # file_path = os.path.join(package_dir, "output_2.json")
-        file_path = pkg_resources.resource_filename(__name__, 'output_2.json')
+        file_path = pkg_resources.resource_filename('Inde_Abbre.Inde_Abbre', 'output_2.json')
         with open(file_path) as jfile:
             loaded_dict = json.load(jfile)
             arr1=arr.lower().strip()
             emty_list=[]
             for i,j in loaded_dict.items():
                 if i==arr1:
                     emty_list.append(j)
```

## Comparing `Inde_Abbre-0.3.dist-info/LICENSE` & `Inde_Abbre-0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `Inde_Abbre-0.3.dist-info/METADATA` & `Inde_Abbre-0.4.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Inde-Abbre
-Version: 0.3
+Version: 0.4
 Summary: A Library that is used to retrieve the INDIAN Abbreviations
 Home-page: UNKNOWN
 Author: Richard Alphone
 Author-email: richardriche96@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

