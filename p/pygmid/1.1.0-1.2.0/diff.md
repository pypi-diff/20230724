# Comparing `tmp/pygmid-1.1.0.tar.gz` & `tmp/pygmid-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygmid-1.1.0.tar", last modified: Fri Jul 14 14:44:18 2023, max compression
+gzip compressed data, was "pygmid-1.2.0.tar", last modified: Mon Jul 24 16:28:03 2023, max compression
```

## Comparing `pygmid-1.1.0.tar` & `pygmid-1.2.0.tar`

### file list

```diff
@@ -1,23 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:44:18.306888 pygmid-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-14 14:43:45.000000 pygmid-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15847 2023-07-14 14:44:18.306888 pygmid-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-07-14 14:43:45.000000 pygmid-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-14 14:43:45.000000 pygmid-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-14 14:44:18.306888 pygmid-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-14 14:43:45.000000 pygmid-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:44:18.302888 pygmid-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:44:18.306888 pygmid-1.1.0/src/pygmid/
--rw-r--r--   0 runner    (1001) docker     (123)    14287 2023-07-14 14:43:45.000000 pygmid-1.1.0/src/pygmid/Lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-14 14:43:45.000000 pygmid-1.1.0/src/pygmid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-14 14:43:45.000000 pygmid-1.1.0/src/pygmid/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-14 14:43:45.000000 pygmid-1.1.0/src/pygmid/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-14 14:43:45.000000 pygmid-1.1.0/src/pygmid/numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-14 14:43:45.000000 pygmid-1.1.0/src/pygmid/pygmid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-07-14 14:43:45.000000 pygmid-1.1.0/src/pygmid/utility.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 14:43:45.000000 pygmid-1.1.0/src/pygmid/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:44:18.306888 pygmid-1.1.0/src/pygmid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15847 2023-07-14 14:44:18.000000 pygmid-1.1.0/src/pygmid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-14 14:44:18.000000 pygmid-1.1.0/src/pygmid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 14:44:18.000000 pygmid-1.1.0/src/pygmid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-14 14:44:18.000000 pygmid-1.1.0/src/pygmid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-14 14:44:18.000000 pygmid-1.1.0/src/pygmid.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:28:03.800540 pygmid-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-07-24 16:27:26.000000 pygmid-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16034 2023-07-24 16:28:03.800540 pygmid-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-07-24 16:27:26.000000 pygmid-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-24 16:27:26.000000 pygmid-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-24 16:28:03.800540 pygmid-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-24 16:27:26.000000 pygmid-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:28:03.796540 pygmid-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:28:03.800540 pygmid-1.2.0/src/pygmid/
+-rw-r--r--   0 runner    (1001) docker     (123)    14287 2023-07-24 16:27:26.000000 pygmid-1.2.0/src/pygmid/Lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-24 16:27:26.000000 pygmid-1.2.0/src/pygmid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-24 16:27:26.000000 pygmid-1.2.0/src/pygmid/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-24 16:27:26.000000 pygmid-1.2.0/src/pygmid/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-24 16:27:26.000000 pygmid-1.2.0/src/pygmid/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-24 16:27:26.000000 pygmid-1.2.0/src/pygmid/pygmid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:28:03.800540 pygmid-1.2.0/src/pygmid/sweep/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-24 16:27:26.000000 pygmid-1.2.0/src/pygmid/sweep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-24 16:27:26.000000 pygmid-1.2.0/src/pygmid/sweep/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-07-24 16:27:26.000000 pygmid-1.2.0/src/pygmid/sweep/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-24 16:27:26.000000 pygmid-1.2.0/src/pygmid/sweep/pysweep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-24 16:27:26.000000 pygmid-1.2.0/src/pygmid/sweep/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-24 16:27:26.000000 pygmid-1.2.0/src/pygmid/sweep/sweep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-07-24 16:27:26.000000 pygmid-1.2.0/src/pygmid/utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 16:27:26.000000 pygmid-1.2.0/src/pygmid/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:28:03.800540 pygmid-1.2.0/src/pygmid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16034 2023-07-24 16:28:03.000000 pygmid-1.2.0/src/pygmid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-24 16:28:03.000000 pygmid-1.2.0/src/pygmid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 16:28:03.000000 pygmid-1.2.0/src/pygmid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 16:28:03.000000 pygmid-1.2.0/src/pygmid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-24 16:28:03.000000 pygmid-1.2.0/src/pygmid.egg-info/top_level.txt
```

### Comparing `pygmid-1.1.0/LICENSE` & `pygmid-1.2.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright [yyyy] [name of copyright owner]
+   Copyright [2023] [Cian Ó Domhnail]
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pygmid-1.1.0/PKG-INFO` & `pygmid-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pygmid
-Version: 1.1.0
+Version: 1.2.0
 Summary: A python 3 implementation of the gm/ID starter kit
 Home-page: https://github.com/madrasalach/pygmid
-Author: Cian O`Donnell, Danylo Galach, Tiarnach Ó Riada
+Author: Cian Ó Domhnaill, Tiarnach Ó Riada, Danylo Galach
 Author-email: cian.odonnell@tyndall.ie
 Project-URL: Bug Tracker, https://github.com/madrasalach/pygmid/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -36,15 +36,15 @@
 - [About](#about)
 - [Installation](#installation)
 - [Usage](#usage)
 - [Authors](#authors)
 
 ## About
 
-pygmid is a Python 3 port of the gm/ID starter kit by Prof. Boris Murmann 
+pygmid is a Python 3 version of the gm/ID starter kit by Prof. Boris Murmann 
 of Stanford University. The package also offers some scripts from the Paul Jesper's book.
 
 For the gm/ID starter kit, written for MATLAB, please refer to the 'Links'
 section at Prof. Murmann's website: https://web.stanford.edu/~murmann.
 
 ## Installation
 
@@ -94,52 +94,55 @@
 # check bias
 VGS = NCH.look_upVGS(GM_ID = 10, VDS = 0.6, VSB = 0.1, L = 0.18)
 print(f'VGS is: {VGS}')
 
 plt.plot(VDSs, np.transpose(ID))
 ```
 
