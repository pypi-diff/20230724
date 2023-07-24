# Comparing `tmp/deklinacija-1.6.1.tar.gz` & `tmp/deklinacija-1.7.0.tar.gz`

## Comparing `deklinacija-1.6.1.tar` & `deklinacija-1.7.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 deklinacija-1.6.1/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 deklinacija-1.6.1/deklinacija/__init__.py
--rw-r--r--   0        0        0    30068 2020-02-02 00:00:00.000000 deklinacija-1.6.1/deklinacija/main.py
--rw-r--r--   0        0        0     6626 2020-02-02 00:00:00.000000 deklinacija-1.6.1/deklinacija/utils.py
--rw-r--r--   0        0        0     5986 2020-02-02 00:00:00.000000 deklinacija-1.6.1/deklinacija/vokativ_database.csv
--rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 deklinacija-1.6.1/tests/names_female.txt
--rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 deklinacija-1.6.1/tests/names_female_posessive.txt
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 deklinacija-1.6.1/tests/names_male.txt
--rw-r--r--   0        0        0     5378 2020-02-02 00:00:00.000000 deklinacija-1.6.1/tests/names_male_posessive.txt
--rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 deklinacija-1.6.1/tests/test_names.py
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 deklinacija-1.6.1/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 deklinacija-1.6.1/LICENSE
--rw-r--r--   0        0        0     6283 2020-02-02 00:00:00.000000 deklinacija-1.6.1/README.md
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 deklinacija-1.6.1/pyproject.toml
--rw-r--r--   0        0        0     6720 2020-02-02 00:00:00.000000 deklinacija-1.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 deklinacija-1.7.0/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 deklinacija-1.7.0/deklinacija/__init__.py
+-rw-r--r--   0        0        0    23516 2020-02-02 00:00:00.000000 deklinacija-1.7.0/deklinacija/main.py
+-rw-r--r--   0        0        0     8223 2020-02-02 00:00:00.000000 deklinacija-1.7.0/deklinacija/utils.py
+-rw-r--r--   0        0        0     5986 2020-02-02 00:00:00.000000 deklinacija-1.7.0/deklinacija/vokativ_database.csv
+-rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 deklinacija-1.7.0/tests/names_female.txt
+-rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 deklinacija-1.7.0/tests/names_female_posessive.txt
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 deklinacija-1.7.0/tests/names_male.txt
+-rw-r--r--   0        0        0     5378 2020-02-02 00:00:00.000000 deklinacija-1.7.0/tests/names_male_posessive.txt
+-rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 deklinacija-1.7.0/tests/test_names.py
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 deklinacija-1.7.0/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 deklinacija-1.7.0/LICENSE
+-rw-r--r--   0        0        0     6111 2020-02-02 00:00:00.000000 deklinacija-1.7.0/README.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 deklinacija-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0     6550 2020-02-02 00:00:00.000000 deklinacija-1.7.0/PKG-INFO
```

### Comparing `deklinacija-1.6.1/.github/workflows/python-package.yml` & `deklinacija-1.7.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `deklinacija-1.6.1/deklinacija/vokativ_database.csv` & `deklinacija-1.7.0/deklinacija/vokativ_database.csv`

 * *Files identical despite different names*

### Comparing `deklinacija-1.6.1/tests/names_female.txt` & `deklinacija-1.7.0/tests/names_female.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 {'nominativ': 'Jana', 'genitiv': 'Jane', 'dativ': 'Jani', 'akuzativ': 'Janu', 'vokativ': 'Jano', 'instrumental': 'Janom', 'lokativ': 'Jani'}
 {'nominativ': 'Milica', 'genitiv': 'Milice', 'dativ': 'Milici', 'akuzativ': 'Milicu', 'vokativ': 'Milice', 'instrumental': 'Milicom', 'lokativ': 'Milici'}
