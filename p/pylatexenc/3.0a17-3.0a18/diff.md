# Comparing `tmp/pylatexenc-3.0a17.tar.gz` & `tmp/pylatexenc-3.0a18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylatexenc-3.0a17.tar", max compression
+gzip compressed data, was "pylatexenc-3.0a18.tar", max compression
```

## Comparing `pylatexenc-3.0a17.tar` & `pylatexenc-3.0a18.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0     1086 2023-04-15 13:24:30.143033 pylatexenc-3.0a17/LICENSE.txt
--rw-r--r--   0        0        0     3572 2023-04-18 07:57:57.261013 pylatexenc-3.0a17/README.rst
--rw-r--r--   0        0        0     1326 2019-07-25 20:20:56.000000 pylatexenc-3.0a17/pylatexenc/__init__.py
--rw-r--r--   0        0        0     5083 2023-05-10 17:45:32.190520 pylatexenc-3.0a17/pylatexenc/_util.py
--rw-r--r--   0        0        0     3766 2023-04-15 11:29:53.841423 pylatexenc-3.0a17/pylatexenc/_util_support.py
--rw-r--r--   0        0        0    59269 2023-04-15 11:57:13.282343 pylatexenc-3.0a17/pylatexenc/latex2text/__init__.py
--rw-r--r--   0        0        0    10011 2023-04-15 11:55:00.471421 pylatexenc-3.0a17/pylatexenc/latex2text/__main__.py
--rw-r--r--   0        0        0    94342 2023-04-15 11:29:53.843500 pylatexenc-3.0a17/pylatexenc/latex2text/_defaultspecs.py
--rw-r--r--   0        0        0     2526 2021-12-17 19:22:56.000000 pylatexenc-3.0a17/pylatexenc/latex2text/_inputlatexfile.py
--rw-r--r--   0        0        0    12910 2023-05-10 22:25:03.185982 pylatexenc-3.0a17/pylatexenc/latexencode/__init__.py
--rw-r--r--   0        0        0     4426 2019-08-25 13:06:29.000000 pylatexenc-3.0a17/pylatexenc/latexencode/__main__.py
--rw-r--r--   0        0        0     4344 2023-05-10 22:44:33.867148 pylatexenc-3.0a17/pylatexenc/latexencode/_partial_latex_encoder.py
--rw-r--r--   0        0        0     7516 2023-05-10 22:31:54.454547 pylatexenc-3.0a17/pylatexenc/latexencode/_rule.py
--rw-r--r--   0        0        0    99833 2021-09-15 19:08:59.000000 pylatexenc-3.0a17/pylatexenc/latexencode/_uni2latexmap.py
--rw-r--r--   0        0        0    55947 2019-07-27 15:08:32.000000 pylatexenc-3.0a17/pylatexenc/latexencode/_uni2latexmap_xml.py
--rw-r--r--   0        0        0    20901 2023-05-10 22:39:39.968571 pylatexenc-3.0a17/pylatexenc/latexencode/_unicode_to_latex_encoder.py
--rw-r--r--   0        0        0     3748 2023-05-10 22:33:06.225330 pylatexenc-3.0a17/pylatexenc/latexencode/get_builtin_rules.py
--rw-r--r--   0        0        0     2179 2023-04-15 11:29:53.843788 pylatexenc-3.0a17/pylatexenc/latexnodes/__init__.py
--rw-r--r--   0        0        0     2197 2023-04-15 17:44:53.955715 pylatexenc-3.0a17/pylatexenc/latexnodes/_callablespecbase.py
--rw-r--r--   0        0        0    11001 2023-04-15 17:53:09.732071 pylatexenc-3.0a17/pylatexenc/latexnodes/_exctypes.py
--rw-r--r--   0        0        0     6315 2023-04-15 17:52:07.518222 pylatexenc-3.0a17/pylatexenc/latexnodes/_latexcontextdbbase.py
--rw-r--r--   0        0        0    36523 2023-04-27 21:55:57.200105 pylatexenc-3.0a17/pylatexenc/latexnodes/_nodescollector.py
--rw-r--r--   0        0        0    10100 2023-04-27 21:53:07.906038 pylatexenc-3.0a17/pylatexenc/latexnodes/_parsedargs.py
--rw-r--r--   0        0        0    11877 2023-04-15 11:29:53.845584 pylatexenc-3.0a17/pylatexenc/latexnodes/_parsedargsinfo.py
--rw-r--r--   0        0        0    17020 2023-04-15 17:51:09.423753 pylatexenc-3.0a17/pylatexenc/latexnodes/_parsingstate.py
--rw-r--r--   0        0        0     6625 2023-04-27 21:47:43.535760 pylatexenc-3.0a17/pylatexenc/latexnodes/_parsingstatedelta.py
--rw-r--r--   0        0        0     8446 2023-04-15 17:12:48.503604 pylatexenc-3.0a17/pylatexenc/latexnodes/_token.py
--rw-r--r--   0        0        0    27524 2023-04-27 21:49:33.263808 pylatexenc-3.0a17/pylatexenc/latexnodes/_tokenreader.py
--rw-r--r--   0        0        0    10098 2023-04-15 17:13:31.159345 pylatexenc-3.0a17/pylatexenc/latexnodes/_tokenreaderbase.py
--rw-r--r--   0        0        0     4841 2023-04-15 17:50:19.637390 pylatexenc-3.0a17/pylatexenc/latexnodes/_walkerbase.py
--rw-r--r--   0        0        0    42458 2023-04-27 21:51:03.724446 pylatexenc-3.0a17/pylatexenc/latexnodes/nodes.py
--rw-r--r--   0        0        0     2141 2023-04-15 11:29:53.848262 pylatexenc-3.0a17/pylatexenc/latexnodes/parsers/__init__.py
--rw-r--r--   0        0        0     5285 2023-04-15 11:29:53.848639 pylatexenc-3.0a17/pylatexenc/latexnodes/parsers/_base.py
--rw-r--r--   0        0        0    41228 2023-04-27 21:59:01.687959 pylatexenc-3.0a17/pylatexenc/latexnodes/parsers/_delimited.py
--rw-r--r--   0        0        0    18288 2023-04-15 11:29:53.849524 pylatexenc-3.0a17/pylatexenc/latexnodes/parsers/_expression.py
--rw-r--r--   0        0        0    12896 2023-04-15 11:29:53.849773 pylatexenc-3.0a17/pylatexenc/latexnodes/parsers/_generalnodes.py
--rw-r--r--   0        0        0     5658 2023-04-15 11:29:53.849985 pylatexenc-3.0a17/pylatexenc/latexnodes/parsers/_math.py
--rw-r--r--   0        0        0     6180 2023-04-15 11:29:53.850252 pylatexenc-3.0a17/pylatexenc/latexnodes/parsers/_optionals.py
--rw-r--r--   0        0        0    22370 2023-04-15 16:46:34.476752 pylatexenc-3.0a17/pylatexenc/latexnodes/parsers/_stdarg.py
--rw-r--r--   0        0        0    11551 2023-04-18 07:57:57.274724 pylatexenc-3.0a17/pylatexenc/latexnodes/parsers/_verbatim.py
--rw-r--r--   0        0        0     4520 2023-04-15 11:29:53.851132 pylatexenc-3.0a17/pylatexenc/latexwalker/__init__.py
--rw-r--r--   0        0        0     6214 2023-04-15 11:29:53.851406 pylatexenc-3.0a17/pylatexenc/latexwalker/__main__.py
--rw-r--r--   0        0        0    17597 2023-04-26 15:29:33.456920 pylatexenc-3.0a17/pylatexenc/latexwalker/_defaultspecs.py
--rw-r--r--   0        0        0     2937 2023-04-15 11:29:53.852111 pylatexenc-3.0a17/pylatexenc/latexwalker/_get_defaultspecs.py
--rw-r--r--   0        0        0     7833 2023-04-15 11:29:53.852354 pylatexenc-3.0a17/pylatexenc/latexwalker/_helpers.py
--rw-r--r--   0        0        0     7487 2023-04-15 11:29:53.852626 pylatexenc-3.0a17/pylatexenc/latexwalker/_legacy_py1x.py
--rw-r--r--   0        0        0    52642 2023-04-15 11:37:07.707893 pylatexenc-3.0a17/pylatexenc/latexwalker/_walker.py
--rw-r--r--   0        0        0     2449 2023-05-01 13:36:34.698244 pylatexenc-3.0a17/pylatexenc/macrospec/__init__.py
--rw-r--r--   0        0        0     8819 2023-04-18 07:57:57.275339 pylatexenc-3.0a17/pylatexenc/macrospec/_argumentsparser.py
--rw-r--r--   0        0        0     7372 2023-04-15 11:29:53.853904 pylatexenc-3.0a17/pylatexenc/macrospec/_environmentbodyparser.py
--rw-r--r--   0        0        0    29928 2023-04-27 08:01:22.265622 pylatexenc-3.0a17/pylatexenc/macrospec/_latexcontextdb.py
--rw-r--r--   0        0        0    10046 2023-04-15 20:38:58.126785 pylatexenc-3.0a17/pylatexenc/macrospec/_macrocallparser.py
--rw-r--r--   0        0        0     1535 2023-04-15 11:29:53.854841 pylatexenc-3.0a17/pylatexenc/macrospec/_pyltxenc2_argparsers/__init__.py
--rw-r--r--   0        0        0     9488 2023-04-18 07:57:57.275664 pylatexenc-3.0a17/pylatexenc/macrospec/_pyltxenc2_argparsers/_base.py
--rw-r--r--   0        0        0    16735 2023-04-18 07:57:57.276084 pylatexenc-3.0a17/pylatexenc/macrospec/_pyltxenc2_argparsers/_verbatimargsparser.py
--rw-r--r--   0        0        0    21655 2023-05-01 13:56:41.086895 pylatexenc-3.0a17/pylatexenc/macrospec/_specclasses.py
--rw-r--r--   0        0        0     8951 2023-04-15 11:29:53.855874 pylatexenc-3.0a17/pylatexenc/macrospec/_spechelpers.py
--rw-r--r--   0        0        0     2115 2023-05-10 22:59:12.276101 pylatexenc-3.0a17/pylatexenc/version.py
--rw-r--r--   0        0        0     1091 2023-05-10 22:59:04.979992 pylatexenc-3.0a17/pyproject.toml
--rw-r--r--   0        0        0     4209 1970-01-01 00:00:00.000000 pylatexenc-3.0a17/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-07-24 13:49:02.058283 pylatexenc-3.0a18/LICENSE.txt
+-rw-r--r--   0        0        0     3572 2023-07-24 13:49:02.058283 pylatexenc-3.0a18/README.rst
+-rw-r--r--   0        0        0     1326 2023-07-24 13:49:02.058283 pylatexenc-3.0a18/pylatexenc/__init__.py
+-rw-r--r--   0        0        0     5083 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/_util.py
+-rw-r--r--   0        0        0     3766 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/_util_support.py
+-rw-r--r--   0        0        0    59269 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latex2text/__init__.py
+-rw-r--r--   0        0        0    10011 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latex2text/__main__.py
+-rw-r--r--   0        0        0    94342 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latex2text/_defaultspecs.py
+-rw-r--r--   0        0        0     2526 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latex2text/_inputlatexfile.py
+-rw-r--r--   0        0        0    12910 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latexencode/__init__.py
+-rw-r--r--   0        0        0     4426 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latexencode/__main__.py
+-rw-r--r--   0        0        0     4344 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latexencode/_partial_latex_encoder.py
+-rw-r--r--   0        0        0     7516 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latexencode/_rule.py
+-rw-r--r--   0        0        0    99833 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latexencode/_uni2latexmap.py
+-rw-r--r--   0        0        0    55947 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latexencode/_uni2latexmap_xml.py
+-rw-r--r--   0        0        0    20894 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latexencode/_unicode_to_latex_encoder.py
+-rw-r--r--   0        0        0     3748 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latexencode/get_builtin_rules.py
+-rw-r--r--   0        0        0     2209 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latexnodes/__init__.py
+-rw-r--r--   0        0        0     2197 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latexnodes/_callablespecbase.py
+-rw-r--r--   0        0        0    11001 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latexnodes/_exctypes.py
+-rw-r--r--   0        0        0     6315 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latexnodes/_latexcontextdbbase.py
+-rw-r--r--   0        0        0    36523 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latexnodes/_nodescollector.py
+-rw-r--r--   0        0        0    10100 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latexnodes/_parsedargs.py
+-rw-r--r--   0        0        0    11877 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latexnodes/_parsedargsinfo.py
+-rw-r--r--   0        0        0    17020 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latexnodes/_parsingstate.py
+-rw-r--r--   0        0        0     7279 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latexnodes/_parsingstatedelta.py
+-rw-r--r--   0        0        0     8446 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latexnodes/_token.py
+-rw-r--r--   0        0        0    27524 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latexnodes/_tokenreader.py
+-rw-r--r--   0        0        0    10098 2023-07-24 13:49:02.062283 pylatexenc-3.0a18/pylatexenc/latexnodes/_tokenreaderbase.py
+-rw-r--r--   0        0        0     4841 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/latexnodes/_walkerbase.py
+-rw-r--r--   0        0        0    42458 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/latexnodes/nodes.py
+-rw-r--r--   0        0        0     2141 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/latexnodes/parsers/__init__.py
+-rw-r--r--   0        0        0     5285 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/latexnodes/parsers/_base.py
+-rw-r--r--   0        0        0    41228 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/latexnodes/parsers/_delimited.py
+-rw-r--r--   0        0        0    18288 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/latexnodes/parsers/_expression.py
+-rw-r--r--   0        0        0    12896 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/latexnodes/parsers/_generalnodes.py
+-rw-r--r--   0        0        0     5658 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/latexnodes/parsers/_math.py
+-rw-r--r--   0        0        0     6180 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/latexnodes/parsers/_optionals.py
+-rw-r--r--   0        0        0    22370 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/latexnodes/parsers/_stdarg.py
+-rw-r--r--   0        0        0    11551 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/latexnodes/parsers/_verbatim.py
+-rw-r--r--   0        0        0     4520 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/latexwalker/__init__.py
+-rw-r--r--   0        0        0     6214 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/latexwalker/__main__.py
+-rw-r--r--   0        0        0    17597 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/latexwalker/_defaultspecs.py
+-rw-r--r--   0        0        0     2937 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/latexwalker/_get_defaultspecs.py
+-rw-r--r--   0        0        0     7833 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/latexwalker/_helpers.py
+-rw-r--r--   0        0        0     7487 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/latexwalker/_legacy_py1x.py
+-rw-r--r--   0        0        0    52642 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/latexwalker/_walker.py
+-rw-r--r--   0        0        0     2449 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/macrospec/__init__.py
+-rw-r--r--   0        0        0     8819 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/macrospec/_argumentsparser.py
+-rw-r--r--   0        0        0     7372 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/macrospec/_environmentbodyparser.py
+-rw-r--r--   0        0        0    29928 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/macrospec/_latexcontextdb.py
+-rw-r--r--   0        0        0    10046 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/macrospec/_macrocallparser.py
+-rw-r--r--   0        0        0     1535 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/macrospec/_pyltxenc2_argparsers/__init__.py
+-rw-r--r--   0        0        0     9488 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/macrospec/_pyltxenc2_argparsers/_base.py
+-rw-r--r--   0        0        0    16735 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/macrospec/_pyltxenc2_argparsers/_verbatimargsparser.py
+-rw-r--r--   0        0        0    22030 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/macrospec/_specclasses.py
+-rw-r--r--   0        0        0     8951 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/macrospec/_spechelpers.py
+-rw-r--r--   0        0        0     2115 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pylatexenc/version.py
+-rw-r--r--   0        0        0     1091 2023-07-24 13:49:02.066283 pylatexenc-3.0a18/pyproject.toml
+-rw-r--r--   0        0        0     4209 1970-01-01 00:00:00.000000 pylatexenc-3.0a18/PKG-INFO
```

### Comparing `pylatexenc-3.0a17/LICENSE.txt` & `pylatexenc-3.0a18/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/README.rst` & `pylatexenc-3.0a18/README.rst`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/__init__.py` & `pylatexenc-3.0a18/pylatexenc/__init__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/_util.py` & `pylatexenc-3.0a18/pylatexenc/_util.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/_util_support.py` & `pylatexenc-3.0a18/pylatexenc/_util_support.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/latex2text/__init__.py` & `pylatexenc-3.0a18/pylatexenc/latex2text/__init__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/latex2text/__main__.py` & `pylatexenc-3.0a18/pylatexenc/latex2text/__main__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/latex2text/_defaultspecs.py` & `pylatexenc-3.0a18/pylatexenc/latex2text/_defaultspecs.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/latex2text/_inputlatexfile.py` & `pylatexenc-3.0a18/pylatexenc/latex2text/_inputlatexfile.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/latexencode/__init__.py` & `pylatexenc-3.0a18/pylatexenc/latexencode/__init__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/latexencode/__main__.py` & `pylatexenc-3.0a18/pylatexenc/latexencode/__main__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/latexencode/_partial_latex_encoder.py` & `pylatexenc-3.0a18/pylatexenc/latexencode/_partial_latex_encoder.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/latexencode/_rule.py` & `pylatexenc-3.0a18/pylatexenc/latexencode/_rule.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/latexencode/_uni2latexmap.py` & `pylatexenc-3.0a18/pylatexenc/latexencode/_uni2latexmap.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/latexencode/_uni2latexmap_xml.py` & `pylatexenc-3.0a18/pylatexenc/latexencode/_uni2latexmap_xml.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/latexencode/_unicode_to_latex_encoder.py` & `pylatexenc-3.0a18/pylatexenc/latexencode/_unicode_to_latex_encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 #__pragma__('ecom')
 """?
 __pragma__('js', 'var HexstrN = (v, N=4) => (+v).toString(16).toUpperCase().padStart(N, "0")');
 ?"""
 
 #__pragma__('skip')
 def HexstrN(value, N=4):
-    return f'{value:x}' .zfill(N).upper()
+    return ('%X'%(value)).zfill(N)
 #__pragma__('noskip')
 
 
 
 ## Transcrypt currently does not provide an implementation of m.expand() or
 ## rx.match(..., pos=) ... :/
```

