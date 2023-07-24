# Comparing `tmp/torch_snippets-0.499.9.tar.gz` & `tmp/torch_snippets-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_snippets-0.499.9.tar", last modified: Thu Nov 10 10:02:31 2022, max compression
+gzip compressed data, was "torch_snippets-0.5.tar", last modified: Mon Jul 24 14:55:52 2023, max compression
```

## Comparing `torch_snippets-0.499.9.tar` & `torch_snippets-0.5.tar`

### file list

```diff
@@ -1,47 +1,49 @@
-drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2022-11-10 10:02:31.111435 torch_snippets-0.499.9/
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    11357 2021-12-31 15:06:08.000000 torch_snippets-0.499.9/LICENSE
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1061 2021-12-31 15:06:08.000000 torch_snippets-0.499.9/LICENSE.txt
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      111 2021-12-31 15:06:08.000000 torch_snippets-0.499.9/MANIFEST.in
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     5723 2022-11-10 10:02:31.111589 torch_snippets-0.499.9/PKG-INFO
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     5009 2022-08-28 14:48:04.000000 torch_snippets-0.499.9/README.md
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     2483 2022-11-10 10:02:23.000000 torch_snippets-0.499.9/settings.ini
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       79 2022-11-10 10:02:31.112130 torch_snippets-0.499.9/setup.cfg
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     2001 2022-06-03 13:10:38.000000 torch_snippets-0.499.9/setup.py
-drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2022-11-10 10:02:31.106986 torch_snippets-0.499.9/torch_snippets/
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      240 2022-11-10 10:02:06.000000 torch_snippets-0.499.9/torch_snippets/__init__.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    38859 2022-11-10 10:02:06.000000 torch_snippets-0.499.9/torch_snippets/_modidx.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     5125 2022-09-08 06:13:05.000000 torch_snippets-0.499.9/torch_snippets/_nbdev.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     5464 2022-11-10 10:02:05.000000 torch_snippets-0.499.9/torch_snippets/adapters.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     9446 2022-11-10 10:02:05.000000 torch_snippets-0.499.9/torch_snippets/bb_utils.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1416 2022-11-10 10:02:06.000000 torch_snippets-0.499.9/torch_snippets/bokeh_loader.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1955 2022-11-10 10:02:05.000000 torch_snippets-0.499.9/torch_snippets/charts.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       73 2022-05-07 11:30:59.000000 torch_snippets-0.499.9/torch_snippets/fastcores.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     3953 2022-11-10 10:02:06.000000 torch_snippets-0.499.9/torch_snippets/imgaug_loader.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     3284 2022-11-10 10:02:06.000000 torch_snippets-0.499.9/torch_snippets/inspector.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     6572 2022-11-10 10:02:05.000000 torch_snippets-0.499.9/torch_snippets/interactive_show.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      654 2022-11-10 10:02:05.000000 torch_snippets-0.499.9/torch_snippets/ipython.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      596 2022-11-10 10:02:05.000000 torch_snippets-0.499.9/torch_snippets/load_defaults.py
--rwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    19593 2022-11-06 15:18:28.000000 torch_snippets-0.499.9/torch_snippets/loader.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     3392 2022-11-10 10:02:06.000000 torch_snippets-0.499.9/torch_snippets/logger.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     7567 2022-11-10 10:02:05.000000 torch_snippets-0.499.9/torch_snippets/markup.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      793 2022-11-10 10:02:05.000000 torch_snippets-0.499.9/torch_snippets/misc.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     9672 2022-11-10 10:02:05.000000 torch_snippets-0.499.9/torch_snippets/paths.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1207 2022-11-10 10:02:05.000000 torch_snippets-0.499.9/torch_snippets/pdf_loader.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      601 2022-11-10 10:02:05.000000 torch_snippets-0.499.9/torch_snippets/registry.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     6144 2022-11-10 10:02:05.000000 torch_snippets-0.499.9/torch_snippets/sklegos.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    11830 2022-10-19 12:07:21.000000 torch_snippets-0.499.9/torch_snippets/text_utils.py
-drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2022-11-10 10:02:31.110449 torch_snippets-0.499.9/torch_snippets/thinc_parser/
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2022-11-10 10:02:06.000000 torch_snippets-0.499.9/torch_snippets/thinc_parser/__init__.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1082 2022-10-16 17:20:20.000000 torch_snippets-0.499.9/torch_snippets/thinc_parser/parser.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    13258 2022-11-08 11:22:58.000000 torch_snippets-0.499.9/torch_snippets/torch_loader.py
-drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2022-11-10 10:02:31.111142 torch_snippets-0.499.9/torch_snippets/trainer/
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       23 2022-11-10 10:02:06.000000 torch_snippets-0.499.9/torch_snippets/trainer/__init__.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     6804 2022-11-10 10:02:06.000000 torch_snippets-0.499.9/torch_snippets/trainer/capsule.py
-drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2022-11-10 10:02:31.109819 torch_snippets-0.499.9/torch_snippets.egg-info/
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     5723 2022-11-10 10:02:30.000000 torch_snippets-0.499.9/torch_snippets.egg-info/PKG-INFO
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1120 2022-11-10 10:02:30.000000 torch_snippets-0.499.9/torch_snippets.egg-info/SOURCES.txt
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        1 2022-11-10 10:02:30.000000 torch_snippets-0.499.9/torch_snippets.egg-info/dependency_links.txt
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       20 2022-11-10 10:02:30.000000 torch_snippets-0.499.9/torch_snippets.egg-info/entry_points.txt
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        1 2021-12-31 15:06:08.000000 torch_snippets-0.499.9/torch_snippets.egg-info/not-zip-safe
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      229 2022-11-10 10:02:30.000000 torch_snippets-0.499.9/torch_snippets.egg-info/requires.txt
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       15 2022-11-10 10:02:30.000000 torch_snippets-0.499.9/torch_snippets.egg-info/top_level.txt
+drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-07-24 14:55:52.808132 torch_snippets-0.5/
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    11357 2021-12-31 15:06:08.000000 torch_snippets-0.5/LICENSE
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1062 2023-01-17 16:58:23.000000 torch_snippets-0.5/LICENSE.txt
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      111 2021-12-31 15:06:08.000000 torch_snippets-0.5/MANIFEST.in
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     5689 2023-07-24 14:55:52.808416 torch_snippets-0.5/PKG-INFO
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     4999 2023-01-17 16:58:23.000000 torch_snippets-0.5/README.md
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      860 2023-07-24 14:53:09.000000 torch_snippets-0.5/settings.ini
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       79 2023-07-24 14:55:52.809464 torch_snippets-0.5/setup.cfg
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     2001 2022-06-03 13:10:38.000000 torch_snippets-0.5/setup.py
+drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-07-24 14:55:52.801138 torch_snippets-0.5/torch_snippets/
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      305 2023-07-24 14:55:50.000000 torch_snippets-0.5/torch_snippets/__init__.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    46227 2023-07-24 14:55:50.000000 torch_snippets-0.5/torch_snippets/_modidx.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     4482 2023-01-17 16:58:25.000000 torch_snippets-0.5/torch_snippets/_nbdev.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     6211 2023-07-24 14:55:50.000000 torch_snippets-0.5/torch_snippets/adapters.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    12112 2023-07-24 14:55:50.000000 torch_snippets-0.5/torch_snippets/bb_utils.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1436 2023-07-24 14:55:50.000000 torch_snippets-0.5/torch_snippets/bokeh_loader.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1672 2023-07-24 14:55:50.000000 torch_snippets-0.5/torch_snippets/charts.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1483 2023-07-24 13:12:35.000000 torch_snippets-0.5/torch_snippets/dates.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1206 2023-07-24 14:55:50.000000 torch_snippets-0.5/torch_snippets/decorators.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       73 2022-05-07 11:30:59.000000 torch_snippets-0.5/torch_snippets/fastcores.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     4126 2023-07-24 14:55:50.000000 torch_snippets-0.5/torch_snippets/imgaug_loader.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     3429 2023-07-24 14:55:50.000000 torch_snippets-0.5/torch_snippets/inspector.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     8376 2023-07-24 14:55:50.000000 torch_snippets-0.5/torch_snippets/interactive_show.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     4662 2023-07-24 14:55:50.000000 torch_snippets-0.5/torch_snippets/ipython.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      597 2023-07-24 14:55:50.000000 torch_snippets-0.5/torch_snippets/load_defaults.py
+-rwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    20934 2023-07-24 14:02:41.000000 torch_snippets-0.5/torch_snippets/loader.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     3464 2023-07-24 14:55:50.000000 torch_snippets-0.5/torch_snippets/logger.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     7555 2023-07-24 14:55:50.000000 torch_snippets-0.5/torch_snippets/markup.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1654 2023-07-24 14:55:50.000000 torch_snippets-0.5/torch_snippets/misc.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     9763 2023-07-24 14:55:50.000000 torch_snippets-0.5/torch_snippets/paths.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1370 2023-07-24 14:55:50.000000 torch_snippets-0.5/torch_snippets/pdf_loader.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      822 2023-07-24 14:55:50.000000 torch_snippets-0.5/torch_snippets/registry.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     6144 2023-07-24 14:55:50.000000 torch_snippets-0.5/torch_snippets/sklegos.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    14237 2023-06-10 19:35:22.000000 torch_snippets-0.5/torch_snippets/text_utils.py
+drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-07-24 14:55:52.805593 torch_snippets-0.5/torch_snippets/thinc_parser/
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-07-24 14:55:50.000000 torch_snippets-0.5/torch_snippets/thinc_parser/__init__.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1082 2022-10-16 17:20:20.000000 torch_snippets-0.5/torch_snippets/thinc_parser/parser.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    13258 2022-11-08 11:22:58.000000 torch_snippets-0.5/torch_snippets/torch_loader.py
+drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-07-24 14:55:52.807533 torch_snippets-0.5/torch_snippets/trainer/
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       23 2023-07-24 14:55:50.000000 torch_snippets-0.5/torch_snippets/trainer/__init__.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     6802 2023-07-24 14:55:50.000000 torch_snippets-0.5/torch_snippets/trainer/capsule.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1537 2023-07-24 14:55:50.000000 torch_snippets-0.5/torch_snippets/trainer/config.py
+drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-07-24 14:55:52.804443 torch_snippets-0.5/torch_snippets.egg-info/
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     5689 2023-07-24 14:55:52.000000 torch_snippets-0.5/torch_snippets.egg-info/PKG-INFO
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1165 2023-07-24 14:55:52.000000 torch_snippets-0.5/torch_snippets.egg-info/SOURCES.txt
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        1 2023-07-24 14:55:52.000000 torch_snippets-0.5/torch_snippets.egg-info/dependency_links.txt
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-01-17 16:58:23.000000 torch_snippets-0.5/torch_snippets.egg-info/not-zip-safe
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      272 2023-07-24 14:55:52.000000 torch_snippets-0.5/torch_snippets.egg-info/requires.txt
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       15 2023-07-24 14:55:52.000000 torch_snippets-0.5/torch_snippets.egg-info/top_level.txt
```

### Comparing `torch_snippets-0.499.9/LICENSE` & `torch_snippets-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.499.9/LICENSE.txt` & `torch_snippets-0.5/LICENSE.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 copies or substantial portions of the Software.
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `torch_snippets-0.499.9/PKG-INFO` & `torch_snippets-0.5/torch_snippets.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
-Name: torch_snippets
-Version: 0.499.9
+Name: torch-snippets
+Version: 0.5
 Summary: One line functions for common tasks
 Home-page: https://github.com/sizhky/torch_snippets/tree/master/
 Author: Yeshwanth Reddy
 Author-email: 1992chinna@gmail.com
 License: Apache Software License 2.0
 Keywords: snippets,torch
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.7
@@ -21,15 +20,15 @@
 
 # Utilities for simple needs
 
 
 
 ## torch snippets does a lot of default importing for you
 Whether it is numpy, pandas, matplotlib or the useful functions that are mentioned below
-Simply call 
+Simply call
 ```python
 from torch_snippets import *
 ```
 All the imports are lightweight and thus should not take more than a couple of seconds
 
 ## Auxiliary Functions
 There are simple functions that are overloaded to take inputs and perform repetitive tasks that usually take a few lines to write
@@ -37,44 +36,44 @@
 #### Images
 `show`, `inspect`, `Glob`, `read`, `resize`, `rotate`
 
 #### Files and Paths
 `stem`, `Glob`, `parent`, `name`, `fname`,
 
 
-`makedir`, `zip_files`, `unzip_file`,   
+`makedir`, `zip_files`, `unzip_file`,
 
 
-`find`, `extn`,  
+`find`, `extn`,
 
 
 `readlines`, `writelines`
 
 #### Lists
 `L`, `flatten`
 
 #### Dump and load python objects
 `loaddill`,`dumpdill`
 
-#### Misc 
+#### Misc
 `Tqdm`, `Timer`, `randint`, `Logger`
 
 #### Sets
 `unique`, `diff`, `choose`, `common`
 
 #### Pytorch Modules
 `Reshape` and `Permute` (`nn.Modules`)
 
 #### Report as Pytorch Lightning Callback
 `LightningReport`
 
 #### Charts
 `Chart` from altair
 
-and many more to come... 
+and many more to come...
 
 ## Install
 `pip install torch_snippets`
 
 ## Usage
 
 
@@ -328,11 +327,7 @@
      'with_cast',
      'wrap_class',
      'write',
      'writelines',
      'xywh2xyXY',
      'zip_cycle',
      'zip_files']
-
-
-
-
```