-{'nominativ': 'Mia', 'genitiv': 'Mije', 'dativ': 'Miji', 'akuzativ': 'Miju', 'vokativ': 'Mia', 'instrumental': 'Mijom', 'lokativ': 'Miji'}
+{'nominativ': 'Mia', 'genitiv': 'Mie', 'dativ': 'Miji', 'akuzativ': 'Miu', 'vokativ': 'Mia', 'instrumental': 'Mijom', 'lokativ': 'Miji'}
 {'nominativ': 'Ines', 'genitiv': 'Ines', 'dativ': 'Ines', 'akuzativ': 'Ines', 'vokativ': 'Ines', 'instrumental': 'Ines', 'lokativ': 'Ines'}
 {'nominativ': 'Tea', 'genitiv': 'Tee', 'dativ': 'Tei', 'akuzativ': 'Teu', 'vokativ': 'Tea', 'instrumental': 'Teom', 'lokativ': 'Tei'}
 {'nominativ': 'Ina', 'genitiv': 'Ine', 'dativ': 'Ini', 'akuzativ': 'Inu', 'vokativ': 'Ina', 'instrumental': 'Inom', 'lokativ': 'Ini'}
 {'nominativ': 'Petrović', 'genitiv': 'Petrović', 'dativ': 'Petrović', 'akuzativ': 'Petrović', 'vokativ': 'Petrović', 'instrumental': 'Petrović', 'lokativ': 'Petrović'}
 {'nominativ': 'Daria', 'genitiv': 'Darije', 'dativ': 'Dariji', 'akuzativ': 'Dariju', 'vokativ': 'Daria', 'instrumental': 'Darijom', 'lokativ': 'Dariji'}
-{'nominativ': 'Anžujska', 'genitiv': 'Anžujske', 'dativ': 'Anžujskoj', 'akuzativ': 'Anžujsku', 'vokativ': 'Anžujska', 'instrumental': 'Anžujskom', 'lokativ': 'Anžujskoj'}
 {'nominativ': 'Subotički', 'genitiv': 'Subotički', 'dativ': 'Subotički', 'akuzativ': 'Subotički', 'vokativ': 'Subotički', 'instrumental': 'Subotički', 'lokativ': 'Subotički'}
-{'nominativ': 'Petka', 'genitiv': 'Petke', 'dativ': 'Petkoj', 'akuzativ': 'Petku', 'vokativ': 'Petko', 'instrumental': 'Petkom', 'lokativ': 'Petkoj'}
 {'nominativ': 'Lana Petrović', 'genitiv': 'Lane Petrović', 'dativ': 'Lani Petrović', 'akuzativ': 'Lanu Petrović', 'vokativ': 'Lano Petrović', 'instrumental': 'Lanom Petrović', 'lokativ': 'Lani Petrović'}
 {'nominativ': 'Sandra Anžujska', 'genitiv': 'Sandre Anžujske', 'dativ': 'Sandri Anžujskoj', 'akuzativ': 'Sandru Anžujsku', 'vokativ': 'Sandra Anžujska', 'instrumental': 'Sandrom Anžujskom', 'lokativ': 'Sandri Anžujskoj'}
 {'nominativ': 'Milica Tabova', 'genitiv': 'Milice Tabove', 'dativ': 'Milici Tabovoj', 'akuzativ': 'Milicu Tabovu', 'vokativ': 'Milice Tabova', 'instrumental': 'Milicom Tabovom', 'lokativ': 'Milici Tabovoj'}
 {'nominativ': 'Milica Releva', 'genitiv': 'Milice Releve', 'dativ': 'Milici Relevoj', 'akuzativ': 'Milicu Relevu', 'vokativ': 'Milice Releva', 'instrumental': 'Milicom Relevom', 'lokativ': 'Milici Relevoj'}
 {'nominativ': 'Ivana', 'genitiv': 'Ivane', 'dativ': 'Ivani', 'akuzativ': 'Ivanu', 'vokativ': 'Ivana', 'instrumental': 'Ivanom', 'lokativ': 'Ivani'}
 {'nominativ': 'IVANA', 'genitiv': 'IVANE', 'dativ': 'IVANI', 'akuzativ': 'IVANU', 'vokativ': 'IVANA', 'instrumental': 'IVANOM', 'lokativ': 'IVANI'}
 {'nominativ': 'STRUJA', 'genitiv': 'STRUJE', 'dativ': 'STRUJI', 'akuzativ': 'STRUJU', 'vokativ': 'STRUJO', 'instrumental': 'STRUJOM', 'lokativ': 'STRUJI'}
```

### Comparing `deklinacija-1.6.1/tests/names_female_posessive.txt` & `deklinacija-1.7.0/tests/names_female_posessive.txt`

 * *Files identical despite different names*

### Comparing `deklinacija-1.6.1/tests/names_male.txt` & `deklinacija-1.7.0/tests/names_male.txt`

 * *Files identical despite different names*

### Comparing `deklinacija-1.6.1/tests/names_male_posessive.txt` & `deklinacija-1.7.0/tests/names_male_posessive.txt`

 * *Files identical despite different names*

### Comparing `deklinacija-1.6.1/tests/test_names.py` & `deklinacija-1.7.0/tests/test_names.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,37 +26,37 @@
     read_content_female_p = fileFP.readlines()
 
 def testMaleNames():
     n = 0
     for i in read_content_male:
         nameDict = ast.literal_eval(read_content_male[n].strip())
         name = nameDict['nominativ']