### Comparing `pylatexenc-3.0a17/pylatexenc/latexencode/get_builtin_rules.py` & `pylatexenc-3.0a18/pylatexenc/latexencode/get_builtin_rules.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/latexnodes/__init__.py` & `pylatexenc-3.0a18/pylatexenc/latexnodes/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 from ._parsingstate import (
     ParsingState
 )
 
 from ._parsingstatedelta import (
     ParsingStateDelta,
     ParsingStateDeltaReplaceParsingState,
+    ParsingStateDeltaChained,
     ParsingStateDeltaWalkerEvent,
     ParsingStateDeltaEnterMathMode,
     ParsingStateDeltaLeaveMathMode,
     get_updated_parsing_state_from_delta,
 )
 from ._parsedargs import (
     LatexArgumentSpec,
```

### Comparing `pylatexenc-3.0a17/pylatexenc/latexnodes/_callablespecbase.py` & `pylatexenc-3.0a18/pylatexenc/latexnodes/_callablespecbase.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/latexnodes/_exctypes.py` & `pylatexenc-3.0a18/pylatexenc/latexnodes/_exctypes.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/latexnodes/_latexcontextdbbase.py` & `pylatexenc-3.0a18/pylatexenc/latexnodes/_latexcontextdbbase.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/latexnodes/_nodescollector.py` & `pylatexenc-3.0a18/pylatexenc/latexnodes/_nodescollector.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/latexnodes/_parsedargs.py` & `pylatexenc-3.0a18/pylatexenc/latexnodes/_parsedargs.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/latexnodes/_parsedargsinfo.py` & `pylatexenc-3.0a18/pylatexenc/latexnodes/_parsedargsinfo.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/latexnodes/_parsingstate.py` & `pylatexenc-3.0a18/pylatexenc/latexnodes/_parsingstate.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/latexnodes/_parsingstatedelta.py` & `pylatexenc-3.0a18/pylatexenc/latexnodes/_parsingstatedelta.py`

 * *Files 5% similar despite different names*

```diff
@@ -97,14 +97,36 @@
 
     def get_updated_parsing_state(self, parsing_state, latex_walker):
         if self.set_parsing_state is not None:
             return self.set_parsing_state
         return parsing_state
 
 
+
+
+class ParsingStateDeltaChained(ParsingStateDelta):
+    r"""
+    Apply multiple parsing state deltas, in the order specified.
+    """
+    def __init__(self, parsing_state_deltas, **kwargs):
+        super(ParsingStateDeltaChained, self).__init__(
+            _fields=('parsing_state_deltas',),
+            **kwargs
+        )
+        self.parsing_state_deltas = parsing_state_deltas
+
+    def get_updated_parsing_state(self, parsing_state, latex_walker):
+        ps = parsing_state
+        for delta in self.parsing_state_deltas:
+            if delta is not None:
+                ps = delta.get_updated_parsing_state(ps, latex_walker)
+        return ps
+
+
+
 # ------------------------------------------------------------------------------
 
 #
 # parsing state delta's associated with walker events
 #
 
 class ParsingStateDeltaWalkerEvent(ParsingStateDelta):
```

### Comparing `pylatexenc-3.0a17/pylatexenc/latexnodes/_token.py` & `pylatexenc-3.0a18/pylatexenc/latexnodes/_token.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/latexnodes/_tokenreader.py` & `pylatexenc-3.0a18/pylatexenc/latexnodes/_tokenreader.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/latexnodes/_tokenreaderbase.py` & `pylatexenc-3.0a18/pylatexenc/latexnodes/_tokenreaderbase.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/latexnodes/_walkerbase.py` & `pylatexenc-3.0a18/pylatexenc/latexnodes/_walkerbase.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/latexnodes/nodes.py` & `pylatexenc-3.0a18/pylatexenc/latexnodes/nodes.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/latexnodes/parsers/__init__.py` & `pylatexenc-3.0a18/pylatexenc/latexnodes/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/latexnodes/parsers/_base.py` & `pylatexenc-3.0a18/pylatexenc/latexnodes/parsers/_base.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/latexnodes/parsers/_delimited.py` & `pylatexenc-3.0a18/pylatexenc/latexnodes/parsers/_delimited.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/latexnodes/parsers/_expression.py` & `pylatexenc-3.0a18/pylatexenc/latexnodes/parsers/_expression.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/latexnodes/parsers/_generalnodes.py` & `pylatexenc-3.0a18/pylatexenc/latexnodes/parsers/_generalnodes.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/latexnodes/parsers/_math.py` & `pylatexenc-3.0a18/pylatexenc/latexnodes/parsers/_math.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/latexnodes/parsers/_optionals.py` & `pylatexenc-3.0a18/pylatexenc/latexnodes/parsers/_optionals.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/latexnodes/parsers/_stdarg.py` & `pylatexenc-3.0a18/pylatexenc/latexnodes/parsers/_stdarg.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/latexnodes/parsers/_verbatim.py` & `pylatexenc-3.0a18/pylatexenc/latexnodes/parsers/_verbatim.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/latexwalker/__init__.py` & `pylatexenc-3.0a18/pylatexenc/latexwalker/__init__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/latexwalker/__main__.py` & `pylatexenc-3.0a18/pylatexenc/latexwalker/__main__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/latexwalker/_defaultspecs.py` & `pylatexenc-3.0a18/pylatexenc/latexwalker/_defaultspecs.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/latexwalker/_get_defaultspecs.py` & `pylatexenc-3.0a18/pylatexenc/latexwalker/_get_defaultspecs.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/latexwalker/_helpers.py` & `pylatexenc-3.0a18/pylatexenc/latexwalker/_helpers.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/latexwalker/_legacy_py1x.py` & `pylatexenc-3.0a18/pylatexenc/latexwalker/_legacy_py1x.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/latexwalker/_walker.py` & `pylatexenc-3.0a18/pylatexenc/latexwalker/_walker.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/macrospec/__init__.py` & `pylatexenc-3.0a18/pylatexenc/macrospec/__init__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/macrospec/_argumentsparser.py` & `pylatexenc-3.0a18/pylatexenc/macrospec/_argumentsparser.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/macrospec/_environmentbodyparser.py` & `pylatexenc-3.0a18/pylatexenc/macrospec/_environmentbodyparser.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/macrospec/_latexcontextdb.py` & `pylatexenc-3.0a18/pylatexenc/macrospec/_latexcontextdb.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/macrospec/_macrocallparser.py` & `pylatexenc-3.0a18/pylatexenc/macrospec/_macrocallparser.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/macrospec/_pyltxenc2_argparsers/__init__.py` & `pylatexenc-3.0a18/pylatexenc/macrospec/_pyltxenc2_argparsers/__init__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/macrospec/_pyltxenc2_argparsers/_base.py` & `pylatexenc-3.0a18/pylatexenc/macrospec/_pyltxenc2_argparsers/_base.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/macrospec/_pyltxenc2_argparsers/_verbatimargsparser.py` & `pylatexenc-3.0a18/pylatexenc/macrospec/_pyltxenc2_argparsers/_verbatimargsparser.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/macrospec/_specclasses.py` & `pylatexenc-3.0a18/pylatexenc/macrospec/_specclasses.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,21 @@
 _legacy_pyltxenc2_do = lambda *args: None
 
 
 class _NotSpecified:
     pass
 
 
+_spec_node_parser_types = {
+    'macro': LatexMacroCallParser,
+    'environment': LatexEnvironmentCallParser,
+    'specials': LatexSpecialsCallParser,
+}
+
+
 class CallableSpec(CallableSpecBase):
     r"""
     Base class for :py:class:`MacroSpec`, :py:class:`EnvironmentSpec` and
     :py:class:`SpecialsSpec` classes regrouping common functionality.
 
     Doc. ................
 
@@ -91,19 +98,23 @@
                  environmentname=_NotSpecified,
                  specials_chars=_NotSpecified,
                  make_arguments_parsing_state_delta=None,
                  make_body_parsing_state_delta=None,
                  make_after_parsing_state_delta=None,
                  make_body_parser=None,
                  finalize_node=None,
+                 # also accepts `body_parsing_state_delta` as kwargs ->
                  **kwargs):
 
         self.arguments_spec_list = arguments_spec_list
 
         self.spec_node_parser_type = spec_node_parser_type
+        if isinstance(spec_node_parser_type, _basestring):
+            self.spec_node_parser_type = _spec_node_parser_types[spec_node_parser_type]
+
         if macroname is not _NotSpecified:
             self.macroname = macroname
         if environmentname is not _NotSpecified:
             self.environmentname = environmentname
         if specials_chars is not _NotSpecified:
             self.specials_chars = specials_chars
```

### Comparing `pylatexenc-3.0a17/pylatexenc/macrospec/_spechelpers.py` & `pylatexenc-3.0a18/pylatexenc/macrospec/_spechelpers.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a17/pylatexenc/version.py` & `pylatexenc-3.0a18/pylatexenc/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,8 +51,8 @@
 #   7) on github.com, fill in release details with a summary of changes etc.
 #
 #   8) create the source package for PyPI (" python3 setup.py sdist ")
 #   
 #   8) upload package to PyPI (twine upload dist/pylatexenc-X.X.tar.gz -r realpypi)
 #
 
-version_str = "3.0alpha000017"
+version_str = "3.0alpha000018"
```

### Comparing `pylatexenc-3.0a17/pyproject.toml` & `pylatexenc-3.0a18/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pylatexenc"
-version = "3.0alpha000017" # ALSO BUMP IN pylatexenc/version.py
+version = "3.0alpha000018" # ALSO BUMP IN pylatexenc/version.py
 description = "Simple LaTeX parser providing latex-to-unicode and unicode-to-latex conversion"
 authors = ["Philippe Faist <philippe.faist@bluewin.ch>"]
 license = "MIT"
 readme = "README.rst"
 
 [tool.poetry.scripts]
 latexwalker = 'pylatexenc.latexwalker.__main__:main'
```

### Comparing `pylatexenc-3.0a17/PKG-INFO` & `pylatexenc-3.0a18/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylatexenc
-Version: 3.0a17
+Version: 3.0a18
 Summary: Simple LaTeX parser providing latex-to-unicode and unicode-to-latex conversion
 License: MIT
 Author: Philippe Faist
 Author-email: philippe.faist@bluewin.ch
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