### Comparing `torch_snippets-0.499.9/README.md` & `torch_snippets-0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Utilities for simple needs
 
 
 
 ## torch snippets does a lot of default importing for you
 Whether it is numpy, pandas, matplotlib or the useful functions that are mentioned below
-Simply call 
+Simply call
 ```python
 from torch_snippets import *
 ```
 All the imports are lightweight and thus should not take more than a couple of seconds
 
 ## Auxiliary Functions
 There are simple functions that are overloaded to take inputs and perform repetitive tasks that usually take a few lines to write
@@ -16,44 +16,44 @@
 #### Images
 `show`, `inspect`, `Glob`, `read`, `resize`, `rotate`
 
 #### Files and Paths
 `stem`, `Glob`, `parent`, `name`, `fname`,
 
 
-`makedir`, `zip_files`, `unzip_file`,   
+`makedir`, `zip_files`, `unzip_file`,
 
 
-`find`, `extn`,  
+`find`, `extn`,
 
 
 `readlines`, `writelines`
 
 #### Lists
 `L`, `flatten`
 
 #### Dump and load python objects
 `loaddill`,`dumpdill`
 
-#### Misc 
+#### Misc
 `Tqdm`, `Timer`, `randint`, `Logger`
 
 #### Sets
 `unique`, `diff`, `choose`, `common`
 
 #### Pytorch Modules
 `Reshape` and `Permute` (`nn.Modules`)
 
 #### Report as Pytorch Lightning Callback
 `LightningReport`
 
 #### Charts
 `Chart` from altair
 
-and many more to come... 
+and many more to come...
 
 ## Install
 `pip install torch_snippets`
 
 ## Usage
 
 
@@ -307,9 +307,7 @@
      'with_cast',
      'wrap_class',
      'write',
      'writelines',
      'xywh2xyXY',
      'zip_cycle',
      'zip_files']
-
-
```

### Comparing `torch_snippets-0.499.9/setup.py` & `torch_snippets-0.5/setup.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.499.9/torch_snippets/_modidx.py` & `torch_snippets-0.5/torch_snippets/_modidx.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,16 +10,20 @@
                                          'torch_snippets.adapters._get_attribute_columns': ( 'adapters.html#_get_attribute_columns',
                                                                                              'torch_snippets/adapters.py'),
                                          'torch_snippets.adapters._get_attribute_data': ( 'adapters.html#_get_attribute_data',
                                                                                           'torch_snippets/adapters.py'),
                                          'torch_snippets.adapters._process': ('adapters.html#_process', 'torch_snippets/adapters.py'),
                                          'torch_snippets.adapters.b64_2_file': ('adapters.html#b64_2_file', 'torch_snippets/adapters.py'),
                                          'torch_snippets.adapters.b64_2_np': ('adapters.html#b64_2_np', 'torch_snippets/adapters.py'),
+                                         'torch_snippets.adapters.bytes_2_file': ( 'adapters.html#bytes_2_file',
+                                                                                   'torch_snippets/adapters.py'),
                                          'torch_snippets.adapters.csvs_2_cvat': ('adapters.html#csvs_2_cvat', 'torch_snippets/adapters.py'),
                                          'torch_snippets.adapters.cvat_2_csvs': ('adapters.html#cvat_2_csvs', 'torch_snippets/adapters.py'),
+                                         'torch_snippets.adapters.file_2_bytes': ( 'adapters.html#file_2_bytes',
+                                                                                   'torch_snippets/adapters.py'),
                                          'torch_snippets.adapters.np_2_b64': ('adapters.html#np_2_b64', 'torch_snippets/adapters.py')},
             'torch_snippets.bb_utils': { 'torch_snippets.bb_utils.BB': ('bounding_boxes.html#bb', 'torch_snippets/bb_utils.py'),
                                          'torch_snippets.bb_utils.BB.__add__': ( 'bounding_boxes.html#bb.__add__',
                                                                                  'torch_snippets/bb_utils.py'),
                                          'torch_snippets.bb_utils.BB.__eq__': ( 'bounding_boxes.html#bb.__eq__',
                                                                                 'torch_snippets/bb_utils.py'),
                                          'torch_snippets.bb_utils.BB.__getitem__': ( 'bounding_boxes.html#bb.__getitem__',
@@ -48,20 +52,29 @@
                                          'torch_snippets.bb_utils.BB.remap': ('bounding_boxes.html#bb.remap', 'torch_snippets/bb_utils.py'),
                                          'torch_snippets.bb_utils.BB.shrink_inplace': ( 'bounding_boxes.html#bb.shrink_inplace',
                                                                                         'torch_snippets/bb_utils.py'),
                                          'torch_snippets.bb_utils.bbfy': ('bounding_boxes.html#bbfy', 'torch_snippets/bb_utils.py'),
                                          'torch_snippets.bb_utils.bbs2df': ('bounding_boxes.html#bbs2df', 'torch_snippets/bb_utils.py'),
                                          'torch_snippets.bb_utils.combine_xyXY_to_bb': ( 'bounding_boxes.html#combine_xyxy_to_bb',
                                                                                          'torch_snippets/bb_utils.py'),
+                                         'torch_snippets.bb_utils.compute_distance_matrix': ( 'bounding_boxes.html#compute_distance_matrix',
+                                                                                              'torch_snippets/bb_utils.py'),
+                                         'torch_snippets.bb_utils.compute_distances': ( 'bounding_boxes.html#compute_distances',
+                                                                                        'torch_snippets/bb_utils.py'),
                                          'torch_snippets.bb_utils.compute_eps': ( 'bounding_boxes.html#compute_eps',
                                                                                   'torch_snippets/bb_utils.py'),
                                          'torch_snippets.bb_utils.df2bbs': ('bounding_boxes.html#df2bbs', 'torch_snippets/bb_utils.py'),
                                          'torch_snippets.bb_utils.enlarge_bbs': ( 'bounding_boxes.html#enlarge_bbs',
                                                                                   'torch_snippets/bb_utils.py'),
                                          'torch_snippets.bb_utils.iou': ('bounding_boxes.html#iou', 'torch_snippets/bb_utils.py'),
+                                         'torch_snippets.bb_utils.is_absolute': ( 'bounding_boxes.html#is_absolute',
+                                                                                  'torch_snippets/bb_utils.py'),
+                                         'torch_snippets.bb_utils.is_relative': ( 'bounding_boxes.html#is_relative',
+                                                                                  'torch_snippets/bb_utils.py'),
+                                         'torch_snippets.bb_utils.isin': ('bounding_boxes.html#isin', 'torch_snippets/bb_utils.py'),
                                          'torch_snippets.bb_utils.jitter': ('bounding_boxes.html#jitter', 'torch_snippets/bb_utils.py'),
                                          'torch_snippets.bb_utils.merge_by_bb': ( 'bounding_boxes.html#merge_by_bb',
                                                                                   'torch_snippets/bb_utils.py'),
                                          'torch_snippets.bb_utils.shrink_bbs': ( 'bounding_boxes.html#shrink_bbs',
                                                                                  'torch_snippets/bb_utils.py'),
                                          'torch_snippets.bb_utils.split_bb_to_xyXY': ( 'bounding_boxes.html#split_bb_to_xyxy',
                                                                                        'torch_snippets/bb_utils.py'),
@@ -71,14 +84,19 @@
                                                                                   'torch_snippets/bb_utils.py')},
             'torch_snippets.bokeh_loader': { 'torch_snippets.bokeh_loader.get_bplot': ( 'bokeh_plotting.html#get_bplot',
                                                                                         'torch_snippets/bokeh_loader.py'),
                                              'torch_snippets.bokeh_loader.parse_sz': ( 'bokeh_plotting.html#parse_sz',
                                                                                        'torch_snippets/bokeh_loader.py')},
             'torch_snippets.charts': { 'torch_snippets.charts.confusion_matrix': ( 'charts.html#confusion_matrix',
                                                                                    'torch_snippets/charts.py')},
+            'torch_snippets.dates': {},
+            'torch_snippets.decorators': { 'torch_snippets.decorators.check_kwargs_not_none': ( 'decorators.html#check_kwargs_not_none',
+                                                                                                'torch_snippets/decorators.py'),
+                                           'torch_snippets.decorators.io': ('decorators.html#io', 'torch_snippets/decorators.py'),
+                                           'torch_snippets.decorators.timeit': ('decorators.html#timeit', 'torch_snippets/decorators.py')},
             'torch_snippets.fastcores': {},
             'torch_snippets.imgaug_loader': { 'torch_snippets.imgaug_loader.bbs2imgaugbbs': ( 'imgaug_loader.html#bbs2imgaugbbs',
                                                                                               'torch_snippets/imgaug_loader.py'),
                                               'torch_snippets.imgaug_loader.bw': ( 'imgaug_loader.html#bw',
                                                                                    'torch_snippets/imgaug_loader.py'),
                                               'torch_snippets.imgaug_loader.crop': ( 'imgaug_loader.html#crop',
                                                                                      'torch_snippets/imgaug_loader.py'),
@@ -101,22 +119,40 @@
                                                                                                      'torch_snippets/interactive_show.py'),
                                                  'torch_snippets.interactive_show.ishow': ( 'interactive_show.html#ishow',
                                                                                             'torch_snippets/interactive_show.py'),
                                                  'torch_snippets.interactive_show.plot_graph': ( 'interactive_show.html#plot_graph',
                                                                                                  'torch_snippets/interactive_show.py'),
                                                  'torch_snippets.interactive_show.plot_image': ( 'interactive_show.html#plot_image',
                                                                                                  'torch_snippets/interactive_show.py'),
+                                                 'torch_snippets.interactive_show.to_networkx': ( 'interactive_show.html#to_networkx',
+                                                                                                  'torch_snippets/interactive_show.py'),
                                                  'torch_snippets.interactive_show.tolist': ( 'interactive_show.html#tolist',
                                                                                              'torch_snippets/interactive_show.py'),
                                                  'torch_snippets.interactive_show.tonp': ( 'interactive_show.html#tonp',
                                                                                            'torch_snippets/interactive_show.py'),
                                                  'torch_snippets.interactive_show.viz2': ( 'interactive_show.html#viz2',
                                                                                            'torch_snippets/interactive_show.py')},