-        compare = dek.declineAll(name,"male")
+        compare = dek.declineAll(name,dek.Gender.MALE)
         assert compare == nameDict
         n += 1
 
 def testFemaleNames():
     n = 0
     for i in read_content_female:
         nameDict = ast.literal_eval(read_content_female[n].strip())
         name = nameDict['nominativ']
-        compare = dek.declineAll(name,"female")
+        compare = dek.declineAll(name,dek.Gender.FEMALE)
         assert compare == nameDict
         n += 1
 
 def testPosessiveMaleNames():
     n = 0
     for i in read_content_male_p:
         nameDict = ast.literal_eval(read_content_male_p[n].strip())
         name = nameDict['name']
-        compare = dek.posessiveAll(name,"male")
+        compare = dek.posessiveAll(name,dek.Gender.MALE)
         assert compare == nameDict
         n += 1
 
 def testPosessiveFemaleNames():
     n = 0
     for i in read_content_female_p:
         nameDict = ast.literal_eval(read_content_female_p[n].strip())
         name = nameDict['name']
-        compare = dek.posessiveAll(name,"female")
+        compare = dek.posessiveAll(name,dek.Gender.FEMALE)
         assert compare == nameDict
         n += 1
```

### Comparing `deklinacija-1.6.1/.gitignore` & `deklinacija-1.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `deklinacija-1.6.1/LICENSE` & `deklinacija-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deklinacija-1.6.1/README.md` & `deklinacija-1.7.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -5,81 +5,79 @@
 The source code is currently hosted on GitHub: [https://github.com/urelja/deklinacija](https://github.com/urelja/deklinacija)
 
 The latest binary versions are hosted on the Python Package Index (PyPI): [https://pypi.org/project/deklinacija/](https://pypi.org/project/deklinacija/)
 ```properties
 pip install deklinacija
 ```
 ## Usage
-Simply `import` the package. It is recommended to set the alias to `dek`.
+Simply `import` the package and the `Gender` and `Number` enums. It is recommended to set the alias to `dek`.
 
 ```python
 import deklinacija as dek
+from deklinacija import Gender, Number
 ```
 To decline names, all you have to do is to call the appropriate function for the grammatical case you want to use, and specify the `name` and the `gender` parameter. The name parameter must be a `string`, can have either Latin or Cyrillic characters (automatically detected), and can contain uppercase or lowercase letters (the script respects the capitalisation of the name and will capitalise the added suffixes according to the last character's capitalisation, see `vokativ2` below). You can also input a full name (with a first name and a last name, multiple last names are supported too, separated with a whitespace character) and the script will change the name accordingly. 
 
 The functions in this example return a `string`.
 ```python
 import deklinacija as dek
+from deklinacija import Gender, Number
 
-genitiv = dek.genitiv("Velja","male") #Velje
-genitiv2 = dek.genitiv("Velja Petrović","male") #Velje Petrovića
-dativ = dek.dativ("Jana","female") #Jani
-dativ2 = dek.dativ("Jana Paunovska","female") #Jani Paunovskoj
-akuzativ = dek.akuzativ("Петар","male") #Петра
-akuzativ2 = dek.akuzativ("Петар Петровић","male") #Петра Петровића
-vokativ = dek.vokativ("Predrag","male") #Predraže
-vokativ2 = dek.vokativ("PREDRAG JANKOVIĆ","male") #PREDRAŽE JANKOVIĆU
-instrumental = dek.instrumental("Uroš","male") #Urošem
-instrumental2 = dek.instrumental("Uroš Konstantinović","male") #Urošem Konstantinovićem
-lokativ = dek.lokativ("Lana","female") #Lani
-lokativ = dek.lokativ("Lana Petrović","female") #Lani Petrović
+genitiv = dek.genitiv("Velja",Gender.MALE) #Velje
+vokativ = dek.vokativ("Predrag",Gender.MALE) #Predraže
+vokativ2 = dek.vokativ("PREDRAG JANKOVIĆ",Gender.MALE) #PREDRAŽE JANKOVIĆU
+instrumental = dek.instrumental("Uroš",Gender.MALE) #Urošem
+lokativ = dek.lokativ("Lana Petrović",Gender.FEMALE) #Lani Petrović
 
