# Comparing `tmp/gaiacalc-1.0.0.tar.gz` & `tmp/gaiacalc-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaiacalc-1.0.0.tar", last modified: Wed Jul 19 11:15:43 2023, max compression
+gzip compressed data, was "gaiacalc-1.1.0.tar", last modified: Mon Jul 24 14:02:23 2023, max compression
```

## Comparing `gaiacalc-1.0.0.tar` & `gaiacalc-1.1.0.tar`

### file list

```diff
@@ -1,70 +1,71 @@
-drwxr-xr-x   0 loutre     (501) staff       (20)        0 2023-07-19 11:15:43.142588 gaiacalc-1.0.0/
--rw-rw-r--   0 loutre     (501) staff       (20)     1074 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/LICENCE
--rw-rw-r--   0 loutre     (501) staff       (20)      151 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/MANIFEST.in
--rw-r--r--   0 loutre     (501) staff       (20)     1581 2023-07-19 11:15:43.142399 gaiacalc-1.0.0/PKG-INFO
--rw-rw-r--   0 loutre     (501) staff       (20)     1157 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/README.txt
--rw-rw-r--   0 loutre     (501) staff       (20)      705 2023-07-19 11:15:26.000000 gaiacalc-1.0.0/pyproject.toml
--rw-r--r--   0 loutre     (501) staff       (20)       38 2023-07-19 11:15:43.142641 gaiacalc-1.0.0/setup.cfg
-drwxr-xr-x   0 loutre     (501) staff       (20)        0 2023-07-19 11:15:43.079686 gaiacalc-1.0.0/src/
-drwxr-xr-x   0 loutre     (501) staff       (20)        0 2023-07-19 11:15:43.082923 gaiacalc-1.0.0/src/gaiacalc/
--rw-rw-r--   0 loutre     (501) staff       (20)        0 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/__init__.py
-drwxr-xr-x   0 loutre     (501) staff       (20)        0 2023-07-19 11:15:43.092973 gaiacalc-1.0.0/src/gaiacalc/data/
-drwxr-xr-x   0 loutre     (501) staff       (20)        0 2023-07-19 11:15:43.125372 gaiacalc-1.0.0/src/gaiacalc/data/DA/
--rw-rw-r--   0 loutre     (501) staff       (20)   197356 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DA/024DA.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   297389 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DA/027DA.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   345908 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DA/032DA.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   377655 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DA/036DA.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   399219 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DA/043DA.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   843078 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DA/045DA.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   203346 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DA/053DA.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   193163 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DA/058DA.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   193163 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DA/066DA.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   212331 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DA/083DA.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   205143 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DA/095DA.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   206341 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DA/09DA.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   193762 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DA/100DA.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   203346 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DA/105DA.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   365076 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DA/110DA.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   354893 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DA/116DA.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   336923 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DA/122DA.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   390234 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DA/129DA.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   766467 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DA.grid
-drwxr-xr-x   0 loutre     (501) staff       (20)        0 2023-07-19 11:15:43.138830 gaiacalc-1.0.0/src/gaiacalc/data/DB/
--rw-rw-r--   0 loutre     (501) staff       (20)   413398 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DB/051DB.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   210322 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DB/054DB.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   189686 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DB/058DB.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   170457 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DB/066DB.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   237993 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DB/074DB.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   258160 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DB/087DB.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   162015 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DB/095DB.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   165298 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DB/100DB.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   169519 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DB/110DB.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   264726 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DB/116DB.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   442008 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DB/122DB.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   238462 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DB/129DB.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   751111 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DB.grid
--rw-rw-r--   0 loutre     (501) staff       (20)      499 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/bye.html
--rw-rw-r--   0 loutre     (501) staff       (20)    84806 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/gaiacalc.png
--rw-rw-r--   0 loutre     (501) staff       (20)     1241 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/guide.html
--rw-rw-r--   0 loutre     (501) staff       (20)     6744 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/guide.png
--rw-rw-r--   0 loutre     (501) staff       (20)     4053 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/install.html
--rw-rw-r--   0 loutre     (501) staff       (20)    17103 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/logoUPC.jpg
--rw-rw-r--   0 loutre     (501) staff       (20)     5613 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/page.html
--rw-rw-r--   0 loutre     (501) staff       (20)     1710 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/question.jpg
--rw-rw-r--   0 loutre     (501) staff       (20)     7503 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/quit.jpg
--rw-rw-r--   0 loutre     (501) staff       (20)   981440 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/samples.csv
--rw-rw-r--   0 loutre     (501) staff       (20)     4394 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/gaiacalc.py
--rw-rw-r--   0 loutre     (501) staff       (20)    16031 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/index.py
-drwxr-xr-x   0 loutre     (501) staff       (20)        0 2023-07-19 11:15:43.142047 gaiacalc-1.0.0/src/gaiacalc/log/
--rw-rw-r--   0 loutre     (501) staff       (20)       71 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/log/empty.log
--rw-rw-r--   0 loutre     (501) staff       (20)     7124 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/loop.py
--rw-rw-r--   0 loutre     (501) staff       (20)     6348 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/show.py
--rw-rw-r--   0 loutre     (501) staff       (20)     4668 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/util.py
--rw-rw-r--   0 loutre     (501) staff       (20)     4036 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/webserver.py
-drwxr-xr-x   0 loutre     (501) staff       (20)        0 2023-07-19 11:15:43.084037 gaiacalc-1.0.0/src/gaiacalc.egg-info/
--rw-r--r--   0 loutre     (501) staff       (20)     1581 2023-07-19 11:15:43.000000 gaiacalc-1.0.0/src/gaiacalc.egg-info/PKG-INFO
--rw-r--r--   0 loutre     (501) staff       (20)     1724 2023-07-19 11:15:43.000000 gaiacalc-1.0.0/src/gaiacalc.egg-info/SOURCES.txt
--rw-r--r--   0 loutre     (501) staff       (20)        1 2023-07-19 11:15:43.000000 gaiacalc-1.0.0/src/gaiacalc.egg-info/dependency_links.txt
--rw-r--r--   0 loutre     (501) staff       (20)       56 2023-07-19 11:15:43.000000 gaiacalc-1.0.0/src/gaiacalc.egg-info/entry_points.txt
--rw-r--r--   0 loutre     (501) staff       (20)       75 2023-07-19 11:15:43.000000 gaiacalc-1.0.0/src/gaiacalc.egg-info/requires.txt
--rw-r--r--   0 loutre     (501) staff       (20)        9 2023-07-19 11:15:43.000000 gaiacalc-1.0.0/src/gaiacalc.egg-info/top_level.txt
+drwxr-xr-x   0 nicolas    (502) staff       (20)        0 2023-07-24 14:02:23.986984 gaiacalc-1.1.0/
+-rw-r--r--   0 nicolas    (502) staff       (20)     1074 2023-07-24 13:57:14.000000 gaiacalc-1.1.0/LICENCE
+-rw-r--r--   0 nicolas    (502) staff       (20)      151 2023-07-24 13:57:13.000000 gaiacalc-1.1.0/MANIFEST.in
+-rw-r--r--   0 nicolas    (502) staff       (20)     1581 2023-07-24 14:02:23.986323 gaiacalc-1.1.0/PKG-INFO
+-rw-r--r--   0 nicolas    (502) staff       (20)     1157 2023-07-24 13:57:24.000000 gaiacalc-1.1.0/README.txt
+-rw-r--r--   0 nicolas    (502) staff       (20)      705 2023-07-24 14:01:23.000000 gaiacalc-1.1.0/pyproject.toml
+-rw-r--r--   0 nicolas    (502) staff       (20)       38 2023-07-24 14:02:23.987311 gaiacalc-1.1.0/setup.cfg
+drwxr-xr-x   0 nicolas    (502) staff       (20)        0 2023-07-24 14:02:23.769744 gaiacalc-1.1.0/src/
+drwxr-xr-x   0 nicolas    (502) staff       (20)        0 2023-07-24 14:02:23.780232 gaiacalc-1.1.0/src/gaiacalc/
+-rw-r--r--   0 nicolas    (502) staff       (20)        0 2023-07-24 13:57:15.000000 gaiacalc-1.1.0/src/gaiacalc/__init__.py
+drwxr-xr-x   0 nicolas    (502) staff       (20)        0 2023-07-24 14:02:23.821052 gaiacalc-1.1.0/src/gaiacalc/data/
+-rw-r--r--   0 nicolas    (502) staff       (20)     6148 2023-07-24 13:57:19.000000 gaiacalc-1.1.0/src/gaiacalc/data/.DS_Store
+drwxr-xr-x   0 nicolas    (502) staff       (20)        0 2023-07-24 14:02:23.918384 gaiacalc-1.1.0/src/gaiacalc/data/DA/
+-rw-r--r--   0 nicolas    (502) staff       (20)   197356 2023-07-24 13:57:17.000000 gaiacalc-1.1.0/src/gaiacalc/data/DA/024DA.dat
+-rw-r--r--   0 nicolas    (502) staff       (20)   297389 2023-07-24 13:57:17.000000 gaiacalc-1.1.0/src/gaiacalc/data/DA/027DA.dat
+-rw-r--r--   0 nicolas    (502) staff       (20)   345908 2023-07-24 13:57:19.000000 gaiacalc-1.1.0/src/gaiacalc/data/DA/032DA.dat
+-rw-r--r--   0 nicolas    (502) staff       (20)   377655 2023-07-24 13:57:16.000000 gaiacalc-1.1.0/src/gaiacalc/data/DA/036DA.dat
+-rw-r--r--   0 nicolas    (502) staff       (20)   399219 2023-07-24 13:57:15.000000 gaiacalc-1.1.0/src/gaiacalc/data/DA/043DA.dat
+-rw-r--r--   0 nicolas    (502) staff       (20)   843078 2023-07-24 13:57:17.000000 gaiacalc-1.1.0/src/gaiacalc/data/DA/045DA.dat
+-rw-r--r--   0 nicolas    (502) staff       (20)   203346 2023-07-24 13:57:17.000000 gaiacalc-1.1.0/src/gaiacalc/data/DA/053DA.dat
+-rw-r--r--   0 nicolas    (502) staff       (20)   193163 2023-07-24 13:57:16.000000 gaiacalc-1.1.0/src/gaiacalc/data/DA/058DA.dat
+-rw-r--r--   0 nicolas    (502) staff       (20)   193163 2023-07-24 13:57:16.000000 gaiacalc-1.1.0/src/gaiacalc/data/DA/066DA.dat
+-rw-r--r--   0 nicolas    (502) staff       (20)   212331 2023-07-24 13:57:18.000000 gaiacalc-1.1.0/src/gaiacalc/data/DA/083DA.dat
+-rw-r--r--   0 nicolas    (502) staff       (20)   205143 2023-07-24 13:57:19.000000 gaiacalc-1.1.0/src/gaiacalc/data/DA/095DA.dat
+-rw-r--r--   0 nicolas    (502) staff       (20)   206341 2023-07-24 13:57:19.000000 gaiacalc-1.1.0/src/gaiacalc/data/DA/09DA.dat
+-rw-r--r--   0 nicolas    (502) staff       (20)   193762 2023-07-24 13:57:18.000000 gaiacalc-1.1.0/src/gaiacalc/data/DA/100DA.dat
+-rw-r--r--   0 nicolas    (502) staff       (20)   203346 2023-07-24 13:57:18.000000 gaiacalc-1.1.0/src/gaiacalc/data/DA/105DA.dat
+-rw-r--r--   0 nicolas    (502) staff       (20)   365076 2023-07-24 13:57:18.000000 gaiacalc-1.1.0/src/gaiacalc/data/DA/110DA.dat
+-rw-r--r--   0 nicolas    (502) staff       (20)   354893 2023-07-24 13:57:18.000000 gaiacalc-1.1.0/src/gaiacalc/data/DA/116DA.dat
+-rw-r--r--   0 nicolas    (502) staff       (20)   336923 2023-07-24 13:57:17.000000 gaiacalc-1.1.0/src/gaiacalc/data/DA/122DA.dat
+-rw-r--r--   0 nicolas    (502) staff       (20)   390234 2023-07-24 13:57:16.000000 gaiacalc-1.1.0/src/gaiacalc/data/DA/129DA.dat
+-rw-r--r--   0 nicolas    (502) staff       (20)   766467 2023-07-24 13:57:21.000000 gaiacalc-1.1.0/src/gaiacalc/data/DA.grid
+drwxr-xr-x   0 nicolas    (502) staff       (20)        0 2023-07-24 14:02:23.982045 gaiacalc-1.1.0/src/gaiacalc/data/DB/
+-rw-r--r--   0 nicolas    (502) staff       (20)   413398 2023-07-24 13:57:22.000000 gaiacalc-1.1.0/src/gaiacalc/data/DB/051DB.dat
+-rw-r--r--   0 nicolas    (502) staff       (20)   210322 2023-07-24 13:57:23.000000 gaiacalc-1.1.0/src/gaiacalc/data/DB/054DB.dat
+-rw-r--r--   0 nicolas    (502) staff       (20)   189686 2023-07-24 13:57:21.000000 gaiacalc-1.1.0/src/gaiacalc/data/DB/058DB.dat
+-rw-r--r--   0 nicolas    (502) staff       (20)   170457 2023-07-24 13:57:22.000000 gaiacalc-1.1.0/src/gaiacalc/data/DB/066DB.dat
+-rw-r--r--   0 nicolas    (502) staff       (20)   237993 2023-07-24 13:57:22.000000 gaiacalc-1.1.0/src/gaiacalc/data/DB/074DB.dat
+-rw-r--r--   0 nicolas    (502) staff       (20)   258160 2023-07-24 13:57:23.000000 gaiacalc-1.1.0/src/gaiacalc/data/DB/087DB.dat
+-rw-r--r--   0 nicolas    (502) staff       (20)   162015 2023-07-24 13:57:22.000000 gaiacalc-1.1.0/src/gaiacalc/data/DB/095DB.dat
+-rw-r--r--   0 nicolas    (502) staff       (20)   165298 2023-07-24 13:57:22.000000 gaiacalc-1.1.0/src/gaiacalc/data/DB/100DB.dat
+-rw-r--r--   0 nicolas    (502) staff       (20)   169519 2023-07-24 13:57:23.000000 gaiacalc-1.1.0/src/gaiacalc/data/DB/110DB.dat
+-rw-r--r--   0 nicolas    (502) staff       (20)   264726 2023-07-24 13:57:22.000000 gaiacalc-1.1.0/src/gaiacalc/data/DB/116DB.dat
+-rw-r--r--   0 nicolas    (502) staff       (20)   442008 2023-07-24 13:57:23.000000 gaiacalc-1.1.0/src/gaiacalc/data/DB/122DB.dat
+-rw-r--r--   0 nicolas    (502) staff       (20)   238462 2023-07-24 13:57:23.000000 gaiacalc-1.1.0/src/gaiacalc/data/DB/129DB.dat
+-rw-r--r--   0 nicolas    (502) staff       (20)   751111 2023-07-24 13:57:20.000000 gaiacalc-1.1.0/src/gaiacalc/data/DB.grid
+-rw-r--r--   0 nicolas    (502) staff       (20)      499 2023-07-24 13:57:21.000000 gaiacalc-1.1.0/src/gaiacalc/data/bye.html
+-rw-r--r--   0 nicolas    (502) staff       (20)    84806 2023-07-24 13:57:19.000000 gaiacalc-1.1.0/src/gaiacalc/data/gaiacalc.png
+-rw-r--r--   0 nicolas    (502) staff       (20)    15400 2023-07-24 13:57:20.000000 gaiacalc-1.1.0/src/gaiacalc/data/guide.html
+-rw-r--r--   0 nicolas    (502) staff       (20)     6744 2023-07-24 13:57:19.000000 gaiacalc-1.1.0/src/gaiacalc/data/guide.png
+-rw-r--r--   0 nicolas    (502) staff       (20)     4081 2023-07-24 13:57:20.000000 gaiacalc-1.1.0/src/gaiacalc/data/install.html
+-rw-r--r--   0 nicolas    (502) staff       (20)    17103 2023-07-24 13:57:21.000000 gaiacalc-1.1.0/src/gaiacalc/data/logoUPC.jpg
+-rw-r--r--   0 nicolas    (502) staff       (20)     5613 2023-07-24 13:57:21.000000 gaiacalc-1.1.0/src/gaiacalc/data/page.html
+-rw-r--r--   0 nicolas    (502) staff       (20)     1710 2023-07-24 13:57:21.000000 gaiacalc-1.1.0/src/gaiacalc/data/question.jpg
+-rw-r--r--   0 nicolas    (502) staff       (20)     7503 2023-07-24 13:57:21.000000 gaiacalc-1.1.0/src/gaiacalc/data/quit.jpg
+-rw-r--r--   0 nicolas    (502) staff       (20)   981440 2023-07-24 13:57:21.000000 gaiacalc-1.1.0/src/gaiacalc/data/samples.csv
+-rw-r--r--   0 nicolas    (502) staff       (20)     4394 2023-07-24 13:57:15.000000 gaiacalc-1.1.0/src/gaiacalc/gaiacalc.py
+-rw-r--r--   0 nicolas    (502) staff       (20)    16031 2023-07-24 13:57:15.000000 gaiacalc-1.1.0/src/gaiacalc/index.py
+drwxr-xr-x   0 nicolas    (502) staff       (20)        0 2023-07-24 14:02:23.985327 gaiacalc-1.1.0/src/gaiacalc/log/
+-rw-r--r--   0 nicolas    (502) staff       (20)       71 2023-07-24 13:57:14.000000 gaiacalc-1.1.0/src/gaiacalc/log/empty.log
+-rw-r--r--   0 nicolas    (502) staff       (20)     7124 2023-07-24 13:57:15.000000 gaiacalc-1.1.0/src/gaiacalc/loop.py
+-rw-r--r--   0 nicolas    (502) staff       (20)     6348 2023-07-24 13:57:14.000000 gaiacalc-1.1.0/src/gaiacalc/show.py
+-rw-r--r--   0 nicolas    (502) staff       (20)     4668 2023-07-24 13:57:14.000000 gaiacalc-1.1.0/src/gaiacalc/util.py
+-rw-r--r--   0 nicolas    (502) staff       (20)     4036 2023-07-24 13:57:15.000000 gaiacalc-1.1.0/src/gaiacalc/webserver.py
+drwxr-xr-x   0 nicolas    (502) staff       (20)        0 2023-07-24 14:02:23.785891 gaiacalc-1.1.0/src/gaiacalc.egg-info/
+-rw-r--r--   0 nicolas    (502) staff       (20)     1581 2023-07-24 14:02:23.000000 gaiacalc-1.1.0/src/gaiacalc.egg-info/PKG-INFO
+-rw-r--r--   0 nicolas    (502) staff       (20)     1752 2023-07-24 14:02:23.000000 gaiacalc-1.1.0/src/gaiacalc.egg-info/SOURCES.txt
+-rw-r--r--   0 nicolas    (502) staff       (20)        1 2023-07-24 14:02:23.000000 gaiacalc-1.1.0/src/gaiacalc.egg-info/dependency_links.txt
+-rw-r--r--   0 nicolas    (502) staff       (20)       56 2023-07-24 14:02:23.000000 gaiacalc-1.1.0/src/gaiacalc.egg-info/entry_points.txt
+-rw-r--r--   0 nicolas    (502) staff       (20)       75 2023-07-24 14:02:23.000000 gaiacalc-1.1.0/src/gaiacalc.egg-info/requires.txt
+-rw-r--r--   0 nicolas    (502) staff       (20)        9 2023-07-24 14:02:23.000000 gaiacalc-1.1.0/src/gaiacalc.egg-info/top_level.txt
```

### Comparing `gaiacalc-1.0.0/LICENCE` & `gaiacalc-1.1.0/LICENCE`

 * *Files identical despite different names*

### Comparing `gaiacalc-1.0.0/PKG-INFO` & `gaiacalc-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaiacalc
-Version: 1.0.0
+Version: 1.1.0
 Summary: Gaia white dwarfs parameter interpolator
 Author-email: Julie Doligez <julie@doligez.fr>
 Project-URL: Homepage, http://gaia.doligez.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `gaiacalc-1.0.0/README.txt` & `gaiacalc-1.1.0/README.txt`

 * *Files identical despite different names*