-            'torch_snippets.ipython': { 'torch_snippets.ipython.is_in_notebook': ( 'jupyter_notebook.html#is_in_notebook',
-                                                                                   'torch_snippets/ipython.py')},
+            'torch_snippets.ipython': { 'torch_snippets.ipython.backup_this_notebook': ( 'jupyter_notebook.html#backup_this_notebook',
+                                                                                         'torch_snippets/ipython.py'),
+                                        'torch_snippets.ipython.display_dfs_side_by_side': ( 'jupyter_notebook.html#display_dfs_side_by_side',
+                                                                                             'torch_snippets/ipython.py'),
+                                        'torch_snippets.ipython.h1': ('jupyter_notebook.html#h1', 'torch_snippets/ipython.py'),
+                                        'torch_snippets.ipython.h2': ('jupyter_notebook.html#h2', 'torch_snippets/ipython.py'),
+                                        'torch_snippets.ipython.h3': ('jupyter_notebook.html#h3', 'torch_snippets/ipython.py'),
+                                        'torch_snippets.ipython.h4': ('jupyter_notebook.html#h4', 'torch_snippets/ipython.py'),
+                                        'torch_snippets.ipython.h5': ('jupyter_notebook.html#h5', 'torch_snippets/ipython.py'),
+                                        'torch_snippets.ipython.h6': ('jupyter_notebook.html#h6', 'torch_snippets/ipython.py'),
+                                        'torch_snippets.ipython.is_in_notebook': ( 'jupyter_notebook.html#is_in_notebook',
+                                                                                   'torch_snippets/ipython.py'),
+                                        'torch_snippets.ipython.save_notebook': ( 'jupyter_notebook.html#save_notebook',
+                                                                                  'torch_snippets/ipython.py'),
+                                        'torch_snippets.ipython.show_big_dataframe': ( 'jupyter_notebook.html#show_big_dataframe',
+                                                                                       'torch_snippets/ipython.py'),
+                                        'torch_snippets.ipython.shutdown_current_notebook': ( 'jupyter_notebook.html#shutdown_current_notebook',
+                                                                                              'torch_snippets/ipython.py')},
             'torch_snippets.load_defaults': { 'torch_snippets.load_defaults.exists': ( 'load_defautls.html#exists',
                                                                                        'torch_snippets/load_defaults.py'),
                                               'torch_snippets.load_defaults.loadifexists': ( 'load_defautls.html#loadifexists',
                                                                                              'torch_snippets/load_defaults.py')},
             'torch_snippets.loader': {},
             'torch_snippets.logger': { 'torch_snippets.logger.RichHandler.render': ( 'logging.html#richhandler.render',
                                                                                      'torch_snippets/logger.py'),
@@ -165,15 +201,17 @@
                                        'torch_snippets.markup.unpack': ('markups.html#unpack', 'torch_snippets/markup.py'),
                                        'torch_snippets.markup.write_json': ('markups.html#write_json', 'torch_snippets/markup.py'),
                                        'torch_snippets.markup.write_jsonl': ('markups.html#write_jsonl', 'torch_snippets/markup.py'),
                                        'torch_snippets.markup.write_xml': ('markups.html#write_xml', 'torch_snippets/markup.py'),
                                        'torch_snippets.markup.write_yaml': ('markups.html#write_yaml', 'torch_snippets/markup.py')},
             'torch_snippets.misc': { 'torch_snippets.misc.Timer': ('misc.html#timer', 'torch_snippets/misc.py'),
                                      'torch_snippets.misc.Timer.__call__': ('misc.html#timer.__call__', 'torch_snippets/misc.py'),
-                                     'torch_snippets.misc.Timer.__init__': ('misc.html#timer.__init__', 'torch_snippets/misc.py')},
+                                     'torch_snippets.misc.Timer.__init__': ('misc.html#timer.__init__', 'torch_snippets/misc.py'),
+                                     'torch_snippets.misc.io': ('misc.html#io', 'torch_snippets/misc.py'),
+                                     'torch_snippets.misc.timeit': ('misc.html#timeit', 'torch_snippets/misc.py')},
             'torch_snippets.paths': { 'torch_snippets.paths.Glob': ('paths.html#glob', 'torch_snippets/paths.py'),
                                       'torch_snippets.paths.P.Glob': ('paths.html#p.glob', 'torch_snippets/paths.py'),
                                       'torch_snippets.paths.P.cp': ('paths.html#p.cp', 'torch_snippets/paths.py'),
                                       'torch_snippets.paths.P.extn': ('paths.html#p.extn', 'torch_snippets/paths.py'),
                                       'torch_snippets.paths.P.mv': ('paths.html#p.mv', 'torch_snippets/paths.py'),
                                       'torch_snippets.paths.P.read_lines': ('paths.html#p.read_lines', 'torch_snippets/paths.py'),
                                       'torch_snippets.paths.P.rm': ('paths.html#p.rm', 'torch_snippets/paths.py'),
@@ -205,20 +243,23 @@
             'torch_snippets.pdf_loader': { 'torch_snippets.pdf_loader.PDF': ('pdf.html#pdf', 'torch_snippets/pdf_loader.py'),
                                            'torch_snippets.pdf_loader.PDF.__getitem__': ( 'pdf.html#pdf.__getitem__',
                                                                                           'torch_snippets/pdf_loader.py'),
                                            'torch_snippets.pdf_loader.PDF.__init__': ( 'pdf.html#pdf.__init__',
                                                                                        'torch_snippets/pdf_loader.py'),
                                            'torch_snippets.pdf_loader.PDF.__len__': ( 'pdf.html#pdf.__len__',
                                                                                       'torch_snippets/pdf_loader.py'),
+                                           'torch_snippets.pdf_loader.PDF.get_image': ( 'pdf.html#pdf.get_image',
+                                                                                        'torch_snippets/pdf_loader.py'),
                                            'torch_snippets.pdf_loader.PDF.show': ('pdf.html#pdf.show', 'torch_snippets/pdf_loader.py')},
             'torch_snippets.registry': { 'torch_snippets.registry.parse': ('registry.html#parse', 'torch_snippets/registry.py'),
                                          'torch_snippets.registry.parse_and_resolve': ( 'registry.html#parse_and_resolve',
                                                                                         'torch_snippets/registry.py'),
                                          'torch_snippets.registry.parse_string': ( 'registry.html#parse_string',
-                                                                                   'torch_snippets/registry.py')},
+                                                                                   'torch_snippets/registry.py'),
+                                         'torch_snippets.registry.tryeval': ('registry.html#tryeval', 'torch_snippets/registry.py')},
             'torch_snippets.sklegos': { 'torch_snippets.sklegos.Cat2Num': ('sklegos.html#cat2num', 'torch_snippets/sklegos.py'),
                                         'torch_snippets.sklegos.Cat2Num.__init__': ( 'sklegos.html#cat2num.__init__',
                                                                                      'torch_snippets/sklegos.py'),
                                         'torch_snippets.sklegos.Cat2Num.fit': ('sklegos.html#cat2num.fit', 'torch_snippets/sklegos.py'),
                                         'torch_snippets.sklegos.Cat2Num.fit_transform': ( 'sklegos.html#cat2num.fit_transform',
                                                                                           'torch_snippets/sklegos.py'),
                                         'torch_snippets.sklegos.Cat2Num.transform': ( 'sklegos.html#cat2num.transform',
@@ -311,8 +352,24 @@
                                                 'torch_snippets.trainer.capsule.predict': ( 'capsule.html#predict',
                                                                                             'torch_snippets/trainer/capsule.py'),
                                                 'torch_snippets.trainer.capsule.to': ( 'capsule.html#to',
                                                                                        'torch_snippets/trainer/capsule.py'),
                                                 'torch_snippets.trainer.capsule.train': ( 'capsule.html#train',
                                                                                           'torch_snippets/trainer/capsule.py'),
                                                 'torch_snippets.trainer.capsule.validate': ( 'capsule.html#validate',
-                                                                                             'torch_snippets/trainer/capsule.py')}}}
+                                                                                             'torch_snippets/trainer/capsule.py')},
+            'torch_snippets.trainer.config': { 'torch_snippets.trainer.config.DeepLearningConfig': ( 'config.html#deeplearningconfig',
+                                                                                                     'torch_snippets/trainer/config.py'),
+                                               'torch_snippets.trainer.config.DeepLearningConfig.__getitem__': ( 'config.html#deeplearningconfig.__getitem__',
+                                                                                                                 'torch_snippets/trainer/config.py'),
+                                               'torch_snippets.trainer.config.DeepLearningConfig.__repr__': ( 'config.html#deeplearningconfig.__repr__',
+                                                                                                              'torch_snippets/trainer/config.py'),
+                                               'torch_snippets.trainer.config.DeepLearningConfig.from_ini_file': ( 'config.html#deeplearningconfig.from_ini_file',
+                                                                                                                   'torch_snippets/trainer/config.py'),
+                                               'torch_snippets.trainer.config.DeepLearningConfig.keys': ( 'config.html#deeplearningconfig.keys',
+                                                                                                          'torch_snippets/trainer/config.py'),
+                                               'torch_snippets.trainer.config.GenericConfig': ( 'config.html#genericconfig',
+                                                                                                'torch_snippets/trainer/config.py'),
+                                               'torch_snippets.trainer.config.GenericConfig.__init__': ( 'config.html#genericconfig.__init__',
+                                                                                                         'torch_snippets/trainer/config.py'),
+                                               'torch_snippets.trainer.config.GenericConfig.from_ini_file': ( 'config.html#genericconfig.from_ini_file',
+                                                                                                              'torch_snippets/trainer/config.py')}}}
```

### Comparing `torch_snippets-0.499.9/torch_snippets/_nbdev.py` & `torch_snippets-0.5/torch_snippets/_nbdev.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,140 +1,145 @@
 # AUTOGENERATED BY NBDEV! DO NOT EDIT!
 
 __all__ = ["index", "modules", "custom_doc_links", "git_url"]
 
-index = {"np_2_b64": "adapters.ipynb",
-         "b64_2_np": "adapters.ipynb",
-         "b64_2_pdf": "adapters.ipynb",
-         "parse_sz": "bokeh_plotting.ipynb",
-         "get_bplot": "bokeh_plotting.ipynb",
-         "BB": "bounding_boxes.ipynb",
-         "df2bbs": "bounding_boxes.ipynb",
-         "bbs2df": "bounding_boxes.ipynb",
-         "bbfy": "bounding_boxes.ipynb",
-         "jitter": "bounding_boxes.ipynb",
-         "compute_eps": "bounding_boxes.ipynb",
-         "enlarge_bbs": "bounding_boxes.ipynb",
-         "shrink_bbs": "bounding_boxes.ipynb",
-         "randint": "bounding_boxes.ipynb",
-         "iou": "bounding_boxes.ipynb",
-         "split_bb_to_xyXY": "bounding_boxes.ipynb",
-         "combine_xyXY_to_bb": "bounding_boxes.ipynb",
-         "to_relative": "bounding_boxes.ipynb",
-         "to_absolute": "bounding_boxes.ipynb",
-         "to": "capsule.ipynb",
-         "train": "capsule.ipynb",
-         "validate": "capsule.ipynb",
-         "predict": "capsule.ipynb",
-         "Capsule": "capsule.ipynb",
-         "alt": "charts.ipynb",
-         "Chart": "charts.ipynb",
-         "confusion_matrix": "charts.ipynb",
-         "CM": "charts.ipynb",
-         "do": "imgaug_loader.ipynb",
-         "bw": "imgaug_loader.ipynb",
-         "rotate": "imgaug_loader.ipynb",
-         "pad": "imgaug_loader.ipynb",
-         "get_size": "imgaug_loader.ipynb",
-         "rescale": "imgaug_loader.ipynb",
-         "crop": "imgaug_loader.ipynb",
-         "imgaugbbs2bbs": "imgaug_loader.ipynb",
-         "bbs2imgaugbbs": "imgaug_loader.ipynb",
-         "inspect": "inspector.ipynb",
-         "is_in_notebook": "jupyter_notebook.ipynb",
-         "ifexists": "load_defautls.ipynb",
-         "ifnone": "load_defautls.ipynb",
-         "get_console": "logging.ipynb",
-         "console": "logging.ipynb",
-         "print": "logging.ipynb",
-         "render": "logging.ipynb",
-         "logger": "logging.ipynb",
-         "Debug": "logging.ipynb",
-         "Info": "logging.ipynb",
-         "Warn": "logging.ipynb",
-         "Excep": "logging.ipynb",
-         "reset_logger_width": "logging.ipynb",
-         "isnamedtupleinstance": "markups.ipynb",
-         "unpack": "markups.ipynb",
-         "read_json": "markups.ipynb",
-         "write_json": "markups.ipynb",
-         "AttrDict": "registry.ipynb",
-         "pretty_json": "markups.ipynb",
-         "write_jsonl": "markups.ipynb",
-         "read_jsonl": "markups.ipynb",
-         "read_yaml": "markups.ipynb",
-         "write_yaml": "markups.ipynb",
-         "read_xml": "markups.ipynb",
-         "write_xml": "markups.ipynb",
-         "Config": "registry.ipynb",
-         "input_to_str": "paths.ipynb",
-         "output_to_path": "paths.ipynb",
-         "size": "paths.ipynb",
-         "extn": "paths.ipynb",
-         "Glob": "paths.ipynb",
-         "sample": "paths.ipynb",
-         "mv": "paths.ipynb",
-         "cp": "paths.ipynb",
-         "rm": "paths.ipynb",
-         "P": "paths.ipynb",
-         "P.ls": "paths.ipynb",
-         "P.__repr__": "paths.ipynb",
-         "isdir": "paths.ipynb",
-         "makedir": "paths.ipynb",
-         "fname": "paths.ipynb",
-         "fname2": "paths.ipynb",
-         "stem": "paths.ipynb",
-         "stems": "paths.ipynb",
-         "parent": "paths.ipynb",
-         "find": "paths.ipynb",
-         "P.stems": "paths.ipynb",
-         "zip_files": "paths.ipynb",
-         "unzip_file": "paths.ipynb",
-         "md5": "paths.ipynb",
-         "remove_duplicates": "paths.ipynb",
-         "readlines": "paths.ipynb",
-         "read_lines": "paths.ipynb",
-         "writelines": "paths.ipynb",
-         "write_lines": "paths.ipynb",
-         "rename_batch": "paths.ipynb",
-         "dumpdill": "paths.ipynb",
-         "loaddill": "paths.ipynb",
-         "dill": "paths.ipynb",
-         "PDF": "pdf.ipynb",
-         "parse": "registry.ipynb",
-         "parse_and_resolve": "registry.ipynb",
-         "parse_string": "registry.ipynb",
-         "registry": "registry.ipynb",
-         "train_test_split": "sklegos.ipynb",
-         "ColumnSelector": "sklegos.ipynb",
-         "transform": "sklegos.ipynb",
-         "GroupedEstimator": "sklegos.ipynb",
-         "GroupedPredictor": "sklegos.ipynb",
-         "EstimatorTransformer": "sklegos.ipynb",
-         "MakeFrame": "sklegos.ipynb",
-         "ImputeMissingValues": "sklegos.ipynb",
-         "LambdaTransformer": "sklegos.ipynb",
-         "Cat2Num": "sklegos.ipynb",
-         "SplitDateColumn": "sklegos.ipynb"}
-
-modules = ["adapters.py",
-           "bokeh_loader.py",
-           "bb_utils.py",
-           "trainer/capsule.py",
-           "charts.py",
-           "imgaug_loader.py",
-           "inspector.py",
-           "ipython.py",
-           "load_defaults.py",
-           "logger.py",
-           "markup.py",
-           "paths.py",
-           "pdf_loader.py",
-           "registry.py",
-           "sklegos.py"]
+index = {
+    "np_2_b64": "adapters.ipynb",
+    "b64_2_np": "adapters.ipynb",
+    "b64_2_pdf": "adapters.ipynb",
+    "parse_sz": "bokeh_plotting.ipynb",
+    "get_bplot": "bokeh_plotting.ipynb",
+    "BB": "bounding_boxes.ipynb",
+    "df2bbs": "bounding_boxes.ipynb",
+    "bbs2df": "bounding_boxes.ipynb",
+    "bbfy": "bounding_boxes.ipynb",
+    "jitter": "bounding_boxes.ipynb",
+    "compute_eps": "bounding_boxes.ipynb",
+    "enlarge_bbs": "bounding_boxes.ipynb",
+    "shrink_bbs": "bounding_boxes.ipynb",
+    "randint": "bounding_boxes.ipynb",
+    "iou": "bounding_boxes.ipynb",
+    "split_bb_to_xyXY": "bounding_boxes.ipynb",
+    "combine_xyXY_to_bb": "bounding_boxes.ipynb",
+    "to_relative": "bounding_boxes.ipynb",
+    "to_absolute": "bounding_boxes.ipynb",
+    "to": "capsule.ipynb",
+    "train": "capsule.ipynb",
+    "validate": "capsule.ipynb",
+    "predict": "capsule.ipynb",
+    "Capsule": "capsule.ipynb",
+    "alt": "charts.ipynb",
+    "Chart": "charts.ipynb",
+    "confusion_matrix": "charts.ipynb",
+    "CM": "charts.ipynb",
+    "do": "imgaug_loader.ipynb",
+    "bw": "imgaug_loader.ipynb",
+    "rotate": "imgaug_loader.ipynb",
+    "pad": "imgaug_loader.ipynb",
+    "get_size": "imgaug_loader.ipynb",
+    "rescale": "imgaug_loader.ipynb",
+    "crop": "imgaug_loader.ipynb",
+    "imgaugbbs2bbs": "imgaug_loader.ipynb",
+    "bbs2imgaugbbs": "imgaug_loader.ipynb",
+    "inspect": "inspector.ipynb",
+    "is_in_notebook": "jupyter_notebook.ipynb",
+    "ifexists": "load_defautls.ipynb",
+    "ifnone": "load_defautls.ipynb",
+    "get_console": "logging.ipynb",
+    "console": "logging.ipynb",
+    "print": "logging.ipynb",
+    "render": "logging.ipynb",
+    "logger": "logging.ipynb",
+    "Debug": "logging.ipynb",
+    "Info": "logging.ipynb",
+    "Warn": "logging.ipynb",
+    "Excep": "logging.ipynb",
+    "reset_logger_width": "logging.ipynb",
+    "isnamedtupleinstance": "markups.ipynb",
+    "unpack": "markups.ipynb",
+    "read_json": "markups.ipynb",
+    "write_json": "markups.ipynb",
+    "AttrDict": "registry.ipynb",
+    "pretty_json": "markups.ipynb",
+    "write_jsonl": "markups.ipynb",
+    "read_jsonl": "markups.ipynb",
+    "read_yaml": "markups.ipynb",
+    "write_yaml": "markups.ipynb",
+    "read_xml": "markups.ipynb",
+    "write_xml": "markups.ipynb",
+    "Config": "registry.ipynb",
+    "input_to_str": "paths.ipynb",
+    "output_to_path": "paths.ipynb",
+    "size": "paths.ipynb",
+    "extn": "paths.ipynb",
+    "Glob": "paths.ipynb",
+    "sample": "paths.ipynb",
+    "mv": "paths.ipynb",
+    "cp": "paths.ipynb",
+    "rm": "paths.ipynb",
+    "P": "paths.ipynb",
+    "P.ls": "paths.ipynb",
+    "P.__repr__": "paths.ipynb",
+    "isdir": "paths.ipynb",
+    "makedir": "paths.ipynb",
+    "fname": "paths.ipynb",
+    "fname2": "paths.ipynb",
+    "stem": "paths.ipynb",
+    "stems": "paths.ipynb",
+    "parent": "paths.ipynb",
+    "find": "paths.ipynb",
+    "P.stems": "paths.ipynb",
+    "zip_files": "paths.ipynb",
+    "unzip_file": "paths.ipynb",
+    "md5": "paths.ipynb",
+    "remove_duplicates": "paths.ipynb",
+    "readlines": "paths.ipynb",
+    "read_lines": "paths.ipynb",
+    "writelines": "paths.ipynb",
+    "write_lines": "paths.ipynb",
+    "rename_batch": "paths.ipynb",
+    "dumpdill": "paths.ipynb",
+    "loaddill": "paths.ipynb",
+    "dill": "paths.ipynb",
+    "PDF": "pdf.ipynb",
+    "parse": "registry.ipynb",
+    "parse_and_resolve": "registry.ipynb",
+    "parse_string": "registry.ipynb",
+    "registry": "registry.ipynb",
+    "train_test_split": "sklegos.ipynb",
+    "ColumnSelector": "sklegos.ipynb",
+    "transform": "sklegos.ipynb",
+    "GroupedEstimator": "sklegos.ipynb",
+    "GroupedPredictor": "sklegos.ipynb",
+    "EstimatorTransformer": "sklegos.ipynb",
+    "MakeFrame": "sklegos.ipynb",
+    "ImputeMissingValues": "sklegos.ipynb",
+    "LambdaTransformer": "sklegos.ipynb",
+    "Cat2Num": "sklegos.ipynb",
+    "SplitDateColumn": "sklegos.ipynb",
+}
+
+modules = [
+    "adapters.py",
+    "bokeh_loader.py",
+    "bb_utils.py",
+    "trainer/capsule.py",
+    "charts.py",
+    "imgaug_loader.py",
+    "inspector.py",
+    "ipython.py",
+    "load_defaults.py",
+    "logger.py",
+    "markup.py",
+    "paths.py",
+    "pdf_loader.py",
+    "registry.py",
+    "sklegos.py",
+]
 
 doc_url = "https://sizhky.github.io/torch_snippets/"
 
 git_url = "https://github.com/sizhky/torch_snippets/tree/master/"
 
