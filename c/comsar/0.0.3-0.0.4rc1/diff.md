# Comparing `tmp/comsar-0.0.3.tar.gz` & `tmp/comsar-0.0.4rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comsar-0.0.3.tar", last modified: Fri Apr 23 11:03:30 2021, max compression
+gzip compressed data, was "comsar-0.0.4rc1.tar", max compression
```

## Comparing `comsar-0.0.3.tar` & `comsar-0.0.4rc1.tar`

### file list

```diff
@@ -1,23 +1,15 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2021-04-23 11:03:30.042039 comsar-0.0.3/
--rw-r--r--   0 michael    (501) staff       (20)     1521 2021-04-19 13:28:49.000000 comsar-0.0.3/LICENSE
--rw-r--r--   0 michael    (501) staff       (20)      975 2021-04-23 11:03:30.042201 comsar-0.0.3/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)       90 2021-03-24 11:32:53.000000 comsar-0.0.3/pyproject.toml
--rw-r--r--   0 michael    (501) staff       (20)     1109 2021-04-23 11:03:30.042901 comsar-0.0.3/setup.cfg
--rw-r--r--   0 michael    (501) staff       (20)      130 2020-02-26 12:54:46.000000 comsar-0.0.3/setup.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2021-04-23 11:03:30.012696 comsar-0.0.3/src/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2021-04-23 11:03:30.014296 comsar-0.0.3/src/comsar/
--rw-r--r--   0 michael    (501) staff       (20)       84 2021-03-24 11:32:53.000000 comsar-0.0.3/src/comsar/__init__.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2021-04-23 11:03:30.041707 comsar-0.0.3/src/comsar/tracks/
--rw-r--r--   0 michael    (501) staff       (20)       34 2021-04-23 08:18:20.000000 comsar-0.0.3/src/comsar/tracks/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)        0 2021-04-19 13:28:49.000000 comsar-0.0.3/src/comsar/tracks/_form.py
--rw-r--r--   0 michael    (501) staff       (20)        0 2021-04-19 13:28:49.000000 comsar-0.0.3/src/comsar/tracks/_pitch.py
--rw-r--r--   0 michael    (501) staff       (20)     1305 2021-04-19 13:28:49.000000 comsar-0.0.3/src/comsar/tracks/_rhythm.py
--rw-r--r--   0 michael    (501) staff       (20)     7647 2021-04-23 08:18:20.000000 comsar-0.0.3/src/comsar/tracks/_timbre.py
--rw-r--r--   0 michael    (501) staff       (20)     3630 2021-04-19 13:28:49.000000 comsar-0.0.3/src/comsar/tracks/utilities.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2021-04-23 11:03:30.039651 comsar-0.0.3/src/comsar.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)      975 2021-04-23 11:03:29.000000 comsar-0.0.3/src/comsar.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      440 2021-04-23 11:03:30.000000 comsar-0.0.3/src/comsar.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2021-04-23 11:03:29.000000 comsar-0.0.3/src/comsar.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2020-09-08 07:44:01.000000 comsar-0.0.3/src/comsar.egg-info/not-zip-safe
--rw-r--r--   0 michael    (501) staff       (20)       36 2021-04-23 11:03:29.000000 comsar-0.0.3/src/comsar.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)        7 2021-04-23 11:03:29.000000 comsar-0.0.3/src/comsar.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1521 2023-06-11 11:45:32.143861 comsar-0.0.4rc1/LICENSE
+-rw-r--r--   0        0        0       53 2023-07-23 03:46:41.489047 comsar-0.0.4rc1/README.md
+-rw-r--r--   0        0        0     1928 2023-07-24 13:12:42.240862 comsar-0.0.4rc1/pyproject.toml
+-rw-r--r--   0        0        0       84 2023-07-24 13:12:42.194465 comsar-0.0.4rc1/src/comsar/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-24 13:12:42.212034 comsar-0.0.4rc1/src/comsar/data/__init__.py
+-rw-r--r--   0        0        0    61731 2023-07-24 13:12:42.212758 comsar-0.0.4rc1/src/comsar/data/scales.csv
+-rw-r--r--   0        0        0        0 2023-07-24 13:12:41.973412 comsar-0.0.4rc1/src/comsar/py.typed
+-rw-r--r--   0        0        0       64 2023-07-24 13:12:42.195101 comsar-0.0.4rc1/src/comsar/tracks/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-11 11:45:32.151289 comsar-0.0.4rc1/src/comsar/tracks/_form.py
+-rw-r--r--   0        0        0    19436 2023-07-24 13:12:42.226012 comsar-0.0.4rc1/src/comsar/tracks/_pitch.py
+-rw-r--r--   0        0        0     1121 2023-07-24 13:12:42.197636 comsar-0.0.4rc1/src/comsar/tracks/_rhythm.py
+-rw-r--r--   0        0        0     7269 2023-07-24 13:12:42.198076 comsar-0.0.4rc1/src/comsar/tracks/_timbre.py
+-rw-r--r--   0        0        0     1891 2023-07-24 13:12:42.198549 comsar-0.0.4rc1/src/comsar/tracks/models.py
+-rw-r--r--   0        0        0     2672 2023-07-24 13:12:42.199431 comsar-0.0.4rc1/src/comsar/tracks/utilities.py
+-rw-r--r--   0        0        0     1210 1970-01-01 00:00:00.000000 comsar-0.0.4rc1/PKG-INFO
```

### Comparing `comsar-0.0.3/LICENSE` & `comsar-0.0.4rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `comsar-0.0.3/PKG-INFO` & `comsar-0.0.4rc1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,33 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: comsar
-Version: 0.0.3
+Version: 0.0.4rc1
 Summary: Computational Music and Sound Archiving
-Home-page: UNKNOWN
+Home-page: https://github.com/ifsm/comsar
+License: BSD-3-Clause
 Author: Michael Blaß
 Author-email: mblass@posteo.net
-License: BSD-3-Clause
-Project-URL: Source code, https://github.com/ifsm/comsar
-Project-URL: Bug tracker, https://github.com/ifsm/comsar/issues
-Project-URL: Documentation, http://comsar.readthedocs.io
-Description: UNKNOWN
-Keywords: comsar,music,analysis,ethnomusicology
-Platform: UNKNOWN
+Requires-Python: >=3.9,<3.13
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Database
+Classifier: Topic :: Education
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Information Technology
-Classifier: License :: OSI Approved :: BSD License
+Classifier: Topic :: Scientific/Engineering
+Requires-Dist: apollon (>=0.1.3,<0.2.0)
+Requires-Dist: numpy (>=1.25.1,<2.0.0)
+Requires-Dist: pandas (>=2.0.3,<3.0.0)
+Requires-Dist: scipy (>=1.11.1,<2.0.0)
+Description-Content-Type: text/markdown
+
+# CoMSAr
+
+## Computational Music and Sound Archiving
+
```

