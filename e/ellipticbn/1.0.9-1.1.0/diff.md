# Comparing `tmp/ElliptiCBn-1.0.9.tar.gz` & `tmp/ellipticbn-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ElliptiCBn-1.0.9.tar", last modified: Mon Jul 10 18:23:59 2023, max compression
+gzip compressed data, was "ellipticbn-1.1.0.tar", last modified: Mon Jul 24 19:19:50 2023, max compression
```

## Comparing `ElliptiCBn-1.0.9.tar` & `ellipticbn-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 18:23:59.108484 ElliptiCBn-1.0.9/
-drwxrwxrwx   0        0        0        0 2023-07-10 18:23:59.083526 ElliptiCBn-1.0.9/ElliptiC/
--rw-rw-rw-   0        0        0    27466 2023-06-28 19:43:33.000000 ElliptiCBn-1.0.9/ElliptiC/ElliptiC.py
--rw-rw-rw-   0        0        0       30 2023-06-28 19:22:14.000000 ElliptiCBn-1.0.9/ElliptiC/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-10 18:23:59.104491 ElliptiCBn-1.0.9/ElliptiCBn.egg-info/
--rw-rw-rw-   0        0        0     4731 2023-07-10 18:23:59.000000 ElliptiCBn-1.0.9/ElliptiCBn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-07-10 18:23:59.000000 ElliptiCBn-1.0.9/ElliptiCBn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 18:23:59.000000 ElliptiCBn-1.0.9/ElliptiCBn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2023-07-10 18:23:59.000000 ElliptiCBn-1.0.9/ElliptiCBn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-10 18:23:59.000000 ElliptiCBn-1.0.9/ElliptiCBn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1108 2023-06-23 18:27:33.000000 ElliptiCBn-1.0.9/LICENSE
--rw-rw-rw-   0        0        0     4731 2023-07-10 18:23:59.108484 ElliptiCBn-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     3959 2023-07-10 18:20:18.000000 ElliptiCBn-1.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 18:23:59.104491 ElliptiCBn-1.0.9/bin/
--rw-rw-rw-   0        0        0      899 2023-07-07 18:41:14.000000 ElliptiCBn-1.0.9/bin/ElliptiC
--rw-rw-rw-   0        0        0      919 2023-07-10 18:23:07.000000 ElliptiCBn-1.0.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-10 18:23:59.108484 ElliptiCBn-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1340 2023-07-10 18:23:30.000000 ElliptiCBn-1.0.9/setup.py
+drwxr-xr-x   0 ryshavlik   (501) staff       (20)        0 2023-07-24 19:19:50.770644 ellipticbn-1.1.0/
+drwxr-xr-x   0 ryshavlik   (501) staff       (20)        0 2023-07-24 19:19:50.754870 ellipticbn-1.1.0/ElliptiCBn/
+-rwxrwxrwx   0 ryshavlik   (501) staff       (20)    27466 2023-06-28 19:43:34.000000 ellipticbn-1.1.0/ElliptiCBn/ElliptiCBn.py
+-rw-rw-r--   0 ryshavlik   (501) staff       (20)       30 2023-06-28 19:22:16.000000 ellipticbn-1.1.0/ElliptiCBn/__init__.py
+-rw-rw-r--   0 ryshavlik   (501) staff       (20)     1108 2023-06-23 18:27:34.000000 ellipticbn-1.1.0/LICENSE
+-rw-r--r--   0 ryshavlik   (501) staff       (20)     4651 2023-07-24 19:19:50.769587 ellipticbn-1.1.0/PKG-INFO
+-rw-rw-r--   0 ryshavlik   (501) staff       (20)     3967 2023-07-10 20:44:12.000000 ellipticbn-1.1.0/README.md
+drwxr-xr-x   0 ryshavlik   (501) staff       (20)        0 2023-07-24 19:19:50.758856 ellipticbn-1.1.0/bin/
+-rwxrwxrwx   0 ryshavlik   (501) staff       (20)      903 2023-07-10 20:42:00.000000 ellipticbn-1.1.0/bin/ElliptiCBn
+drwxr-xr-x   0 ryshavlik   (501) staff       (20)        0 2023-07-24 19:19:50.768111 ellipticbn-1.1.0/ellipticbn.egg-info/
+-rw-r--r--   0 ryshavlik   (501) staff       (20)     4651 2023-07-24 19:19:50.000000 ellipticbn-1.1.0/ellipticbn.egg-info/PKG-INFO
+-rw-r--r--   0 ryshavlik   (501) staff       (20)      273 2023-07-24 19:19:50.000000 ellipticbn-1.1.0/ellipticbn.egg-info/SOURCES.txt
+-rw-r--r--   0 ryshavlik   (501) staff       (20)        1 2023-07-24 19:19:50.000000 ellipticbn-1.1.0/ellipticbn.egg-info/dependency_links.txt
+-rw-r--r--   0 ryshavlik   (501) staff       (20)       91 2023-07-24 19:19:50.000000 ellipticbn-1.1.0/ellipticbn.egg-info/requires.txt
+-rw-r--r--   0 ryshavlik   (501) staff       (20)       11 2023-07-24 19:19:50.000000 ellipticbn-1.1.0/ellipticbn.egg-info/top_level.txt
+-rw-rw-r--   0 ryshavlik   (501) staff       (20)      921 2023-07-24 19:19:14.000000 ellipticbn-1.1.0/pyproject.toml
+-rw-r--r--   0 ryshavlik   (501) staff       (20)       38 2023-07-24 19:19:50.770883 ellipticbn-1.1.0/setup.cfg
+-rw-rw-r--   0 ryshavlik   (501) staff       (20)     1348 2023-07-10 20:47:26.000000 ellipticbn-1.1.0/setup.py
```

### Comparing `ElliptiCBn-1.0.9/ElliptiC/ElliptiC.py` & `ellipticbn-1.1.0/ElliptiCBn/ElliptiCBn.py`

 * *Files identical despite different names*

### Comparing `ElliptiCBn-1.0.9/ElliptiCBn.egg-info/PKG-INFO` & `ellipticbn-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-Metadata-Version: 2.1
-Name: ElliptiCBn
-Version: 1.0.9
-Summary: Python package for analyzing Cucurbituril crystal structures automatically
-Home-page: https://github.com/harmslab/ElliptiC
-Author: Michael Shavlik
-Author-email: Michael Shavlik <mshavlik@uoregon.edu>
-License: MIT
-Project-URL: Homepage, https://github.com/harmslab/ElliptiC
-Keywords: CBn; Crystal structure
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# ElliptiC - an automated command line tool for visualizing and measuring ellipticity of cucurbituril host/guest structures
-
-<br />
-
-
-## How to install
-**In a terminal, the command for installation is a simple**
-
-_pip install ElliptiCBn_
-
-**If you would rather not use pip and prefer installing source, the installation of the package can be done by the following:**
-* Clone this git repository to your local machine
-* In the cloned repository, install the cbn_analysis package through _python -m pip install . vv_ 
-* Next, install the required dependencies by running _pip install -r requirements.txt_
-
-<br />
-
-## How to run the analysis
-### The ElliptiC package takes a single command line argument: an xyz file containing atom coordinates, or a folder of xyz files containing atom coordinates
-
-**To run the analysis package on a single file, navigate to the directory with the ElliptiC script and execute it:**
-(NOTE: if there are spaces in your file name, you will need quotes around the file name)
-![](https://github.com/harmslab/ElliptiC/raw/main/images/single_file.png)
-
-
-**The same convention can be used to execute the package on a folder of xyz files**
-![](https://github.com/harmslab/ElliptiC/raw/main/images/folder_test.png)
-    
-<br />
-
-## How the package works
-### Below is a diagram of the analysis steps the software completes on any given file
-![](https://github.com/harmslab/ElliptiC/raw/main/images/pipeline_image.svg)
-
-### 1. In a given XYZ file, extract the coordinates of all carbon atoms (and oxygen atoms used later on in the analysis).
-### 2. Identify strongly connected components to differentiate between host and guest structures.
-### 3. Remove the guest structure since we only care about calculating ellipticity of the host.
-### 4. Using proximity to oxygen atoms, remove the top and bottom rings of the hosts for accurate ellipticity calculation.
-### 5 & 6. Using a Principal Components Analysis, calculate the variance along both major axes of the host ring. The ellipticity is thus (Vax1-Vax2)/Vax1 where Vax1 is the variance on the longest axis (length) and Vax2 is the variance on the second-longest axis (width). 
-### 7. Output graphs of both the single ring hosts and the full host-guest structures, as well as a spreadsheet with the calculated ellipticity for each structure.
-
-<br />
-<br />
-
-## How to interpret the output
-
-### Each xyz file analyzed with this package will produce at least 3 pieces of data: 
-* 1 interactive 3D scatter plot with all carbons in the CBn structures visualized 
-* 1 interactive 3D scatter plot with only the central carbon ring of the CBn structures visualized
-* 1 spreadsheet with all of the carbons, their positions, distance to the centroid of the structure, and the measured ellipticity
-
-**In the case of host CBn structures with an internally situated guest structure, an additional 3D graph will be produced with the guests visualized in the structures (see below)**
-
-![](https://github.com/harmslab/ElliptiC/raw/main/images/testing_cbn_interactive.png)
-
-To see the interactive version of this plot that gets generated from the script, [Click Here](https://plotly.com/~Mshavlik/63/)
-
-**The user can visually see the ellipticity in the structues and compare them to the measured values in the spreadsheets:**                 
-_CB7 structures from above with guests removed_
-![](https://github.com/harmslab/ElliptiC/raw/main/images/CB7_circular.png)
-
-Calculated ellipticity for each structure on a scale of circular (0) to linear (1)  
-![](https://github.com/harmslab/ElliptiC/raw/main/images/circular_ellipticity.png)
-
-
-_CB10 wide structures with guests removed_
-![](https://github.com/harmslab/ElliptiC/raw/main/images/ellipsoid_example.png)
-
-Calculated ellipticity for each structure on a scale of circular (0) to linear (1)  
-![](https://github.com/harmslab/ElliptiC/raw/main/images/ellipse_ellipticity.png)
-
-
+Metadata-Version: 2.1
+Name: ellipticbn
+Version: 1.1.0
+Summary: Python package for analyzing Cucurbituril crystal structures automatically
+Home-page: https://github.com/harmslab/ElliptiCBn
+Author: Michael Shavlik
+Author-email: Michael Shavlik <mshavlik@uoregon.edu>
+License: MIT
+Project-URL: Homepage, https://github.com/harmslab/ElliptiCBn
+Keywords: CBn; Crystal structure
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.7.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# ElliptiCBn - an automated command line tool for visualizing and measuring ellipticity of cucurbituril host/guest structures
+
+<br />
+
+
+## How to install
+**In a terminal, the command for installation is a simple**
+
+_pip install ElliptiCBn_
+
+**If you would rather not use pip and prefer installing source, the installation of the package can be done by the following:**
+* Clone this git repository to your local machine
+* In the cloned repository, install ElliptiCBn through _python -m pip install . vv_ 
+* Next, install the required dependencies by running _pip install -r requirements.txt_
+
+<br />
+
+## How to run the analysis
+### The ElliptiCBn package takes a single command line argument: an xyz file containing atom coordinates, or a folder of xyz files containing atom coordinates
+
+**To run the analysis package on a single file, navigate to the directory with the ElliptiCBn script and execute it:**
+(NOTE: if there are spaces in your file name, you will need quotes around the file name)
+![](https://github.com/harmslab/ElliptiCBn/raw/main/images/single_file.png)
+
+
+**The same convention can be used to execute the package on a folder of xyz files**
+![](https://github.com/harmslab/ElliptiCBn/raw/main/images/folder_test.png)
+    
+<br />
+
+## How the package works
+### Below is a diagram of the analysis steps the software completes on any given file
+![](https://github.com/harmslab/ElliptiCBn/raw/main/images/pipeline_image.svg)
+
+### 1. In a given XYZ file, extract the coordinates of all carbon atoms (and oxygen atoms used later on in the analysis).
+### 2. Identify strongly connected components to differentiate between host and guest structures.
+### 3. Remove the guest structure since we only care about calculating ellipticity of the host.
+### 4. Using proximity to oxygen atoms, remove the top and bottom rings of the hosts for accurate ellipticity calculation.
+### 5 & 6. Using a Principal Components Analysis, calculate the variance along both major axes of the host ring. The ellipticity is thus (Vax1-Vax2)/Vax1 where Vax1 is the variance on the longest axis (length) and Vax2 is the variance on the second-longest axis (width). 
+### 7. Output graphs of both the single ring hosts and the full host-guest structures, as well as a spreadsheet with the calculated ellipticity for each structure.
+
+<br />
+<br />
+
+## How to interpret the output
+
+### Each xyz file analyzed with this package will produce at least 3 pieces of data: 
+* 1 interactive 3D scatter plot with all carbons in the CBn structures visualized 
+* 1 interactive 3D scatter plot with only the central carbon ring of the CBn structures visualized
+* 1 spreadsheet with all of the carbons, their positions, distance to the centroid of the structure, and the measured ellipticity
+
+**In the case of host CBn structures with an internally situated guest structure, an additional 3D graph will be produced with the guests visualized in the structures (see below)**
+
+![](https://github.com/harmslab/ElliptiCBn/raw/main/images/testing_cbn_interactive.png)
+
+To see the interactive version of this plot that gets generated from the script, [Click Here](https://plotly.com/~Mshavlik/63/)
+
+**The user can visually see the ellipticity in the structues and compare them to the measured values in the spreadsheets:**                 
+_CB7 structures from above with guests removed_
+![](https://github.com/harmslab/ElliptiCBn/raw/main/images/CB7_circular.png)
+
+Calculated ellipticity for each structure on a scale of circular (0) to linear (1)  
+![](https://github.com/harmslab/ElliptiCBn/raw/main/images/circular_ellipticity.png)
+
+
+_CB10 wide structures with guests removed_
+![](https://github.com/harmslab/ElliptiCBn/raw/main/images/ellipsoid_example.png)
+
+Calculated ellipticity for each structure on a scale of circular (0) to linear (1)  
+![](https://github.com/harmslab/ElliptiCBn/raw/main/images/ellipse_ellipticity.png)
+
+
```

### Comparing `ElliptiCBn-1.0.9/LICENSE` & `ellipticbn-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ElliptiCBn-1.0.9/PKG-INFO` & `ellipticbn-1.1.0/ellipticbn.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-Metadata-Version: 2.1
-Name: ElliptiCBn
-Version: 1.0.9
-Summary: Python package for analyzing Cucurbituril crystal structures automatically
-Home-page: https://github.com/harmslab/ElliptiC
-Author: Michael Shavlik
-Author-email: Michael Shavlik <mshavlik@uoregon.edu>
-License: MIT
-Project-URL: Homepage, https://github.com/harmslab/ElliptiC
-Keywords: CBn; Crystal structure
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# ElliptiC - an automated command line tool for visualizing and measuring ellipticity of cucurbituril host/guest structures
-
-<br />
-
-
-## How to install
-**In a terminal, the command for installation is a simple**
-
-_pip install ElliptiCBn_
-
-**If you would rather not use pip and prefer installing source, the installation of the package can be done by the following:**
-* Clone this git repository to your local machine
-* In the cloned repository, install the cbn_analysis package through _python -m pip install . vv_ 
-* Next, install the required dependencies by running _pip install -r requirements.txt_
-
-<br />
-
-## How to run the analysis
-### The ElliptiC package takes a single command line argument: an xyz file containing atom coordinates, or a folder of xyz files containing atom coordinates
-
-**To run the analysis package on a single file, navigate to the directory with the ElliptiC script and execute it:**
-(NOTE: if there are spaces in your file name, you will need quotes around the file name)
-![](https://github.com/harmslab/ElliptiC/raw/main/images/single_file.png)
-
-
-**The same convention can be used to execute the package on a folder of xyz files**
-![](https://github.com/harmslab/ElliptiC/raw/main/images/folder_test.png)
-    
-<br />
-
-## How the package works
-### Below is a diagram of the analysis steps the software completes on any given file
-![](https://github.com/harmslab/ElliptiC/raw/main/images/pipeline_image.svg)
-
-### 1. In a given XYZ file, extract the coordinates of all carbon atoms (and oxygen atoms used later on in the analysis).
-### 2. Identify strongly connected components to differentiate between host and guest structures.
-### 3. Remove the guest structure since we only care about calculating ellipticity of the host.
-### 4. Using proximity to oxygen atoms, remove the top and bottom rings of the hosts for accurate ellipticity calculation.
-### 5 & 6. Using a Principal Components Analysis, calculate the variance along both major axes of the host ring. The ellipticity is thus (Vax1-Vax2)/Vax1 where Vax1 is the variance on the longest axis (length) and Vax2 is the variance on the second-longest axis (width). 
-### 7. Output graphs of both the single ring hosts and the full host-guest structures, as well as a spreadsheet with the calculated ellipticity for each structure.
-
-<br />
-<br />
-
-## How to interpret the output
-
-### Each xyz file analyzed with this package will produce at least 3 pieces of data: 
-* 1 interactive 3D scatter plot with all carbons in the CBn structures visualized 
-* 1 interactive 3D scatter plot with only the central carbon ring of the CBn structures visualized
-* 1 spreadsheet with all of the carbons, their positions, distance to the centroid of the structure, and the measured ellipticity
-
-**In the case of host CBn structures with an internally situated guest structure, an additional 3D graph will be produced with the guests visualized in the structures (see below)**
-
-![](https://github.com/harmslab/ElliptiC/raw/main/images/testing_cbn_interactive.png)
-
-To see the interactive version of this plot that gets generated from the script, [Click Here](https://plotly.com/~Mshavlik/63/)
-
-**The user can visually see the ellipticity in the structues and compare them to the measured values in the spreadsheets:**                 
-_CB7 structures from above with guests removed_
-![](https://github.com/harmslab/ElliptiC/raw/main/images/CB7_circular.png)
-
-Calculated ellipticity for each structure on a scale of circular (0) to linear (1)  
-![](https://github.com/harmslab/ElliptiC/raw/main/images/circular_ellipticity.png)
-
-
-_CB10 wide structures with guests removed_
-![](https://github.com/harmslab/ElliptiC/raw/main/images/ellipsoid_example.png)
-
-Calculated ellipticity for each structure on a scale of circular (0) to linear (1)  
-![](https://github.com/harmslab/ElliptiC/raw/main/images/ellipse_ellipticity.png)
-
-
+Metadata-Version: 2.1
+Name: ellipticbn
+Version: 1.1.0
+Summary: Python package for analyzing Cucurbituril crystal structures automatically
+Home-page: https://github.com/harmslab/ElliptiCBn
+Author: Michael Shavlik
+Author-email: Michael Shavlik <mshavlik@uoregon.edu>
+License: MIT
+Project-URL: Homepage, https://github.com/harmslab/ElliptiCBn
+Keywords: CBn; Crystal structure
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.7.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# ElliptiCBn - an automated command line tool for visualizing and measuring ellipticity of cucurbituril host/guest structures
+
+<br />
+
+
+## How to install
+**In a terminal, the command for installation is a simple**
+
+_pip install ElliptiCBn_
+
+**If you would rather not use pip and prefer installing source, the installation of the package can be done by the following:**
+* Clone this git repository to your local machine
+* In the cloned repository, install ElliptiCBn through _python -m pip install . vv_ 
+* Next, install the required dependencies by running _pip install -r requirements.txt_
+
+<br />
+
+## How to run the analysis
+### The ElliptiCBn package takes a single command line argument: an xyz file containing atom coordinates, or a folder of xyz files containing atom coordinates
+
+**To run the analysis package on a single file, navigate to the directory with the ElliptiCBn script and execute it:**
+(NOTE: if there are spaces in your file name, you will need quotes around the file name)
+![](https://github.com/harmslab/ElliptiCBn/raw/main/images/single_file.png)
+
+
+**The same convention can be used to execute the package on a folder of xyz files**
+![](https://github.com/harmslab/ElliptiCBn/raw/main/images/folder_test.png)
+    
+<br />
+
+## How the package works
+### Below is a diagram of the analysis steps the software completes on any given file
+![](https://github.com/harmslab/ElliptiCBn/raw/main/images/pipeline_image.svg)
+
+### 1. In a given XYZ file, extract the coordinates of all carbon atoms (and oxygen atoms used later on in the analysis).
+### 2. Identify strongly connected components to differentiate between host and guest structures.
+### 3. Remove the guest structure since we only care about calculating ellipticity of the host.
+### 4. Using proximity to oxygen atoms, remove the top and bottom rings of the hosts for accurate ellipticity calculation.
+### 5 & 6. Using a Principal Components Analysis, calculate the variance along both major axes of the host ring. The ellipticity is thus (Vax1-Vax2)/Vax1 where Vax1 is the variance on the longest axis (length) and Vax2 is the variance on the second-longest axis (width). 
+### 7. Output graphs of both the single ring hosts and the full host-guest structures, as well as a spreadsheet with the calculated ellipticity for each structure.
+
+<br />
+<br />
+
+## How to interpret the output
+
+### Each xyz file analyzed with this package will produce at least 3 pieces of data: 
+* 1 interactive 3D scatter plot with all carbons in the CBn structures visualized 
+* 1 interactive 3D scatter plot with only the central carbon ring of the CBn structures visualized
+* 1 spreadsheet with all of the carbons, their positions, distance to the centroid of the structure, and the measured ellipticity
+
+**In the case of host CBn structures with an internally situated guest structure, an additional 3D graph will be produced with the guests visualized in the structures (see below)**
+
+![](https://github.com/harmslab/ElliptiCBn/raw/main/images/testing_cbn_interactive.png)
+
+To see the interactive version of this plot that gets generated from the script, [Click Here](https://plotly.com/~Mshavlik/63/)
+
+**The user can visually see the ellipticity in the structues and compare them to the measured values in the spreadsheets:**                 
+_CB7 structures from above with guests removed_
+![](https://github.com/harmslab/ElliptiCBn/raw/main/images/CB7_circular.png)
+
+Calculated ellipticity for each structure on a scale of circular (0) to linear (1)  
+![](https://github.com/harmslab/ElliptiCBn/raw/main/images/circular_ellipticity.png)
+
+
+_CB10 wide structures with guests removed_
+![](https://github.com/harmslab/ElliptiCBn/raw/main/images/ellipsoid_example.png)
+
+Calculated ellipticity for each structure on a scale of circular (0) to linear (1)  
+![](https://github.com/harmslab/ElliptiCBn/raw/main/images/ellipse_ellipticity.png)
+
+
```

### Comparing `ElliptiCBn-1.0.9/README.md` & `ellipticbn-1.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-# ElliptiC - an automated command line tool for visualizing and measuring ellipticity of cucurbituril host/guest structures
+# ElliptiCBn - an automated command line tool for visualizing and measuring ellipticity of cucurbituril host/guest structures
 
 <br />
 
 
 ## How to install
 **In a terminal, the command for installation is a simple**
 
 _pip install ElliptiCBn_
 
 **If you would rather not use pip and prefer installing source, the installation of the package can be done by the following:**
 * Clone this git repository to your local machine
-* In the cloned repository, install the cbn_analysis package through _python -m pip install . vv_ 
+* In the cloned repository, install ElliptiCBn through _python -m pip install . vv_ 
 * Next, install the required dependencies by running _pip install -r requirements.txt_
 
 <br />
 
 ## How to run the analysis
-### The ElliptiC package takes a single command line argument: an xyz file containing atom coordinates, or a folder of xyz files containing atom coordinates
+### The ElliptiCBn package takes a single command line argument: an xyz file containing atom coordinates, or a folder of xyz files containing atom coordinates
 
-**To run the analysis package on a single file, navigate to the directory with the ElliptiC script and execute it:**
+**To run the analysis package on a single file, navigate to the directory with the ElliptiCBn script and execute it:**
 (NOTE: if there are spaces in your file name, you will need quotes around the file name)
-![](https://github.com/harmslab/ElliptiC/raw/main/images/single_file.png)
+![](https://github.com/harmslab/ElliptiCBn/raw/main/images/single_file.png)
 
 
 **The same convention can be used to execute the package on a folder of xyz files**
-![](https://github.com/harmslab/ElliptiC/raw/main/images/folder_test.png)
+![](https://github.com/harmslab/ElliptiCBn/raw/main/images/folder_test.png)
     
 <br />
 
 ## How the package works
 ### Below is a diagram of the analysis steps the software completes on any given file
-![](https://github.com/harmslab/ElliptiC/raw/main/images/pipeline_image.svg)
+![](https://github.com/harmslab/ElliptiCBn/raw/main/images/pipeline_image.svg)
 
 ### 1. In a given XYZ file, extract the coordinates of all carbon atoms (and oxygen atoms used later on in the analysis).
 ### 2. Identify strongly connected components to differentiate between host and guest structures.
 ### 3. Remove the guest structure since we only care about calculating ellipticity of the host.
 ### 4. Using proximity to oxygen atoms, remove the top and bottom rings of the hosts for accurate ellipticity calculation.
 ### 5 & 6. Using a Principal Components Analysis, calculate the variance along both major axes of the host ring. The ellipticity is thus (Vax1-Vax2)/Vax1 where Vax1 is the variance on the longest axis (length) and Vax2 is the variance on the second-longest axis (width). 
 ### 7. Output graphs of both the single ring hosts and the full host-guest structures, as well as a spreadsheet with the calculated ellipticity for each structure.
@@ -47,26 +47,26 @@
 ### Each xyz file analyzed with this package will produce at least 3 pieces of data: 
 * 1 interactive 3D scatter plot with all carbons in the CBn structures visualized 
 * 1 interactive 3D scatter plot with only the central carbon ring of the CBn structures visualized
 * 1 spreadsheet with all of the carbons, their positions, distance to the centroid of the structure, and the measured ellipticity
 
 **In the case of host CBn structures with an internally situated guest structure, an additional 3D graph will be produced with the guests visualized in the structures (see below)**
 
-![](https://github.com/harmslab/ElliptiC/raw/main/images/testing_cbn_interactive.png)
+![](https://github.com/harmslab/ElliptiCBn/raw/main/images/testing_cbn_interactive.png)
 
 To see the interactive version of this plot that gets generated from the script, [Click Here](https://plotly.com/~Mshavlik/63/)
 
 **The user can visually see the ellipticity in the structues and compare them to the measured values in the spreadsheets:**                 
 _CB7 structures from above with guests removed_
-![](https://github.com/harmslab/ElliptiC/raw/main/images/CB7_circular.png)
+![](https://github.com/harmslab/ElliptiCBn/raw/main/images/CB7_circular.png)
 
 Calculated ellipticity for each structure on a scale of circular (0) to linear (1)  
-![](https://github.com/harmslab/ElliptiC/raw/main/images/circular_ellipticity.png)
+![](https://github.com/harmslab/ElliptiCBn/raw/main/images/circular_ellipticity.png)
 
 
 _CB10 wide structures with guests removed_
-![](https://github.com/harmslab/ElliptiC/raw/main/images/ellipsoid_example.png)
+![](https://github.com/harmslab/ElliptiCBn/raw/main/images/ellipsoid_example.png)
 
 Calculated ellipticity for each structure on a scale of circular (0) to linear (1)  
-![](https://github.com/harmslab/ElliptiC/raw/main/images/ellipse_ellipticity.png)
+![](https://github.com/harmslab/ElliptiCBn/raw/main/images/ellipse_ellipticity.png)
```

### Comparing `ElliptiCBn-1.0.9/bin/ElliptiC` & `ellipticbn-1.1.0/bin/ElliptiCBn`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # coding: utf-8
 
 """
-Command line interface to use the ElliptiC.run_all
+Command line interface to use the ElliptiCBn.run_all
 """
 
-from ElliptiC import run_all
+from ElliptiCBn import run_all
 import sys
 import os
 import glob
 
 __usage__ = "No xyz file or folder of xyz files specified. \n \n Please specify either an xyz file or folder of xyz files"
 
 def main(argv=None):
```

### Comparing `ElliptiCBn-1.0.9/pyproject.toml` & `ellipticbn-1.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
-name = "ElliptiCBn"
-version = "1.0.9"
+name = "ellipticbn"
+version = "1.1.0"
 authors = [{name="Michael Shavlik", email="mshavlik@uoregon.edu"}]
 description = "Python package for analyzing Cucurbituril crystal structures automatically"
 readme = "README.md"
 requires-python = ">=3.7.0"
 classifiers = [
                   "Development Status :: 3 - Alpha",
                   "Intended Audience :: Science/Research",
@@ -29,9 +29,9 @@
 "xlsxwriter",
 "openpyxl",
 ]
 
 
 
 [project.urls]
-"Homepage" = "https://github.com/harmslab/ElliptiC"
+"Homepage" = "https://github.com/harmslab/ElliptiCBn"
```

### Comparing `ElliptiCBn-1.0.9/setup.py` & `ellipticbn-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,44 +3,44 @@
 
 import io
 import os
 import glob
 
 from setuptools import find_packages, setup
 
-# name of package ElliptiC
+# name of package ElliptiCBn
 
 #Package meta-data
 DESCRIPTION= \
 """ Python package for analyzing CBn crystal structures automatically. """
-URL = "https://github.com/harmslab/ElliptiC"  # temp URL
+URL = "https://github.com/harmslab/ElliptiCBn"  # temp URL
 EMAIL = "mshavlik@uoregon.edu"
 AUTHOR = "Michael Shavlik"
 REQUIRES_PYTHON = ">=3.7.0"
-VERSION = "1.0.9"
+VERSION = "1.1.0"
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # Import README for description
 with io.open(os.path.join(here,'README.md'),encoding='utf-8') as f:
     full_description = '\n' + f.read()
 
     
 # Now the part where we do setup
 setup(
     name='ElliptiCBn',
-    version='1.0.9',
+    version='1.1.0',
     author=AUTHOR,
     author_email=EMAIL,
     description=DESCRIPTION,
     long_description=full_description,
     url=URL,
     license='MIT',
-    packages=['ElliptiC'],
-    scripts=glob.glob("bin/ElliptiC*"),
+    packages=['ElliptiCBn'],
+    scripts=glob.glob("bin/ElliptiCBn*"),
     keywords='CBn; Crystal structure',
     classifiers = ["Development Status :: 3 - Alpha",
                   'Intended Audience :: Science/Research',
                   'Programming Language :: Python :: 3.7'
                   'Programming Language :: Python :: 3.8',
                   'Programming Language :: Python :: 3.9',
                   'Programming Language :: Python :: 3.10'])
```