+
 def custom_doc_links(name):
     return None
```

### Comparing `torch_snippets-0.499.9/torch_snippets/adapters.py` & `torch_snippets-0.5/torch_snippets/adapters.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/adapters.ipynb.
 
 # %% auto 0
-__all__ = ['np_2_b64', 'b64_2_np', 'b64_2_file', 'csvs_2_cvat', 'cvat_2_csvs']
+__all__ = ['np_2_b64', 'b64_2_np', 'b64_2_file', 'bytes_2_file', 'file_2_bytes', 'csvs_2_cvat', 'cvat_2_csvs']
 
 # %% ../nbs/adapters.ipynb 2
 import base64, cv2, numpy as np
 from typing import Union
 from .loader import *
 from .paths import P, stems, stem, parent, makedir
 from .markup import write_xml, read_xml, AttrDict
@@ -24,36 +24,59 @@
     img_nparr = np.frombuffer(input, np.uint8)
     img_cv2 = cv2.imdecode(img_nparr, cv2.IMREAD_COLOR)
     img_rgb = cv2.cvtColor(img_cv2, cv2.COLOR_BGR2RGB)
     return img_rgb
 
 
 def b64_2_file(
-    input: str, # base64 encoded string
-    fpath: Union[str, P] # Place where you want to save the file
-    ) -> None:
+    input: str,  # base64 encoded string
+    fpath: Union[str, P],  # Place where you want to save the file
+) -> None:
     """Save a file encoded as a base64 `input` at given `fpath`"""
     with open(fpath, "wb") as pdf_file:
         input = bytes(input, "utf-8")
         input = base64.b64decode(input)
         pdf_file.write(input)
         logger.info(f"wrote pdf file to {fpath}")
 
+
+def bytes_2_file(
+    input: bytes,  # bytes
+    fpath: Union[str, P],  # Place where you want to save the file
+    silent: bool = False,
+) -> None:
+    """Save bytes `input` at given `fpath`"""
+    with open(fpath, "wb") as file_to_write:
+        file_to_write.write(input)
+        if not silent:
+            logger.info(f"wrote pdf file to {fpath}")
+
+
+def file_2_bytes(fpath):
+    with open(fpath, "rb") as f:
+        output = f.read()
+    return output
+
 # %% ../nbs/adapters.ipynb 4
-def _process(df: pd.DataFrame, label_column, default_label):
+def _process(
+    df: pd.DataFrame, label_column="readable_label", default_label="Background"
+):
     df["@xbr"] = df["X"]
     df["@xtl"] = df["x"]
     df["@ybr"] = df["Y"]
     df["@ytl"] = df["y"]
-    if 'text' in df.columns:
-        df['attribute'] = df['text'].map(lambda text: {'@name': "OCR", "#text": text})
     df["@label"] = df[label_column] if label_column in df.columns else default_label
     df["@occluded"] = "0"
     df["@source"] = "manual"
     df["@z_order"] = "0"
+    if "text" in df.columns:
+        df["attribute"] = [
+            [{"@name": "OCR", "#text": text if text == text else ""}]
+            for text in df["text"]
+        ]
     df.drop(
         [
             c
             for c in df.columns
             if c
             not in set(
                 [
@@ -61,50 +84,56 @@
                     "@xtl",
                     "@ybr",
                     "@ytl",
                     "@label",
                     "@occluded",
                     "@source",
                     "@z_order",
-                    'attribute'
+                    "attribute",
                 ]
             )
         ],
         axis=1,
         inplace=True,
     )
     records = df.to_dict(orient="records")
     return records
 
 
-def csvs_2_cvat(images_folder, csvs_folder, xml_output_file, label_column='readable_label', default_label="Background", items=None, extn='png'):
-    if csvs_folder is None:
-        images_folder = P(images_folder)
-    else:
-        images_folder, csvs_folder = [P(_) for _ in [images_folder, csvs_folder]]
-
+def csvs_2_cvat(
+    images_folder,
+    csvs_folder,
+    xml_output_file,
+    items=None,
+    parquet=False,
+    relative_df=True,
+    default_label="Background",
+    extension="jpg",
+):
+    images_folder, csvs_folder = [P(_) for _ in [images_folder, csvs_folder]]
     data = AttrDict({"annotations": {"image": []}})
-    if csvs_folder is None:
-        items = stems(images_folder)
     if items is None:
         items = common(stems(images_folder), stems(csvs_folder))
 
     items = sorted(items)
 
     for ix, item in enumerate(track(items)):
         _ia = _image_annotation = AttrDict({})
-        image = images_folder / f"{item}.{extn}"
-        _ia["@height"], _ia["@width"] = read(image).shape[:2]
-        _ia["@id"] = str(ix)
-        _ia["@name"] = f"{item}.{extn}"
-        if csvs_folder is not None:
-            df = pd.read_csv(f"{csvs_folder}/{item}.csv")
-            _ia["box"] = _process(df, label_column=label_column, default_label=default_label)
+        image = images_folder / f"{item}.{extension}"
+        height, width = read(image).shape[:2]
+        if parquet:
+            df = pd.read_parquet(f"{csvs_folder}/{item}.parquet")
         else:
-            _ia["box"] = []
+            df = pd.read_csv(f"{csvs_folder}/{item}.csv")
+        if relative_df:
+            df = to_absolute(df, height, width)
+        _ia["@height"], _ia["@width"] = height, width
+        _ia["@id"] = str(ix)
+        _ia["@name"] = f"{item}.jpg"
+        _ia["box"] = _process(df, default_label=default_label)
         data.annotations.image.append(_ia)
     write_xml(data, xml_output_file)
 
 
 def _get_attribute_columns(column):
     def _get_columns_from_row(item):
         if item != item:
@@ -131,15 +160,21 @@
         if item:
             return item[0].get("#text", np.nan)
         else:
             return np.nan
 
 
 def _cvat_ann_2_csv(ann):
