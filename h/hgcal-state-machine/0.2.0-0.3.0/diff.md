# Comparing `tmp/hgcal_state_machine-0.2.0.tar.gz` & `tmp/hgcal_state_machine-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hgcal_state_machine-0.2.0.tar", last modified: Mon Jul 24 13:45:37 2023, max compression
+gzip compressed data, was "hgcal_state_machine-0.3.0.tar", last modified: Mon Jul 24 14:11:13 2023, max compression
```

## Comparing `hgcal_state_machine-0.2.0.tar` & `hgcal_state_machine-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
-drwxr-xr-x   0 simondejean   (501) staff       (20)        0 2023-07-24 13:45:37.695663 hgcal_state_machine-0.2.0/
--rw-r--r--   0 simondejean   (501) staff       (20)      144 2023-07-24 13:45:37.695569 hgcal_state_machine-0.2.0/PKG-INFO
-drwxr-xr-x   0 simondejean   (501) staff       (20)        0 2023-07-24 13:45:37.695413 hgcal_state_machine-0.2.0/hgcal_state_machine.egg-info/
--rw-r--r--   0 simondejean   (501) staff       (20)      144 2023-07-24 13:45:37.000000 hgcal_state_machine-0.2.0/hgcal_state_machine.egg-info/PKG-INFO
--rw-r--r--   0 simondejean   (501) staff       (20)      222 2023-07-24 13:45:37.000000 hgcal_state_machine-0.2.0/hgcal_state_machine.egg-info/SOURCES.txt
--rw-r--r--   0 simondejean   (501) staff       (20)        1 2023-07-24 13:45:37.000000 hgcal_state_machine-0.2.0/hgcal_state_machine.egg-info/dependency_links.txt
--rw-r--r--   0 simondejean   (501) staff       (20)       12 2023-07-24 13:45:37.000000 hgcal_state_machine-0.2.0/hgcal_state_machine.egg-info/requires.txt
--rw-r--r--   0 simondejean   (501) staff       (20)       14 2023-07-24 13:45:37.000000 hgcal_state_machine-0.2.0/hgcal_state_machine.egg-info/top_level.txt
--rw-r--r--   0 simondejean   (501) staff       (20)       38 2023-07-24 13:45:37.695699 hgcal_state_machine-0.2.0/setup.cfg
--rw-r--r--   0 simondejean   (501) staff       (20)      192 2023-07-24 13:45:18.000000 hgcal_state_machine-0.2.0/setup.py
+drwxr-xr-x   0 simondejean   (501) staff       (20)        0 2023-07-24 14:11:13.415924 hgcal_state_machine-0.3.0/
+-rw-r--r--   0 simondejean   (501) staff       (20)      144 2023-07-24 14:11:13.415814 hgcal_state_machine-0.3.0/PKG-INFO
+drwxr-xr-x   0 simondejean   (501) staff       (20)        0 2023-07-24 14:11:13.415636 hgcal_state_machine-0.3.0/hgcal_state_machine.egg-info/
+-rw-r--r--   0 simondejean   (501) staff       (20)      144 2023-07-24 14:11:13.000000 hgcal_state_machine-0.3.0/hgcal_state_machine.egg-info/PKG-INFO
+-rw-r--r--   0 simondejean   (501) staff       (20)      245 2023-07-24 14:11:13.000000 hgcal_state_machine-0.3.0/hgcal_state_machine.egg-info/SOURCES.txt
+-rw-r--r--   0 simondejean   (501) staff       (20)        1 2023-07-24 14:11:13.000000 hgcal_state_machine-0.3.0/hgcal_state_machine.egg-info/dependency_links.txt
+-rw-r--r--   0 simondejean   (501) staff       (20)       12 2023-07-24 14:11:13.000000 hgcal_state_machine-0.3.0/hgcal_state_machine.egg-info/requires.txt
+-rw-r--r--   0 simondejean   (501) staff       (20)       20 2023-07-24 14:11:13.000000 hgcal_state_machine-0.3.0/hgcal_state_machine.egg-info/top_level.txt
+-rw-r--r--   0 simondejean   (501) staff       (20)     3980 2023-07-24 13:46:44.000000 hgcal_state_machine-0.3.0/hgcal_state_machine.py
+-rw-r--r--   0 simondejean   (501) staff       (20)       38 2023-07-24 14:11:13.415966 hgcal_state_machine-0.3.0/setup.cfg
+-rw-r--r--   0 simondejean   (501) staff       (20)      198 2023-07-24 14:11:09.000000 hgcal_state_machine-0.3.0/setup.py
```

