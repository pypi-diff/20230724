# Comparing `tmp/mkdocs-plotly-plugin-0.1.2.tar.gz` & `tmp/mkdocs-plotly-plugin-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-plotly-plugin-0.1.2.tar", last modified: Fri Jan 20 19:03:17 2023, max compression
+gzip compressed data, was "mkdocs-plotly-plugin-0.1.3.tar", last modified: Mon Jul 24 15:05:59 2023, max compression
```

## Comparing `mkdocs-plotly-plugin-0.1.2.tar` & `mkdocs-plotly-plugin-0.1.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-01-20 19:03:17.113928 mkdocs-plotly-plugin-0.1.2/
--rw-rw-rw-   0        0        0     1084 2023-01-19 06:37:59.000000 mkdocs-plotly-plugin-0.1.2/LICENSE
--rw-rw-rw-   0        0        0       92 2023-01-20 07:54:07.000000 mkdocs-plotly-plugin-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3733 2023-01-20 19:03:17.113928 mkdocs-plotly-plugin-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2954 2023-01-20 19:02:25.000000 mkdocs-plotly-plugin-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-01-20 19:03:17.089927 mkdocs-plotly-plugin-0.1.2/mkdocs_plotly_plugin/
--rw-rw-rw-   0        0        0        0 2023-01-19 06:37:59.000000 mkdocs-plotly-plugin-0.1.2/mkdocs_plotly_plugin/__init__.py
--rw-rw-rw-   0        0        0      645 2023-01-19 21:16:24.000000 mkdocs-plotly-plugin-0.1.2/mkdocs_plotly_plugin/fences.py
-drwxrwxrwx   0        0        0        0 2023-01-20 19:03:17.104927 mkdocs-plotly-plugin-0.1.2/mkdocs_plotly_plugin/javascripts/
--rw-rw-rw-   0        0        0     3519 2023-01-20 07:08:30.000000 mkdocs-plotly-plugin-0.1.2/mkdocs_plotly_plugin/javascripts/mkdocs-plotly-plugin.js
--rw-rw-rw-   0        0        0     5114 2023-01-20 19:00:48.000000 mkdocs-plotly-plugin-0.1.2/mkdocs_plotly_plugin/plugin.py
-drwxrwxrwx   0        0        0        0 2023-01-20 19:03:17.112928 mkdocs-plotly-plugin-0.1.2/mkdocs_plotly_plugin/templates/
--rw-rw-rw-   0        0        0     3594 2023-01-19 06:37:59.000000 mkdocs-plotly-plugin-0.1.2/mkdocs_plotly_plugin/templates/ggplot2.json
--rw-rw-rw-   0        0        0        2 2023-01-19 06:37:59.000000 mkdocs-plotly-plugin-0.1.2/mkdocs_plotly_plugin/templates/none.json
--rw-rw-rw-   0        0        0     4629 2023-01-19 06:37:59.000000 mkdocs-plotly-plugin-0.1.2/mkdocs_plotly_plugin/templates/plotly.json
--rw-rw-rw-   0        0        0     4959 2023-01-19 06:37:59.000000 mkdocs-plotly-plugin-0.1.2/mkdocs_plotly_plugin/templates/plotly_dark.json
--rw-rw-rw-   0        0        0     1721 2023-01-20 06:18:42.000000 mkdocs-plotly-plugin-0.1.2/mkdocs_plotly_plugin/templates/plotly_dark_min.json
--rw-rw-rw-   0        0        0     1612 2023-01-20 06:18:46.000000 mkdocs-plotly-plugin-0.1.2/mkdocs_plotly_plugin/templates/plotly_min.json
--rw-rw-rw-   0        0        0     4659 2023-01-19 06:37:59.000000 mkdocs-plotly-plugin-0.1.2/mkdocs_plotly_plugin/templates/plotly_white.json
--rw-rw-rw-   0        0        0     5590 2023-01-19 06:37:59.000000 mkdocs-plotly-plugin-0.1.2/mkdocs_plotly_plugin/templates/seaborn.json
--rw-rw-rw-   0        0        0     5635 2023-01-19 06:37:59.000000 mkdocs-plotly-plugin-0.1.2/mkdocs_plotly_plugin/templates/simple_white.json
-drwxrwxrwx   0        0        0        0 2023-01-20 19:03:17.103928 mkdocs-plotly-plugin-0.1.2/mkdocs_plotly_plugin.egg-info/
--rw-rw-rw-   0        0        0     3733 2023-01-20 19:03:16.000000 mkdocs-plotly-plugin-0.1.2/mkdocs_plotly_plugin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      873 2023-01-20 19:03:17.000000 mkdocs-plotly-plugin-0.1.2/mkdocs_plotly_plugin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-20 19:03:16.000000 mkdocs-plotly-plugin-0.1.2/mkdocs_plotly_plugin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-01-20 19:03:16.000000 mkdocs-plotly-plugin-0.1.2/mkdocs_plotly_plugin.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       59 2023-01-20 19:03:16.000000 mkdocs-plotly-plugin-0.1.2/mkdocs_plotly_plugin.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-01-20 19:03:17.000000 mkdocs-plotly-plugin-0.1.2/mkdocs_plotly_plugin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-20 19:03:17.113928 mkdocs-plotly-plugin-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1253 2023-01-20 19:03:06.000000 mkdocs-plotly-plugin-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 15:05:59.780632 mkdocs-plotly-plugin-0.1.3/
+-rw-rw-rw-   0        0        0     1084 2023-07-24 14:44:03.000000 mkdocs-plotly-plugin-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0       92 2023-07-24 14:44:03.000000 mkdocs-plotly-plugin-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3456 2023-07-24 15:05:59.780632 mkdocs-plotly-plugin-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2882 2023-07-24 14:44:03.000000 mkdocs-plotly-plugin-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 15:05:59.756626 mkdocs-plotly-plugin-0.1.3/mkdocs_plotly_plugin/
+-rw-rw-rw-   0        0        0        0 2023-07-24 14:44:03.000000 mkdocs-plotly-plugin-0.1.3/mkdocs_plotly_plugin/__init__.py
+-rw-rw-rw-   0        0        0      645 2023-07-24 14:44:03.000000 mkdocs-plotly-plugin-0.1.3/mkdocs_plotly_plugin/fences.py
+drwxrwxrwx   0        0        0        0 2023-07-24 15:05:59.771629 mkdocs-plotly-plugin-0.1.3/mkdocs_plotly_plugin/javascripts/
+-rw-rw-rw-   0        0        0     3519 2023-07-24 14:44:03.000000 mkdocs-plotly-plugin-0.1.3/mkdocs_plotly_plugin/javascripts/mkdocs-plotly-plugin.js
+-rw-rw-rw-   0        0        0     5825 2023-07-24 15:03:38.000000 mkdocs-plotly-plugin-0.1.3/mkdocs_plotly_plugin/plugin.py
+drwxrwxrwx   0        0        0        0 2023-07-24 15:05:59.779631 mkdocs-plotly-plugin-0.1.3/mkdocs_plotly_plugin/templates/
+-rw-rw-rw-   0        0        0     3594 2023-07-24 14:44:03.000000 mkdocs-plotly-plugin-0.1.3/mkdocs_plotly_plugin/templates/ggplot2.json
+-rw-rw-rw-   0        0        0        2 2023-07-24 14:44:03.000000 mkdocs-plotly-plugin-0.1.3/mkdocs_plotly_plugin/templates/none.json
+-rw-rw-rw-   0        0        0     4629 2023-07-24 14:44:03.000000 mkdocs-plotly-plugin-0.1.3/mkdocs_plotly_plugin/templates/plotly.json
+-rw-rw-rw-   0        0        0     4959 2023-07-24 14:44:03.000000 mkdocs-plotly-plugin-0.1.3/mkdocs_plotly_plugin/templates/plotly_dark.json
+-rw-rw-rw-   0        0        0     1721 2023-07-24 14:44:03.000000 mkdocs-plotly-plugin-0.1.3/mkdocs_plotly_plugin/templates/plotly_dark_min.json
+-rw-rw-rw-   0        0        0     1612 2023-07-24 14:44:03.000000 mkdocs-plotly-plugin-0.1.3/mkdocs_plotly_plugin/templates/plotly_min.json
+-rw-rw-rw-   0        0        0     4659 2023-07-24 14:44:03.000000 mkdocs-plotly-plugin-0.1.3/mkdocs_plotly_plugin/templates/plotly_white.json
+-rw-rw-rw-   0        0        0     5590 2023-07-24 14:44:03.000000 mkdocs-plotly-plugin-0.1.3/mkdocs_plotly_plugin/templates/seaborn.json
+-rw-rw-rw-   0        0        0     5635 2023-07-24 14:44:03.000000 mkdocs-plotly-plugin-0.1.3/mkdocs_plotly_plugin/templates/simple_white.json
+drwxrwxrwx   0        0        0        0 2023-07-24 15:05:59.771629 mkdocs-plotly-plugin-0.1.3/mkdocs_plotly_plugin.egg-info/
+-rw-rw-rw-   0        0        0     3456 2023-07-24 15:05:59.000000 mkdocs-plotly-plugin-0.1.3/mkdocs_plotly_plugin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      873 2023-07-24 15:05:59.000000 mkdocs-plotly-plugin-0.1.3/mkdocs_plotly_plugin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 15:05:59.000000 mkdocs-plotly-plugin-0.1.3/mkdocs_plotly_plugin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-07-24 15:05:59.000000 mkdocs-plotly-plugin-0.1.3/mkdocs_plotly_plugin.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       79 2023-07-24 15:05:59.000000 mkdocs-plotly-plugin-0.1.3/mkdocs_plotly_plugin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-07-24 15:05:59.000000 mkdocs-plotly-plugin-0.1.3/mkdocs_plotly_plugin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 15:05:59.780632 mkdocs-plotly-plugin-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1075 2023-07-24 15:03:38.000000 mkdocs-plotly-plugin-0.1.3/setup.py
```

### Comparing `mkdocs-plotly-plugin-0.1.2/LICENSE` & `mkdocs-plotly-plugin-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-plotly-plugin-0.1.2/PKG-INFO` & `mkdocs-plotly-plugin-0.1.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,31 @@
 Metadata-Version: 2.1
 Name: mkdocs-plotly-plugin