-    df = pd.DataFrame([a.to_dict() for a in ann.box])
+    if "box" not in ann:
+        return pd.DataFrame()
+    if isinstance(ann.box, AttrDict):
+        rows = [a.to_dict() for a in [ann.box]]
+    else:
+        rows = [a.to_dict() for a in ann.box]
+    df = pd.DataFrame(rows)
     df.rename(
         {
             "@xtl": "x",
             "@ytl": "y",
             "@xbr": "X",
             "@ybr": "Y",
             "@label": "readable_label",
@@ -167,9 +202,7 @@
         try:
             df = _cvat_ann_2_csv(item)
             save_at = f'{csvs_folder}/{stem(item["@name"])}.csv'
             makedir(parent(save_at))
             df.to_csv(save_at, index=False)
         except Exception as e:
             Warn(f'{e} @ {item["@name"]}')
-
-
```

### Comparing `torch_snippets-0.499.9/torch_snippets/bb_utils.py` & `torch_snippets-0.5/torch_snippets/bb_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/bounding_boxes.ipynb.
 
 # %% auto 0
 __all__ = ['randint', 'BB', 'df2bbs', 'bbs2df', 'bbfy', 'jitter', 'compute_eps', 'enlarge_bbs', 'shrink_bbs', 'iou',
-           'split_bb_to_xyXY', 'combine_xyXY_to_bb', 'to_relative', 'to_absolute', 'merge_by_bb']
+           'compute_distance_matrix', 'compute_distances', 'split_bb_to_xyXY', 'combine_xyXY_to_bb', 'is_absolute',
+           'is_relative', 'to_relative', 'to_absolute', 'merge_by_bb', 'isin']
 
 # %% ../nbs/bounding_boxes.ipynb 2
 import numpy as np
 import pandas as pd
 from PIL.Image import Image
 from typing import Tuple
 
 # %% ../nbs/bounding_boxes.ipynb 3
 randint = np.random.randint
 
+
 class BB:
     """A Bounding Box defined by the top-left and bottom-right coordinates"""
+
     def __init__(self, *bb):
         # assert len(bb) == 4, 'expecting a list/tuple of 4 values respectively for (x,y,X,Y)'
         if len(bb) == 4:
             x, y, X, Y = bb
         elif len(bb) == 1:
             ((x, y, X, Y),) = bb
         rel = True if max(x, y, X, Y) < 1 else False
@@ -142,15 +145,14 @@
                 output = [
                     (ix, bb, self.l2(bb, xyfactor=(1, 1000))) for (ix, bb) in other_bbs
                 ]
                 return pd.DataFrame(output, columns="ix,bb,dist".split(","))
             raise NotImplementedError("")
         return sorted(other_bbs, key=lambda obj: self.l2(obj[1]))
 
-
 # %% ../nbs/bounding_boxes.ipynb 8
 def df2bbs(df):
     if "bb" in df.columns:
         try:
             return bbfy(df["bb"].values.tolist())
         except:
             return bbfy(df["bb"].map(lambda x: eval(x)).values.tolist())
@@ -166,15 +168,14 @@
     return [BB(bb) for bb in bbs]
 
 
 def jitter(bbs, noise):
     return [BB(bb).jitter(noise) for bb in bbs]
 
 
-
 def compute_eps(eps):
     if isinstance(eps, tuple):
         if len(eps) == 4:
             epsx, epsy, epsX, epsY = eps
         else:
             epsx, epsy = eps
             epsx, epsy, epsX, epsY = epsx / 2, epsy / 2, epsx / 2, epsy / 2
@@ -212,85 +213,165 @@
     bboxes2 = np.array(bboxes2)
     x11, y11, x12, y12 = np.split(bboxes1, 4, axis=1)
     x21, y21, x22, y22 = np.split(bboxes2, 4, axis=1)
     xA = np.maximum(x11, np.transpose(x21))
     yA = np.maximum(y11, np.transpose(y21))
     xB = np.minimum(x12, np.transpose(x22))
     yB = np.minimum(y12, np.transpose(y22))
-    interArea = np.maximum((xB - xA + 1), 0) * np.maximum((yB - yA + 1), 0)
-    boxAArea = (x12 - x11 + 1) * (y12 - y11 + 1)
-    boxBArea = (x22 - x21 + 1) * (y22 - y21 + 1)
+    interArea = np.maximum((xB - xA), 0) * np.maximum((yB - yA), 0)
+    boxAArea = (x12 - x11) * (y12 - y11)
+    boxBArea = (x22 - x21) * (y22 - y21)
     iou = interArea / (boxAArea + np.transpose(boxBArea) - interArea)
     return iou
 
+
+def compute_distance_matrix(bboxes1, bboxes2):
+    # Convert the bounding box lists to NumPy arrays
+    bboxes1 = np.array(bboxes1)
+    bboxes2 = np.array(bboxes2)
+
+    # Extract the x, y coordinates of the bounding boxes
+    xy1 = bboxes1[:, :2]
+    xy2 = bboxes2[:, :2]
+
+    # Compute the squared Euclidean distances between all pairs of bounding box coordinates
+    distance_matrix = np.sum((xy1[:, np.newaxis] - xy2) ** 2, axis=-1)
+
+    # Take the square root to get the Euclidean distances
+    distance_matrix = np.sqrt(distance_matrix)
+
+    return distance_matrix
+
+
+def compute_distances(df1, df2, shrink_factors=(1, 1)):
+    """Return euclidean distance mxn matrix for all boxes from df1 with all boxes from df2"""
+    sx, sy = shrink_factors
+    bbs1 = np.array(df2bbs(df1)) / np.array([sx, sy, sx, sy])
+    bbs2 = np.array(df2bbs(df2)) / np.array([sx, sy, sx, sy])
+
+    distances = compute_distance_matrix(bbs1, bbs2)
+    return distances
+
 # %% ../nbs/bounding_boxes.ipynb 10
 def split_bb_to_xyXY(df):
     "convert bb column to separate x,y,X,Y columns"
     df = df.copy()
     assert isinstance(df, pd.DataFrame)
-    if all([item in df.columns for item in 'xyXY']):
+    if all([item in df.columns for item in "xyXY"]):
         return df
-    assert 'bb' in df.columns, 'Expecting the df\'s bounding boxes to be in `bb` column'
+    assert "bb" in df.columns, "Expecting the df's bounding boxes to be in `bb` column"
     try:
-        df['bb'] = df['bb'].map(eval)
+        df["bb"] = df["bb"].map(eval)
     except:
         pass
-    df['x'] = df['bb'].map(lambda x: x[0])
-    df['y'] = df['bb'].map(lambda x: x[1])
-    df['X'] = df['bb'].map(lambda x: x[2])
-    df['Y'] = df['bb'].map(lambda x: x[3])
-    df.drop(['bb'], axis=1, inplace=True)
+    df["x"] = df["bb"].map(lambda x: x[0])
+    df["y"] = df["bb"].map(lambda x: x[1])
+    df["X"] = df["bb"].map(lambda x: x[2])
+    df["Y"] = df["bb"].map(lambda x: x[3])
+    df.drop(["bb"], axis=1, inplace=True)
     return df
 
+
 def combine_xyXY_to_bb(df):
     "combine `x,y,X,Y` to `bb` column"
     df = df.copy()
-    assert all([item in df.columns for item in 'xyXY']), "All the columns `x`, `y`, `X`, `Y` should be in df"
-    df['bb'] = df[[*'xyXY']].values.tolist()
-    df.drop([*'xyXY'], inplace=True, axis=1)
+    assert all(
+        [item in df.columns for item in "xyXY"]
+    ), "All the columns `x`, `y`, `X`, `Y` should be in df"
+    df["bb"] = df[[*"xyXY"]].values.tolist()
+    df.drop([*"xyXY"], inplace=True, axis=1)
     return df
-    
+
+
+def is_absolute(df):
+    bbs = df2bbs(df)
+    bbs = np.array(bbs)
+    return bbs.max() > 1.1
+
+
+def is_relative(df):
+    return not is_absolute(df)
+
 
 def to_relative(df, height, width):
+    if is_relative(df):
+        return df
     df = df.copy()
-    if 'x' not in df.columns and 'bb' in df.columns:
+    if "x" not in df.columns and "bb" in df.columns:
         _recombine = True
         df = split_bb_to_xyXY(df)
     else:
         _recombine = False
     df["x"] = df["x"] / width
     df["y"] = df["y"] / height
     df["X"] = df["X"] / width
     df["Y"] = df["Y"] / height
     if _recombine:
         df = combine_xyXY_to_bb(df)
     return df
 
+
 def to_absolute(df, height, width):
+    if is_absolute(df):
+        return df
     df = df.copy()
-    if 'x' not in df.columns and 'bb' in df.columns:
+    if "x" not in df.columns and "bb" in df.columns:
         _recombine = True
         df = split_bb_to_xyXY(df)
     else:
         _recombine = False
-    df["x"] = (df["x"] * width).astype(np.uint16)
-    df["y"] = (df["y"] * height).astype(np.uint16)
-    df["X"] = (df["X"] * width).astype(np.uint16)
-    df["Y"] = (df["Y"] * height).astype(np.uint16)
+    df["x"] = (np.clip(df["x"], 0, 1) * width).astype(np.uint16)
+    df["y"] = (np.clip(df["y"], 0, 1) * height).astype(np.uint16)
+    df["X"] = (np.clip(df["X"], 0, 1) * width).astype(np.uint16)
+    df["Y"] = (np.clip(df["Y"], 0, 1) * height).astype(np.uint16)
     if _recombine:
         df = combine_xyXY_to_bb(df)
     return df
 
-# %% ../nbs/bounding_boxes.ipynb 17
-def merge_by_bb(df1, df2):
-    """Merge df2 columns to df1 by using iou
+# %% ../nbs/bounding_boxes.ipynb 18
+def merge_by_bb(df1, df2, suffixes=("_x", "_y"), iou_threshold=0.1):
+    """Merge df1 columns to df2 by using iou
     Make sure both df1 & df2 are relative or both absolute
     """
-    df1, df2 = [df.copy() for df in [df1, df2]]
+    # df1, df2 = [df.copy().reset_index(drop=True) for df in [df1, df2]]
     assert all([c in df1.columns for c in "xyXY"])
     assert all([c in df2.columns for c in "xyXY"])
     ious = iou(df2bbs(df1), df2bbs(df2))
-    df2["ix"] = ious.argmax(0)
-    df2.drop([*"xyXY"], axis=1, inplace=True)
-    df = pd.merge(df1, df2, left_index=True, right_on="ix")
-    df.drop(["ix"], axis=1, inplace=True)
-    return df
+    _isin = isin(df2bbs(df1), df2bbs(df2), return_matrix=True)
+    _isin_r = isin(df2bbs(df2), df2bbs(df1), return_matrix=True)
+    (ixs, jxs) = np.nonzero(ious)
+    ious = ious[ixs, jxs]
+    _df1 = df1.iloc[ixs]
+    _df1.columns = [f"{c}{suffixes[0]}" for c in df1.columns]
+    _df2 = df2.iloc[jxs]
+    _df2.columns = [f"{c}{suffixes[1]}" for c in df2.columns]
+    output = pd.concat(
+        [
+            _df1.reset_index(names=f"index_{suffixes[0]}"),
+            _df2.reset_index(names=f"index_{suffixes[1]}"),
+        ],
+        axis=1,
+    )
+    output["iou"] = ious
+    output["isin"] = _isin[ixs, jxs]
+    output["isin_r"] = _isin_r.T[ixs, jxs]
+    output = output.query("iou > @iou_threshold")
+    return output
+
+
+def isin(bboxes1, bboxes2, return_matrix=True):
+    """return indexes of those boxes from `bboxes1` that are completely inside `bboxes2`"""
+    bboxes1 = np.array(bboxes1)
+    bboxes2 = np.array(bboxes2)
+    x11, y11, x12, y12 = np.split(bboxes1, 4, axis=1)
+    x21, y21, x22, y22 = np.split(bboxes2, 4, axis=1)
+    xA = np.maximum(x11, np.transpose(x21))
+    yA = np.maximum(y11, np.transpose(y21))
+    xB = np.minimum(x12, np.transpose(x22))
+    yB = np.minimum(y12, np.transpose(y22))
+    interArea = np.maximum((xB - xA + 1), 0) * np.maximum((yB - yA + 1), 0)
+    boxAArea = (x12 - x11 + 1) * (y12 - y11 + 1)
+    output = interArea / boxAArea
+    if return_matrix:
+        return output
+    ixs = np.where(output == 1)[0]
+    return ixs
```

### Comparing `torch_snippets-0.499.9/torch_snippets/bokeh_loader.py` & `torch_snippets-0.5/torch_snippets/bokeh_loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,24 +17,26 @@
     NodesAndLinkedEdges,
     EdgesAndLinkedNodes,
     HoverTool,
     TapTool,
     BoxSelectTool,
 )
 from bokeh.palettes import Spectral7
+import numpy as np
 
 # %% ../nbs/bokeh_plotting.ipynb 3
 def parse_sz(size):
     if isinstance(size, int):
         return size, size
     elif isinstance(size, tuple):
         if len(size) == 2:
             return size
     raise NotImplementedError(f"function is not implemented for {size}")
 
+
 def get_bplot(sz=500, **kwargs):
     h, w = parse_sz(sz)
     output_notebook()
     plot = figure(
         tools=[WheelZoomTool(), PanTool(), BoxZoomTool(), ResetTool()],
         plot_width=w,
         plot_height=h,
```

### Comparing `torch_snippets-0.499.9/torch_snippets/imgaug_loader.py` & `torch_snippets-0.5/torch_snippets/imgaug_loader.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,79 +3,91 @@
 # %% auto 0
 __all__ = ['do', 'bw', 'rotate', 'pad', 'get_size', 'rescale', 'crop', 'imgaugbbs2bbs', 'bbs2imgaugbbs']
 
 # %% ../nbs/imgaug_loader.ipynb 2
 import imgaug.augmenters as iaa
 from imgaug.augmentables.bbs import BoundingBox, BoundingBoxesOnImage
 from .loader import BB, PIL, bbs2df, df2bbs, np, pd, Image
-from .bb_utils import split_bb_to_xyXY, combine_xyXY_to_bb, to_relative, to_absolute
+from torch_snippets.bb_utils import (
+    split_bb_to_xyXY,
+    combine_xyXY_to_bb,
+    to_relative,
+    to_absolute,
+)
 
 # %% ../nbs/imgaug_loader.ipynb 3
-def do(img, bbs, aug, cval=255):
+def do(img, bbs=None, aug=None, cval=255):
     if isinstance(img, PIL.Image.Image):
         _Image = True
         img = np.array(img)
     else:
         _Image = False
+    no_bbs = False
+    if bbs is None:
+        no_bbs = True
+        bbs = []
     H, W = img.shape[:2]
     if isinstance(bbs, pd.DataFrame):
         _df = bbs.copy()
-        _separate = True if 'x' in _df.columns else False
+        _separate = True if "x" in _df.columns else False
         if not _separate:
             _df = split_bb_to_xyXY(_df)
-        _relative = True if _df['x'].max() < 1 else False
+        _relative = True if _df["x"].max() < 1 else False
         if _relative:
             _df = to_absolute(_df, H, W)
         bbs = df2bbs(_df)
-        remaining_columns = [c for c in _df.columns if c not in 'xyXY']
+        remaining_columns = [c for c in _df.columns if c not in "xyXY"]
         __df = _df[remaining_columns]
         _data_frame = True
     else:
         _data_frame = False
 
     bbs = bbs2imgaugbbs(bbs, img)
     img, bbs = aug(images=[img], bounding_boxes=[bbs])
     img, bbs = (img[0], imgaugbbs2bbs(bbs))
     H, W = img.shape[:2]
-    
+
     if _Image:
         img = Image.fromarray(img)
     if _data_frame:
         _df = bbs2df(bbs)
-        __df[[*'xyXY']] = _df.values
+        __df[[*"xyXY"]] = _df.values
         if _relative:
             __df = to_relative(__df, H, W)
         if not _separate:
             __df = combine_xyXY_to_bb(__df)
         bbs = __df
+    if no_bbs:
+        return img
     return img, bbs
 
 
 def bw(img, bbs):
     aug = iaa.Grayscale()
     return do(img, bbs, aug)
 
 
-def rotate(img, bbs, angle, cval=255):
+def rotate(img, bbs=None, angle=None, cval=255):
     aug = iaa.Rotate(angle, cval=cval, fit_output=True)
-    return do(img, bbs, aug)
+    return do(img, bbs=bbs, aug=aug)
 
 
 def pad(img, bbs, sz=None, deltas=None, cval=0):
     if isinstance(img, np.ndarray):
         h, w = img.shape[:2]
     else:
         w, h = img.size
     if sz:
         H, W = sz
         deltas = (H - h) // 2, (W - w) // 2, (H - h) // 2, (W - w) // 2
 
     aug = iaa.Pad(deltas, pad_cval=cval)
     return do(img, bbs, aug)
 
+
 def get_size(sz, h, w):
     if isinstance(sz, (tuple, list)) and isinstance(sz[0], str):
         signal, (H, W) = sz
         assert signal in "at-least,at-most".split(
             ","
         ), "Resize type must be one of `at-least` or `at-most`"
         if signal == "at-least":
@@ -101,14 +113,15 @@
         elif isinstance(H, float):
             H = H * h
         elif isinstance(W, float):
             W = W * h
     H, W = int(H), int(W)
     return H, W
 
+
 def rescale(im, bbs, sz):
     if isinstance(im, PIL.Image.Image):
         to_pil = True
         im = np.array(im)
     else:
         to_pil = False
     h, w = im.shape[:2]
```

### Comparing `torch_snippets-0.499.9/torch_snippets/inspector.py` & `torch_snippets-0.5/torch_snippets/inspector.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,16 +45,18 @@
             inspect(*arr[: kwargs.get("max_items", 5)], depth=depth + 1, **kwargs)
             if len(arr) > kwargs.get("max_items", 5):
                 print(
                     "\t" * (depth + 1)
                     + f"and ... ... {len(arr) - kwargs.get('max_items', 5)} more item(s)"
                 )
 
-        elif (isinstance(arr, dict) and (dict not in kwargs.get("suppress", []))) or hasattr(arr, 'dict'):
-            if hasattr(arr, 'dict'):
+        elif (
+            isinstance(arr, dict) and (dict not in kwargs.get("suppress", []))
+        ) or hasattr(arr, "dict"):
+            if hasattr(arr, "dict"):
                 arr = dcopy(arr).dict()
             print(f"{name}{typ} of {len(arr)} items")
             for ix, (k, v) in enumerate(arr.items()):
                 inspect(v, depth=depth + 1, names=[k])
                 if ix == kwargs.get("max_items", 5) - 1:
                     break
 
@@ -67,22 +69,25 @@
         elif isinstance(arr, pd.DataFrame):
             print(f"{name}{typ}\tShape: {arr.shape}")
 
         elif isinstance(arr, BB):
             info = f"{name}{typ}\t{arr}"
 
         elif hasattr(arr, "shape"):
-            sh, m, M, dtype = arr.shape, arr.min(), arr.max(), arr.dtype
-            try:
-                me = arr.mean()
-            except:
-                me = arr.float().mean()
-            info = f"{name}{typ}\tShape: {sh}\tMin: {m:.3f}\tMax: {M:.3f}\tMean: {me:.3f}\tdtype: {dtype}"
-            if hasattr(arr, "device"):
-                info += f" @ {arr.device}"
+            if isinstance(arr, torch.Tensor):
+                info = arr
+            else:
+                sh, m, M, dtype = arr.shape, arr.min(), arr.max(), arr.dtype
+                try:
+                    me = arr.mean()
+                except:
+                    me = arr.float().mean()
+                info = f"{name}{typ}\tShape: {sh}\tMin: {m:.3f}\tMax: {M:.3f}\tMean: {me:.3f}\tdtype: {dtype}"
+                if hasattr(arr, "device"):
+                    info += f" @ {arr.device}"
             print(info)
 
         elif isinstance(arr, str):
             if len(arr) > 50:
                 arr = arr[:25] + "..." + arr[-25:]
             print(f"{name}{typ} `{arr}`")
         else:
```

### Comparing `torch_snippets-0.499.9/torch_snippets/load_defaults.py` & `torch_snippets-0.5/torch_snippets/load_defaults.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,19 @@
 from .paths import loaddill
 
 from fastcore.basics import ifnone
 
 # %% ../nbs/load_defautls.ipynb 3
 ifnone = ifnone
 
+
 def exists(fpath):
     """Alias for `os.path.exists`"""
     return os.path.exists(fpath)
 
+
 def loadifexists(fpath, default):
-    """Load data from a `dill` file if it exists, else return default value """
+    """Load data from a `dill` file if it exists, else return default value"""
     if exists(fpath):
         return loaddill(fpath)
     else:
         return default
```

### Comparing `torch_snippets-0.499.9/torch_snippets/loader.py` & `torch_snippets-0.5/torch_snippets/loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,37 +65,51 @@
     "Excep",
     "reset_logger_width",
     "display",
     "typedispatch",
     "defaultdict",
     "Counter",
     "dcopy",
+    "patch_to",
 ]
 
+
 from .logger import *
 from .bb_utils import *
 from pathlib import Path
 from fastcore.foundation import L
 from fastcore.dispatch import typedispatch
+from fastcore.basics import patch_to
 
 import glob, numpy as np, pandas as pd, tqdm, os, sys, re
-from IPython.display import display
+from IPython.display import display, display_html
 import PIL
 from PIL import Image
 
 try:
     import torch
     import torch.nn as nn
     from torch import optim
     from torch.nn import functional as F
     from torch.utils.data import Dataset, DataLoader
 
     __all__ += ["torch", "nn", "F", "Dataset", "DataLoader", "optim"]
 except:
+    Warn(
+        "Unable to load torch and dependent libraries from torch-snippets. \n"
+        "Functionalities might be limited. pip install lovely-tensors in case there are torch related errors"
+    )
+
+try:
+    import lovely_tensors as lt
+
+    lt.monkey_patch()
+except:
     ...
+
 import matplotlib  # ; matplotlib.use('Agg')
 import matplotlib.pyplot as plt
 import matplotlib.patheffects as path_effects
 import pdb, datetime
 from typing import Union, Tuple
 
 E = enumerate
@@ -163,14 +177,22 @@
 
 @typedispatch
 def choose(i: set, n=1):
     i = list(i)
     return choose(i, n=n)
 
 
+@typedispatch
+def choose(i: pd.DataFrame, n=1):
+    o = i.sample(n)
+    if n == 1:
+        return o.squeeze()
+    return o
+
+
 rand = lambda n=6: "".join(
     choose(list("1234567890qwertyuiopasdfghjklzxcvbnmQWERTYUIOPASDFGHJKLZXCVBNM"), n=n)
 )
 
 
 randint = lambda high: np.random.randint(high)
 randint = np.random.randint
@@ -207,15 +229,15 @@
         h, w = im.shape[:2]
         x, y, X, Y = BB(bb).absolute((h, w))
     return im.copy()[y:Y, x:X]
 
 
 def rect(im, bb, c=None, th=2):
     c = "g" if c is None else c
-    _d = {"r": (255, 0, 0), "g": (0, 255, 0), "b": (0, 0, 255)}
+    _d = {"r": (255, 0, 0), "g": (0, 255, 0), "b": (0, 0, 255), "y": (255, 0, 255)}
     c = _d[c] if isinstance(c, str) else c
     x, y, X, Y = bb
     cv2.rectangle(im, (x, y), (X, Y), c, th)
 
 
 def B(im, th=180):
     "Binarize Image"
@@ -226,24 +248,38 @@
     "make bw into 3 channels"
     if im.shape == 3:
         return im
     else:
         return np.repeat(im[..., None], 3, 2)
 
 
-def common(a, b):
+def common_old(a, b):
     """Wrapper around set intersection"""
     x = set(a).intersection(set(b))
     logger.opt(depth=1).log(
         "INFO",
         f"{len(x)} items found common from containers of {len(a)} and {len(b)} items respectively",
     )
     return set(sorted(x))
 
 
+def common(*items, silent=True):
+    """Wrapper around set intersection"""
+    x = set(items[0])
+    for item in items[1:]:
+        x = set(item).intersection(x)
+    lens = [str(len(i)) for i in items]
+    if not silent:
+        logger.opt(depth=1).log(
+            "INFO",
+            f"{len(x)} items found common from containers of {', '.join(lens)} items respectively",
+        )
+    return set(sorted(x))
+
+
 def diff(a, b, rev=False, silent=False):
     if not rev:
         o = set(sorted(set(a) - set(b)))
     else:
         o = set(sorted(set(b) - set(a)))
     if not silent:
         logger.opt(depth=1).log("INFO", f"{len(o)} items found to differ")
@@ -288,21 +324,32 @@
     **kwargs,
 ):
     "show an image"
 
     try:
         if isinstance(img, (str, Path)):
             img = read(str(img), 1)
-        if isinstance(img, torch.Tensor):
             img = img.cpu().detach().numpy().copy()
         if isinstance(img, PIL.Image.Image):
             img = np.array(img)
 
     except Exception as e:
         print(e)
+    if isinstance(img, pd.DataFrame):
+        df = img
+        html_str = ""
+        html_str += '<th style="text-align:center"><td style="vertical-align:top">'
+        if title is not None:
+            html_str += f'<h2 style="text-align: center;">{title}</h2>'
+        html_str += df.to_html(max_rows=kwargs.pop("max_rows", 30)).replace(
+            "table", 'table style="display:inline"'
+        )
+        html_str += "</td></th>"
+        display_html(html_str, raw=True)
+        return
     if not isinstance(img, np.ndarray):
         display(img)
         return
 
     if len(img.shape) == 3 and len(img) == 3:
         # this is likely a torch tensor
         img = img.transpose(1, 2, 0)
@@ -326,16 +373,23 @@
     if ax is None:
         fig, ax = plt.subplots(figsize=kwargs.get("figsize", sz))
         _show = True
     else:
         _show = False
 
     if df is not None:
+        if isinstance(df, (str, Path)):
+            df = str(df)
+            df = pd.read_csv(df) if df.endswith("csv") else pd.read_parquet(df)
         try:
-            texts = df[kwargs.pop("text_col", "text")]
+            text_col = kwargs.pop("text_col", "text")
+            if text_col == "ixs":
+                texts = df.index.tolist()
+            else:
+                texts = df[text_col]
         except:
             pass
         bbs = df2bbs(df)  # assumes df has 'x,y,X,Y' columns or a single 'bb' column
     kwargs.pop("text_col") if "text_col" in kwargs else ...
     if isinstance(texts, pd.core.series.Series):
         texts = texts.tolist()
     if confs:
@@ -453,19 +507,23 @@
     if not silent:
         logger.opt(depth=1).log(
             "INFO", f"plotting {len(ims)} images in a grid of {nr}x{nc} @ {figsize}"
         )
     figsize = kwargs.pop("sz", figsize)
     figsize = (figsize, figsize) if isinstance(figsize, int) else figsize
     fig, axes = plt.subplots(nr, nc, figsize=figsize)
+    return_axes = kwargs.pop("return_axes", False)
     axes = axes.flat
     fig.suptitle(kwargs.pop("suptitle", ""))
     dfs = kwargs.pop("dfs", [None] * len(ims))
     bbss = kwargs.pop("bbss", [None] * len(ims))
-    text_cols = kwargs.pop("text_cols", [None] * len(ims))
+    if "text_col" in kwargs:
+        text_cols = [kwargs.pop("text_col")] * len(ims)
+    else:
+        text_cols = kwargs.pop("text_cols", [None] * len(ims))
     titles = titles.split(",") if isinstance(titles, str) else titles
     for ix, (im, ax) in enumerate(zip(ims, axes)):
         show(
             im,
             ax=ax,
             title=titles[ix],
             df=dfs[ix],
@@ -473,14 +531,16 @@
             text_col=text_cols[ix],
             **kwargs,
         )
     blank = np.eye(100) + np.eye(100)[::-1]
     for ax in axes:
         show(blank, ax=ax)
     plt.tight_layout()
+    if return_axes:
+        return axes
     plt.show()
 
 
 class L_old(list):
     def __getitem__(self, keys):
         if isinstance(keys, (int, slice)):
             return list.__getitem__(self, keys)
@@ -657,57 +717,14 @@
     cv2.imwrite(fpath, image)
 
 
 def lzip(*x):
     return list(zip(*x))
 
 
-# def to_absolute(input, shape):
-#     if isinstance(shape, np.ndarray) and shape.ndim >= 2:
-#         shape = shape.shape[:2]
-#     h, w = shape
-#     if isinstance(input, BB):
-#         return input.absolute((h, w))
-#     elif isinstance(input, pd.DataFrame):
-
-#         def _round(x):
-#             return np.round(x.values.astype(np.double)).astype(np.uint16)
-
-#         df = input.copy()
-#         df["x"] = _round(df.x * w)
-#         df["X"] = _round(df.X * w)
-#         df["y"] = _round(df.y * h)
-#         df["Y"] = _round(df.Y * h)
-#         return df
-#     elif isinstance(input, list):
-#         bbs = bbfy(input)
-#         return [bb.absolute((h, w)) for bb in bbs]
-
-
-# def to_relative(input, shape):
-#     if isinstance(shape, np.ndarray) and shape.ndim >= 2:
-#         shape = shape.shape[:2]
-#     h, w = shape
-#     if isinstance(input, BB):
-#         return input.relative((h, w))
-#     elif isinstance(input, pd.DataFrame):
-#         df = input.copy()
-#         df["x"] = df.x / w
-#         df["X"] = df.X / w
-#         df["y"] = df.y / h
-#         df["Y"] = df.Y / h
-#         return df
-#     elif isinstance(input, list):
-#         bbs = bbfy(input)
-#         return [bb.relative((h, w)) for bb in bbs]
-
-
-from fastcore.basics import patch_to
-
-
 @patch_to(L)
 def first(self):
     if len(self) > 0:
         return self[0]
     else:
         return None
 
@@ -736,7 +753,30 @@
         batch = items[head:tail]
         yield batch
         head = tail
 
 
 def toss(frac: float, pass_=True, fail_=False):
     return [fail_, pass_][np.random.uniform() < frac]
+
+
+def phasify(items, n_phases: int):
+    """
+    [Doc generated by AI]
+    Distributes a list of items into multiple phases and returns a list of lists, each containing items from a specific phase.
+
+    Parameters:
+        items (list): A list of items to be distributed among phases.
+        n_phases (int): The number of phases to divide the items into.
+
+    Returns:
+        list: A list of lists, where each sublist contains items assigned to a specific phase.
+
+    Example:
+        items = [1, 2, 3, 4, 5, 6, 7, 8, 9]
+        n_phases = 3
+        result = phasify(items, n_phases)
+        # Output: [[1, 4, 7], [2, 5, 8], [3, 6, 9]]
+    """
+    iterators = defaultdict(L)
+    [iterators[ix % n_phases].append(item) for ix, item in enumerate(items)]
+    return L(iterators.values())
```

### Comparing `torch_snippets-0.499.9/torch_snippets/logger.py` & `torch_snippets-0.5/torch_snippets/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from rich.theme import Theme
 from loguru import logger
 from datetime import datetime
 from fastcore.basics import patch_to
 from rich.logging import RichHandler
 from pathlib import Path
 
-from .ipython import is_in_notebook
+# from torch_snippets.ipython import is_in_notebook
 
 from functools import wraps
 import time
 
 # %% ../nbs/logging.ipynb 3
 def get_console(width=None):
     return Console(
@@ -60,23 +60,25 @@
         path=path,
         line_no=f"{record.funcName}:{record.lineno}",
         link_path=record.pathname if self.enable_link_path else None,
     )
     return log_renderable
 
 
-logger.configure(handlers=[{
-    "sink":RichHandler(
-        rich_tracebacks=True,
-        console=console,
-        tracebacks_show_locals=False
-    ),
-    "format":'<level>{message}</level>',
-    "backtrace": True
-}])
+logger.configure(
+    handlers=[
+        {
+            "sink": RichHandler(
+                rich_tracebacks=True, console=console, tracebacks_show_locals=False
+            ),
+            "format": "<level>{message}</level>",
+            "backtrace": True,
+        }
+    ]
+)
 
 logger = logger
 
 Debug = lambda x, depth=0: logger.opt(depth=depth + 1).log("DEBUG", x)
 Info = lambda x, depth=0: logger.opt(depth=depth + 1).log("INFO", x)
 Warn = lambda x, depth=0: logger.opt(depth=depth + 1).log("WARNING", x)
 Excep = lambda x, depth=0: logger.opt(depth=depth + 1).log("ERROR", x)
@@ -87,14 +89,15 @@
         try:
             handler = logger._core.handlers[handler_id]
             handler._sink._handler.console = get_console(width=width)
             logger.info(f"reset logger's console width to {width}!")
         except:
             ...
 
+
 # Excep("TESTING {1,2,3}")
 # if is_in_notebook():
 #     reset_logger_width(logger, 115)
 # Excep("TESTING {1,2,3}")
 
 # %% ../nbs/logging.ipynb 10
 def enter_exit(func):
```

### Comparing `torch_snippets-0.499.9/torch_snippets/markup.py` & `torch_snippets-0.5/torch_snippets/markup.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,28 +36,29 @@
     elif isnamedtupleinstance(obj):
         return {key: unpack(value) for key, value in obj._asdict().items()}
     elif isinstance(obj, tuple):
         return tuple(unpack(value) for value in obj)
     else:
         return obj
 
+
 class AttrDict(object):
-    """Utility to call a dictionary like an object  
-    FEATURES:  
-    0. Get and Set any key (or a nested key) like it's an object, tab-completion supported  
-    `self.key1.key2[0].key3` ...   
-    1. Keys and Values are recursively parsed as AttrDicts  
-    2. Formatting with self.pretty()  
+    """Utility to call a dictionary like an object
+    FEATURES:
+    0. Get and Set any key (or a nested key) like it's an object, tab-completion supported
+    `self.key1.key2[0].key3` ...
+    1. Keys and Values are recursively parsed as AttrDicts
+    2. Formatting with self.pretty()
     3. Convert everything to dict at any time via `self.to_dict()`
-    3. Recursively drop keys using `self.drop(key)` from a json object  
+    3. Recursively drop keys using `self.drop(key)` from a json object
     4. Recursively call a function on all values at all levels using `map`
 
-    GOTCHAS:  
-    1. Due to enforcing a `self.key` format all integer keys are converted to strings implicitly.   
-    2. You can still call `self[int]` but this internally converts the int to string  
+    GOTCHAS:
+    1. Due to enforcing a `self.key` format all integer keys are converted to strings implicitly.
+    2. You can still call `self[int]` but this internally converts the int to string
     """
 
     def __init__(self, data):
         for name, value in data.items():
             setattr(self, str(name), self._wrap(value))
 
     def items(self):
@@ -78,15 +79,15 @@
         else:
             return AttrDict(value) if isinstance(value, dict) else value
 
     __getitem__ = lambda self, x: getattr(self, str(x))
     __setitem__ = lambda self, k, v: setattr(self, str(k), self._wrap(v))
 
     def update(self, dict):
-        for k,v in dict.items():
+        for k, v in dict.items():
             self[k] = v
 
     def get(self, key, default=None):
         key = str(key)
         return self[key] if key in self else default
 
     def __iter__(self):
@@ -148,17 +149,19 @@
             self.to_dict(), print_with_logger=print_with_logger, *args, **kwargs
         )
 
     def __eq__(self, other):
         return AttrDict(other).to_dict() == self.to_dict()
 
 
