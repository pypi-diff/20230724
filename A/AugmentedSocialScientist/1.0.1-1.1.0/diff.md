# Comparing `tmp/AugmentedSocialScientist-1.0.1.tar.gz` & `tmp/AugmentedSocialScientist-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AugmentedSocialScientist-1.0.1.tar", last modified: Fri Jul 14 21:51:22 2023, max compression
+gzip compressed data, was "AugmentedSocialScientist-1.1.0.tar", last modified: Sun Jul 23 23:36:21 2023, max compression
```

## Comparing `AugmentedSocialScientist-1.0.1.tar` & `AugmentedSocialScientist-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,26 @@
-drwxr-xr-x   0 rubing     (501) staff       (20)        0 2023-07-14 21:51:22.048439 AugmentedSocialScientist-1.0.1/
-drwxr-xr-x   0 rubing     (501) staff       (20)        0 2023-07-14 21:51:22.045601 AugmentedSocialScientist-1.0.1/AugmentedSocialScientist/
--rw-r--r--   0 rubing     (501) staff       (20)    16696 2023-07-14 20:35:01.000000 AugmentedSocialScientist-1.0.1/AugmentedSocialScientist/bert.py
--rw-r--r--   0 rubing     (501) staff       (20)    16751 2023-07-14 20:34:59.000000 AugmentedSocialScientist-1.0.1/AugmentedSocialScientist/camembert.py
--rw-r--r--   0 rubing     (501) staff       (20)    16728 2023-07-14 20:34:58.000000 AugmentedSocialScientist-1.0.1/AugmentedSocialScientist/german_bert.py
--rw-r--r--   0 rubing     (501) staff       (20)    16747 2023-07-14 20:34:57.000000 AugmentedSocialScientist-1.0.1/AugmentedSocialScientist/spanish_bert.py
--rw-r--r--   0 rubing     (501) staff       (20)    16756 2023-07-14 20:34:54.000000 AugmentedSocialScientist-1.0.1/AugmentedSocialScientist/xlmroberta.py
-drwxr-xr-x   0 rubing     (501) staff       (20)        0 2023-07-14 21:51:22.048081 AugmentedSocialScientist-1.0.1/AugmentedSocialScientist.egg-info/
--rw-r--r--   0 rubing     (501) staff       (20)     2266 2023-07-14 21:51:21.000000 AugmentedSocialScientist-1.0.1/AugmentedSocialScientist.egg-info/PKG-INFO
--rw-r--r--   0 rubing     (501) staff       (20)      513 2023-07-14 21:51:21.000000 AugmentedSocialScientist-1.0.1/AugmentedSocialScientist.egg-info/SOURCES.txt
--rw-r--r--   0 rubing     (501) staff       (20)        1 2023-07-14 21:51:21.000000 AugmentedSocialScientist-1.0.1/AugmentedSocialScientist.egg-info/dependency_links.txt
--rw-r--r--   0 rubing     (501) staff       (20)        1 2023-07-14 21:48:17.000000 AugmentedSocialScientist-1.0.1/AugmentedSocialScientist.egg-info/not-zip-safe
--rw-r--r--   0 rubing     (501) staff       (20)       92 2023-07-14 21:51:21.000000 AugmentedSocialScientist-1.0.1/AugmentedSocialScientist.egg-info/requires.txt
--rw-r--r--   0 rubing     (501) staff       (20)       25 2023-07-14 21:51:21.000000 AugmentedSocialScientist-1.0.1/AugmentedSocialScientist.egg-info/top_level.txt
--rw-r--r--   0 rubing     (501) staff       (20)     1068 2023-07-14 19:52:59.000000 AugmentedSocialScientist-1.0.1/LICENSE
--rw-r--r--   0 rubing     (501) staff       (20)     2266 2023-07-14 21:51:22.048640 AugmentedSocialScientist-1.0.1/PKG-INFO
--rw-r--r--   0 rubing     (501) staff       (20)     1801 2023-07-14 21:43:23.000000 AugmentedSocialScientist-1.0.1/README.md
--rw-r--r--   0 rubing     (501) staff       (20)       79 2023-07-14 21:51:22.049393 AugmentedSocialScientist-1.0.1/setup.cfg
--rw-r--r--   0 rubing     (501) staff       (20)      910 2023-07-14 21:51:04.000000 AugmentedSocialScientist-1.0.1/setup.py
+drwxr-xr-x   0 rubing     (501) staff       (20)        0 2023-07-23 23:36:21.677699 AugmentedSocialScientist-1.1.0/
+drwxr-xr-x   0 rubing     (501) staff       (20)        0 2023-07-23 23:36:21.673166 AugmentedSocialScientist-1.1.0/AugmentedSocialScientist/
+-rw-r--r--   0 rubing     (501) staff       (20)    16710 2023-07-23 23:08:49.000000 AugmentedSocialScientist-1.1.0/AugmentedSocialScientist/arabic_bert.py
+-rw-r--r--   0 rubing     (501) staff       (20)    16696 2023-07-14 20:35:01.000000 AugmentedSocialScientist-1.1.0/AugmentedSocialScientist/bert.py
+-rw-r--r--   0 rubing     (501) staff       (20)    16751 2023-07-14 20:34:59.000000 AugmentedSocialScientist-1.1.0/AugmentedSocialScientist/camembert.py
+-rw-r--r--   0 rubing     (501) staff       (20)    16696 2023-07-23 23:15:49.000000 AugmentedSocialScientist-1.1.0/AugmentedSocialScientist/chinese_bert.py
+-rw-r--r--   0 rubing     (501) staff       (20)    16728 2023-07-14 20:34:58.000000 AugmentedSocialScientist-1.1.0/AugmentedSocialScientist/german_bert.py
+-rw-r--r--   0 rubing     (501) staff       (20)    16706 2023-07-23 23:18:30.000000 AugmentedSocialScientist-1.1.0/AugmentedSocialScientist/hindi_bert.py
+-rw-r--r--   0 rubing     (501) staff       (20)    16726 2023-07-23 23:11:56.000000 AugmentedSocialScientist-1.1.0/AugmentedSocialScientist/italian_bert.py
+-rw-r--r--   0 rubing     (501) staff       (20)    16736 2023-07-23 23:10:31.000000 AugmentedSocialScientist-1.1.0/AugmentedSocialScientist/portuguese_bert.py
+-rw-r--r--   0 rubing     (501) staff       (20)    16725 2023-07-23 23:14:58.000000 AugmentedSocialScientist-1.1.0/AugmentedSocialScientist/russian_bert.py
+-rw-r--r--   0 rubing     (501) staff       (20)    16747 2023-07-14 20:34:57.000000 AugmentedSocialScientist-1.1.0/AugmentedSocialScientist/spanish_bert.py
+-rw-r--r--   0 rubing     (501) staff       (20)    16714 2023-07-23 23:12:48.000000 AugmentedSocialScientist-1.1.0/AugmentedSocialScientist/swedish_bert.py
+-rw-r--r--   0 rubing     (501) staff       (20)    16756 2023-07-14 20:34:54.000000 AugmentedSocialScientist-1.1.0/AugmentedSocialScientist/xlmroberta.py
+drwxr-xr-x   0 rubing     (501) staff       (20)        0 2023-07-23 23:36:21.677238 AugmentedSocialScientist-1.1.0/AugmentedSocialScientist.egg-info/
+-rw-r--r--   0 rubing     (501) staff       (20)     2535 2023-07-23 23:36:20.000000 AugmentedSocialScientist-1.1.0/AugmentedSocialScientist.egg-info/PKG-INFO
+-rw-r--r--   0 rubing     (501) staff       (20)      800 2023-07-23 23:36:21.000000 AugmentedSocialScientist-1.1.0/AugmentedSocialScientist.egg-info/SOURCES.txt
+-rw-r--r--   0 rubing     (501) staff       (20)        1 2023-07-23 23:36:20.000000 AugmentedSocialScientist-1.1.0/AugmentedSocialScientist.egg-info/dependency_links.txt
+-rw-r--r--   0 rubing     (501) staff       (20)        1 2023-07-23 23:36:20.000000 AugmentedSocialScientist-1.1.0/AugmentedSocialScientist.egg-info/not-zip-safe
+-rw-r--r--   0 rubing     (501) staff       (20)       92 2023-07-23 23:36:21.000000 AugmentedSocialScientist-1.1.0/AugmentedSocialScientist.egg-info/requires.txt
+-rw-r--r--   0 rubing     (501) staff       (20)       25 2023-07-23 23:36:21.000000 AugmentedSocialScientist-1.1.0/AugmentedSocialScientist.egg-info/top_level.txt
+-rw-r--r--   0 rubing     (501) staff       (20)     1068 2023-07-14 19:52:59.000000 AugmentedSocialScientist-1.1.0/LICENSE
+-rw-r--r--   0 rubing     (501) staff       (20)     2535 2023-07-23 23:36:21.677885 AugmentedSocialScientist-1.1.0/PKG-INFO
+-rw-r--r--   0 rubing     (501) staff       (20)     2070 2023-07-23 23:36:07.000000 AugmentedSocialScientist-1.1.0/README.md
+-rw-r--r--   0 rubing     (501) staff       (20)       79 2023-07-23 23:36:21.679037 AugmentedSocialScientist-1.1.0/setup.cfg
+-rw-r--r--   0 rubing     (501) staff       (20)      910 2023-07-23 23:20:42.000000 AugmentedSocialScientist-1.1.0/setup.py
```

### Comparing `AugmentedSocialScientist-1.0.1/AugmentedSocialScientist/bert.py` & `AugmentedSocialScientist-1.1.0/AugmentedSocialScientist/bert.py`

 * *Files identical despite different names*

### Comparing `AugmentedSocialScientist-1.0.1/AugmentedSocialScientist/camembert.py` & `AugmentedSocialScientist-1.1.0/AugmentedSocialScientist/camembert.py`

 * *Files identical despite different names*

### Comparing `AugmentedSocialScientist-1.0.1/AugmentedSocialScientist/german_bert.py` & `AugmentedSocialScientist-1.1.0/AugmentedSocialScientist/german_bert.py`

 * *Files identical despite different names*

### Comparing `AugmentedSocialScientist-1.0.1/AugmentedSocialScientist/spanish_bert.py` & `AugmentedSocialScientist-1.1.0/AugmentedSocialScientist/spanish_bert.py`

 * *Files identical despite different names*

### Comparing `AugmentedSocialScientist-1.0.1/AugmentedSocialScientist/xlmroberta.py` & `AugmentedSocialScientist-1.1.0/AugmentedSocialScientist/xlmroberta.py`

 * *Files identical despite different names*

### Comparing `AugmentedSocialScientist-1.0.1/AugmentedSocialScientist.egg-info/PKG-INFO` & `AugmentedSocialScientist-1.1.0/AugmentedSocialScientist.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: AugmentedSocialScientist
-Version: 1.0.1
+Version: 1.1.0
 Summary: A Simple Package to Train Bert-Like Model for Text Classification
 Home-page: https://github.com/rubingshen/AugmentedSocialScientist