### Comparing `gaiacalc-1.0.0/pyproject.toml` & `gaiacalc-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gaiacalc"
-version = "1.0.0"
+version = "1.1.0"
 authors = [
 { name="Julie Doligez", email="julie@doligez.fr" }
 ]
 description = "Gaia white dwarfs parameter interpolator"
 readme = "README.txt"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `gaiacalc-1.0.0/src/gaiacalc/data/DA/024DA.dat` & `gaiacalc-1.1.0/src/gaiacalc/data/DA/024DA.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-1.0.0/src/gaiacalc/data/DA/027DA.dat` & `gaiacalc-1.1.0/src/gaiacalc/data/DA/027DA.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-1.0.0/src/gaiacalc/data/DA/032DA.dat` & `gaiacalc-1.1.0/src/gaiacalc/data/DA/032DA.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-1.0.0/src/gaiacalc/data/DA/036DA.dat` & `gaiacalc-1.1.0/src/gaiacalc/data/DA/036DA.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-1.0.0/src/gaiacalc/data/DA/043DA.dat` & `gaiacalc-1.1.0/src/gaiacalc/data/DA/043DA.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-1.0.0/src/gaiacalc/data/DA/045DA.dat` & `gaiacalc-1.1.0/src/gaiacalc/data/DA/045DA.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-1.0.0/src/gaiacalc/data/DA/053DA.dat` & `gaiacalc-1.1.0/src/gaiacalc/data/DA/053DA.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-1.0.0/src/gaiacalc/data/DA/058DA.dat` & `gaiacalc-1.1.0/src/gaiacalc/data/DA/058DA.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-1.0.0/src/gaiacalc/data/DA/066DA.dat` & `gaiacalc-1.1.0/src/gaiacalc/data/DA/066DA.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-1.0.0/src/gaiacalc/data/DA/083DA.dat` & `gaiacalc-1.1.0/src/gaiacalc/data/DA/083DA.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-1.0.0/src/gaiacalc/data/DA/095DA.dat` & `gaiacalc-1.1.0/src/gaiacalc/data/DA/095DA.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-1.0.0/src/gaiacalc/data/DA/09DA.dat` & `gaiacalc-1.1.0/src/gaiacalc/data/DA/09DA.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-1.0.0/src/gaiacalc/data/DA/100DA.dat` & `gaiacalc-1.1.0/src/gaiacalc/data/DA/100DA.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-1.0.0/src/gaiacalc/data/DA/105DA.dat` & `gaiacalc-1.1.0/src/gaiacalc/data/DA/105DA.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-1.0.0/src/gaiacalc/data/DA/110DA.dat` & `gaiacalc-1.1.0/src/gaiacalc/data/DA/110DA.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-1.0.0/src/gaiacalc/data/DA/116DA.dat` & `gaiacalc-1.1.0/src/gaiacalc/data/DA/116DA.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-1.0.0/src/gaiacalc/data/DA/122DA.dat` & `gaiacalc-1.1.0/src/gaiacalc/data/DA/122DA.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-1.0.0/src/gaiacalc/data/DA/129DA.dat` & `gaiacalc-1.1.0/src/gaiacalc/data/DA/129DA.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-1.0.0/src/gaiacalc/data/DA.grid` & `gaiacalc-1.1.0/src/gaiacalc/data/DA.grid`

 * *Files identical despite different names*

