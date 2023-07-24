# Comparing `tmp/urlscan-1.0.0.tar.gz` & `tmp/urlscan-1.0.1.tar.gz`

## Comparing `urlscan-1.0.0.tar` & `urlscan-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 urlscan-1.0.0/urlscan/__init__.py
--rw-r--r--   0        0        0     8296 2020-02-02 00:00:00.000000 urlscan-1.0.0/urlscan/__main__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 urlscan-1.0.0/urlscan/_version.py
--rw-r--r--   0        0        0    37006 2020-02-02 00:00:00.000000 urlscan-1.0.0/urlscan/urlchoose.py
--rw-r--r--   0        0        0    17573 2020-02-02 00:00:00.000000 urlscan-1.0.0/urlscan/urlscan.py
--rw-r--r--   0        0        0     9912 2020-02-02 00:00:00.000000 urlscan-1.0.0/urlscan/assets/tlds-alpha-by-domain.txt
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 urlscan-1.0.0/.gitignore
--rw-r--r--   0        0        0    17987 2020-02-02 00:00:00.000000 urlscan-1.0.0/LICENSE
--rw-r--r--   0        0        0     7902 2020-02-02 00:00:00.000000 urlscan-1.0.0/README.md
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 urlscan-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     8866 2020-02-02 00:00:00.000000 urlscan-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     7322 2020-02-02 00:00:00.000000 urlscan-1.0.1/urlscan.1
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 urlscan-1.0.1/urlscan/__init__.py
+-rw-r--r--   0        0        0     8296 2020-02-02 00:00:00.000000 urlscan-1.0.1/urlscan/__main__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 urlscan-1.0.1/urlscan/_version.py
+-rw-r--r--   0        0        0    37006 2020-02-02 00:00:00.000000 urlscan-1.0.1/urlscan/urlchoose.py
+-rw-r--r--   0        0        0    17573 2020-02-02 00:00:00.000000 urlscan-1.0.1/urlscan/urlscan.py
+-rw-r--r--   0        0        0     9912 2020-02-02 00:00:00.000000 urlscan-1.0.1/urlscan/assets/tlds-alpha-by-domain.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 urlscan-1.0.1/.gitignore
+-rw-r--r--   0        0        0    17987 2020-02-02 00:00:00.000000 urlscan-1.0.1/LICENSE
+-rw-r--r--   0        0        0     7902 2020-02-02 00:00:00.000000 urlscan-1.0.1/README.md
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 urlscan-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     8866 2020-02-02 00:00:00.000000 urlscan-1.0.1/PKG-INFO
```

### Comparing `urlscan-1.0.0/urlscan/__main__.py` & `urlscan-1.0.1/urlscan/__main__.py`

 * *Files identical despite different names*

### Comparing `urlscan-1.0.0/urlscan/urlchoose.py` & `urlscan-1.0.1/urlscan/urlchoose.py`

 * *Files identical despite different names*

### Comparing `urlscan-1.0.0/urlscan/urlscan.py` & `urlscan-1.0.1/urlscan/urlscan.py`

 * *Files identical despite different names*

### Comparing `urlscan-1.0.0/urlscan/assets/tlds-alpha-by-domain.txt` & `urlscan-1.0.1/urlscan/assets/tlds-alpha-by-domain.txt`

 * *Files identical despite different names*

### Comparing `urlscan-1.0.0/LICENSE` & `urlscan-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `urlscan-1.0.0/README.md` & `urlscan-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `urlscan-1.0.0/pyproject.toml` & `urlscan-1.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -52,8 +52,9 @@
 LICENSE = "share/doc/urlscan/LICENSE"
 "README.md" = "share/doc/urlscan/README.md"
 "urlscan.1" = "share/man/man1/urlscan.1"
 
 [tool.hatch.build.targets.sdist]
 include = [
     "/urlscan",
+    "urlscan.1",
 ]
```

### Comparing `urlscan-1.0.0/PKG-INFO` & `urlscan-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urlscan
-Version: 1.0.0
+Version: 1.0.1
 Summary: View/select the URLs in an email message or file
 Project-URL: Homepage, https://github.com/firecat53/urlscan
 Author-email: Scott Hansen <tech@firecat53.net>
 License-Expression: GPL-2.0
 License-File: LICENSE
 Keywords: email,mutt,tmux,urlscan,urlview
 Classifier: Development Status :: 5 - Production/Stable
```