-def pretty_json(i, fpath=None, indent=4, print_with_logger=True, return_as_string=False):
+def pretty_json(
+    i, fpath=None, indent=4, print_with_logger=True, return_as_string=False
+):
     def set_default(obj):
-        if isinstance(obj, (set, BB)):
+        if isinstance(obj, (set, BB, L)):
             return list(obj)
         if isinstance(obj, np.ndarray):
             return obj.tolist()
         if isinstance(obj, P):
             return str(obj)
 
     assert isinstance(i, (dict, list))
@@ -173,15 +176,14 @@
     if print_with_logger:
         return logger.opt(depth=1).log("DEBUG", f"\n{dump}")
     else:
         if return_as_string:
             return dump
         print(dump)
 
-
 # %% ../nbs/markups.ipynb 7
 def read_json(fpath):
     import json
 
     with open(fpath, "r") as f:
         return json.load(f)
 
@@ -195,21 +197,21 @@
     if not silent:
         logger.opt(depth=1).log("DEBUG", f"Dumping json to {fpath}")
     with open(fpath, "w") as f:
         json.dump(obj, f, indent=4, default=set_default)
     return P(fpath)
 
 # %% ../nbs/markups.ipynb 9
-def write_jsonl(items, dest, mode='w'):
+def write_jsonl(items, dest, mode="w"):
     makedir(parent(dest))
     with jsonlines.open(dest, mode) as writer:
         writer.write_all(items)
