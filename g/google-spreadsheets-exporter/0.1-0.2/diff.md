# Comparing `tmp/google_spreadsheets_exporter-0.1.tar.gz` & `tmp/google_spreadsheets_exporter-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google_spreadsheets_exporter-0.1.tar", last modified: Sun Jul 23 15:01:19 2023, max compression
+gzip compressed data, was "google_spreadsheets_exporter-0.2.tar", last modified: Mon Jul 24 14:08:27 2023, max compression
```

## Comparing `google_spreadsheets_exporter-0.1.tar` & `google_spreadsheets_exporter-0.2.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-23 15:01:19.030836 google_spreadsheets_exporter-0.1/
--rw-rw-rw-   0        0        0       73 2023-07-23 15:01:19.030836 google_spreadsheets_exporter-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-23 15:01:18.984607 google_spreadsheets_exporter-0.1/google_spreadsheets_exporter/
--rw-rw-rw-   0        0        0        0 2023-07-23 14:47:50.000000 google_spreadsheets_exporter-0.1/google_spreadsheets_exporter/__init__.py
--rw-rw-rw-   0        0        0      186 2023-07-23 14:52:23.000000 google_spreadsheets_exporter-0.1/google_spreadsheets_exporter/exporter.py
-drwxrwxrwx   0        0        0        0 2023-07-23 15:01:19.028836 google_spreadsheets_exporter-0.1/google_spreadsheets_exporter.egg-info/
--rw-rw-rw-   0        0        0       73 2023-07-23 15:01:18.000000 google_spreadsheets_exporter-0.1/google_spreadsheets_exporter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      349 2023-07-23 15:01:18.000000 google_spreadsheets_exporter-0.1/google_spreadsheets_exporter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-23 15:01:18.000000 google_spreadsheets_exporter-0.1/google_spreadsheets_exporter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-07-23 15:01:18.000000 google_spreadsheets_exporter-0.1/google_spreadsheets_exporter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-07-23 15:01:18.000000 google_spreadsheets_exporter-0.1/google_spreadsheets_exporter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-23 15:01:19.031836 google_spreadsheets_exporter-0.1/setup.cfg
--rw-rw-rw-   0        0        0      286 2023-07-23 14:51:50.000000 google_spreadsheets_exporter-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 14:08:27.074205 google_spreadsheets_exporter-0.2/
+-rw-rw-rw-   0        0        0       97 2023-07-24 13:56:18.000000 google_spreadsheets_exporter-0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0       73 2023-07-24 14:08:27.073204 google_spreadsheets_exporter-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-24 14:08:27.063206 google_spreadsheets_exporter-0.2/google_spreadsheets_exporter/
+-rw-rw-rw-   0        0        0        0 2023-07-23 14:47:50.000000 google_spreadsheets_exporter-0.2/google_spreadsheets_exporter/__init__.py
+-rw-rw-rw-   0        0        0      369 2023-07-24 13:45:30.000000 google_spreadsheets_exporter-0.2/google_spreadsheets_exporter/data_handler.py
+-rw-rw-rw-   0        0        0     1631 2023-07-24 13:45:30.000000 google_spreadsheets_exporter-0.2/google_spreadsheets_exporter/exporter.py
+-rw-rw-rw-   0        0        0      530 2023-07-23 15:45:17.000000 google_spreadsheets_exporter-0.2/google_spreadsheets_exporter/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-24 14:08:27.072207 google_spreadsheets_exporter-0.2/google_spreadsheets_exporter.egg-info/
+-rw-rw-rw-   0        0        0       73 2023-07-24 14:08:26.000000 google_spreadsheets_exporter-0.2/google_spreadsheets_exporter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      444 2023-07-24 14:08:27.000000 google_spreadsheets_exporter-0.2/google_spreadsheets_exporter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 14:08:26.000000 google_spreadsheets_exporter-0.2/google_spreadsheets_exporter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-07-24 14:08:26.000000 google_spreadsheets_exporter-0.2/google_spreadsheets_exporter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-07-24 14:08:26.000000 google_spreadsheets_exporter-0.2/google_spreadsheets_exporter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 14:08:27.074205 google_spreadsheets_exporter-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      372 2023-07-24 14:01:32.000000 google_spreadsheets_exporter-0.2/setup.py
```