-Download-URL: https://github.com/rubingshen/AugmentedSocialScientist/archive/refs/tags/v1.0.1.tar.gz
+Download-URL: https://github.com/rubingshen/AugmentedSocialScientist/archive/refs/tags/v1.1.0.tar.gz
 Author: Rubing Shen
 Author-email: shenrubing1996@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # The Augmented Social Scientist
 
+
 This package allows to simply train BERT-like models for text classifications. 
 
 It comes with our article "[The Augmented Social Scientist: Using Sequential Transfer Learning to Annotate Millions of Texts with Human-Level Accuracy](https://journals.sagepub.com/doi/abs/10.1177/00491241221134526)" published on *Sociological Methods & Research* by [Salomé Do](https://sally14.github.io), [Étienne Ollion](https://ollion.cnrs.fr/english/) and [Rubing Shen](https://rubingshen.github.io). 
 
 
 
 ## To install the package
@@ -41,21 +42,30 @@
 - `bert.encode()` to preprocess the data;
 - `bert.run_training()` to train, validate and save a model;
 - `bert.predict_with_model()`  to make predictions with a saved model.
 
 ## Tutorial
 Check [here](https://colab.research.google.com/drive/132_oDik-SOWve31tZ8D1VOx1Sj_Cyzn7?usp=sharing) for a Google Colab tutorial.
 
-## Other languages supported
+## Languages supported
 
-The package also contains models for other languages:
+BERT is a pre-trained language model for the English language. The package also contains models for other languages:
 - `camembert` for French;
+- `arabic_bert` for Arabic;
+- `chinese_bert` for Chinese;
 - `german_bert` for German;
+- `hindi_bert` for Hindi;
+- `italian_bert` for Italian;
+- `portuguese_bert` for Portuguese;
+- `russian_bert` for Russian;
 - `spanish_bert` for Spanish;
- - `xlmroberta` which is a multi-lingual model supporting 100 languages.
+- `swedish_bert` for Swedish;
+- `xlmroberta` which is a multi-lingual model supporting 100 languages.
+
+
 To use them, simply import the corresponding model and replace `bert` with the name of the imported model.
 
 For example, to use the French language model `camembert`:
  1. Import the model `camembert`:
 ```python
 from AugmentedSocialScientist import camembert
 ```
```

### Comparing `AugmentedSocialScientist-1.0.1/AugmentedSocialScientist.egg-info/SOURCES.txt` & `AugmentedSocialScientist-1.1.0/AugmentedSocialScientist.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
+AugmentedSocialScientist/arabic_bert.py
 AugmentedSocialScientist/bert.py
 AugmentedSocialScientist/camembert.py
+AugmentedSocialScientist/chinese_bert.py
 AugmentedSocialScientist/german_bert.py
+AugmentedSocialScientist/hindi_bert.py
+AugmentedSocialScientist/italian_bert.py
+AugmentedSocialScientist/portuguese_bert.py
+AugmentedSocialScientist/russian_bert.py
 AugmentedSocialScientist/spanish_bert.py
+AugmentedSocialScientist/swedish_bert.py
 AugmentedSocialScientist/xlmroberta.py
 AugmentedSocialScientist.egg-info/PKG-INFO
 AugmentedSocialScientist.egg-info/SOURCES.txt
 AugmentedSocialScientist.egg-info/dependency_links.txt
 AugmentedSocialScientist.egg-info/not-zip-safe
 AugmentedSocialScientist.egg-info/requires.txt
 AugmentedSocialScientist.egg-info/top_level.txt
```

### Comparing `AugmentedSocialScientist-1.0.1/LICENSE` & `AugmentedSocialScientist-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `AugmentedSocialScientist-1.0.1/PKG-INFO` & `AugmentedSocialScientist-1.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: AugmentedSocialScientist
-Version: 1.0.1
+Version: 1.1.0
 Summary: A Simple Package to Train Bert-Like Model for Text Classification
 Home-page: https://github.com/rubingshen/AugmentedSocialScientist
-Download-URL: https://github.com/rubingshen/AugmentedSocialScientist/archive/refs/tags/v1.0.1.tar.gz
+Download-URL: https://github.com/rubingshen/AugmentedSocialScientist/archive/refs/tags/v1.1.0.tar.gz
 Author: Rubing Shen
 Author-email: shenrubing1996@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # The Augmented Social Scientist
 
+
 This package allows to simply train BERT-like models for text classifications. 
 
 It comes with our article "[The Augmented Social Scientist: Using Sequential Transfer Learning to Annotate Millions of Texts with Human-Level Accuracy](https://journals.sagepub.com/doi/abs/10.1177/00491241221134526)" published on *Sociological Methods & Research* by [Salomé Do](https://sally14.github.io), [Étienne Ollion](https://ollion.cnrs.fr/english/) and [Rubing Shen](https://rubingshen.github.io). 
 
 
 
 ## To install the package
@@ -41,21 +42,30 @@
 - `bert.encode()` to preprocess the data;
 - `bert.run_training()` to train, validate and save a model;
 - `bert.predict_with_model()`  to make predictions with a saved model.
 
 ## Tutorial
 Check [here](https://colab.research.google.com/drive/132_oDik-SOWve31tZ8D1VOx1Sj_Cyzn7?usp=sharing) for a Google Colab tutorial.
 
-## Other languages supported
+## Languages supported
 
-The package also contains models for other languages:
+BERT is a pre-trained language model for the English language. The package also contains models for other languages:
 - `camembert` for French;
+- `arabic_bert` for Arabic;
+- `chinese_bert` for Chinese;
 - `german_bert` for German;
+- `hindi_bert` for Hindi;
+- `italian_bert` for Italian;
+- `portuguese_bert` for Portuguese;
+- `russian_bert` for Russian;
 - `spanish_bert` for Spanish;
- - `xlmroberta` which is a multi-lingual model supporting 100 languages.
+- `swedish_bert` for Swedish;
+- `xlmroberta` which is a multi-lingual model supporting 100 languages.
+
+
 To use them, simply import the corresponding model and replace `bert` with the name of the imported model.
 
 For example, to use the French language model `camembert`:
  1. Import the model `camembert`:
 ```python
 from AugmentedSocialScientist import camembert
 ```
```

### Comparing `AugmentedSocialScientist-1.0.1/README.md` & `AugmentedSocialScientist-1.1.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # The Augmented Social Scientist
 
+
 This package allows to simply train BERT-like models for text classifications. 
 
 It comes with our article "[The Augmented Social Scientist: Using Sequential Transfer Learning to Annotate Millions of Texts with Human-Level Accuracy](https://journals.sagepub.com/doi/abs/10.1177/00491241221134526)" published on *Sociological Methods & Research* by [Salomé Do](https://sally14.github.io), [Étienne Ollion](https://ollion.cnrs.fr/english/) and [Rubing Shen](https://rubingshen.github.io). 
 
 
 
 ## To install the package
@@ -28,21 +29,30 @@
 - `bert.encode()` to preprocess the data;
 - `bert.run_training()` to train, validate and save a model;
 - `bert.predict_with_model()`  to make predictions with a saved model.
 
 ## Tutorial
 Check [here](https://colab.research.google.com/drive/132_oDik-SOWve31tZ8D1VOx1Sj_Cyzn7?usp=sharing) for a Google Colab tutorial.
 
-## Other languages supported
+## Languages supported
 
-The package also contains models for other languages:
+BERT is a pre-trained language model for the English language. The package also contains models for other languages:
 - `camembert` for French;
+- `arabic_bert` for Arabic;
+- `chinese_bert` for Chinese;
 - `german_bert` for German;
+- `hindi_bert` for Hindi;
+- `italian_bert` for Italian;
+- `portuguese_bert` for Portuguese;
+- `russian_bert` for Russian;
 - `spanish_bert` for Spanish;
- - `xlmroberta` which is a multi-lingual model supporting 100 languages.
+- `swedish_bert` for Swedish;
+- `xlmroberta` which is a multi-lingual model supporting 100 languages.
+
+
 To use them, simply import the corresponding model and replace `bert` with the name of the imported model.
 
 For example, to use the French language model `camembert`:
  1. Import the model `camembert`:
 ```python
 from AugmentedSocialScientist import camembert
 ```
```

### Comparing `AugmentedSocialScientist-1.0.1/setup.py` & `AugmentedSocialScientist-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     long_description = fh.read()
     
 setup(name='AugmentedSocialScientist',
       author='Rubing Shen',
       license='MIT',
       author_email='shenrubing1996@gmail.com',
       url='https://github.com/rubingshen/AugmentedSocialScientist',
-      download_url='https://github.com/rubingshen/AugmentedSocialScientist/archive/refs/tags/v1.0.1.tar.gz',
-      version='1.0.1',
+      download_url='https://github.com/rubingshen/AugmentedSocialScientist/archive/refs/tags/v1.1.0.tar.gz',
+      version='1.1.0',
       description='A Simple Package to Train Bert-Like Model for Text Classification',
       long_description=long_description,
       long_description_content_type="text/markdown",
       packages=['AugmentedSocialScientist'],
       zip_safe=False,
       install_requires=environment)
```