-Version: 0.1.2
+Version: 0.1.3
 Summary: MkDocs plugin to add plotly charts from plotly's json data
 Home-page: https://github.com/haoda-li/mkdocs-plotly-plugin
 Author: Haoda Li
 Author-email: haoda_li@berkeley.edu
 License: MIT
 Keywords: mkdocs plugin
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 
 # Mkdocs Plotly Plugin
 
-![PyPI](https://img.shields.io/pypi/v/mkdocs-plotly-plugin)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/mkdocs-plotly-plugin)
-![PyPI - License](https://img.shields.io/pypi/l/mkdocs-plotly-plugin)
+![PyPI](https://img.shields.io/pypi/v/mkdocs-plotly-plugin?style=for-the-badge)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/mkdocs-plotly-plugin?style=for-the-badge)
+![PyPI - License](https://img.shields.io/pypi/l/mkdocs-plotly-plugin?style=for-the-badge)
 
 [MkDocs](https://www.mkdocs.org/) plugin to create interactive charts from data using the declarative [plotly](https://plotly.com/javascript/)'s json syntax. 
 
 Includes supports for [mkdocs-material](https://github.com/squidfunk/mkdocs-material) theme features like [instant loading](https://squidfunk.github.io/mkdocs-material/setup/setting-up-navigation/?h=reload#instant-loading) and [dark color themes](https://squidfunk.github.io/mkdocs-material/setup/changing-the-colors/#color-palette-toggle).
 
 ## Installation
 
@@ -57,24 +53,16 @@
 
 You can insert any valid plotly JSON as a codeblock using:
 ````
 ``` plotly
 {
     "data": [
         {
-            "x": [
-                "giraffes",
-                "orangutans",
-                "monkeys"
-            ],
-            "y": [
-                20,
-                14,
-                23
-            ],
+            "x": ["giraffes", "orangutans", "monkeys"],
+            "y": [20, 14, 23],
             "type": "bar"
         }
     ]
 }
 ```
 ````
```

### Comparing `mkdocs-plotly-plugin-0.1.2/README.md` & `mkdocs-plotly-plugin-0.1.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,185 +1,181 @@
 00000000: 0d0a 0d0a 2320 4d6b 646f 6373 2050 6c6f  ....# Mkdocs Plo
 00000010: 746c 7920 506c 7567 696e 0d0a 0d0a 215b  tly Plugin....![
 00000020: 5079 5049 5d28 6874 7470 733a 2f2f 696d  PyPI](https://im
 00000030: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
 00000040: 692f 762f 6d6b 646f 6373 2d70 6c6f 746c  i/v/mkdocs-plotl
-00000050: 792d 706c 7567 696e 290d 0a21 5b50 7950  y-plugin)..![PyP
-00000060: 4920 2d20 446f 776e 6c6f 6164 735d 2868  I - Downloads](h
-00000070: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000080: 6473 2e69 6f2f 7079 7069 2f64 6d2f 6d6b  ds.io/pypi/dm/mk
-00000090: 646f 6373 2d70 6c6f 746c 792d 706c 7567  docs-plotly-plug
-000000a0: 696e 290d 0a21 5b50 7950 4920 2d20 4c69  in)..![PyPI - Li
-000000b0: 6365 6e73 655d 2868 7474 7073 3a2f 2f69  cense](https://i
-000000c0: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
-000000d0: 7069 2f6c 2f6d 6b64 6f63 732d 706c 6f74  pi/l/mkdocs-plot
-000000e0: 6c79 2d70 6c75 6769 6e29 0d0a 0d0a 5b4d  ly-plugin)....[M
-000000f0: 6b44 6f63 735d 2868 7474 7073 3a2f 2f77  kDocs](https://w
-00000100: 7777 2e6d 6b64 6f63 732e 6f72 672f 2920  ww.mkdocs.org/) 
-00000110: 706c 7567 696e 2074 6f20 6372 6561 7465  plugin to create
-00000120: 2069 6e74 6572 6163 7469 7665 2063 6861   interactive cha
-00000130: 7274 7320 6672 6f6d 2064 6174 6120 7573  rts from data us
-00000140: 696e 6720 7468 6520 6465 636c 6172 6174  ing the declarat
-00000150: 6976 6520 5b70 6c6f 746c 795d 2868 7474  ive [plotly](htt
-00000160: 7073 3a2f 2f70 6c6f 746c 792e 636f 6d2f  ps://plotly.com/
-00000170: 6a61 7661 7363 7269 7074 2f29 2773 206a  javascript/)'s j
-00000180: 736f 6e20 7379 6e74 6178 2e20 0d0a 0d0a  son syntax. ....
-00000190: 496e 636c 7564 6573 2073 7570 706f 7274  Includes support
-000001a0: 7320 666f 7220 5b6d 6b64 6f63 732d 6d61  s for [mkdocs-ma
-000001b0: 7465 7269 616c 5d28 6874 7470 733a 2f2f  terial](https://
-000001c0: 6769 7468 7562 2e63 6f6d 2f73 7175 6964  github.com/squid
-000001d0: 6675 6e6b 2f6d 6b64 6f63 732d 6d61 7465  funk/mkdocs-mate
-000001e0: 7269 616c 2920 7468 656d 6520 6665 6174  rial) theme feat
-000001f0: 7572 6573 206c 696b 6520 5b69 6e73 7461  ures like [insta
-00000200: 6e74 206c 6f61 6469 6e67 5d28 6874 7470  nt loading](http
-00000210: 733a 2f2f 7371 7569 6466 756e 6b2e 6769  s://squidfunk.gi
-00000220: 7468 7562 2e69 6f2f 6d6b 646f 6373 2d6d  thub.io/mkdocs-m
-00000230: 6174 6572 6961 6c2f 7365 7475 702f 7365  aterial/setup/se
-00000240: 7474 696e 672d 7570 2d6e 6176 6967 6174  tting-up-navigat
-00000250: 696f 6e2f 3f68 3d72 656c 6f61 6423 696e  ion/?h=reload#in
-00000260: 7374 616e 742d 6c6f 6164 696e 6729 2061  stant-loading) a
-00000270: 6e64 205b 6461 726b 2063 6f6c 6f72 2074  nd [dark color t
-00000280: 6865 6d65 735d 2868 7474 7073 3a2f 2f73  hemes](https://s
-00000290: 7175 6964 6675 6e6b 2e67 6974 6875 622e  quidfunk.github.
-000002a0: 696f 2f6d 6b64 6f63 732d 6d61 7465 7269  io/mkdocs-materi
-000002b0: 616c 2f73 6574 7570 2f63 6861 6e67 696e  al/setup/changin
-000002c0: 672d 7468 652d 636f 6c6f 7273 2f23 636f  g-the-colors/#co
-000002d0: 6c6f 722d 7061 6c65 7474 652d 746f 6767  lor-palette-togg
-000002e0: 6c65 292e 0d0a 0d0a 2323 2049 6e73 7461  le).....## Insta
-000002f0: 6c6c 6174 696f 6e0d 0a0d 0a49 6e73 7461  llation....Insta
-00000300: 6c6c 2074 6865 2070 6c75 6769 6e20 7573  ll the plugin us
-00000310: 696e 6720 6070 6970 3360 3a0d 0a0d 0a60  ing `pip3`:....`
-00000320: 6060 7368 656c 6c0d 0a70 6970 2069 6e73  ``shell..pip ins
-00000330: 7461 6c6c 206d 6b64 6f63 732d 706c 6f74  tall mkdocs-plot
-00000340: 6c79 2d70 6c75 6769 6e20 0d0a 6060 600d  ly-plugin ..```.
-00000350: 0a0d 0a41 6e64 2074 6865 6e20 6164 6420  ...And then add 
-00000360: 7468 6520 706c 7567 696e 2069 6e74 6f20  the plugin into 
-00000370: 6070 6c75 6769 6e73 6020 616e 6420 7468  `plugins` and th
-00000380: 6520 6375 7374 6f6d 6520 6665 6e63 650d  e custome fence.
-00000390: 0a0d 0a60 6060 796d 6c0d 0a70 6c75 6769  ...```yml..plugi
-000003a0: 6e73 3a0d 0a20 202d 2070 6c6f 746c 790d  ns:..  - plotly.
-000003b0: 0a0d 0a6d 6172 6b64 6f77 6e5f 6578 7465  ...markdown_exte
-000003c0: 6e73 696f 6e73 3a0d 0a20 202d 2070 796d  nsions:..  - pym
-000003d0: 646f 776e 782e 7375 7065 7266 656e 6365  downx.superfence
-000003e0: 733a 0d0a 2020 2020 2020 6375 7374 6f6d  s:..      custom
-000003f0: 5f66 656e 6365 733a 0d0a 2020 2020 2020  _fences:..      
-00000400: 2020 2d20 6e61 6d65 3a20 706c 6f74 6c79    - name: plotly
-00000410: 0d0a 2020 2020 2020 2020 2020 636c 6173  ..          clas
-00000420: 733a 206d 6b64 6f63 732d 706c 6f74 6c79  s: mkdocs-plotly
-00000430: 0d0a 2020 2020 2020 2020 2020 666f 726d  ..          form
-00000440: 6174 3a20 2121 7079 7468 6f6e 2f6e 616d  at: !!python/nam
-00000450: 653a 6d6b 646f 6373 5f70 6c6f 746c 795f  e:mkdocs_plotly_
-00000460: 706c 7567 696e 2e66 656e 6365 732e 6665  plugin.fences.fe
-00000470: 6e63 655f 706c 6f74 6c79 0d0a 6060 600d  nce_plotly..```.
-00000480: 0a0d 0a23 2320 5573 6167 650d 0a0d 0a59  ...## Usage....Y
-00000490: 6f75 2063 616e 2069 6e73 6572 7420 616e  ou can insert an
-000004a0: 7920 7661 6c69 6420 706c 6f74 6c79 204a  y valid plotly J
-000004b0: 534f 4e20 6173 2061 2063 6f64 6562 6c6f  SON as a codeblo
-000004c0: 636b 2075 7369 6e67 3a0d 0a60 6060 600d  ck using:..````.
-000004d0: 0a60 6060 2070 6c6f 746c 790d 0a7b 0d0a  .``` plotly..{..
-000004e0: 2020 2020 2264 6174 6122 3a20 5b0d 0a20      "data": [.. 
-000004f0: 2020 2020 2020 207b 0d0a 2020 2020 2020         {..      
-00000500: 2020 2020 2020 2278 223a 205b 0d0a 2020        "x": [..  
-00000510: 2020 2020 2020 2020 2020 2020 2020 2267                "g
-00000520: 6972 6166 6665 7322 2c0d 0a20 2020 2020  iraffes",..     
-00000530: 2020 2020 2020 2020 2020 2022 6f72 616e             "oran
-00000540: 6775 7461 6e73 222c 0d0a 2020 2020 2020  gutans",..      
-00000550: 2020 2020 2020 2020 2020 226d 6f6e 6b65            "monke
-00000560: 7973 220d 0a20 2020 2020 2020 2020 2020  ys"..           
-00000570: 205d 2c0d 0a20 2020 2020 2020 2020 2020   ],..           
-00000580: 2022 7922 3a20 5b0d 0a20 2020 2020 2020   "y": [..       
-00000590: 2020 2020 2020 2020 2032 302c 0d0a 2020           20,..  
-000005a0: 2020 2020 2020 2020 2020 2020 2020 3134                14
-000005b0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000005c0: 2020 2032 330d 0a20 2020 2020 2020 2020     23..         
-000005d0: 2020 205d 2c0d 0a20 2020 2020 2020 2020     ],..         
-000005e0: 2020 2022 7479 7065 223a 2022 6261 7222     "type": "bar"
-000005f0: 0d0a 2020 2020 2020 2020 7d0d 0a20 2020  ..        }..   
-00000600: 205d 0d0a 7d0d 0a60 6060 0d0a 6060 6060   ]..}..```..````
-00000610: 0d0a 0d0a 0d0a 5468 6973 2069 7320 636f  ......This is co
-00000620: 6d70 6174 6961 626c 6520 7769 7468 2060  mpatiable with `
-00000630: 736e 6970 706c 6574 7360 2061 7320 7765  snipplets` as we
-00000640: 6c6c 0d0a 0d0a 6060 6060 0d0a 6060 6070  ll....````..```p
-00000650: 6c6f 746c 790d 0a2d 2d38 3c2d 2d20 2261  lotly..--8<-- "a
-00000660: 7373 6574 732f 6461 7461 2e6a 736f 6e22  ssets/data.json"
-00000670: 0d0a 6060 600d 0a60 6060 600d 0a0d 0a0d  ..```..````.....
-00000680: 0a6f 7220 796f 7520 6361 6e20 696e 7365  .or you can inse
-00000690: 7274 2061 6e79 2070 6c6f 746c 7920 4a53  rt any plotly JS
-000006a0: 4f4e 2074 6872 6f75 6768 2055 524c 730d  ON through URLs.
-000006b0: 0a0d 0a0d 0a60 6060 600d 0a60 6060 706c  .....````..```pl
-000006c0: 6f74 6c79 0d0a 7b22 6669 6c65 5f70 6174  otly..{"file_pat
-000006d0: 6822 3a20 222e 2f61 7373 6574 732f 6461  h": "./assets/da
-000006e0: 7461 2e6a 736f 6e22 7d0d 0a60 6060 0d0a  ta.json"}..```..
-000006f0: 6060 6060 0d0a 0d0a 0d0a 5573 696e 6720  ````......Using 
-00000700: 6073 6e69 7070 6c65 7473 6020 7769 6c6c  `snipplets` will
-00000710: 2069 6e73 6572 7420 7468 6520 6a73 6f6e   insert the json
-00000720: 2063 6f6e 7465 6e74 2069 6e74 6f20 7468   content into th
-00000730: 6520 6f75 7470 7574 2048 544d 4c20 6669  e output HTML fi
-00000740: 6c65 2c20 7768 6963 6820 6973 206d 6f72  le, which is mor
-00000750: 6520 7375 6974 6162 6c65 2066 6f72 2073  e suitable for s
-00000760: 6d61 6c6c 6572 2064 6174 6173 6574 732e  maller datasets.
-00000770: 2055 7369 6e67 2060 6669 6c65 5f70 6174   Using `file_pat
-00000780: 6860 2077 696c 6c20 6665 7463 6820 7468  h` will fetch th
-00000790: 6520 6a73 6f6e 2063 6f6e 7465 6e74 206f  e json content o
-000007a0: 6e63 6520 7468 6520 7061 6765 2069 7320  nce the page is 
-000007b0: 6c6f 6164 6564 2e0d 0a0d 0a50 6c6f 746c  loaded.....Plotl
-000007c0: 7920 6861 7320 6974 7320 6f77 6e20 6563  y has its own ec
-000007d0: 6f2d 7379 7374 656d 2066 6f72 2063 7265  o-system for cre
-000007e0: 6174 696e 6720 6368 6172 7473 2069 6e20  ating charts in 
-000007f0: 6d6f 7374 2073 7461 7469 7374 6963 616c  most statistical
-00000800: 206c 616e 6775 6167 6573 2e20 596f 7520   languages. You 
-00000810: 6361 6e20 6f75 7470 7574 2074 6865 2070  can output the p
-00000820: 6c6f 7420 6173 2061 206a 736f 6e20 6669  lot as a json fi
-00000830: 6c65 2074 6872 6f75 6768 2060 6669 672e  le through `fig.
-00000840: 746f 5f6a 736f 6e28 2960 2e0d 0a0d 0a23  to_json()`.....#
-00000850: 2323 204f 7074 696f 6e73 0d0a 0d0a 7c20  ## Options....| 
-00000860: 4f70 7469 6f6e 2020 207c 2044 6566 6175  Option   | Defau
-00000870: 6c74 207c 2044 6573 6372 6970 7469 6f6e  lt | Description
-00000880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008b0: 2020 2020 2020 2020 2020 2020 7c0d 0a7c              |..|
-000008c0: 202d 2d2d 2d2d 2d2d 2d20 7c20 2d2d 2d2d   -------- | ----
-000008d0: 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d2d 2d2d  --- | ----------
-000008e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000008f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000900: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000910: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c 0d0a  ------------ |..
-00000920: 7c20 6c69 625f 7061 7468 207c 2060 2060  | lib_path | ` `
-00000930: 2020 2020 2020 7c20 5265 6c61 7469 7665        | Relative
-00000940: 2070 6174 6820 746f 206c 6f63 616c 2060   path to local `
-00000950: 706c 6f74 6c79 2e6a 7360 2066 696c 652c  plotly.js` file,
-00000960: 206f 7220 6c65 6176 6520 6974 2062 6c61   or leave it bla
-00000970: 6e6b 2074 6f20 7573 6520 4344 4e2e 207c  nk to use CDN. |
-00000980: 0d0a 7c20 7465 6d70 6c61 7465 5f64 6566  ..| template_def
-00000990: 6175 6c74 2020 207c 2060 706c 6f74 6c79  ault   | `plotly
-000009a0: 5f6d 696e 6020 207c 2074 656d 706c 6174  _min`  | templat
-000009b0: 6520 666f 7220 706c 6f74 6c79 2063 6861  e for plotly cha
-000009c0: 7274 7320 696e 206c 6967 6874 206d 6f64  rts in light mod
-000009d0: 6520 7c0d 0a7c 2074 656d 706c 6174 655f  e |..| template_
-000009e0: 736c 6174 6520 7c20 6070 6c6f 746c 795f  slate | `plotly_
-000009f0: 6461 726b 5f6d 696e 6020 2020 2020 207c  dark_min`      |
-00000a00: 2074 656d 706c 6174 6520 666f 7220 706c   template for pl
-00000a10: 6f74 6c79 2063 6861 7274 7320 696e 2064  otly charts in d
-00000a20: 6172 6b20 6d6f 6465 207c 0d0a 7c20 656e  ark mode |..| en
-00000a30: 6162 6c65 5f74 656d 706c 6174 6520 7c20  able_template | 
-00000a40: 5472 7565 207c 2075 7365 2074 656d 706c  True | use templ
-00000a50: 6174 6520 746f 2061 7574 6f6d 6174 6963  ate to automatic
-00000a60: 616c 6c79 2063 6861 6e67 6520 7468 656d  ally change them
-00000a70: 6520 7c0d 0a0d 0a41 7661 696c 6162 6c65  e |....Available
-00000a80: 2050 6c6f 746c 7920 7465 6d70 6c61 7465   Plotly template
-00000a90: 7320 6172 6520 605b 2270 6c6f 746c 795f  s are `["plotly_
-00000aa0: 6d69 6e22 2c20 2270 6c6f 746c 795f 6461  min", "plotly_da
-00000ab0: 726b 5f6d 696e 222c 2022 706c 6f74 6c79  rk_min", "plotly
-00000ac0: 222c 2022 706c 6f74 6c79 5f77 6869 7465  ", "plotly_white
-00000ad0: 222c 2022 706c 6f74 6c79 5f64 6172 6b22  ", "plotly_dark"
-00000ae0: 2c20 2267 6770 6c6f 7432 222c 2022 7365  , "ggplot2", "se
-00000af0: 6162 6f72 6e22 2c20 2273 696d 706c 655f  aborn", "simple_
-00000b00: 7768 6974 6522 2c20 226e 6f6e 6522 5d60  white", "none"]`
-00000b10: 2e20 4966 2079 6f75 2077 616e 7420 746f  . If you want to
-00000b20: 2063 7573 746f 6d69 7a65 2079 6f75 7220   customize your 
-00000b30: 6f77 6e20 7465 6d70 6c61 7465 2c20 796f  own template, yo
-00000b40: 7520 6361 6e20 6578 706f 7274 2069 7420  u can export it 
-00000b50: 6173 2061 204a 534f 4e20 6669 6c65 2061  as a JSON file a
-00000b60: 6e64 2070 726f 7669 6465 2069 7473 2072  nd provide its r
-00000b70: 656c 6174 6976 6520 7061 7468 2069 6e20  elative path in 
-00000b80: 6f70 7469 6f6e 732e 0d0a                 options...
+00000050: 792d 706c 7567 696e 3f73 7479 6c65 3d66  y-plugin?style=f
+00000060: 6f72 2d74 6865 2d62 6164 6765 290d 0a21  or-the-badge)..!
+00000070: 5b50 7950 4920 2d20 446f 776e 6c6f 6164  [PyPI - Download
+00000080: 735d 2868 7474 7073 3a2f 2f69 6d67 2e73  s](https://img.s
+00000090: 6869 656c 6473 2e69 6f2f 7079 7069 2f64  hields.io/pypi/d
+000000a0: 6d2f 6d6b 646f 6373 2d70 6c6f 746c 792d  m/mkdocs-plotly-
+000000b0: 706c 7567 696e 3f73 7479 6c65 3d66 6f72  plugin?style=for
+000000c0: 2d74 6865 2d62 6164 6765 290d 0a21 5b50  -the-badge)..![P
+000000d0: 7950 4920 2d20 4c69 6365 6e73 655d 2868  yPI - License](h
+000000e0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+000000f0: 6473 2e69 6f2f 7079 7069 2f6c 2f6d 6b64  ds.io/pypi/l/mkd
+00000100: 6f63 732d 706c 6f74 6c79 2d70 6c75 6769  ocs-plotly-plugi
+00000110: 6e3f 7374 796c 653d 666f 722d 7468 652d  n?style=for-the-
+00000120: 6261 6467 6529 0d0a 0d0a 5b4d 6b44 6f63  badge)....[MkDoc
+00000130: 735d 2868 7474 7073 3a2f 2f77 7777 2e6d  s](https://www.m
+00000140: 6b64 6f63 732e 6f72 672f 2920 706c 7567  kdocs.org/) plug
+00000150: 696e 2074 6f20 6372 6561 7465 2069 6e74  in to create int
+00000160: 6572 6163 7469 7665 2063 6861 7274 7320  eractive charts 
+00000170: 6672 6f6d 2064 6174 6120 7573 696e 6720  from data using 
+00000180: 7468 6520 6465 636c 6172 6174 6976 6520  the declarative 
+00000190: 5b70 6c6f 746c 795d 2868 7474 7073 3a2f  [plotly](https:/
+000001a0: 2f70 6c6f 746c 792e 636f 6d2f 6a61 7661  /plotly.com/java
+000001b0: 7363 7269 7074 2f29 2773 206a 736f 6e20  script/)'s json 
+000001c0: 7379 6e74 6178 2e20 0d0a 0d0a 496e 636c  syntax. ....Incl
+000001d0: 7564 6573 2073 7570 706f 7274 7320 666f  udes supports fo
+000001e0: 7220 5b6d 6b64 6f63 732d 6d61 7465 7269  r [mkdocs-materi
+000001f0: 616c 5d28 6874 7470 733a 2f2f 6769 7468  al](https://gith
+00000200: 7562 2e63 6f6d 2f73 7175 6964 6675 6e6b  ub.com/squidfunk
+00000210: 2f6d 6b64 6f63 732d 6d61 7465 7269 616c  /mkdocs-material
+00000220: 2920 7468 656d 6520 6665 6174 7572 6573  ) theme features
+00000230: 206c 696b 6520 5b69 6e73 7461 6e74 206c   like [instant l
+00000240: 6f61 6469 6e67 5d28 6874 7470 733a 2f2f  oading](https://
+00000250: 7371 7569 6466 756e 6b2e 6769 7468 7562  squidfunk.github
+00000260: 2e69 6f2f 6d6b 646f 6373 2d6d 6174 6572  .io/mkdocs-mater
+00000270: 6961 6c2f 7365 7475 702f 7365 7474 696e  ial/setup/settin
+00000280: 672d 7570 2d6e 6176 6967 6174 696f 6e2f  g-up-navigation/
+00000290: 3f68 3d72 656c 6f61 6423 696e 7374 616e  ?h=reload#instan
+000002a0: 742d 6c6f 6164 696e 6729 2061 6e64 205b  t-loading) and [
+000002b0: 6461 726b 2063 6f6c 6f72 2074 6865 6d65  dark color theme
+000002c0: 735d 2868 7474 7073 3a2f 2f73 7175 6964  s](https://squid
+000002d0: 6675 6e6b 2e67 6974 6875 622e 696f 2f6d  funk.github.io/m
+000002e0: 6b64 6f63 732d 6d61 7465 7269 616c 2f73  kdocs-material/s
+000002f0: 6574 7570 2f63 6861 6e67 696e 672d 7468  etup/changing-th
+00000300: 652d 636f 6c6f 7273 2f23 636f 6c6f 722d  e-colors/#color-
+00000310: 7061 6c65 7474 652d 746f 6767 6c65 292e  palette-toggle).
+00000320: 0d0a 0d0a 2323 2049 6e73 7461 6c6c 6174  ....## Installat
+00000330: 696f 6e0d 0a0d 0a49 6e73 7461 6c6c 2074  ion....Install t
+00000340: 6865 2070 6c75 6769 6e20 7573 696e 6720  he plugin using 
+00000350: 6070 6970 3360 3a0d 0a0d 0a60 6060 7368  `pip3`:....```sh
+00000360: 656c 6c0d 0a70 6970 2069 6e73 7461 6c6c  ell..pip install
+00000370: 206d 6b64 6f63 732d 706c 6f74 6c79 2d70   mkdocs-plotly-p
+00000380: 6c75 6769 6e20 0d0a 6060 600d 0a0d 0a41  lugin ..```....A
+00000390: 6e64 2074 6865 6e20 6164 6420 7468 6520  nd then add the 
+000003a0: 706c 7567 696e 2069 6e74 6f20 6070 6c75  plugin into `plu
+000003b0: 6769 6e73 6020 616e 6420 7468 6520 6375  gins` and the cu
+000003c0: 7374 6f6d 6520 6665 6e63 650d 0a0d 0a60  stome fence....`
+000003d0: 6060 796d 6c0d 0a70 6c75 6769 6e73 3a0d  ``yml..plugins:.
+000003e0: 0a20 202d 2070 6c6f 746c 790d 0a0d 0a6d  .  - plotly....m
+000003f0: 6172 6b64 6f77 6e5f 6578 7465 6e73 696f  arkdown_extensio
+00000400: 6e73 3a0d 0a20 202d 2070 796d 646f 776e  ns:..  - pymdown
+00000410: 782e 7375 7065 7266 656e 6365 733a 0d0a  x.superfences:..
+00000420: 2020 2020 2020 6375 7374 6f6d 5f66 656e        custom_fen
+00000430: 6365 733a 0d0a 2020 2020 2020 2020 2d20  ces:..        - 
+00000440: 6e61 6d65 3a20 706c 6f74 6c79 0d0a 2020  name: plotly..  
+00000450: 2020 2020 2020 2020 636c 6173 733a 206d          class: m
+00000460: 6b64 6f63 732d 706c 6f74 6c79 0d0a 2020  kdocs-plotly..  
+00000470: 2020 2020 2020 2020 666f 726d 6174 3a20          format: 
+00000480: 2121 7079 7468 6f6e 2f6e 616d 653a 6d6b  !!python/name:mk
+00000490: 646f 6373 5f70 6c6f 746c 795f 706c 7567  docs_plotly_plug
+000004a0: 696e 2e66 656e 6365 732e 6665 6e63 655f  in.fences.fence_
+000004b0: 706c 6f74 6c79 0d0a 6060 600d 0a0d 0a23  plotly..```....#
+000004c0: 2320 5573 6167 650d 0a0d 0a59 6f75 2063  # Usage....You c
+000004d0: 616e 2069 6e73 6572 7420 616e 7920 7661  an insert any va
+000004e0: 6c69 6420 706c 6f74 6c79 204a 534f 4e20  lid plotly JSON 
+000004f0: 6173 2061 2063 6f64 6562 6c6f 636b 2075  as a codeblock u
+00000500: 7369 6e67 3a0d 0a60 6060 600d 0a60 6060  sing:..````..```
+00000510: 2070 6c6f 746c 790d 0a7b 0d0a 2020 2020   plotly..{..    
+00000520: 2264 6174 6122 3a20 5b0d 0a20 2020 2020  "data": [..     
+00000530: 2020 207b 0d0a 2020 2020 2020 2020 2020     {..          
+00000540: 2020 2278 223a 205b 2267 6972 6166 6665    "x": ["giraffe
+00000550: 7322 2c20 226f 7261 6e67 7574 616e 7322  s", "orangutans"
+00000560: 2c20 226d 6f6e 6b65 7973 225d 2c0d 0a20  , "monkeys"],.. 
+00000570: 2020 2020 2020 2020 2020 2022 7922 3a20             "y": 
+00000580: 5b32 302c 2031 342c 2032 335d 2c0d 0a20  [20, 14, 23],.. 
+00000590: 2020 2020 2020 2020 2020 2022 7479 7065             "type
+000005a0: 223a 2022 6261 7222 0d0a 2020 2020 2020  ": "bar"..      
+000005b0: 2020 7d0d 0a20 2020 205d 0d0a 7d0d 0a60    }..    ]..}..`
+000005c0: 6060 0d0a 6060 6060 0d0a 0d0a 0d0a 5468  ``..````......Th
+000005d0: 6973 2069 7320 636f 6d70 6174 6961 626c  is is compatiabl
+000005e0: 6520 7769 7468 2060 736e 6970 706c 6574  e with `snipplet
+000005f0: 7360 2061 7320 7765 6c6c 0d0a 0d0a 6060  s` as well....``
+00000600: 6060 0d0a 6060 6070 6c6f 746c 790d 0a2d  ``..```plotly..-
+00000610: 2d38 3c2d 2d20 2261 7373 6574 732f 6461  -8<-- "assets/da
+00000620: 7461 2e6a 736f 6e22 0d0a 6060 600d 0a60  ta.json"..```..`
+00000630: 6060 600d 0a0d 0a0d 0a6f 7220 796f 7520  ```......or you 
+00000640: 6361 6e20 696e 7365 7274 2061 6e79 2070  can insert any p
+00000650: 6c6f 746c 7920 4a53 4f4e 2074 6872 6f75  lotly JSON throu
+00000660: 6768 2055 524c 730d 0a0d 0a0d 0a60 6060  gh URLs......```
+00000670: 600d 0a60 6060 706c 6f74 6c79 0d0a 7b22  `..```plotly..{"
+00000680: 6669 6c65 5f70 6174 6822 3a20 222e 2f61  file_path": "./a
+00000690: 7373 6574 732f 6461 7461 2e6a 736f 6e22  ssets/data.json"
+000006a0: 7d0d 0a60 6060 0d0a 6060 6060 0d0a 0d0a  }..```..````....
+000006b0: 0d0a 5573 696e 6720 6073 6e69 7070 6c65  ..Using `snipple
+000006c0: 7473 6020 7769 6c6c 2069 6e73 6572 7420  ts` will insert 
+000006d0: 7468 6520 6a73 6f6e 2063 6f6e 7465 6e74  the json content
+000006e0: 2069 6e74 6f20 7468 6520 6f75 7470 7574   into the output
+000006f0: 2048 544d 4c20 6669 6c65 2c20 7768 6963   HTML file, whic
+00000700: 6820 6973 206d 6f72 6520 7375 6974 6162  h is more suitab
+00000710: 6c65 2066 6f72 2073 6d61 6c6c 6572 2064  le for smaller d
+00000720: 6174 6173 6574 732e 2055 7369 6e67 2060  atasets. Using `
+00000730: 6669 6c65 5f70 6174 6860 2077 696c 6c20  file_path` will 
+00000740: 6665 7463 6820 7468 6520 6a73 6f6e 2063  fetch the json c
+00000750: 6f6e 7465 6e74 206f 6e63 6520 7468 6520  ontent once the 
+00000760: 7061 6765 2069 7320 6c6f 6164 6564 2e0d  page is loaded..
+00000770: 0a0d 0a50 6c6f 746c 7920 6861 7320 6974  ...Plotly has it
+00000780: 7320 6f77 6e20 6563 6f2d 7379 7374 656d  s own eco-system
+00000790: 2066 6f72 2063 7265 6174 696e 6720 6368   for creating ch
+000007a0: 6172 7473 2069 6e20 6d6f 7374 2073 7461  arts in most sta
+000007b0: 7469 7374 6963 616c 206c 616e 6775 6167  tistical languag
+000007c0: 6573 2e20 596f 7520 6361 6e20 6f75 7470  es. You can outp
+000007d0: 7574 2074 6865 2070 6c6f 7420 6173 2061  ut the plot as a
+000007e0: 206a 736f 6e20 6669 6c65 2074 6872 6f75   json file throu
+000007f0: 6768 2060 6669 672e 746f 5f6a 736f 6e28  gh `fig.to_json(
+00000800: 2960 2e0d 0a0d 0a23 2323 204f 7074 696f  )`.....### Optio
+00000810: 6e73 0d0a 0d0a 7c20 4f70 7469 6f6e 2020  ns....| Option  
+00000820: 207c 2044 6566 6175 6c74 207c 2044 6573   | Default | Des
+00000830: 6372 6970 7469 6f6e 2020 2020 2020 2020  cription        
+00000840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000870: 2020 2020 7c0d 0a7c 202d 2d2d 2d2d 2d2d      |..| -------
+00000880: 2d20 7c20 2d2d 2d2d 2d2d 2d20 7c20 2d2d  - | ------- | --
+00000890: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000008a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000008b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000008c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000008d0: 2d2d 2d2d 207c 0d0a 7c20 6c69 625f 7061  ---- |..| lib_pa
+000008e0: 7468 207c 2060 2060 2020 2020 2020 7c20  th | ` `      | 
+000008f0: 5265 6c61 7469 7665 2070 6174 6820 746f  Relative path to
+00000900: 206c 6f63 616c 2060 706c 6f74 6c79 2e6a   local `plotly.j
+00000910: 7360 2066 696c 652c 206f 7220 6c65 6176  s` file, or leav
+00000920: 6520 6974 2062 6c61 6e6b 2074 6f20 7573  e it blank to us
+00000930: 6520 4344 4e2e 207c 0d0a 7c20 7465 6d70  e CDN. |..| temp
+00000940: 6c61 7465 5f64 6566 6175 6c74 2020 207c  late_default   |
+00000950: 2060 706c 6f74 6c79 5f6d 696e 6020 207c   `plotly_min`  |
+00000960: 2074 656d 706c 6174 6520 666f 7220 706c   template for pl
+00000970: 6f74 6c79 2063 6861 7274 7320 696e 206c  otly charts in l
+00000980: 6967 6874 206d 6f64 6520 7c0d 0a7c 2074  ight mode |..| t
+00000990: 656d 706c 6174 655f 736c 6174 6520 7c20  emplate_slate | 
+000009a0: 6070 6c6f 746c 795f 6461 726b 5f6d 696e  `plotly_dark_min
+000009b0: 6020 2020 2020 207c 2074 656d 706c 6174  `      | templat
+000009c0: 6520 666f 7220 706c 6f74 6c79 2063 6861  e for plotly cha
+000009d0: 7274 7320 696e 2064 6172 6b20 6d6f 6465  rts in dark mode
+000009e0: 207c 0d0a 7c20 656e 6162 6c65 5f74 656d   |..| enable_tem
+000009f0: 706c 6174 6520 7c20 5472 7565 207c 2075  plate | True | u
+00000a00: 7365 2074 656d 706c 6174 6520 746f 2061  se template to a
+00000a10: 7574 6f6d 6174 6963 616c 6c79 2063 6861  utomatically cha
+00000a20: 6e67 6520 7468 656d 6520 7c0d 0a0d 0a41  nge theme |....A
+00000a30: 7661 696c 6162 6c65 2050 6c6f 746c 7920  vailable Plotly 
+00000a40: 7465 6d70 6c61 7465 7320 6172 6520 605b  templates are `[
+00000a50: 2270 6c6f 746c 795f 6d69 6e22 2c20 2270  "plotly_min", "p
+00000a60: 6c6f 746c 795f 6461 726b 5f6d 696e 222c  lotly_dark_min",
+00000a70: 2022 706c 6f74 6c79 222c 2022 706c 6f74   "plotly", "plot
+00000a80: 6c79 5f77 6869 7465 222c 2022 706c 6f74  ly_white", "plot
+00000a90: 6c79 5f64 6172 6b22 2c20 2267 6770 6c6f  ly_dark", "ggplo
+00000aa0: 7432 222c 2022 7365 6162 6f72 6e22 2c20  t2", "seaborn", 
+00000ab0: 2273 696d 706c 655f 7768 6974 6522 2c20  "simple_white", 
+00000ac0: 226e 6f6e 6522 5d60 2e20 4966 2079 6f75  "none"]`. If you
+00000ad0: 2077 616e 7420 746f 2063 7573 746f 6d69   want to customi
+00000ae0: 7a65 2079 6f75 7220 6f77 6e20 7465 6d70  ze your own temp
+00000af0: 6c61 7465 2c20 796f 7520 6361 6e20 6578  late, you can ex
+00000b00: 706f 7274 2069 7420 6173 2061 204a 534f  port it as a JSO
+00000b10: 4e20 6669 6c65 2061 6e64 2070 726f 7669  N file and provi
+00000b20: 6465 2069 7473 2072 656c 6174 6976 6520  de its relative 
+00000b30: 7061 7468 2069 6e20 6f70 7469 6f6e 732e  path in options.
+00000b40: 0d0a                                     ..
```

### Comparing `mkdocs-plotly-plugin-0.1.2/mkdocs_plotly_plugin/fences.py` & `mkdocs-plotly-plugin-0.1.3/mkdocs_plotly_plugin/fences.py`

 * *Files identical despite different names*

### Comparing `mkdocs-plotly-plugin-0.1.2/mkdocs_plotly_plugin/javascripts/mkdocs-plotly-plugin.js` & `mkdocs-plotly-plugin-0.1.3/mkdocs_plotly_plugin/javascripts/mkdocs-plotly-plugin.js`

 * *Files identical despite different names*

### Comparing `mkdocs-plotly-plugin-0.1.2/mkdocs_plotly_plugin/plugin.py` & `mkdocs-plotly-plugin-0.1.3/mkdocs_plotly_plugin/plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 import os
 
 from mkdocs.plugins import BasePlugin
 from mkdocs import utils
 from mkdocs.exceptions import PluginError
 from bs4 import BeautifulSoup
 from mkdocs.config import config_options
+from flatten_dict import flatten
+import json
 
 from mkdocs_plotly_plugin.fences import fence_plotly
 
 base_path = os.path.dirname(os.path.abspath(__file__))
 print(base_path)
 
 CUSTOM_FENCES = [
     {"name": "plotly", "class": "plotly-chart", "format": fence_plotly}]
 
 TEMPLATES = ["plotly", "plotly_min", "plotly_dark_min", "plotly_white", "plotly_dark",
                         "ggplot2", "seaborn", "simple_white", "none"]
 
+
 class PlotlyChartsPlugin(BasePlugin):
     config_scheme = (
         ("lib_path", config_options.Type(str, default='')),
         ("template_default", config_options.Type(str, default='plotly_min')),
         ("template_slate", config_options.Type(str, default='plotly_dark_min')),
         ("enable_template", config_options.Type(bool, default=True))
     )
@@ -50,42 +53,52 @@
             lib_url = utils.get_relative_url(
                 utils.normalize_url("assets/javascripts/plotly.min.js"),
                 page.url
             )
         lib_link.attrs['src'] = lib_url
         soup.head.append(lib_link)
         docs_dir = config['docs_dir']
-        
+
         if self.config['enable_template']:
             if self.config['template_default'] in TEMPLATES:
                 template_default_file = os.path.join(
                     base_path, "templates", f"{self.config['template_default']}.json")
             else:
                 template_default_file = os.path.join(
                     docs_dir, self.config['template_default'])
             if self.config['template_slate'] in TEMPLATES:
                 template_slate_file = os.path.join(
                     base_path, "templates", f"{self.config['template_slate']}.json")
             else:
                 template_slate_file = os.path.join(
                     docs_dir, self.config['template_slate'])
 
-            template_default = soup.new_tag("span")
-            template_default.attrs['hidden'] = True
-            with open(template_default_file) as f:
-                template_default.string = f.read()
-            template_default.attrs['id'] = 'default-template-settings'
+            def create_template_span(span_id, template_file):
+                """
+                Create a span element which holds the default templates for plotly charts.
+                We flatten the template so that plotly only updates specified attributes
+                only and doesn't replace the entire sub-object.
+                https://plotly.com/javascript/plotlyjs-function-reference/#plotlyrestyle
+                The template json file can be nested to improve readability.
+                """
+                template_span = soup.new_tag('span')
+                template_span.attrs['id'] = span_id
+                template_span.attrs['hidden'] = True
+                with open(template_file) as f:
+                    template_dict = json.load(f)
+
+                template_dict = flatten(template_dict, reducer='dot')
+                # json dumps will make the json str short to reduce size of html doc
+                template_span.string = json.dumps(template_dict)
+                return template_span
+
+            template_default = create_template_span('default-template-settings', template_default_file)
             soup.body.append(template_default)
-            
-            
-            template_slate = soup.new_tag("span")
-            template_slate.attrs['hidden'] = True
-            with open(template_slate_file) as f:
-                template_slate.string = f.read()
-            template_slate.attrs['id'] = 'slate-template-settings'
+
+            template_slate = create_template_span('slate-template-settings', template_slate_file)
             soup.body.append(template_slate)
 
         js_code = soup.new_tag("script")
         js_code.attrs['src'] = utils.get_relative_url(
             utils.normalize_url("assets/javascripts/mkdocs-plotly-plugin.js"),
             page.url
         )
```

### Comparing `mkdocs-plotly-plugin-0.1.2/mkdocs_plotly_plugin/templates/ggplot2.json` & `mkdocs-plotly-plugin-0.1.3/mkdocs_plotly_plugin/templates/ggplot2.json`

 * *Files identical despite different names*

### Comparing `mkdocs-plotly-plugin-0.1.2/mkdocs_plotly_plugin/templates/plotly.json` & `mkdocs-plotly-plugin-0.1.3/mkdocs_plotly_plugin/templates/plotly.json`

 * *Files identical despite different names*

### Comparing `mkdocs-plotly-plugin-0.1.2/mkdocs_plotly_plugin/templates/plotly_dark.json` & `mkdocs-plotly-plugin-0.1.3/mkdocs_plotly_plugin/templates/plotly_dark.json`

 * *Files identical despite different names*

### Comparing `mkdocs-plotly-plugin-0.1.2/mkdocs_plotly_plugin/templates/plotly_dark_min.json` & `mkdocs-plotly-plugin-0.1.3/mkdocs_plotly_plugin/templates/plotly_dark_min.json`

 * *Files identical despite different names*

### Comparing `mkdocs-plotly-plugin-0.1.2/mkdocs_plotly_plugin/templates/plotly_min.json` & `mkdocs-plotly-plugin-0.1.3/mkdocs_plotly_plugin/templates/plotly_min.json`

 * *Files identical despite different names*

### Comparing `mkdocs-plotly-plugin-0.1.2/mkdocs_plotly_plugin/templates/plotly_white.json` & `mkdocs-plotly-plugin-0.1.3/mkdocs_plotly_plugin/templates/plotly_white.json`

 * *Files identical despite different names*

### Comparing `mkdocs-plotly-plugin-0.1.2/mkdocs_plotly_plugin/templates/seaborn.json` & `mkdocs-plotly-plugin-0.1.3/mkdocs_plotly_plugin/templates/seaborn.json`

 * *Files identical despite different names*

### Comparing `mkdocs-plotly-plugin-0.1.2/mkdocs_plotly_plugin/templates/simple_white.json` & `mkdocs-plotly-plugin-0.1.3/mkdocs_plotly_plugin/templates/simple_white.json`

 * *Files identical despite different names*

### Comparing `mkdocs-plotly-plugin-0.1.2/mkdocs_plotly_plugin.egg-info/PKG-INFO` & `mkdocs-plotly-plugin-0.1.3/mkdocs_plotly_plugin.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,31 @@
 Metadata-Version: 2.1
 Name: mkdocs-plotly-plugin
-Version: 0.1.2
+Version: 0.1.3
 Summary: MkDocs plugin to add plotly charts from plotly's json data
 Home-page: https://github.com/haoda-li/mkdocs-plotly-plugin
 Author: Haoda Li
 Author-email: haoda_li@berkeley.edu
 License: MIT
 Keywords: mkdocs plugin
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 
 # Mkdocs Plotly Plugin
 
-![PyPI](https://img.shields.io/pypi/v/mkdocs-plotly-plugin)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/mkdocs-plotly-plugin)
-![PyPI - License](https://img.shields.io/pypi/l/mkdocs-plotly-plugin)
+![PyPI](https://img.shields.io/pypi/v/mkdocs-plotly-plugin?style=for-the-badge)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/mkdocs-plotly-plugin?style=for-the-badge)
+![PyPI - License](https://img.shields.io/pypi/l/mkdocs-plotly-plugin?style=for-the-badge)
 
 [MkDocs](https://www.mkdocs.org/) plugin to create interactive charts from data using the declarative [plotly](https://plotly.com/javascript/)'s json syntax. 
 
 Includes supports for [mkdocs-material](https://github.com/squidfunk/mkdocs-material) theme features like [instant loading](https://squidfunk.github.io/mkdocs-material/setup/setting-up-navigation/?h=reload#instant-loading) and [dark color themes](https://squidfunk.github.io/mkdocs-material/setup/changing-the-colors/#color-palette-toggle).
 
 ## Installation
 
@@ -57,24 +53,16 @@
 
 You can insert any valid plotly JSON as a codeblock using:
 ````
 ``` plotly
 {
     "data": [
         {
-            "x": [
-                "giraffes",
-                "orangutans",
-                "monkeys"
-            ],
-            "y": [
-                20,
-                14,
-                23
-            ],
+            "x": ["giraffes", "orangutans", "monkeys"],
+            "y": [20, 14, 23],
             "type": "bar"
         }
     ]
 }
 ```
 ````
```

### Comparing `mkdocs-plotly-plugin-0.1.2/mkdocs_plotly_plugin.egg-info/SOURCES.txt` & `mkdocs-plotly-plugin-0.1.3/mkdocs_plotly_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs-plotly-plugin-0.1.2/setup.py` & `mkdocs-plotly-plugin-0.1.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="mkdocs-plotly-plugin",
-    version="0.1.2",
+    version="0.1.3",
     description="MkDocs plugin to add plotly charts from plotly's json data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="mkdocs plugin",
     url="https://github.com/haoda-li/mkdocs-plotly-plugin",
     author="Haoda Li",
     author_email="haoda_li@berkeley.edu",
     license="MIT",
     python_requires=">=3.6",
     classifiers=[
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: MIT License",
     ],
-    install_requires=["mkdocs>=1.1", "pymdown-extensions>=9.2", "beautifulsoup4>=4.11.1"],
+    install_requires=["mkdocs>=1.1", "pymdown-extensions>=9.2", "beautifulsoup4>=4.11.1", "flatten-dict>=0.4.2"],
     packages=find_packages(),
     include_package_data=True,
     entry_points={
         "mkdocs.plugins": ["plotly = mkdocs_plotly_plugin.plugin:PlotlyChartsPlugin"]
     },
 )
```