### Comparing `comsar-0.0.3/src/comsar/tracks/_rhythm.py` & `comsar-0.0.4rc1/src/comsar/tracks/_rhythm.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,37 @@
-# Licensed under the terms of the BSD-3-Clause license.
-# Copyright (C) 2019 Michael Blaß
-# michael.blass@uni-hamburg.de
-
 import logging
 
+from apollon import onsets, segment, tools
 from apollon.signal import spectral
-from apollon import tools
-from apollon import onsets
-from apollon import segment
 
 
 def rhythm_track(snd: AudioFile) -> dict:
     """Perform rhythm track analysis of given audio file.
 
     Args:
         snd:  Sound data.
         fps:  Sample rate.
 
     Returns:
         Rhythm track parameters and data.
     """
-    logging.info('Starting rhythm track for {!s}'.format(snd.file))
+    logging.info("Starting rhythm track for {!s}".format(snd.file))
     onsets = FluxOnsetDetector(snd.data, snd.fps)
     segs = segment.by_onsets(snd.data, 2**11, onsets.index())
-    spctr = Spectrum(segs, snd.fps, window='hamming', n_fft=2**15)
+    spctr = Spectrum(segs, snd.fps, window="hamming", n_fft=2**15)
 
     onsets_features = {
-        'peaks': onsets.peaks,
-        'index': onsets.index(),
-        'times': onsets.times(snd.fps)
+        "peaks": onsets.peaks,
+        "index": onsets.index(),
+        "times": onsets.times(snd.fps),
     }
 
     track_data = {
-        'meta': {'source': str(snd.file.absolute()),
-                 'time_stamp': time_stamp()},
-        'params': {'onsets': onsets.params(), 'spectrum': spctr.params()},
-        'features': {'onsets': onsets_features,
-                     'spectrum':
-                      spctr.extract(cf_low=100, cf_high=9000).as_dict()}
+        "meta": {"source": str(snd.file.absolute()), "time_stamp": time_stamp()},
+        "params": {"onsets": onsets.params(), "spectrum": spctr.params()},
+        "features": {
+            "onsets": onsets_features,
+            "spectrum": spctr.extract(cf_low=100, cf_high=9000).as_dict(),
+        },
     }