### Comparing `gaiacalc-1.0.0/src/gaiacalc/data/DB/051DB.dat` & `gaiacalc-1.1.0/src/gaiacalc/data/DB/051DB.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-1.0.0/src/gaiacalc/data/DB/054DB.dat` & `gaiacalc-1.1.0/src/gaiacalc/data/DB/054DB.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-1.0.0/src/gaiacalc/data/DB/058DB.dat` & `gaiacalc-1.1.0/src/gaiacalc/data/DB/058DB.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-1.0.0/src/gaiacalc/data/DB/066DB.dat` & `gaiacalc-1.1.0/src/gaiacalc/data/DB/066DB.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-1.0.0/src/gaiacalc/data/DB/074DB.dat` & `gaiacalc-1.1.0/src/gaiacalc/data/DB/074DB.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-1.0.0/src/gaiacalc/data/DB/087DB.dat` & `gaiacalc-1.1.0/src/gaiacalc/data/DB/087DB.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-1.0.0/src/gaiacalc/data/DB/095DB.dat` & `gaiacalc-1.1.0/src/gaiacalc/data/DB/095DB.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-1.0.0/src/gaiacalc/data/DB/100DB.dat` & `gaiacalc-1.1.0/src/gaiacalc/data/DB/100DB.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-1.0.0/src/gaiacalc/data/DB/110DB.dat` & `gaiacalc-1.1.0/src/gaiacalc/data/DB/110DB.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-1.0.0/src/gaiacalc/data/DB/116DB.dat` & `gaiacalc-1.1.0/src/gaiacalc/data/DB/116DB.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-1.0.0/src/gaiacalc/data/DB/122DB.dat` & `gaiacalc-1.1.0/src/gaiacalc/data/DB/122DB.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-1.0.0/src/gaiacalc/data/DB/129DB.dat` & `gaiacalc-1.1.0/src/gaiacalc/data/DB/129DB.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-1.0.0/src/gaiacalc/data/DB.grid` & `gaiacalc-1.1.0/src/gaiacalc/data/DB.grid`

 * *Files identical despite different names*