-~~Currently only lookup modes 1 and 2 are implemented.~~
 Modes 1 (Simple parameter lookup), mode 2 (arbitrary ratio lookup) and mode 3 (cross lookup of ratios) are implemented. The companion lookupVGS function is also included.
 
 ### Technology Extraction Functions
 
 The EKV extraction function can be used as follows:
 
 ```python
 from pygmid import EKV_param_extraction, XTRACT
 
 (VDS, n, VT, JS, d1n, d1VT, d1logJS, d2n, d2VT, d2logJS)\
         = EKV_param_extraction(NCH, 1, L = 0.18, VDS = 0.6, VSB = 0.0)
 
 ```
 
-Sample usage of this and other utility functions can be found in `test_utility.py` .
+Sample usage of this and other utility functions can be found in `debug_utility.py` .
 
 ### Examples
 
-Usage of lookup scripts are given in `test_lookup.py` and `test_lookupVGS.py`.
+Usage of lookup scripts are given in `debug_lookup.py` and `debug_lookupVGS.py`.
 
-Sample outputs are given below:
+Sample outputs for the 180nm generic pdk used in the Murmann starter pack are given below:
 
 ![image](https://github.com/madrasalach/pygmid/blob/main/docs/img/IDvVDS.png?raw=true)
 
 ![image](https://github.com/madrasalach/pygmid/blob/main/docs/img/vtvsL.png?raw=true)
 
 ![image](https://github.com/madrasalach/pygmid/blob/main/docs/img/gm_gds.png?raw=true)
 
 ![image](https://github.com/madrasalach/pygmid/blob/main/docs/img/ft.png?raw=true)
 
 ![image](https://github.com/madrasalach/pygmid/blob/main/docs/img/idwVDS.png?raw=true)
 
 ![image](https://github.com/madrasalach/pygmid/blob/main/docs/img/IDWvsgmID.png?raw=true)
 
-### Command Line Interface (CLI)
+The generic PDK data is hosted <a href="https://github.com/bmurmann/Book-on-gm-ID-design">here</a>.
 
-`pygmid` also features a CLI which can be used to run techweeps to generate transistor data
+### Sweeping a Technology
+
+`pygmid` also features a CLI which can be used to run techweeps to generate transistor data.
+
+*Documentation will be added in due course. This functionality is in a state of flux.*
 
 ## Authors
 
 - Cian O'Donnell : cian.odonnell@mcci.ie
 - Tiarnach Ó Riada : tiarnach.oriada@tyndall.ie
 - Danylo Galach
 
@@ -333,15 +336,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright [yyyy] [name of copyright owner]
+   Copyright [2023] [Cian Ó Domhnail]
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

#### html2text {}

```diff
@@ -1,62 +1,63 @@
-Metadata-Version: 2.1 Name: pygmid Version: 1.1.0 Summary: A python 3
+Metadata-Version: 2.1 Name: pygmid Version: 1.2.0 Summary: A python 3
 implementation of the gm/ID starter kit Home-page: https://github.com/
-madrasalach/pygmid Author: Cian O`Donnell, Danylo Galach, Tiarnach Ã Riada
+madrasalach/pygmid Author: Cian Ã Domhnaill, Tiarnach Ã Riada, Danylo Galach
 Author-email: cian.odonnell@tyndall.ie Project-URL: Bug Tracker, https://
 github.com/madrasalach/pygmid/issues Classifier: Programming Language :: Python
 :: 3 Classifier: Operating System :: OS Independent Requires-Python: >=3.4
 Description-Content-Type: text/markdown License-File: LICENSE ![Tests](https://
 github.com/madrasalach/pygmid/actions/workflows/run-tests.yml/
 badge.svg?branch=main) ![PyPI - Downloads](https://img.shields.io/pypi/dm/
 pygmid)
  [https://github.com/madrasalach/pygmid/blob/main/docs/img/icon.png?raw=true]
                                **** pygmid ****
               A python3 implementation of the gm/ID starter kit
                          Report_bug Â· Request_feature
 ## Table of contents - [About](#about) - [Installation](#installation) -
-[Usage](#usage) - [Authors](#authors) ## About pygmid is a Python 3 port of the
-gm/ID starter kit by Prof. Boris Murmann of Stanford University. The package
-also offers some scripts from the Paul Jesper's book. For the gm/ID starter
-kit, written for MATLAB, please refer to the 'Links' section at Prof. Murmann's
-website: https://web.stanford.edu/~murmann. ## Installation To install pygmid
-from source, download from Github and run pip: `pip install .` in the root
-directory. pygmid can also be installed from PyPI: `pip install pygmid` ##
-Usage ### Scripting with the Lookup Class A gm/ID lookup object can be
-generated with the `Lookup` class. The lookup object requires lookup data for
-initialisation. Currently, only `.mat` files are supported. You can create a
-lookup object as follows: ```python from pygmid import Lookup as lk NCH = lk
+[Usage](#usage) - [Authors](#authors) ## About pygmid is a Python 3 version of
+the gm/ID starter kit by Prof. Boris Murmann of Stanford University. The
+package also offers some scripts from the Paul Jesper's book. For the gm/ID
+starter kit, written for MATLAB, please refer to the 'Links' section at Prof.
+Murmann's website: https://web.stanford.edu/~murmann. ## Installation To
+install pygmid from source, download from Github and run pip: `pip install .`
+in the root directory. pygmid can also be installed from PyPI: `pip install
+pygmid` ## Usage ### Scripting with the Lookup Class A gm/ID lookup object can
+be generated with the `Lookup` class. The lookup object requires lookup data
+for initialisation. Currently, only `.mat` files are supported. You can create
+a lookup object as follows: ```python from pygmid import Lookup as lk NCH = lk
 ('180nch.mat') ``` ### Access MOS Data The `Lookup` class allows for pseudo
 array access of the MOS matrix data. You can access data as follows: ```python
 # get VGS data as array from NCH VGS_array = NCH['VGS'] ``` Data is returned as
 a deep copy of the array contained in the `Lookup` object. ### Lookup
 functionality Lookup of interpolated data occurs as follows: ```python VDSs =
 NCH['VDS'] VGSs = np.arange(0.4, 0.6, 0.05) # Plot ID versus VDS ID =
 NCH.look_up('ID', vds=VDSs, vgs=VGSs) # alias function lookup can also be used
 ID = NCH.lookup('ID', vds=VDSs, vgs=VGSs) # check bias VGS = NCH.look_upVGS
 (GM_ID = 10, VDS = 0.6, VSB = 0.1, L = 0.18) print(f'VGS is: {VGS}') plt.plot
-(VDSs, np.transpose(ID)) ``` ~~Currently only lookup modes 1 and 2 are
-implemented.~~ Modes 1 (Simple parameter lookup), mode 2 (arbitrary ratio
-lookup) and mode 3 (cross lookup of ratios) are implemented. The companion
-lookupVGS function is also included. ### Technology Extraction Functions The
-EKV extraction function can be used as follows: ```python from pygmid import
-EKV_param_extraction, XTRACT (VDS, n, VT, JS, d1n, d1VT, d1logJS, d2n, d2VT,
-d2logJS)\ = EKV_param_extraction(NCH, 1, L = 0.18, VDS = 0.6, VSB = 0.0) ```
-Sample usage of this and other utility functions can be found in
-`test_utility.py` . ### Examples Usage of lookup scripts are given in
-`test_lookup.py` and `test_lookupVGS.py`. Sample outputs are given below: !
+(VDSs, np.transpose(ID)) ``` Modes 1 (Simple parameter lookup), mode 2
+(arbitrary ratio lookup) and mode 3 (cross lookup of ratios) are implemented.
+The companion lookupVGS function is also included. ### Technology Extraction
+Functions The EKV extraction function can be used as follows: ```python from
+pygmid import EKV_param_extraction, XTRACT (VDS, n, VT, JS, d1n, d1VT, d1logJS,
+d2n, d2VT, d2logJS)\ = EKV_param_extraction(NCH, 1, L = 0.18, VDS = 0.6, VSB =
+0.0) ``` Sample usage of this and other utility functions can be found in
+`debug_utility.py` . ### Examples Usage of lookup scripts are given in
+`debug_lookup.py` and `debug_lookupVGS.py`. Sample outputs for the 180nm
+generic pdk used in the Murmann starter pack are given below: ![image](https://
+github.com/madrasalach/pygmid/blob/main/docs/img/IDvVDS.png?raw=true) ![image]
+(https://github.com/madrasalach/pygmid/blob/main/docs/img/vtvsL.png?raw=true) !
 [image](https://github.com/madrasalach/pygmid/blob/main/docs/img/
-IDvVDS.png?raw=true) ![image](https://github.com/madrasalach/pygmid/blob/main/
-docs/img/vtvsL.png?raw=true) ![image](https://github.com/madrasalach/pygmid/
-blob/main/docs/img/gm_gds.png?raw=true) ![image](https://github.com/
-madrasalach/pygmid/blob/main/docs/img/ft.png?raw=true) ![image](https://
-github.com/madrasalach/pygmid/blob/main/docs/img/idwVDS.png?raw=true) ![image]
-(https://github.com/madrasalach/pygmid/blob/main/docs/img/
-IDWvsgmID.png?raw=true) ### Command Line Interface (CLI) `pygmid` also features
-a CLI which can be used to run techweeps to generate transistor data ## Authors
-- Cian O'Donnell : cian.odonnell@mcci.ie - Tiarnach Ã Riada :
+gm_gds.png?raw=true) ![image](https://github.com/madrasalach/pygmid/blob/main/
+docs/img/ft.png?raw=true) ![image](https://github.com/madrasalach/pygmid/blob/
+main/docs/img/idwVDS.png?raw=true) ![image](https://github.com/madrasalach/
+pygmid/blob/main/docs/img/IDWvsgmID.png?raw=true) The generic PDK data is
+hosted here. ### Sweeping a Technology `pygmid` also features a CLI which can
+be used to run techweeps to generate transistor data. *Documentation will be
+added in due course. This functionality is in a state of flux.* ## Authors -
+Cian O'Donnell : cian.odonnell@mcci.ie - Tiarnach Ã Riada :
 tiarnach.oriada@tyndall.ie - Danylo Galach ## Contributors - JosÃ© Rui
 CustÃ³dio A special thanks to Prof. Boris Murmann for giving permission to use
 his work and release this package under the Apache 2.0 License. Apache License
 Version 2.0, January 2004 http://www.apache.org/licenses/ TERMS AND CONDITIONS
 FOR USE, REPRODUCTION, AND DISTRIBUTION 1. Definitions. "License" shall mean
 the terms and conditions for use, reproduction, and distribution as defined by
 Sections 1 through 9 of this document. "Licensor" shall mean the copyright
@@ -178,15 +179,15 @@
 CONDITIONS APPENDIX: How to apply the Apache License to your work. To apply the
 Apache License to your work, attach the following boilerplate notice, with the
 fields enclosed by brackets "[]" replaced with your own identifying
 information. (Don't include the brackets!) The text should be enclosed in the
 appropriate comment syntax for the file format. We also recommend that a file
 or class name and description of purpose be included on the same "printed page"
 as the copyright notice for easier identification within third-party archives.
-Copyright [yyyy] [name of copyright owner] Licensed under the Apache License,
-Version 2.0 (the "License"); you may not use this file except in compliance
-with the License. You may obtain a copy of the License at http://
-www.apache.org/licenses/LICENSE-2.0 Unless required by applicable law or agreed
-to in writing, software distributed under the License is distributed on an "AS
-IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-implied. See the License for the specific language governing permissions and
-limitations under the License.
+Copyright [2023] [Cian Ã Domhnail] Licensed under the Apache License, Version
+2.0 (the "License"); you may not use this file except in compliance with the
+License. You may obtain a copy of the License at http://www.apache.org/
+licenses/LICENSE-2.0 Unless required by applicable law or agreed to in writing,
+software distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See
+the License for the specific language governing permissions and limitations
+under the License.
```

### Comparing `pygmid-1.1.0/README.md` & `pygmid-1.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 - [About](#about)
 - [Installation](#installation)
 - [Usage](#usage)
 - [Authors](#authors)
 
 ## About
 
-pygmid is a Python 3 port of the gm/ID starter kit by Prof. Boris Murmann 
+pygmid is a Python 3 version of the gm/ID starter kit by Prof. Boris Murmann 
 of Stanford University. The package also offers some scripts from the Paul Jesper's book.
 
 For the gm/ID starter kit, written for MATLAB, please refer to the 'Links'
 section at Prof. Murmann's website: https://web.stanford.edu/~murmann.
 
 ## Installation
 
@@ -80,52 +80,55 @@
 # check bias
 VGS = NCH.look_upVGS(GM_ID = 10, VDS = 0.6, VSB = 0.1, L = 0.18)
 print(f'VGS is: {VGS}')
 
 plt.plot(VDSs, np.transpose(ID))
 ```
 
-~~Currently only lookup modes 1 and 2 are implemented.~~
 Modes 1 (Simple parameter lookup), mode 2 (arbitrary ratio lookup) and mode 3 (cross lookup of ratios) are implemented. The companion lookupVGS function is also included.
 
 ### Technology Extraction Functions
 
 The EKV extraction function can be used as follows:
 
 ```python
 from pygmid import EKV_param_extraction, XTRACT
 
 (VDS, n, VT, JS, d1n, d1VT, d1logJS, d2n, d2VT, d2logJS)\
         = EKV_param_extraction(NCH, 1, L = 0.18, VDS = 0.6, VSB = 0.0)
 
 ```
 
-Sample usage of this and other utility functions can be found in `test_utility.py` .
+Sample usage of this and other utility functions can be found in `debug_utility.py` .
 
 ### Examples
 
-Usage of lookup scripts are given in `test_lookup.py` and `test_lookupVGS.py`.
+Usage of lookup scripts are given in `debug_lookup.py` and `debug_lookupVGS.py`.
 
-Sample outputs are given below:
+Sample outputs for the 180nm generic pdk used in the Murmann starter pack are given below:
 
 ![image](https://github.com/madrasalach/pygmid/blob/main/docs/img/IDvVDS.png?raw=true)
 
 ![image](https://github.com/madrasalach/pygmid/blob/main/docs/img/vtvsL.png?raw=true)
 
 ![image](https://github.com/madrasalach/pygmid/blob/main/docs/img/gm_gds.png?raw=true)
 
 ![image](https://github.com/madrasalach/pygmid/blob/main/docs/img/ft.png?raw=true)
 
 ![image](https://github.com/madrasalach/pygmid/blob/main/docs/img/idwVDS.png?raw=true)
 
 ![image](https://github.com/madrasalach/pygmid/blob/main/docs/img/IDWvsgmID.png?raw=true)
 
-### Command Line Interface (CLI)
+The generic PDK data is hosted <a href="https://github.com/bmurmann/Book-on-gm-ID-design">here</a>.
 
-`pygmid` also features a CLI which can be used to run techweeps to generate transistor data
+### Sweeping a Technology
+
+`pygmid` also features a CLI which can be used to run techweeps to generate transistor data.
+
+*Documentation will be added in due course. This functionality is in a state of flux.*
 
 ## Authors
 
 - Cian O'Donnell : cian.odonnell@mcci.ie
 - Tiarnach Ó Riada : tiarnach.oriada@tyndall.ie
 - Danylo Galach
```

#### html2text {}

```diff
@@ -2,50 +2,51 @@
 badge.svg?branch=main) ![PyPI - Downloads](https://img.shields.io/pypi/dm/
 pygmid)
  [https://github.com/madrasalach/pygmid/blob/main/docs/img/icon.png?raw=true]
                                **** pygmid ****
               A python3 implementation of the gm/ID starter kit
                          Report_bug Â· Request_feature
 ## Table of contents - [About](#about) - [Installation](#installation) -
-[Usage](#usage) - [Authors](#authors) ## About pygmid is a Python 3 port of the
-gm/ID starter kit by Prof. Boris Murmann of Stanford University. The package
-also offers some scripts from the Paul Jesper's book. For the gm/ID starter
-kit, written for MATLAB, please refer to the 'Links' section at Prof. Murmann's
-website: https://web.stanford.edu/~murmann. ## Installation To install pygmid
-from source, download from Github and run pip: `pip install .` in the root
-directory. pygmid can also be installed from PyPI: `pip install pygmid` ##
-Usage ### Scripting with the Lookup Class A gm/ID lookup object can be
-generated with the `Lookup` class. The lookup object requires lookup data for
-initialisation. Currently, only `.mat` files are supported. You can create a
-lookup object as follows: ```python from pygmid import Lookup as lk NCH = lk
+[Usage](#usage) - [Authors](#authors) ## About pygmid is a Python 3 version of
+the gm/ID starter kit by Prof. Boris Murmann of Stanford University. The
+package also offers some scripts from the Paul Jesper's book. For the gm/ID
+starter kit, written for MATLAB, please refer to the 'Links' section at Prof.
+Murmann's website: https://web.stanford.edu/~murmann. ## Installation To
+install pygmid from source, download from Github and run pip: `pip install .`
+in the root directory. pygmid can also be installed from PyPI: `pip install
+pygmid` ## Usage ### Scripting with the Lookup Class A gm/ID lookup object can
+be generated with the `Lookup` class. The lookup object requires lookup data
+for initialisation. Currently, only `.mat` files are supported. You can create
+a lookup object as follows: ```python from pygmid import Lookup as lk NCH = lk
 ('180nch.mat') ``` ### Access MOS Data The `Lookup` class allows for pseudo
 array access of the MOS matrix data. You can access data as follows: ```python
 # get VGS data as array from NCH VGS_array = NCH['VGS'] ``` Data is returned as
 a deep copy of the array contained in the `Lookup` object. ### Lookup
 functionality Lookup of interpolated data occurs as follows: ```python VDSs =
 NCH['VDS'] VGSs = np.arange(0.4, 0.6, 0.05) # Plot ID versus VDS ID =
 NCH.look_up('ID', vds=VDSs, vgs=VGSs) # alias function lookup can also be used
 ID = NCH.lookup('ID', vds=VDSs, vgs=VGSs) # check bias VGS = NCH.look_upVGS
 (GM_ID = 10, VDS = 0.6, VSB = 0.1, L = 0.18) print(f'VGS is: {VGS}') plt.plot
-(VDSs, np.transpose(ID)) ``` ~~Currently only lookup modes 1 and 2 are
-implemented.~~ Modes 1 (Simple parameter lookup), mode 2 (arbitrary ratio
-lookup) and mode 3 (cross lookup of ratios) are implemented. The companion
-lookupVGS function is also included. ### Technology Extraction Functions The
-EKV extraction function can be used as follows: ```python from pygmid import
-EKV_param_extraction, XTRACT (VDS, n, VT, JS, d1n, d1VT, d1logJS, d2n, d2VT,
-d2logJS)\ = EKV_param_extraction(NCH, 1, L = 0.18, VDS = 0.6, VSB = 0.0) ```
-Sample usage of this and other utility functions can be found in
-`test_utility.py` . ### Examples Usage of lookup scripts are given in
-`test_lookup.py` and `test_lookupVGS.py`. Sample outputs are given below: !
+(VDSs, np.transpose(ID)) ``` Modes 1 (Simple parameter lookup), mode 2
+(arbitrary ratio lookup) and mode 3 (cross lookup of ratios) are implemented.
+The companion lookupVGS function is also included. ### Technology Extraction
+Functions The EKV extraction function can be used as follows: ```python from
+pygmid import EKV_param_extraction, XTRACT (VDS, n, VT, JS, d1n, d1VT, d1logJS,
+d2n, d2VT, d2logJS)\ = EKV_param_extraction(NCH, 1, L = 0.18, VDS = 0.6, VSB =
+0.0) ``` Sample usage of this and other utility functions can be found in
+`debug_utility.py` . ### Examples Usage of lookup scripts are given in
+`debug_lookup.py` and `debug_lookupVGS.py`. Sample outputs for the 180nm
+generic pdk used in the Murmann starter pack are given below: ![image](https://
+github.com/madrasalach/pygmid/blob/main/docs/img/IDvVDS.png?raw=true) ![image]
+(https://github.com/madrasalach/pygmid/blob/main/docs/img/vtvsL.png?raw=true) !
 [image](https://github.com/madrasalach/pygmid/blob/main/docs/img/
-IDvVDS.png?raw=true) ![image](https://github.com/madrasalach/pygmid/blob/main/
-docs/img/vtvsL.png?raw=true) ![image](https://github.com/madrasalach/pygmid/
-blob/main/docs/img/gm_gds.png?raw=true) ![image](https://github.com/
-madrasalach/pygmid/blob/main/docs/img/ft.png?raw=true) ![image](https://
-github.com/madrasalach/pygmid/blob/main/docs/img/idwVDS.png?raw=true) ![image]
-(https://github.com/madrasalach/pygmid/blob/main/docs/img/
-IDWvsgmID.png?raw=true) ### Command Line Interface (CLI) `pygmid` also features
-a CLI which can be used to run techweeps to generate transistor data ## Authors
-- Cian O'Donnell : cian.odonnell@mcci.ie - Tiarnach Ã Riada :
+gm_gds.png?raw=true) ![image](https://github.com/madrasalach/pygmid/blob/main/
+docs/img/ft.png?raw=true) ![image](https://github.com/madrasalach/pygmid/blob/
+main/docs/img/idwVDS.png?raw=true) ![image](https://github.com/madrasalach/
+pygmid/blob/main/docs/img/IDWvsgmID.png?raw=true) The generic PDK data is
+hosted here. ### Sweeping a Technology `pygmid` also features a CLI which can
+be used to run techweeps to generate transistor data. *Documentation will be
+added in due course. This functionality is in a state of flux.* ## Authors -
+Cian O'Donnell : cian.odonnell@mcci.ie - Tiarnach Ã Riada :
 tiarnach.oriada@tyndall.ie - Danylo Galach ## Contributors - JosÃ© Rui
 CustÃ³dio A special thanks to Prof. Boris Murmann for giving permission to use
 his work and release this package under the Apache 2.0 License.
```

### Comparing `pygmid-1.1.0/setup.cfg` & `pygmid-1.2.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = pygmid
 version = attr: pygmid.__version__
-author = Cian O`Donnell, Danylo Galach, Tiarnach Ó Riada
+author = Cian Ó Domhnaill, Tiarnach Ó Riada, Danylo Galach
 author_email = cian.odonnell@tyndall.ie
 description = A python 3 implementation of the gm/ID starter kit
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 url = https://github.com/madrasalach/pygmid
 project_urls = 
 	Bug Tracker = https://github.com/madrasalach/pygmid/issues
@@ -18,18 +18,22 @@
 	= src
 packages = find:
 python_requires = >=3.4
 setup_requires = 
 	numpy
 	scipy
 	matplotlib
+	psf_utils
+	tqdm
 install_requires = 
 	numpy
 	scipy
 	matplotlib
+	psf_utils
+	tqdm
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `pygmid-1.1.0/src/pygmid/Lookup.py` & `pygmid-1.2.0/src/pygmid/Lookup.py`

 * *Files identical despite different names*

### Comparing `pygmid-1.1.0/src/pygmid/__main__.py` & `pygmid-1.2.0/src/pygmid/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,32 @@
 import logging
 import sys
 
 from .version import __version__
 from . import pygmid
+from . import sweep
 
 def _cli():
     from argparse import ArgumentParser
     description = "CLI for pygmid. Run techsweeps"
     parser = ArgumentParser(description=description)
     parser.add_argument('--version', action='version', version=f"%prog {__version__}")
-    parser.add_argument('-c', action='store_const', dest='constant_value',
-                        const='value-to-store',
-                        help='Store a constant value')
+    parser.add_argument('--mode', choices=['lookup', 'sweep'], default='lookup')
+    parser.add_argument('--config', type=str)
+    parser.add_argument('--skip-run', action="store_true", help="Skip running the simulation, e.g. for testing.")
 
-    results = parser.parse_args()
-    # assign values from results here
-    # val = results.constant_value
-
-    #if opt.backend is not None:
-    #    zookeeper.backend = opt.backend
-    #if opt.configfile is not None:
-    #    zookeeper.configfile = opt.configfile
-
-    #if len(remaining_args) != 0:
-    #    print("Usage: python -m zookeeper [settings] \npython -m zookeeper -h for help")
-    #    sys.exit(1)
-    
-    # setup logger    
-    logging.basicConfig(stream=sys.stdout, level=logging.DEBUG)
-    
-    pygmid.main()
-    sys.exit(0)
+    args = parser.parse_args()
+    if args.mode == 'sweep':
+        if args.config is None:
+            logging.error('Please provide a config file with --config if using the sweep mode')
+            sys.exit(-1)
+        mfn, mfp = sweep.run(args.config, skip_sweep=getattr(args, 'skip_run', False))
+        logging.info(f"Wrote sweep data to files: {mfn} and {mfp}")
+        sys.exit(0)
+    elif args.mode == 'lookup':
+        pygmid.main()
+        sys.exit(0)
+    sys.exit(-1)
         
 if __name__ == '__main__':
-    # setup logger here
+    logging.basicConfig(stream=sys.stdout, level=logging.DEBUG)
     _cli()
```

### Comparing `pygmid-1.1.0/src/pygmid/numerical.py` & `pygmid-1.2.0/src/pygmid/numerical.py`

 * *Files identical despite different names*

### Comparing `pygmid-1.1.0/src/pygmid/utility.py` & `pygmid-1.2.0/src/pygmid/utility.py`

 * *Files identical despite different names*

### Comparing `pygmid-1.1.0/src/pygmid.egg-info/PKG-INFO` & `pygmid-1.2.0/src/pygmid.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pygmid
-Version: 1.1.0
+Version: 1.2.0
 Summary: A python 3 implementation of the gm/ID starter kit
 Home-page: https://github.com/madrasalach/pygmid
-Author: Cian O`Donnell, Danylo Galach, Tiarnach Ó Riada
+Author: Cian Ó Domhnaill, Tiarnach Ó Riada, Danylo Galach
 Author-email: cian.odonnell@tyndall.ie
 Project-URL: Bug Tracker, https://github.com/madrasalach/pygmid/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -36,15 +36,15 @@
 - [About](#about)
 - [Installation](#installation)
 - [Usage](#usage)
 - [Authors](#authors)
 
 ## About
 
-pygmid is a Python 3 port of the gm/ID starter kit by Prof. Boris Murmann 
+pygmid is a Python 3 version of the gm/ID starter kit by Prof. Boris Murmann 
 of Stanford University. The package also offers some scripts from the Paul Jesper's book.
 
 For the gm/ID starter kit, written for MATLAB, please refer to the 'Links'
 section at Prof. Murmann's website: https://web.stanford.edu/~murmann.
 
 ## Installation
 
@@ -94,52 +94,55 @@
 # check bias
 VGS = NCH.look_upVGS(GM_ID = 10, VDS = 0.6, VSB = 0.1, L = 0.18)
 print(f'VGS is: {VGS}')
 
 plt.plot(VDSs, np.transpose(ID))
 ```
 
-~~Currently only lookup modes 1 and 2 are implemented.~~
 Modes 1 (Simple parameter lookup), mode 2 (arbitrary ratio lookup) and mode 3 (cross lookup of ratios) are implemented. The companion lookupVGS function is also included.
 
 ### Technology Extraction Functions
 
 The EKV extraction function can be used as follows:
 
 ```python
 from pygmid import EKV_param_extraction, XTRACT
 
 (VDS, n, VT, JS, d1n, d1VT, d1logJS, d2n, d2VT, d2logJS)\
         = EKV_param_extraction(NCH, 1, L = 0.18, VDS = 0.6, VSB = 0.0)
 
 ```
 
-Sample usage of this and other utility functions can be found in `test_utility.py` .
+Sample usage of this and other utility functions can be found in `debug_utility.py` .
 
 ### Examples
 
-Usage of lookup scripts are given in `test_lookup.py` and `test_lookupVGS.py`.
+Usage of lookup scripts are given in `debug_lookup.py` and `debug_lookupVGS.py`.
 
-Sample outputs are given below:
+Sample outputs for the 180nm generic pdk used in the Murmann starter pack are given below:
 
 ![image](https://github.com/madrasalach/pygmid/blob/main/docs/img/IDvVDS.png?raw=true)
 
 ![image](https://github.com/madrasalach/pygmid/blob/main/docs/img/vtvsL.png?raw=true)
 
 ![image](https://github.com/madrasalach/pygmid/blob/main/docs/img/gm_gds.png?raw=true)
 
 ![image](https://github.com/madrasalach/pygmid/blob/main/docs/img/ft.png?raw=true)
 
 ![image](https://github.com/madrasalach/pygmid/blob/main/docs/img/idwVDS.png?raw=true)
 
 ![image](https://github.com/madrasalach/pygmid/blob/main/docs/img/IDWvsgmID.png?raw=true)
 
-### Command Line Interface (CLI)
+The generic PDK data is hosted <a href="https://github.com/bmurmann/Book-on-gm-ID-design">here</a>.
 
-`pygmid` also features a CLI which can be used to run techweeps to generate transistor data
+### Sweeping a Technology
+
+`pygmid` also features a CLI which can be used to run techweeps to generate transistor data.
+
+*Documentation will be added in due course. This functionality is in a state of flux.*
 
 ## Authors
 
 - Cian O'Donnell : cian.odonnell@mcci.ie
 - Tiarnach Ó Riada : tiarnach.oriada@tyndall.ie
 - Danylo Galach
 
@@ -333,15 +336,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright [yyyy] [name of copyright owner]
+   Copyright [2023] [Cian Ó Domhnail]
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

#### html2text {}

```diff
@@ -1,62 +1,63 @@
-Metadata-Version: 2.1 Name: pygmid Version: 1.1.0 Summary: A python 3
+Metadata-Version: 2.1 Name: pygmid Version: 1.2.0 Summary: A python 3
 implementation of the gm/ID starter kit Home-page: https://github.com/
-madrasalach/pygmid Author: Cian O`Donnell, Danylo Galach, Tiarnach Ã Riada
+madrasalach/pygmid Author: Cian Ã Domhnaill, Tiarnach Ã Riada, Danylo Galach
 Author-email: cian.odonnell@tyndall.ie Project-URL: Bug Tracker, https://
 github.com/madrasalach/pygmid/issues Classifier: Programming Language :: Python
 :: 3 Classifier: Operating System :: OS Independent Requires-Python: >=3.4
 Description-Content-Type: text/markdown License-File: LICENSE ![Tests](https://
 github.com/madrasalach/pygmid/actions/workflows/run-tests.yml/
 badge.svg?branch=main) ![PyPI - Downloads](https://img.shields.io/pypi/dm/
 pygmid)
  [https://github.com/madrasalach/pygmid/blob/main/docs/img/icon.png?raw=true]
                                **** pygmid ****
               A python3 implementation of the gm/ID starter kit
                          Report_bug Â· Request_feature
 ## Table of contents - [About](#about) - [Installation](#installation) -
-[Usage](#usage) - [Authors](#authors) ## About pygmid is a Python 3 port of the
-gm/ID starter kit by Prof. Boris Murmann of Stanford University. The package
-also offers some scripts from the Paul Jesper's book. For the gm/ID starter
-kit, written for MATLAB, please refer to the 'Links' section at Prof. Murmann's
-website: https://web.stanford.edu/~murmann. ## Installation To install pygmid
-from source, download from Github and run pip: `pip install .` in the root
-directory. pygmid can also be installed from PyPI: `pip install pygmid` ##
-Usage ### Scripting with the Lookup Class A gm/ID lookup object can be
-generated with the `Lookup` class. The lookup object requires lookup data for
-initialisation. Currently, only `.mat` files are supported. You can create a
-lookup object as follows: ```python from pygmid import Lookup as lk NCH = lk
+[Usage](#usage) - [Authors](#authors) ## About pygmid is a Python 3 version of
+the gm/ID starter kit by Prof. Boris Murmann of Stanford University. The
+package also offers some scripts from the Paul Jesper's book. For the gm/ID
+starter kit, written for MATLAB, please refer to the 'Links' section at Prof.
+Murmann's website: https://web.stanford.edu/~murmann. ## Installation To
+install pygmid from source, download from Github and run pip: `pip install .`
+in the root directory. pygmid can also be installed from PyPI: `pip install
+pygmid` ## Usage ### Scripting with the Lookup Class A gm/ID lookup object can
+be generated with the `Lookup` class. The lookup object requires lookup data
+for initialisation. Currently, only `.mat` files are supported. You can create
+a lookup object as follows: ```python from pygmid import Lookup as lk NCH = lk
 ('180nch.mat') ``` ### Access MOS Data The `Lookup` class allows for pseudo
 array access of the MOS matrix data. You can access data as follows: ```python
 # get VGS data as array from NCH VGS_array = NCH['VGS'] ``` Data is returned as
 a deep copy of the array contained in the `Lookup` object. ### Lookup
 functionality Lookup of interpolated data occurs as follows: ```python VDSs =
 NCH['VDS'] VGSs = np.arange(0.4, 0.6, 0.05) # Plot ID versus VDS ID =
 NCH.look_up('ID', vds=VDSs, vgs=VGSs) # alias function lookup can also be used
 ID = NCH.lookup('ID', vds=VDSs, vgs=VGSs) # check bias VGS = NCH.look_upVGS
 (GM_ID = 10, VDS = 0.6, VSB = 0.1, L = 0.18) print(f'VGS is: {VGS}') plt.plot
-(VDSs, np.transpose(ID)) ``` ~~Currently only lookup modes 1 and 2 are
-implemented.~~ Modes 1 (Simple parameter lookup), mode 2 (arbitrary ratio
-lookup) and mode 3 (cross lookup of ratios) are implemented. The companion
-lookupVGS function is also included. ### Technology Extraction Functions The
-EKV extraction function can be used as follows: ```python from pygmid import
-EKV_param_extraction, XTRACT (VDS, n, VT, JS, d1n, d1VT, d1logJS, d2n, d2VT,
-d2logJS)\ = EKV_param_extraction(NCH, 1, L = 0.18, VDS = 0.6, VSB = 0.0) ```
-Sample usage of this and other utility functions can be found in
-`test_utility.py` . ### Examples Usage of lookup scripts are given in
-`test_lookup.py` and `test_lookupVGS.py`. Sample outputs are given below: !
+(VDSs, np.transpose(ID)) ``` Modes 1 (Simple parameter lookup), mode 2
+(arbitrary ratio lookup) and mode 3 (cross lookup of ratios) are implemented.
+The companion lookupVGS function is also included. ### Technology Extraction
+Functions The EKV extraction function can be used as follows: ```python from
+pygmid import EKV_param_extraction, XTRACT (VDS, n, VT, JS, d1n, d1VT, d1logJS,
+d2n, d2VT, d2logJS)\ = EKV_param_extraction(NCH, 1, L = 0.18, VDS = 0.6, VSB =
+0.0) ``` Sample usage of this and other utility functions can be found in
+`debug_utility.py` . ### Examples Usage of lookup scripts are given in
+`debug_lookup.py` and `debug_lookupVGS.py`. Sample outputs for the 180nm
+generic pdk used in the Murmann starter pack are given below: ![image](https://
+github.com/madrasalach/pygmid/blob/main/docs/img/IDvVDS.png?raw=true) ![image]
+(https://github.com/madrasalach/pygmid/blob/main/docs/img/vtvsL.png?raw=true) !
 [image](https://github.com/madrasalach/pygmid/blob/main/docs/img/
-IDvVDS.png?raw=true) ![image](https://github.com/madrasalach/pygmid/blob/main/
-docs/img/vtvsL.png?raw=true) ![image](https://github.com/madrasalach/pygmid/
-blob/main/docs/img/gm_gds.png?raw=true) ![image](https://github.com/
-madrasalach/pygmid/blob/main/docs/img/ft.png?raw=true) ![image](https://
-github.com/madrasalach/pygmid/blob/main/docs/img/idwVDS.png?raw=true) ![image]
-(https://github.com/madrasalach/pygmid/blob/main/docs/img/
-IDWvsgmID.png?raw=true) ### Command Line Interface (CLI) `pygmid` also features
-a CLI which can be used to run techweeps to generate transistor data ## Authors
-- Cian O'Donnell : cian.odonnell@mcci.ie - Tiarnach Ã Riada :
+gm_gds.png?raw=true) ![image](https://github.com/madrasalach/pygmid/blob/main/
+docs/img/ft.png?raw=true) ![image](https://github.com/madrasalach/pygmid/blob/
+main/docs/img/idwVDS.png?raw=true) ![image](https://github.com/madrasalach/
+pygmid/blob/main/docs/img/IDWvsgmID.png?raw=true) The generic PDK data is
+hosted here. ### Sweeping a Technology `pygmid` also features a CLI which can
+be used to run techweeps to generate transistor data. *Documentation will be
+added in due course. This functionality is in a state of flux.* ## Authors -
+Cian O'Donnell : cian.odonnell@mcci.ie - Tiarnach Ã Riada :
 tiarnach.oriada@tyndall.ie - Danylo Galach ## Contributors - JosÃ© Rui
 CustÃ³dio A special thanks to Prof. Boris Murmann for giving permission to use
 his work and release this package under the Apache 2.0 License. Apache License
 Version 2.0, January 2004 http://www.apache.org/licenses/ TERMS AND CONDITIONS
 FOR USE, REPRODUCTION, AND DISTRIBUTION 1. Definitions. "License" shall mean
 the terms and conditions for use, reproduction, and distribution as defined by
 Sections 1 through 9 of this document. "Licensor" shall mean the copyright
@@ -178,15 +179,15 @@
 CONDITIONS APPENDIX: How to apply the Apache License to your work. To apply the
 Apache License to your work, attach the following boilerplate notice, with the
 fields enclosed by brackets "[]" replaced with your own identifying
 information. (Don't include the brackets!) The text should be enclosed in the
 appropriate comment syntax for the file format. We also recommend that a file
 or class name and description of purpose be included on the same "printed page"
 as the copyright notice for easier identification within third-party archives.
-Copyright [yyyy] [name of copyright owner] Licensed under the Apache License,
-Version 2.0 (the "License"); you may not use this file except in compliance
-with the License. You may obtain a copy of the License at http://
-www.apache.org/licenses/LICENSE-2.0 Unless required by applicable law or agreed
-to in writing, software distributed under the License is distributed on an "AS
-IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-implied. See the License for the specific language governing permissions and
-limitations under the License.
+Copyright [2023] [Cian Ã Domhnail] Licensed under the Apache License, Version
+2.0 (the "License"); you may not use this file except in compliance with the
+License. You may obtain a copy of the License at http://www.apache.org/
+licenses/LICENSE-2.0 Unless required by applicable law or agreed to in writing,
+software distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See
+the License for the specific language governing permissions and limitations
+under the License.
```