-print(f"Zdravo, {vokativ}! Dobio si zahtev za prijateljstvo od {genitiv2}.") 
-#Zdravo Predraže! Dobio si zahtev za prijateljstvo od Velje Petrovića. // Translation: Hello Predrag! You have received a friend request from Velja Petrović.
+print(f"Zdravo, {vokativ}! Dobio si zahtev za prijateljstvo od {genitiv}.") 
+#Zdravo Predraže! Dobio si zahtev za prijateljstvo od Velje. // Translation: Hello Predrag! You have received a friend request from Velja.
 ```
 
 You can also immediatelly decline a name through all grammatical cases by calling the `declineAll()` function.
 
 The `declineAll()` function returns a `dictionary`, where the keys are the grammatical cases.
 
 ```python
 import deklinacija as dek
+from deklinacija import Gender, Number
 
-name = dek.declineAll("Nikola","male") 
+name = dek.declineAll("Nikola",Gender.MALE) 
 #{'nominativ': 'Nikola', 'genitiv': 'Nikole', 'dativ': 'Nikoli', 'akuzativ': 'Nikolu', 
 #'vokativ':'Nikola', 'instrumental': 'Nikolom', 'lokativ': 'Nikoli'}
 
 print("Dali ste poklon",name['dativ']) 
 #Dali ste poklon Nikoli // Translation: You have given a gift to Nikola
 ```
 
 ## Posessive Forms
-As of version 1.6 there is a new feature: posessive forms. Aside from the name and the gender of the person, you also have to specify the gender of the posessed object and its grammatical number. In case the gender of the posessed object is unknown, you can just pass the object itself to the `object_gender` parameter and the program will figure out which gender it is, provided that the `grammatical_number` is set correctly (default value is "singular").
+As of version 1.6 there is a new feature: posessive forms. Aside from the name and the gender of the person, you also have to specify the gender of the posessed object and its grammatical number. In case the gender of the posessed object is unknown, you can just pass the object itself to the `object_gender` parameter and the program will figure out which gender it is, provided that the `grammatical_number` is set correctly (default value is Number.SINGULAR).
 
 The functions in this example return a `string`.
 ```python
 import deklinacija as dek
+from deklinacija import Gender, Number
 
-name = dek.posessive(name = "Stefan", gender = "male", object_gender = "female", grammatical_number = "singular")
-name2 = dek.posessive(name = "Stefan", gender = "male", object_gender = "grupa") #passing the object "group" instead of "female", default grammatical_number value is "singular" so it's not required to specify it in this case
-name3 = dek.posessive(name = "Stefan", gender = "male", object_gender = "slušalice", grammatical_number = "plural") #passing the object "headphones"
+name = dek.posessive(name = "Stefan", gender = Gender.MALE, object_gender = Gender.FEMALE, grammatical_number = Number.SINGULAR)
+name2 = dek.posessive(name = "Stefan", gender = Gender.MALE, object_gender = "grupa") #passing the object "group" instead of Gender.FEMALE, default grammatical_number value is Number.SINGULAR so it's not required to specify it in this case
+name3 = dek.posessive(name = "Stefan", gender = Gender.MALE, object_gender = "slušalice", grammatical_number = Number.PLURAL) #passing the object "headphones"
 
 print(name,"grupa") #Stefanova grupa // Translation: Stefan's group
 print(name2,"grupa") #Stefanova grupa
 print(name3,"slušalice") #Stefanove slušalice // Translation: Stefan's headphones
 ```
 
 You can also immediately transform the name through all possible posessive forms (male, female, neutral in singular and plural) by calling the `posessiveAll()` function. Only the `name` and `gender` parameters are required.
 
 The `posessiveAll()` function returns a `dictionary` where the keys are in the "GENDER_NUMBER" format.
 
 ```python
 import deklinacija as dek
+from deklinacija import Gender, Number
 
-name = dek.posessiveAll("Stefan","male") #{'name': 'Stefan', 'male_singular': 'Stefanov', 'male_plural': 'Stefanovi', 'female_singular': 'Stefanova', 'female_plural': 'Stefanove', 'neutral_singular': 'Stefanovo', 'neutral_plural': 'Stefanova'}
+name = dek.posessiveAll("Stefan",Gender.MALE) #{'name': 'Stefan', 'male_singular': 'Stefanov', 'male_plural': 'Stefanovi', 'female_singular': 'Stefanova', 'female_plural': 'Stefanove', 'neutral_singular': 'Stefanovo', 'neutral_plural': 'Stefanova'}
 
 print(name['male_plural'],"prijatelji") #Stefanovi prijatelji // Translation: Stefan's friends
 ```
 ## Other tools
 This library makes extensive use of a few internal utilities that one may find useful when working with the Serbian language. These include:
 
 `toLatin(word)`, `toCyrillic(word)`: Converts input string from Latin into Cyrillic and vice versa. Works with Serbian Latin letter pairs (lj, nj, dž, etc.)
```