### Comparing `gaiacalc-1.0.0/src/gaiacalc/data/gaiacalc.png` & `gaiacalc-1.1.0/src/gaiacalc/data/gaiacalc.png`

 * *Files identical despite different names*

### Comparing `gaiacalc-1.0.0/src/gaiacalc/data/guide.png` & `gaiacalc-1.1.0/src/gaiacalc/data/guide.png`

 * *Files identical despite different names*

### Comparing `gaiacalc-1.0.0/src/gaiacalc/data/install.html` & `gaiacalc-1.1.0/src/gaiacalc/data/install.html`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
       
       On Windows, use a cmd window and type this:
       py -m pip install gaiacalc
       Then you get a gaiacalc command : type "gaiacalc" then RETURN key
       
       ------------------------------------------------------------------------------------------------------
       
-      <a id=deb></a>Download deb package for linux debian
+      <a id=deb href=drop?file=gaiacalc.deb></a>Download deb package for linux debian
 
       This package is for IT administrators.
       It will turn your debian 11 server as a gaiacalc server.
       The user will access gaiacalc web page with URL : http://yourservername.com
       
       First ensure that pip3 is installed (not included in debian11 on OVH cloud)
       Otherwise type this :
```

### Comparing `gaiacalc-1.0.0/src/gaiacalc/data/logoUPC.jpg` & `gaiacalc-1.1.0/src/gaiacalc/data/logoUPC.jpg`

 * *Files identical despite different names*

### Comparing `gaiacalc-1.0.0/src/gaiacalc/data/page.html` & `gaiacalc-1.1.0/src/gaiacalc/data/page.html`

 * *Files 1% similar despite different names*

```diff
@@ -179,12 +179,12 @@
 
       <div id="rectangle">
       Download your gaiacalc<br><br>
       <a href=page?name=install.html#app>app for MacOS</a><br>
       <a href=page?name=install.html#exe>exe for Windows</a><br>
       <a href=page?name=install.html#pip>python pip3 package</a><br>
       <a href=page?name=install.html#deb>linux debian package</a><br>