-    logging.info(f'Done with rhythm track for {snd.file!s}.')
+    logging.info(f"Done with rhythm track for {snd.file!s}.")
     return track_data
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `comsar-0.0.3/src/comsar/tracks/_timbre.py` & `comsar-0.0.4rc1/src/comsar/tracks/_timbre.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,207 +1,251 @@
 """comsar/tracks/timbre.py -- TimbreTack implementation
-License: BSD-3-Clasuse
-Copyright (C) 2020, Michael Blaß, michael.blass@uni-hamburg.de
 """
 from datetime import datetime
 from timeit import default_timer as timer
 from typing import Optional
 
 import numpy as np
 import pandas as pd
-
 from apollon.audio import AudioFile
 from apollon.segment import Segmentation
 from apollon.signal import container, features
 from apollon.signal.spectral import StftSegments
 
 import comsar
-from . utilities import (TrackMeta, TrackResult, SourceMeta,
-                         TimbreTrackParams, TimbreTrackCorrGramParams)
 
-STFT_DEFAULT = container.StftParams(fps=44100, window='hamming', n_fft=None,
-                                    n_perseg=2**15, n_overlap=2**14,
-                                    extend=True, pad=True)
+from .models import SourceMeta, TimbreTrackCorrGramParams, TimbreTrackParams, TrackMeta
+from .utilities import TrackResult
 
-CORR_DIM_DEFAULT = container.CorrDimParams(delay=14, m_dim=80, n_bins=1000,
-                                           scaling_size=10)
+STFT_DEFAULT = container.StftParams(
+    fps=44100,
+    window="hamming",
+    n_fft=None,
+    n_perseg=2**15,
+    n_overlap=2**14,
+    extend=True,
+    pad=True,
+)
+
+CORR_DIM_DEFAULT = container.CorrDimParams(
+    delay=14, m_dim=80, n_bins=1000, scaling_size=10
+)
 
-CORR_GRAM_DEFAULT = container.CorrGramParams(wlen=2**10, n_delay=2**8,
-                                             total=True)
+CORR_GRAM_DEFAULT = container.CorrGramParams(wlen=2**10, n_delay=2**8, total=True)
 
 
 class TimbreTrack:
     """High-level interface for timbre feature extraction."""
-    def __init__(self,
-                 stft_params: Optional[container.StftParams] = None,
-                 corr_dim_params: Optional[container.CorrDimParams] = None,
-                 ) -> None:
+
+    def __init__(
+        self,
+        stft_params: Optional[container.StftParams] = None,
+        corr_dim_params: Optional[container.CorrDimParams] = None,
+    ) -> None:
         """
         Args:
             stft_params:        Parameter for STFT.
             corr_dim_params:    Parameter set for correlation dimension.
         """
-        self.params = TimbreTrackParams(stft_params or STFT_DEFAULT,
-                                        corr_dim_params or CORR_DIM_DEFAULT)
-
-        self.cutter = Segmentation(self.params.stft.n_perseg,
-                                   self.params.stft.n_overlap,
-                                   self.params.stft.extend,
-                                   self.params.stft.pad)
-
-        self.stft = StftSegments(self.params.stft.fps, self.params.stft.window,
-                                 self.params.stft.n_fft)
-
-        self.feature_names = ('SpectralCentroid', 'SpectralSpread',
-                              'SpectralFlux', 'Roughness', 'Sharpness',
-                              'SPL', 'CorrelationDimension')
-
-        self.funcs = [features.spectral_centroid,
-                      features.spectral_spread,
-                      features.spectral_flux,
-                      features.roughness_helmholtz,
-                      features.sharpness,
-                      features.spl,
-                      features.cdim]
+        self.params = TimbreTrackParams(
+            stft_params or STFT_DEFAULT, corr_dim_params or CORR_DIM_DEFAULT
+        )
+
+        self.cutter = Segmentation(
+            self.params.stft.n_perseg,
+            self.params.stft.n_overlap,
+            self.params.stft.extend,
+            self.params.stft.pad,
+        )
+
+        self.stft = StftSegments(
+            self.params.stft.fps, self.params.stft.window, self.params.stft.n_fft
+        )
+
+        self.feature_names = (
+            "SpectralCentroid",
+            "SpectralSpread",
+            "SpectralFlux",
+            "Roughness",
+            "Sharpness",
+            "SPL",
+            "CorrelationDimension",
+        )
+
+        self.funcs = [
+            features.spectral_centroid,
+            features.spectral_spread,
+            features.spectral_flux,
+            features.roughness_helmholtz,
+            features.sharpness,
+            features.spl,
+            features.cdim,
+        ]
 
         self.pace = np.zeros(self.n_features)
         self.verbose = False
 
     @property
     def n_features(self) -> int:
         """Number of features.
 
         Returns:
             Number of audio features.
         """
         return len(self.feature_names)
 
-    def extract(self, path) -> pd.DataFrame:
+    def extract(self, path) -> TrackResult:
         """Run TimbreTrack on audio file.
 
         Args:
             path:   Path to audio file.
 
         Returns:
            Extracted features.
         """
         snd = AudioFile(path)
         if snd.fps != self.params.stft.fps:
             snd.close()
-            raise ValueError('Sample rate of {snd!str} differs from init.')
+            raise ValueError("Sample rate of {snd!str} differs from init.")
 
         segs = self.cutter.transform(snd.data.squeeze())
         sxx = self.stft.transform(segs)
 
-        args = [(sxx.frqs, sxx.power),
-                (sxx.frqs, sxx.power),
-                (sxx.abs,),
-                (sxx.d_frq, sxx.abs, 15000),
-                (sxx.frqs, sxx.abs),
-                (segs.data,),
-                (segs.data,)]
+        args = [
+            (sxx.frqs, sxx.power),
+            (sxx.frqs, sxx.power),
+            (sxx.abs,),
+            (sxx.d_frq, sxx.abs, 15000),
+            (sxx.frqs, sxx.abs),
+            (segs.data,),
+            (segs.data,),
+        ]
 
         kwargs = [{}, {}, {}, {}, {}, {}, self.params.corr_dim.to_dict()]
 
         out = np.zeros((segs.n_segs, self.n_features))
         for i, (fun, arg, kwarg) in enumerate(zip(self.funcs, args, kwargs)):
             out[:, i] = self._worker(i, fun, arg, kwarg)
 
-        file_meta = SourceMeta(*snd.file_name.split('.'), snd.hash)
-        track_meta = TrackMeta(comsar.__version__, datetime.utcnow(),
-                               file_meta)
-        out = pd.DataFrame(data=out, columns=self.feature_names)
+        file_meta = SourceMeta(*snd.file_name.split("."), snd.hash)
+        track_meta = TrackMeta(comsar.__version__, datetime.utcnow(), file_meta)
+        data = pd.DataFrame(data=out, columns=self.feature_names)
         snd.close()
-        return TrackResult(track_meta, self.params, out)
+        return TrackResult(track_meta, self.params, data)
 
     def _worker(self, idx, func, args, kwargs) -> np.ndarray:
-        print(self.feature_names[idx], end=' ... ')
+        print(self.feature_names[idx], end=" ... ")
         pace = timer()
         res = func(*args, **kwargs)
         pace = timer() - pace
         self.pace[idx] = pace
-        print(f'{pace:.4} s.')
+        print(f"{pace:.4} s.")
         return res
 
 
 class TimbreTrackCorrGram:
-    """Compute timbre track of an audio file.
-    """
-    def __init__(self,
-                 stft_params: Optional[container.StftParams] = None,
-                 corr_dim_params: Optional[container.CorrDimParams] = None,
-                 corr_gram_params: Optional[container.CorrGramParams] = None) -> None:
+    """Compute timbre track of an audio file."""
+
+    def __init__(
+        self,
+        stft_params: Optional[container.StftParams] = None,
+        corr_dim_params: Optional[container.CorrDimParams] = None,
+        corr_gram_params: Optional[container.CorrGramParams] = None,
+    ) -> None:
         """
         Args:
         """
-        self.params = TimbreTrackCorrGramParams(stft_params or STFT_DEFAULT,
-                                        corr_dim_params or CORR_DIM_DEFAULT,
-                                        corr_gram_params or CORR_GRAM_DEFAULT)
-
-        self.cutter = Segmentation(self.params.stft.n_perseg,
-                                   self.params.stft.n_overlap,
-                                   self.params.stft.extend,
-                                   self.params.stft.pad)
-        self.stft = StftSegments(self.params.stft.fps, self.params.stft.window,
-                                 self.params.stft.n_fft)
-
-        self.feature_names = ('SpectralCentroid', 'SpectralSpread',
-                              'SpectralFlux', 'Roughness', 'Sharpness',
-                              'SPL', 'CorrelationDimension', 'Correlogram')
-
-        self.funcs = [features.spectral_centroid,
-                      features.spectral_spread,
-                      features.spectral_flux,
-                      features.roughness_helmholtz,
-                      features.sharpness,
-                      features.spl,
-                      features.cdim,
-                      features.correlogram]
+        self.params = TimbreTrackCorrGramParams(
+            stft_params or STFT_DEFAULT,
+            corr_dim_params or CORR_DIM_DEFAULT,
+            corr_gram_params or CORR_GRAM_DEFAULT,
+        )
+
+        self.cutter = Segmentation(
+            self.params.stft.n_perseg,
+            self.params.stft.n_overlap,
+            self.params.stft.extend,
+            self.params.stft.pad,
+        )
+        self.stft = StftSegments(
+            self.params.stft.fps, self.params.stft.window, self.params.stft.n_fft
+        )
+
+        self.feature_names = (
+            "SpectralCentroid",
+            "SpectralSpread",
+            "SpectralFlux",
+            "Roughness",
+            "Sharpness",
+            "SPL",
+            "CorrelationDimension",
+            "Correlogram",
+        )
+
+        self.funcs = [
+            features.spectral_centroid,
+            features.spectral_spread,
+            features.spectral_flux,
+            features.roughness_helmholtz,
+            features.sharpness,
+            features.spl,
+            features.cdim,
+            features.correlogram,
+        ]
 
         self.pace = np.zeros(self.n_features)
         self.verbose = False
 
     @property
     def n_features(self) -> int:
         """Number of features on track"""
         return len(self.feature_names)
 
-    def extract(self, path) -> pd.DataFrame:
-        """Perform extraction.
-        """
+    def extract(self, path) -> TrackResult:
+        """Perform extraction."""
         snd = AudioFile(path)
         if snd.fps != self.params.stft.fps:
             snd.close()
-            raise ValueError('Sample rate of {snd!str} differs from init.')
+            raise ValueError("Sample rate of {snd!str} differs from init.")
 
         segs = self.cutter.transform(snd.data.squeeze())
         sxx = self.stft.transform(segs)
 
-        args = [(sxx.frqs, sxx.power),
-                (sxx.frqs, sxx.power),
-                (sxx.abs,),
-                (sxx.d_frq, sxx.abs, 15000),
-                (sxx.frqs, sxx.abs),
-                (segs.data,),
-                (segs.data,),
-                (segs.data,)]
-
-        kwargs = [{}, {}, {}, {}, {}, {}, self.params.corr_dim.to_dict(),
-                  self.params.corr_gram.to_dict()]
+        args = [
+            (sxx.frqs, sxx.power),
+            (sxx.frqs, sxx.power),
+            (sxx.abs,),
+            (sxx.d_frq, sxx.abs, 15000),
+            (sxx.frqs, sxx.abs),
+            (segs.data,),
+            (segs.data,),
+            (segs.data,),
+        ]
+
+        kwargs = [
+            {},
+            {},
+            {},
+            {},
+            {},
+            {},
+            self.params.corr_dim.to_dict(),
+            self.params.corr_gram.to_dict(),
+        ]
 
         out = np.zeros((segs.n_segs, self.n_features))
         for i, (fun, arg, kwarg) in enumerate(zip(self.funcs, args, kwargs)):
             out[:, i] = self._worker(i, fun, arg, kwarg)
         snd.close()
 
         meta = TrackMeta(comsar.__version__, datetime.utcnow(), snd.file_name)
-        out = pd.DataFrame(data=out, columns=self.feature_names)
-        return TrackResult(meta, self.params, out)
+        data = pd.DataFrame(data=out, columns=self.feature_names)
+        return TrackResult(meta, self.params, data)
 
     def _worker(self, idx, func, args, kwargs) -> np.ndarray:
-        print(self.feature_names[idx], end=' ... ')
+        print(self.feature_names[idx], end=" ... ")
         pace = timer()
         res = func(*args, **kwargs)
         pace = timer() - pace
         self.pace[idx] = pace
-        print(f'{pace:.4} s.')
+        print(f"{pace:.4} s.")
         return res
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

