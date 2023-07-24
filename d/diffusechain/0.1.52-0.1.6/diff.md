# Comparing `tmp/diffusechain-0.1.52.tar.gz` & `tmp/diffusechain-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diffusechain-0.1.52.tar", max compression
+gzip compressed data, was "diffusechain-0.1.6.tar", max compression
```

## Comparing `diffusechain-0.1.52.tar` & `diffusechain-0.1.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      233 2023-07-09 12:50:06.797797 diffusechain-0.1.52/diffusechain/__init__.py
--rw-r--r--   0        0        0    20316 2023-07-11 19:04:12.747191 diffusechain-0.1.52/diffusechain/Automatic1111.py
--rw-r--r--   0        0        0        0 2023-07-09 12:48:39.750318 diffusechain-0.1.52/diffusechain/chains/__init__.py
--rw-r--r--   0        0        0       73 2023-07-09 12:53:17.902435 diffusechain-0.1.52/diffusechain/chains/consistentFaceChain.py
--rw-r--r--   0        0        0       63 2023-07-09 12:14:22.417256 diffusechain-0.1.52/diffusechain/Diffusers.py
--rw-r--r--   0        0        0     1086 2023-07-11 20:22:56.335908 diffusechain-0.1.52/LICENSE
--rw-r--r--   0        0        0      415 2023-07-11 20:22:01.531309 diffusechain-0.1.52/pyproject.toml
--rw-r--r--   0        0        0     2453 2023-07-11 20:21:49.289325 diffusechain-0.1.52/README.md
--rw-r--r--   0        0        0     3028 1970-01-01 00:00:00.000000 diffusechain-0.1.52/PKG-INFO
+-rw-r--r--   0        0        0      233 2023-07-09 12:50:06.797797 diffusechain-0.1.6/diffusechain/__init__.py
+-rw-r--r--   0        0        0    36491 2023-07-24 18:09:30.941186 diffusechain-0.1.6/diffusechain/Automatic1111.py
+-rw-r--r--   0        0        0        0 2023-07-09 12:48:39.750318 diffusechain-0.1.6/diffusechain/chains/__init__.py
+-rw-r--r--   0        0        0       73 2023-07-09 12:53:17.902435 diffusechain-0.1.6/diffusechain/chains/consistentFaceChain.py
+-rw-r--r--   0        0        0       63 2023-07-09 12:14:22.417256 diffusechain-0.1.6/diffusechain/Diffusers.py
+-rw-r--r--   0        0        0     1086 2023-07-11 20:22:56.335908 diffusechain-0.1.6/LICENSE
+-rw-r--r--   0        0        0      414 2023-07-24 18:02:41.116014 diffusechain-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2453 2023-07-11 20:21:49.289325 diffusechain-0.1.6/README.md
+-rw-r--r--   0        0        0     3027 1970-01-01 00:00:00.000000 diffusechain-0.1.6/PKG-INFO
```

### Comparing `diffusechain-0.1.52/LICENSE` & `diffusechain-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `diffusechain-0.1.52/README.md` & `diffusechain-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `diffusechain-0.1.52/PKG-INFO` & `diffusechain-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffusechain
-Version: 0.1.52
+Version: 0.1.6
 Summary: 
 Author: Adithya S K
 Author-email: adithyaskolavi@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