-      <a href=page?name=install.html#git>code source github</a><br>
+      <a href=page?name=install.html#git>github source code</a><br>
       </div>
       
   </body>
 </html>
```

#### html2text {}

```diff
@@ -48,8 +48,8 @@
 oh_yeah,_I_want_this_one
 Download your gaiacalc
 
 app_for_MacOS
 exe_for_Windows
 python_pip3_package
 linux_debian_package
-code_source_github
+github_source_code
```

### Comparing `gaiacalc-1.0.0/src/gaiacalc/data/question.jpg` & `gaiacalc-1.1.0/src/gaiacalc/data/question.jpg`

 * *Files identical despite different names*

### Comparing `gaiacalc-1.0.0/src/gaiacalc/data/quit.jpg` & `gaiacalc-1.1.0/src/gaiacalc/data/quit.jpg`

 * *Files identical despite different names*

### Comparing `gaiacalc-1.0.0/src/gaiacalc/data/samples.csv` & `gaiacalc-1.1.0/src/gaiacalc/data/samples.csv`

 * *Files identical despite different names*

### Comparing `gaiacalc-1.0.0/src/gaiacalc/gaiacalc.py` & `gaiacalc-1.1.0/src/gaiacalc/gaiacalc.py`

 * *Files identical despite different names*

### Comparing `gaiacalc-1.0.0/src/gaiacalc/index.py` & `gaiacalc-1.1.0/src/gaiacalc/index.py`

 * *Files identical despite different names*

### Comparing `gaiacalc-1.0.0/src/gaiacalc/loop.py` & `gaiacalc-1.1.0/src/gaiacalc/loop.py`

 * *Files identical despite different names*

### Comparing `gaiacalc-1.0.0/src/gaiacalc/show.py` & `gaiacalc-1.1.0/src/gaiacalc/show.py`

 * *Files identical despite different names*

### Comparing `gaiacalc-1.0.0/src/gaiacalc/util.py` & `gaiacalc-1.1.0/src/gaiacalc/util.py`

 * *Files identical despite different names*

### Comparing `gaiacalc-1.0.0/src/gaiacalc/webserver.py` & `gaiacalc-1.1.0/src/gaiacalc/webserver.py`

 * *Files identical despite different names*

### Comparing `gaiacalc-1.0.0/src/gaiacalc.egg-info/PKG-INFO` & `gaiacalc-1.1.0/src/gaiacalc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaiacalc
-Version: 1.0.0
+Version: 1.1.0
 Summary: Gaia white dwarfs parameter interpolator
 Author-email: Julie Doligez <julie@doligez.fr>
 Project-URL: Homepage, http://gaia.doligez.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `gaiacalc-1.0.0/src/gaiacalc.egg-info/SOURCES.txt` & `gaiacalc-1.1.0/src/gaiacalc.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 src/gaiacalc/webserver.py
 src/gaiacalc.egg-info/PKG-INFO
 src/gaiacalc.egg-info/SOURCES.txt
 src/gaiacalc.egg-info/dependency_links.txt
 src/gaiacalc.egg-info/entry_points.txt
 src/gaiacalc.egg-info/requires.txt
 src/gaiacalc.egg-info/top_level.txt
+src/gaiacalc/data/.DS_Store
 src/gaiacalc/data/DA.grid
 src/gaiacalc/data/DB.grid
 src/gaiacalc/data/bye.html
 src/gaiacalc/data/gaiacalc.png
 src/gaiacalc/data/guide.html
 src/gaiacalc/data/guide.png
 src/gaiacalc/data/install.html
```

