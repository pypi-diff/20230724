# Comparing `tmp/neurosift-0.2.1.tar.gz` & `tmp/neurosift-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurosift-0.2.1.tar", last modified: Mon Jul 24 14:38:45 2023, max compression
+gzip compressed data, was "neurosift-0.2.2.tar", last modified: Mon Jul 24 14:42:54 2023, max compression
```

## Comparing `neurosift-0.2.1.tar` & `neurosift-0.2.2.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-07-24 14:38:45.314655 neurosift-0.2.1/
--rw-rw-r--   0 magland   (1000) magland   (1000)      122 2023-07-24 14:35:52.000000 neurosift-0.2.1/MANIFEST.in
--rw-rw-r--   0 magland   (1000) magland   (1000)      431 2023-07-24 14:38:45.314655 neurosift-0.2.1/PKG-INFO
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-07-24 14:38:45.306655 neurosift-0.2.1/neurosift/
--rw-rw-r--   0 magland   (1000) magland   (1000)     8807 2023-07-19 19:27:57.000000 neurosift-0.2.1/neurosift/RtcsharePlugin.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1446 2023-07-24 14:14:28.000000 neurosift-0.2.1/neurosift/TemporaryDirectory.py
--rw-rw-r--   0 magland   (1000) magland   (1000)       42 2023-06-20 12:11:47.000000 neurosift-0.2.1/neurosift/__init__.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     2769 2023-07-24 14:34:14.000000 neurosift-0.2.1/neurosift/cli.py
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-07-24 14:38:45.310655 neurosift-0.2.1/neurosift/experimental-local-file-access/
--rw-rw-r--   0 magland   (1000) magland   (1000)      341 2023-07-21 19:24:32.000000 neurosift-0.2.1/neurosift/experimental-local-file-access/package.json
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-07-24 14:38:45.310655 neurosift-0.2.1/neurosift/views/
--rw-rw-r--   0 magland   (1000) magland   (1000)     2045 2023-06-22 16:40:24.000000 neurosift-0.2.1/neurosift/views/Autocorrelograms.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1748 2023-06-22 16:58:40.000000 neurosift-0.2.1/neurosift/views/AverageWaveforms.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     2220 2023-06-23 13:34:39.000000 neurosift-0.2.1/neurosift/views/CrossCorrelograms.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     2510 2023-06-19 17:29:34.000000 neurosift-0.2.1/neurosift/views/PositionDecodeField.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     2885 2023-06-20 14:07:42.000000 neurosift-0.2.1/neurosift/views/SpikeTrains.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1597 2023-06-15 19:12:09.000000 neurosift-0.2.1/neurosift/views/TimeseriesAnnotation.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     7414 2023-07-05 20:01:40.000000 neurosift-0.2.1/neurosift/views/TimeseriesGraph.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     2605 2023-06-14 19:14:07.000000 neurosift-0.2.1/neurosift/views/VideoAnnotation.py
--rw-rw-r--   0 magland   (1000) magland   (1000)      841 2023-06-22 17:52:19.000000 neurosift-0.2.1/neurosift/views/__init__.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     2528 2023-06-14 13:34:04.000000 neurosift-0.2.1/neurosift/views/_serialize.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     4763 2023-06-16 11:49:45.000000 neurosift-0.2.1/neurosift/views/create_audio_spectrogram.py
--rw-rw-r--   0 magland   (1000) magland   (1000)    14775 2023-06-23 15:34:16.000000 neurosift-0.2.1/neurosift/views/create_spike_sorting_digest.py
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-07-24 14:38:45.314655 neurosift-0.2.1/neurosift/views/helpers/
--rw-rw-r--   0 magland   (1000) magland   (1000)        0 2023-06-21 11:12:21.000000 neurosift-0.2.1/neurosift/views/helpers/__init__.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     3459 2023-06-21 13:38:40.000000 neurosift-0.2.1/neurosift/views/helpers/compute_correlogram_data.py
--rw-rw-r--   0 magland   (1000) magland   (1000)      831 2023-06-21 13:38:50.000000 neurosift-0.2.1/neurosift/views/helpers/compute_templates.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1059 2023-06-21 11:12:21.000000 neurosift-0.2.1/neurosift/views/helpers/extract_snippets.py
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-07-24 14:38:45.306655 neurosift-0.2.1/neurosift.egg-info/
--rw-rw-r--   0 magland   (1000) magland   (1000)      431 2023-07-24 14:38:45.000000 neurosift-0.2.1/neurosift.egg-info/PKG-INFO
--rw-rw-r--   0 magland   (1000) magland   (1000)      998 2023-07-24 14:38:45.000000 neurosift-0.2.1/neurosift.egg-info/SOURCES.txt
--rw-rw-r--   0 magland   (1000) magland   (1000)        1 2023-07-24 14:38:45.000000 neurosift-0.2.1/neurosift.egg-info/dependency_links.txt
--rw-rw-r--   0 magland   (1000) magland   (1000)       54 2023-07-24 14:38:45.000000 neurosift-0.2.1/neurosift.egg-info/entry_points.txt
--rw-rw-r--   0 magland   (1000) magland   (1000)       44 2023-07-24 14:38:45.000000 neurosift-0.2.1/neurosift.egg-info/requires.txt
--rw-rw-r--   0 magland   (1000) magland   (1000)       10 2023-07-24 14:38:45.000000 neurosift-0.2.1/neurosift.egg-info/top_level.txt
--rw-rw-r--   0 magland   (1000) magland   (1000)      478 2023-07-24 14:38:45.314655 neurosift-0.2.1/setup.cfg
--rw-rw-r--   0 magland   (1000) magland   (1000)      383 2023-07-24 14:36:11.000000 neurosift-0.2.1/setup.py
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-07-24 14:42:54.076858 neurosift-0.2.2/
+-rw-rw-r--   0 magland   (1000) magland   (1000)      123 2023-07-24 14:42:20.000000 neurosift-0.2.2/MANIFEST.in
+-rw-rw-r--   0 magland   (1000) magland   (1000)      431 2023-07-24 14:42:54.076858 neurosift-0.2.2/PKG-INFO
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-07-24 14:42:54.072858 neurosift-0.2.2/neurosift/
+-rw-rw-r--   0 magland   (1000) magland   (1000)     8807 2023-07-19 19:27:57.000000 neurosift-0.2.2/neurosift/RtcsharePlugin.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1446 2023-07-24 14:14:28.000000 neurosift-0.2.2/neurosift/TemporaryDirectory.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)       42 2023-06-20 12:11:47.000000 neurosift-0.2.2/neurosift/__init__.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     2769 2023-07-24 14:34:14.000000 neurosift-0.2.2/neurosift/cli.py
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-07-24 14:42:54.072858 neurosift-0.2.2/neurosift/experimental-local-file-access/
+-rw-rw-r--   0 magland   (1000) magland   (1000)      341 2023-07-21 19:24:32.000000 neurosift-0.2.2/neurosift/experimental-local-file-access/package.json
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-07-24 14:42:54.072858 neurosift-0.2.2/neurosift/experimental-local-file-access/src/
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1867 2023-07-24 13:53:45.000000 neurosift-0.2.2/neurosift/experimental-local-file-access/src/index.js
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-07-24 14:42:54.076858 neurosift-0.2.2/neurosift/views/
+-rw-rw-r--   0 magland   (1000) magland   (1000)     2045 2023-06-22 16:40:24.000000 neurosift-0.2.2/neurosift/views/Autocorrelograms.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1748 2023-06-22 16:58:40.000000 neurosift-0.2.2/neurosift/views/AverageWaveforms.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     2220 2023-06-23 13:34:39.000000 neurosift-0.2.2/neurosift/views/CrossCorrelograms.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     2510 2023-06-19 17:29:34.000000 neurosift-0.2.2/neurosift/views/PositionDecodeField.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     2885 2023-06-20 14:07:42.000000 neurosift-0.2.2/neurosift/views/SpikeTrains.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1597 2023-06-15 19:12:09.000000 neurosift-0.2.2/neurosift/views/TimeseriesAnnotation.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     7414 2023-07-05 20:01:40.000000 neurosift-0.2.2/neurosift/views/TimeseriesGraph.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     2605 2023-06-14 19:14:07.000000 neurosift-0.2.2/neurosift/views/VideoAnnotation.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)      841 2023-06-22 17:52:19.000000 neurosift-0.2.2/neurosift/views/__init__.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     2528 2023-06-14 13:34:04.000000 neurosift-0.2.2/neurosift/views/_serialize.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     4763 2023-06-16 11:49:45.000000 neurosift-0.2.2/neurosift/views/create_audio_spectrogram.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)    14775 2023-06-23 15:34:16.000000 neurosift-0.2.2/neurosift/views/create_spike_sorting_digest.py
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-07-24 14:42:54.076858 neurosift-0.2.2/neurosift/views/helpers/
+-rw-rw-r--   0 magland   (1000) magland   (1000)        0 2023-06-21 11:12:21.000000 neurosift-0.2.2/neurosift/views/helpers/__init__.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     3459 2023-06-21 13:38:40.000000 neurosift-0.2.2/neurosift/views/helpers/compute_correlogram_data.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)      831 2023-06-21 13:38:50.000000 neurosift-0.2.2/neurosift/views/helpers/compute_templates.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1059 2023-06-21 11:12:21.000000 neurosift-0.2.2/neurosift/views/helpers/extract_snippets.py
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-07-24 14:42:54.072858 neurosift-0.2.2/neurosift.egg-info/
+-rw-rw-r--   0 magland   (1000) magland   (1000)      431 2023-07-24 14:42:54.000000 neurosift-0.2.2/neurosift.egg-info/PKG-INFO
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1052 2023-07-24 14:42:54.000000 neurosift-0.2.2/neurosift.egg-info/SOURCES.txt
+-rw-rw-r--   0 magland   (1000) magland   (1000)        1 2023-07-24 14:42:54.000000 neurosift-0.2.2/neurosift.egg-info/dependency_links.txt
+-rw-rw-r--   0 magland   (1000) magland   (1000)       54 2023-07-24 14:42:54.000000 neurosift-0.2.2/neurosift.egg-info/entry_points.txt
+-rw-rw-r--   0 magland   (1000) magland   (1000)       44 2023-07-24 14:42:54.000000 neurosift-0.2.2/neurosift.egg-info/requires.txt
+-rw-rw-r--   0 magland   (1000) magland   (1000)       10 2023-07-24 14:42:54.000000 neurosift-0.2.2/neurosift.egg-info/top_level.txt
+-rw-rw-r--   0 magland   (1000) magland   (1000)      478 2023-07-24 14:42:54.076858 neurosift-0.2.2/setup.cfg
+-rw-rw-r--   0 magland   (1000) magland   (1000)      383 2023-07-24 14:36:11.000000 neurosift-0.2.2/setup.py
```

### Comparing `neurosift-0.2.1/neurosift/RtcsharePlugin.py` & `neurosift-0.2.2/neurosift/RtcsharePlugin.py`

 * *Files identical despite different names*

### Comparing `neurosift-0.2.1/neurosift/TemporaryDirectory.py` & `neurosift-0.2.2/neurosift/TemporaryDirectory.py`

 * *Files identical despite different names*

### Comparing `neurosift-0.2.1/neurosift/cli.py` & `neurosift-0.2.2/neurosift/cli.py`

 * *Files identical despite different names*

### Comparing `neurosift-0.2.1/neurosift/views/Autocorrelograms.py` & `neurosift-0.2.2/neurosift/views/Autocorrelograms.py`

 * *Files identical despite different names*

### Comparing `neurosift-0.2.1/neurosift/views/AverageWaveforms.py` & `neurosift-0.2.2/neurosift/views/AverageWaveforms.py`

 * *Files identical despite different names*

### Comparing `neurosift-0.2.1/neurosift/views/CrossCorrelograms.py` & `neurosift-0.2.2/neurosift/views/CrossCorrelograms.py`

 * *Files identical despite different names*

### Comparing `neurosift-0.2.1/neurosift/views/PositionDecodeField.py` & `neurosift-0.2.2/neurosift/views/PositionDecodeField.py`

 * *Files identical despite different names*

### Comparing `neurosift-0.2.1/neurosift/views/SpikeTrains.py` & `neurosift-0.2.2/neurosift/views/SpikeTrains.py`

 * *Files identical despite different names*

### Comparing `neurosift-0.2.1/neurosift/views/TimeseriesAnnotation.py` & `neurosift-0.2.2/neurosift/views/TimeseriesAnnotation.py`

 * *Files identical despite different names*

### Comparing `neurosift-0.2.1/neurosift/views/TimeseriesGraph.py` & `neurosift-0.2.2/neurosift/views/TimeseriesGraph.py`

 * *Files identical despite different names*

### Comparing `neurosift-0.2.1/neurosift/views/VideoAnnotation.py` & `neurosift-0.2.2/neurosift/views/VideoAnnotation.py`

 * *Files identical despite different names*

### Comparing `neurosift-0.2.1/neurosift/views/__init__.py` & `neurosift-0.2.2/neurosift/views/__init__.py`

 * *Files identical despite different names*

### Comparing `neurosift-0.2.1/neurosift/views/_serialize.py` & `neurosift-0.2.2/neurosift/views/_serialize.py`

 * *Files identical despite different names*

### Comparing `neurosift-0.2.1/neurosift/views/create_audio_spectrogram.py` & `neurosift-0.2.2/neurosift/views/create_audio_spectrogram.py`

 * *Files identical despite different names*

### Comparing `neurosift-0.2.1/neurosift/views/create_spike_sorting_digest.py` & `neurosift-0.2.2/neurosift/views/create_spike_sorting_digest.py`

 * *Files identical despite different names*

### Comparing `neurosift-0.2.1/neurosift/views/helpers/compute_correlogram_data.py` & `neurosift-0.2.2/neurosift/views/helpers/compute_correlogram_data.py`

 * *Files identical despite different names*

### Comparing `neurosift-0.2.1/neurosift/views/helpers/compute_templates.py` & `neurosift-0.2.2/neurosift/views/helpers/compute_templates.py`

 * *Files identical despite different names*

### Comparing `neurosift-0.2.1/neurosift/views/helpers/extract_snippets.py` & `neurosift-0.2.2/neurosift/views/helpers/extract_snippets.py`

 * *Files identical despite different names*

### Comparing `neurosift-0.2.1/neurosift.egg-info/SOURCES.txt` & `neurosift-0.2.2/neurosift.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 neurosift.egg-info/PKG-INFO
 neurosift.egg-info/SOURCES.txt
 neurosift.egg-info/dependency_links.txt
 neurosift.egg-info/entry_points.txt
 neurosift.egg-info/requires.txt
 neurosift.egg-info/top_level.txt
 neurosift/experimental-local-file-access/package.json
+neurosift/experimental-local-file-access/src/index.js
 neurosift/views/Autocorrelograms.py
 neurosift/views/AverageWaveforms.py
 neurosift/views/CrossCorrelograms.py
 neurosift/views/PositionDecodeField.py
 neurosift/views/SpikeTrains.py
 neurosift/views/TimeseriesAnnotation.py
 neurosift/views/TimeseriesGraph.py
```