### Comparing `deklinacija-1.6.1/pyproject.toml` & `deklinacija-1.7.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "deklinacija"
-version = "1.6.1"
+version = "1.7.0"
 authors = [
   { name="urelja", email="code.relja@gmail.com" },
 ]
 description = "A Python library for declension of personal names in Serbian"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `deklinacija-1.6.1/PKG-INFO` & `deklinacija-1.7.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deklinacija
-Version: 1.6.1
+Version: 1.7.0
 Summary: A Python library for declension of personal names in Serbian
 Project-URL: Homepage, https://github.com/urelja/deklinacija
 Project-URL: Bug Tracker, https://github.com/urelja/deklinacija/issues
 Author-email: urelja <code.relja@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,81 +19,79 @@
 The source code is currently hosted on GitHub: [https://github.com/urelja/deklinacija](https://github.com/urelja/deklinacija)
 
 The latest binary versions are hosted on the Python Package Index (PyPI): [https://pypi.org/project/deklinacija/](https://pypi.org/project/deklinacija/)
 ```properties
 pip install deklinacija
 ```
 ## Usage
-Simply `import` the package. It is recommended to set the alias to `dek`.
+Simply `import` the package and the `Gender` and `Number` enums. It is recommended to set the alias to `dek`.
 
 ```python
 import deklinacija as dek
+from deklinacija import Gender, Number
 ```
 To decline names, all you have to do is to call the appropriate function for the grammatical case you want to use, and specify the `name` and the `gender` parameter. The name parameter must be a `string`, can have either Latin or Cyrillic characters (automatically detected), and can contain uppercase or lowercase letters (the script respects the capitalisation of the name and will capitalise the added suffixes according to the last character's capitalisation, see `vokativ2` below). You can also input a full name (with a first name and a last name, multiple last names are supported too, separated with a whitespace character) and the script will change the name accordingly. 
 
 The functions in this example return a `string`.
 ```python
 import deklinacija as dek
+from deklinacija import Gender, Number
 
-genitiv = dek.genitiv("Velja","male") #Velje
-genitiv2 = dek.genitiv("Velja Petrović","male") #Velje Petrovića
-dativ = dek.dativ("Jana","female") #Jani
-dativ2 = dek.dativ("Jana Paunovska","female") #Jani Paunovskoj
-akuzativ = dek.akuzativ("Петар","male") #Петра
-akuzativ2 = dek.akuzativ("Петар Петровић","male") #Петра Петровића
-vokativ = dek.vokativ("Predrag","male") #Predraže
-vokativ2 = dek.vokativ("PREDRAG JANKOVIĆ","male") #PREDRAŽE JANKOVIĆU
-instrumental = dek.instrumental("Uroš","male") #Urošem
-instrumental2 = dek.instrumental("Uroš Konstantinović","male") #Urošem Konstantinovićem
-lokativ = dek.lokativ("Lana","female") #Lani
-lokativ = dek.lokativ("Lana Petrović","female") #Lani Petrović
+genitiv = dek.genitiv("Velja",Gender.MALE) #Velje
+vokativ = dek.vokativ("Predrag",Gender.MALE) #Predraže
+vokativ2 = dek.vokativ("PREDRAG JANKOVIĆ",Gender.MALE) #PREDRAŽE JANKOVIĆU
+instrumental = dek.instrumental("Uroš",Gender.MALE) #Urošem
+lokativ = dek.lokativ("Lana Petrović",Gender.FEMALE) #Lani Petrović
 
-print(f"Zdravo, {vokativ}! Dobio si zahtev za prijateljstvo od {genitiv2}.") 
-#Zdravo Predraže! Dobio si zahtev za prijateljstvo od Velje Petrovića. // Translation: Hello Predrag! You have received a friend request from Velja Petrović.
+print(f"Zdravo, {vokativ}! Dobio si zahtev za prijateljstvo od {genitiv}.") 
+#Zdravo Predraže! Dobio si zahtev za prijateljstvo od Velje. // Translation: Hello Predrag! You have received a friend request from Velja.
 ```
 
 You can also immediatelly decline a name through all grammatical cases by calling the `declineAll()` function.
 
 The `declineAll()` function returns a `dictionary`, where the keys are the grammatical cases.
 
 ```python
 import deklinacija as dek