-        if mode == 'a':
+        if mode == "a":
             Info(f"Appended {len(items)} items to {dest}")
-        elif mode == 'w':
+        elif mode == "w":
             Info(f"Wrote {len(items)} jsons to {dest}")
 
 
 def read_jsonl(file):
     return [json.loads(line) for line in readlines(file, silent=True)]
 
 # %% ../nbs/markups.ipynb 10
```

### Comparing `torch_snippets-0.499.9/torch_snippets/paths.py` & `torch_snippets-0.5/torch_snippets/paths.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,26 @@
 # %% auto 0
 __all__ = ['P', 'dill', 'input_to_str', 'output_to_path', 'isdir', 'makedir', 'fname', 'fname2', 'stem', 'stems', 'parent',
            'extn', 'Glob', 'find', 'zip_files', 'unzip_file', 'list_zip', 'md5', 'remove_duplicates', 'readlines',
            'writelines', 'rename_batch', 'dumpdill', 'loaddill']
 
 # %% ../nbs/paths.ipynb 2
 from fastcore.basics import patch_to
+from fastcore.foundation import L
 from functools import wraps
-from .loader import choose as ts_choose, Tqdm, os, logger, Info, Debug, Warn, Excep
+from torch_snippets.loader import (
+    choose as ts_choose,
+    Tqdm,
+    os,
+    logger,
+    Info,
+    Debug,
+    Warn,
+    Excep,
+)
 from pathlib import Path
 import hashlib, shutil
 import glob
 import dill, time
 
 # %% ../nbs/paths.ipynb 3
 def input_to_str(func):
@@ -39,29 +49,28 @@
                 out = [P(o) for o in out]
         return out
 
     return inner
 
 # %% ../nbs/paths.ipynb 4
 P = Path
-P.ls = lambda self: list(self.iterdir())
+P.ls = lambda self: L(self.iterdir())
 P.__repr__ = lambda self: f"» {self}"
 
 
 @patch_to(P)
 def rmtree(self, prompt="Really remove `{self}` and its contents? [y/n] ", force=False):
     if force:
         shutil.rmtree(self)
     elif prompt and input(prompt.format(self=self)).lower() == "y":
         shutil.rmtree(self)
     else:
         raise OSError(f"{self} exists and is not empty")
 
 
-
 @patch_to(P)
 def size(self):
     if self.is_dir():
         raise Exception(f"`{self}` is a directory")
     fsize = os.path.getsize(self) >> 20
     fsize = f"{fsize} MB" if fsize > 0 else f"{os.path.getsize(self) >> 10} KB"
     return fsize
@@ -70,15 +79,15 @@
 @patch_to(P)
 def extn(self, pattern="*"):
     return self.suffix.replace(".", "")
 
 
 @patch_to(P)
 def Glob(self, pattern="*"):
-    return list(self.glob(pattern))
+    return L(self.glob(pattern))
 
 
 @patch_to(P)
 def sample(self, pattern="*"):
     return ts_choose(self.Glob(pattern))
 
 
@@ -93,20 +102,21 @@
 
 @patch_to(P)
 def cp(self, to):
     return P(shutil.copy(self, to))
 
 
 @patch_to(P)
-def rm(self, confirm_prompt="Are you sure you want to delete `{self}`? [y/N]", silent=True, missing_ok=True):
-    confirm = (
-        input(confirm_prompt.format(self=self))
-        if confirm_prompt
-        else "y"
-    )
+def rm(
+    self,
+    confirm_prompt="Are you sure you want to delete `{self}`? [y/N]",
+    silent=True,
+    missing_ok=True,
+):
+    confirm = input(confirm_prompt.format(self=self)) if confirm_prompt else "y"
     if confirm.lower() == "y":
         if missing_ok:
             try:
                 os.remove(self)
             except:
                 ...
         else:
@@ -120,19 +130,19 @@
 # %% ../nbs/paths.ipynb 20
 def isdir(fpath):
     return os.path.isdir(fpath)
 
 
 @input_to_str
 def makedir(x, prompt=False, silent=True):
-    create = input(f'Creating folder {x}. Are you sure? [y/n]') if prompt else 'y'
+    create = input(f"Creating folder {x}. Are you sure? [y/n]") if prompt else "y"
     if create:
         os.makedirs(x, exist_ok=True)
     if not silent:
-        Info(f'Created folder {x}')
+        Info(f"Created folder {x}")
 
 
 @input_to_str
 def fname(fpath):
     return fpath.split("/")[-1]
 
 
@@ -148,16 +158,18 @@
 @input_to_str
 def stems(folder, silent=False):
     if isinstance(folder, (str, P)):
         return [stem(str(x)) for x in Glob(folder, silent=silent)]
     if isinstance(folder, list):
         return [stem(x) for x in folder]
 
+
 P.stems = lambda self: stems(self.ls())
 
+
 @input_to_str
 @output_to_path
 def parent(fpath):
     out = "/".join(fpath.split("/")[:-1])
     if out == "":
         return "./"
     else:
@@ -213,14 +225,15 @@
         else:
             return filtered_items
 
 # %% ../nbs/paths.ipynb 22
 import zipfile
 import tarfile
 
+
 def zip_files(list_of_files, dest):
     dest = str(dest)
     logger.info(f"Zipping {len(list_of_files)} files to {dest}...")
     if dest.lower().endswith(".zip"):
         with zipfile.ZipFile(dest, "w") as zipMe:
             for file in Tqdm(list_of_files):
                 zipMe.write(file, compress_type=zipfile.ZIP_DEFLATED)
@@ -237,23 +250,23 @@
         with zipfile.ZipFile(file, "r") as zip_ref:
             zip_ref.extractall(dest)
     elif file.lower().endswith(".tar.xz") or file.endswith(".tar.gz"):
         with tarfile.open(file, "r") as f:
             f.extractall(dest)
     return P(dest)
 
+
 def list_zip(file):
     elements = []
     with zipfile.ZipFile(file, "r") as zipObj:
         listOfiles = zipObj.namelist()
         for elem in listOfiles:
             elements.append(elem)
     return elements
 
-
 # %% ../nbs/paths.ipynb 24
 def md5(fname):
     hash_md5 = hashlib.md5()
     with open(fname, "rb") as f:
         for chunk in iter(lambda: f.read(4096), b""):
             hash_md5.update(chunk)
     return hash_md5.hexdigest()
@@ -284,33 +297,33 @@
 
 
 @patch_to(P)
 def read_lines(self, silent=False, encoding=None):
     return readlines(self, silent=silent, encoding=encoding)
 
 
-def writelines(lines, file):
+def writelines(lines, file, mode="w"):
     makedir(parent(file))
     failed = []
-    with open(file, "w") as f:
+    with open(file, mode) as f:
         for line in lines:
             try:
                 f.write(f"{line}\n")
             except:
                 failed.append(line)
     if failed != []:
         logger.opt(depth=1).log(
             "INFO", f"Failed to write {len(failed)} lines out of {len(lines)}"
         )
         return failed
 
 
 @patch_to(P)
-def write_lines(self, lines):
-    return writelines(lines, self)
+def write_lines(self, lines, mode):
+    return writelines(lines, self, mode)
 
 # %% ../nbs/paths.ipynb 28
 def rename_batch(folder, func, debug=False, one_file=False):
     from torch_snippets.loader import now
 
     "V.V.Imp: Use debug=True first to confirm file name changes are as expected"
     if isinstance(folder, (str, P)):
```

### Comparing `torch_snippets-0.499.9/torch_snippets/pdf_loader.py` & `torch_snippets-0.5/torch_snippets/pdf_loader.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/pdf.ipynb.
 
 # %% auto 0
 __all__ = ['PDF']
 
 # %% ../nbs/pdf.ipynb 2
-from .loader import np, subplots, show, resize, L
-
-try:
-    from pdf2image import convert_from_path
-except:
-    ...
+from .loader import np, subplots, show, resize, L, Image
+import fitz
 
 # %% ../nbs/pdf.ipynb 3
 class PDF:
     """Load a PDF file from `path` as a list of images
-    Use `show` function to see the images  
+    Use `show` function to see the images
     **WIP**"""
-    def __init__(self, path, bbss=None):
+
+    def __init__(self, path, dfs=None):
         self.path = path
-        self.ims = convert_from_path(path)
-        self.ims = L([resize(np.array(im), 1.5) for im in self.ims])
-        self.bbss = L(bbss) if bbss is not None else L([None] * len(self))
+        self.doc = fitz.open(path)
+        self.ims = L([self.get_image(page_no) for page_no in range(len(self))])
+        self.dfs = L(dfs) if dfs is not None else L([None] * len(self))
+
+    def get_image(self, page_no):
+        page = self.doc.load_page(page_no)
+        pix = page.get_pixmap(dpi=150)
+        mode = "RGBA" if pix.alpha else "RGB"
+        img = Image.frombytes(mode, [pix.width, pix.height], pix.samples)
+        return img
 
     def __len__(self):
-        return len(self.ims)
+        return len(self.doc)
 
     def __getitem__(self, ix):
         return self.ims[ix]
 
     def show(self, ix=None, ixs=None, **kwargs):
         if ixs is not None:
             assert isinstance(ixs, (list, L))
-            subplots(L(self.ims)[ixs], bbss=self.bbss[ixs], **kwargs)
+            subplots(L(self.ims)[ixs], **kwargs)
         if ix is not None:
-            show(self.ims[ix], bbs=self.bbss[ix], **kwargs)
+            show(self.ims[ix], **kwargs)
             return
 
         if len(self) == 1:
-            show(self.ims[0], bbs=self.bbss[0], **kwargs)
+            show(self.ims[0], df=self.dfs[0], **kwargs)
         else:
-            subplots(self.ims, bbss=self.bbss, **kwargs)
+            subplots(self.ims, dfs=self.dfs, **kwargs)
```

### Comparing `torch_snippets-0.499.9/torch_snippets/sklegos.py` & `torch_snippets-0.5/torch_snippets/sklegos.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.499.9/torch_snippets/text_utils.py` & `torch_snippets-0.5/torch_snippets/text_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 __all__ = [
     "textify",
     "find_lines",
     "find_blocks",
     "find_substring",
     "get_line_data_from_word_data",
+    "edit_distance_path",
+    "group_blocks",
 ]
 import string
 
 import pandas as pd, numpy as np
 from fuzzywuzzy import fuzz
 from sklearn.cluster import dbscan
 from statistics import mean
@@ -375,7 +377,87 @@
             "X": max,
             "Y": max,
             "text": lambda x: " ".join(x),
             **{c: lambda x: list(x) for c in df.columns if c not in [*"xyXY", "text"]},
         }
     )
     return df
+
+
+def edit_distance_path(string1, string2):
+    if string1 is None or string2 is None:
+        return -1, []
+    m = len(string1)
+    n = len(string2)
+
+    # Create a matrix to store the edit distances
+    distance_matrix = [[0] * (n + 1) for _ in range(m + 1)]
+
+    # Initialize the first row and column
+    for i in range(m + 1):
+        distance_matrix[i][0] = i
+    for j in range(n + 1):
+        distance_matrix[0][j] = j
+
+    # Calculate the edit distances
+    for i in range(1, m + 1):
+        for j in range(1, n + 1):
+            if string1[i - 1] == string2[j - 1]:
+                distance_matrix[i][j] = distance_matrix[i - 1][j - 1]
+            else:
+                distance_matrix[i][j] = min(
+                    distance_matrix[i - 1][j] + 1,  # deletion
+                    distance_matrix[i][j - 1] + 1,  # insertion
+                    distance_matrix[i - 1][j - 1] + 1,  # substitution
+                )
+
+    # Trace back the edit distance path
+    i = m
+    j = n
+    path = []
+
+    while i > 0 and j > 0:
+        if string1[i - 1] == string2[j - 1]:
+            path.append((string1[i - 1], string2[j - 1], ""))
+            i -= 1
+            j -= 1
+        else:
+            if distance_matrix[i][j] == distance_matrix[i - 1][j] + 1:
+                path.append((string1[i - 1], "", "delete"))
+                i -= 1
+            elif distance_matrix[i][j] == distance_matrix[i][j - 1] + 1:
+                path.append(("", string2[j - 1], "insert"))
+                j -= 1
+            else:
+                path.append((string1[i - 1], string2[j - 1], "replace"))
+                i -= 1
+                j -= 1
+
+    while i > 0:
+        path.append((string1[i - 1], "", "delete"))
+        i -= 1
+
+    while j > 0:
+        path.append(("", string2[j - 1], "insert"))
+        j -= 1
+
+    # Reverse the path to get the correct order
+    path.reverse()
+
+    return distance_matrix[m][n], path
+
+
+def group_blocks(df):
+    output = []
+    for block, _df in df.groupby("line_block"):
+        texts = [t for t in _df.text if isinstance(t, str)]
+        _block = {
+            "text": " ".join(texts),
+            "x": _df.x.min(),
+            "y": _df.y.min(),
+            "X": _df.X.max(),
+            "Y": _df.Y.max(),
+            "line_block": block,
+        }
+        output.append(_block)
+    output = pd.DataFrame(output)
+    return output
```

### Comparing `torch_snippets-0.499.9/torch_snippets/thinc_parser/parser.py` & `torch_snippets-0.5/torch_snippets/thinc_parser/parser.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.499.9/torch_snippets/torch_loader.py` & `torch_snippets-0.5/torch_snippets/torch_loader.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.499.9/torch_snippets/trainer/capsule.py` & `torch_snippets-0.5/torch_snippets/trainer/capsule.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,14 @@
         args = self.before_predict(args)
         kwargs = self.before_predict(kwargs)
         outputs = predict_function(self, *args, **kwargs)
         return outputs
 
     return _predict
 
-
 # %% ../../nbs/capsule.ipynb 4
 class Capsule(nn.Module):
     """
     Inherit from Capsule and train with fewer lines of code
     """
 
     def __init__(self, report=None):
@@ -224,8 +223,7 @@
         return {"loss": loss}
 
     @predict
     def predict_batch(self, data):
         x, _ = data
         outputs = self(x)
         return outputs
-
```

### Comparing `torch_snippets-0.499.9/torch_snippets.egg-info/PKG-INFO` & `torch_snippets-0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
-Name: torch-snippets
-Version: 0.499.9
+Name: torch_snippets
+Version: 0.5
 Summary: One line functions for common tasks
 Home-page: https://github.com/sizhky/torch_snippets/tree/master/
 Author: Yeshwanth Reddy
 Author-email: 1992chinna@gmail.com
 License: Apache Software License 2.0
 Keywords: snippets,torch
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.7
@@ -21,15 +20,15 @@
 
 # Utilities for simple needs
 
 
 
 ## torch snippets does a lot of default importing for you
 Whether it is numpy, pandas, matplotlib or the useful functions that are mentioned below
-Simply call 
+Simply call
 ```python
 from torch_snippets import *
 ```
 All the imports are lightweight and thus should not take more than a couple of seconds
 
 ## Auxiliary Functions
 There are simple functions that are overloaded to take inputs and perform repetitive tasks that usually take a few lines to write
@@ -37,44 +36,44 @@
 #### Images
 `show`, `inspect`, `Glob`, `read`, `resize`, `rotate`
 
 #### Files and Paths
 `stem`, `Glob`, `parent`, `name`, `fname`,
 
 
-`makedir`, `zip_files`, `unzip_file`,   
+`makedir`, `zip_files`, `unzip_file`,
 
 
-`find`, `extn`,  
+`find`, `extn`,
 
 
 `readlines`, `writelines`
 
 #### Lists
 `L`, `flatten`
 
 #### Dump and load python objects
 `loaddill`,`dumpdill`
 
-#### Misc 
+#### Misc
 `Tqdm`, `Timer`, `randint`, `Logger`
 
 #### Sets
 `unique`, `diff`, `choose`, `common`
 
 #### Pytorch Modules
 `Reshape` and `Permute` (`nn.Modules`)
 
 #### Report as Pytorch Lightning Callback
 `LightningReport`
 
 #### Charts
 `Chart` from altair
 
-and many more to come... 
+and many more to come...
 
 ## Install
 `pip install torch_snippets`
 
 ## Usage
 
 
@@ -328,11 +327,7 @@
      'with_cast',
      'wrap_class',
      'write',
      'writelines',
      'xywh2xyXY',
      'zip_cycle',
      'zip_files']
-
-
-
-
```

### Comparing `torch_snippets-0.499.9/torch_snippets.egg-info/SOURCES.txt` & `torch_snippets-0.5/torch_snippets.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 torch_snippets/__init__.py
 torch_snippets/_modidx.py
 torch_snippets/_nbdev.py
 torch_snippets/adapters.py
 torch_snippets/bb_utils.py
 torch_snippets/bokeh_loader.py
 torch_snippets/charts.py
+torch_snippets/dates.py
+torch_snippets/decorators.py
 torch_snippets/fastcores.py
 torch_snippets/imgaug_loader.py
 torch_snippets/inspector.py
 torch_snippets/interactive_show.py
 torch_snippets/ipython.py
 torch_snippets/load_defaults.py
 torch_snippets/loader.py
@@ -27,15 +29,15 @@
 torch_snippets/registry.py
 torch_snippets/sklegos.py
 torch_snippets/text_utils.py
 torch_snippets/torch_loader.py
 torch_snippets.egg-info/PKG-INFO
 torch_snippets.egg-info/SOURCES.txt
 torch_snippets.egg-info/dependency_links.txt
-torch_snippets.egg-info/entry_points.txt
 torch_snippets.egg-info/not-zip-safe
 torch_snippets.egg-info/requires.txt
 torch_snippets.egg-info/top_level.txt
 torch_snippets/thinc_parser/__init__.py
 torch_snippets/thinc_parser/parser.py
 torch_snippets/trainer/__init__.py
-torch_snippets/trainer/capsule.py
+torch_snippets/trainer/capsule.py
+torch_snippets/trainer/config.py
```