+from deklinacija import Gender, Number
 
-name = dek.declineAll("Nikola","male") 
+name = dek.declineAll("Nikola",Gender.MALE) 
 #{'nominativ': 'Nikola', 'genitiv': 'Nikole', 'dativ': 'Nikoli', 'akuzativ': 'Nikolu', 
 #'vokativ':'Nikola', 'instrumental': 'Nikolom', 'lokativ': 'Nikoli'}
 
 print("Dali ste poklon",name['dativ']) 
 #Dali ste poklon Nikoli // Translation: You have given a gift to Nikola
 ```
 
 ## Posessive Forms
-As of version 1.6 there is a new feature: posessive forms. Aside from the name and the gender of the person, you also have to specify the gender of the posessed object and its grammatical number. In case the gender of the posessed object is unknown, you can just pass the object itself to the `object_gender` parameter and the program will figure out which gender it is, provided that the `grammatical_number` is set correctly (default value is "singular").
+As of version 1.6 there is a new feature: posessive forms. Aside from the name and the gender of the person, you also have to specify the gender of the posessed object and its grammatical number. In case the gender of the posessed object is unknown, you can just pass the object itself to the `object_gender` parameter and the program will figure out which gender it is, provided that the `grammatical_number` is set correctly (default value is Number.SINGULAR).
 
 The functions in this example return a `string`.
 ```python
 import deklinacija as dek
+from deklinacija import Gender, Number
 
-name = dek.posessive(name = "Stefan", gender = "male", object_gender = "female", grammatical_number = "singular")
-name2 = dek.posessive(name = "Stefan", gender = "male", object_gender = "grupa") #passing the object "group" instead of "female", default grammatical_number value is "singular" so it's not required to specify it in this case
-name3 = dek.posessive(name = "Stefan", gender = "male", object_gender = "slušalice", grammatical_number = "plural") #passing the object "headphones"
+name = dek.posessive(name = "Stefan", gender = Gender.MALE, object_gender = Gender.FEMALE, grammatical_number = Number.SINGULAR)
+name2 = dek.posessive(name = "Stefan", gender = Gender.MALE, object_gender = "grupa") #passing the object "group" instead of Gender.FEMALE, default grammatical_number value is Number.SINGULAR so it's not required to specify it in this case
+name3 = dek.posessive(name = "Stefan", gender = Gender.MALE, object_gender = "slušalice", grammatical_number = Number.PLURAL) #passing the object "headphones"
 
 print(name,"grupa") #Stefanova grupa // Translation: Stefan's group
 print(name2,"grupa") #Stefanova grupa
 print(name3,"slušalice") #Stefanove slušalice // Translation: Stefan's headphones
 ```
 
 You can also immediately transform the name through all possible posessive forms (male, female, neutral in singular and plural) by calling the `posessiveAll()` function. Only the `name` and `gender` parameters are required.
 
 The `posessiveAll()` function returns a `dictionary` where the keys are in the "GENDER_NUMBER" format.
 
 ```python
 import deklinacija as dek
+from deklinacija import Gender, Number
 
-name = dek.posessiveAll("Stefan","male") #{'name': 'Stefan', 'male_singular': 'Stefanov', 'male_plural': 'Stefanovi', 'female_singular': 'Stefanova', 'female_plural': 'Stefanove', 'neutral_singular': 'Stefanovo', 'neutral_plural': 'Stefanova'}
+name = dek.posessiveAll("Stefan",Gender.MALE) #{'name': 'Stefan', 'male_singular': 'Stefanov', 'male_plural': 'Stefanovi', 'female_singular': 'Stefanova', 'female_plural': 'Stefanove', 'neutral_singular': 'Stefanovo', 'neutral_plural': 'Stefanova'}
 
 print(name['male_plural'],"prijatelji") #Stefanovi prijatelji // Translation: Stefan's friends
 ```
 ## Other tools
 This library makes extensive use of a few internal utilities that one may find useful when working with the Serbian language. These include:
 
 `toLatin(word)`, `toCyrillic(word)`: Converts input string from Latin into Cyrillic and vice versa. Works with Serbian Latin letter pairs (lj, nj, dž, etc.)
```

