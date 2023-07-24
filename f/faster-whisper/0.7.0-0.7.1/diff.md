# Comparing `tmp/faster-whisper-0.7.0.tar.gz` & `tmp/faster-whisper-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faster-whisper-0.7.0.tar", last modified: Tue Jul 18 13:25:41 2023, max compression
+gzip compressed data, was "faster-whisper-0.7.1.tar", last modified: Mon Jul 24 09:12:29 2023, max compression
```

## Comparing `faster-whisper-0.7.0.tar` & `faster-whisper-0.7.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:25:41.022580 faster-whisper-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-18 13:25:35.000000 faster-whisper-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-18 13:25:35.000000 faster-whisper-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10942 2023-07-18 13:25:41.022580 faster-whisper-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-07-18 13:25:35.000000 faster-whisper-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:25:41.018580 faster-whisper-0.7.0/faster_whisper/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-18 13:25:35.000000 faster-whisper-0.7.0/faster_whisper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:25:41.022580 faster-whisper-0.7.0/faster_whisper/assets/
--rw-r--r--   0 runner    (1001) docker     (123)  1807524 2023-07-18 13:25:35.000000 faster-whisper-0.7.0/faster_whisper/assets/silero_vad.onnx
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-07-18 13:25:35.000000 faster-whisper-0.7.0/faster_whisper/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-07-18 13:25:35.000000 faster-whisper-0.7.0/faster_whisper/feature_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-07-18 13:25:35.000000 faster-whisper-0.7.0/faster_whisper/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    36931 2023-07-18 13:25:35.000000 faster-whisper-0.7.0/faster_whisper/transcribe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-07-18 13:25:35.000000 faster-whisper-0.7.0/faster_whisper/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10515 2023-07-18 13:25:35.000000 faster-whisper-0.7.0/faster_whisper/vad.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-18 13:25:35.000000 faster-whisper-0.7.0/faster_whisper/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:25:41.022580 faster-whisper-0.7.0/faster_whisper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10942 2023-07-18 13:25:40.000000 faster-whisper-0.7.0/faster_whisper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-18 13:25:41.000000 faster-whisper-0.7.0/faster_whisper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 13:25:40.000000 faster-whisper-0.7.0/faster_whisper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-18 13:25:40.000000 faster-whisper-0.7.0/faster_whisper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-18 13:25:40.000000 faster-whisper-0.7.0/faster_whisper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-18 13:25:35.000000 faster-whisper-0.7.0/requirements.conversion.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-18 13:25:35.000000 faster-whisper-0.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-18 13:25:41.022580 faster-whisper-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-18 13:25:35.000000 faster-whisper-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:12:29.817716 faster-whisper-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-24 09:12:24.000000 faster-whisper-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-24 09:12:24.000000 faster-whisper-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10942 2023-07-24 09:12:29.817716 faster-whisper-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-07-24 09:12:24.000000 faster-whisper-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:12:29.813717 faster-whisper-0.7.1/faster_whisper/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-24 09:12:24.000000 faster-whisper-0.7.1/faster_whisper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:12:29.813717 faster-whisper-0.7.1/faster_whisper/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)  1807524 2023-07-24 09:12:24.000000 faster-whisper-0.7.1/faster_whisper/assets/silero_vad.onnx
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-07-24 09:12:24.000000 faster-whisper-0.7.1/faster_whisper/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-07-24 09:12:24.000000 faster-whisper-0.7.1/faster_whisper/feature_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-07-24 09:12:24.000000 faster-whisper-0.7.1/faster_whisper/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37280 2023-07-24 09:12:24.000000 faster-whisper-0.7.1/faster_whisper/transcribe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-07-24 09:12:24.000000 faster-whisper-0.7.1/faster_whisper/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10515 2023-07-24 09:12:24.000000 faster-whisper-0.7.1/faster_whisper/vad.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-24 09:12:24.000000 faster-whisper-0.7.1/faster_whisper/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:12:29.813717 faster-whisper-0.7.1/faster_whisper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10942 2023-07-24 09:12:29.000000 faster-whisper-0.7.1/faster_whisper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-24 09:12:29.000000 faster-whisper-0.7.1/faster_whisper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 09:12:29.000000 faster-whisper-0.7.1/faster_whisper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-24 09:12:29.000000 faster-whisper-0.7.1/faster_whisper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-24 09:12:29.000000 faster-whisper-0.7.1/faster_whisper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-24 09:12:24.000000 faster-whisper-0.7.1/requirements.conversion.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-24 09:12:24.000000 faster-whisper-0.7.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-24 09:12:29.817716 faster-whisper-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-24 09:12:24.000000 faster-whisper-0.7.1/setup.py
```

### Comparing `faster-whisper-0.7.0/LICENSE` & `faster-whisper-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `faster-whisper-0.7.0/PKG-INFO` & `faster-whisper-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faster-whisper
-Version: 0.7.0
+Version: 0.7.1
 Summary: Faster Whisper transcription with CTranslate2
 Home-page: https://github.com/guillaumekln/faster-whisper
 Author: Guillaume Klein
 License: MIT
 Description: [![CI](https://github.com/guillaumekln/faster-whisper/workflows/CI/badge.svg)](https://github.com/guillaumekln/faster-whisper/actions?query=workflow%3ACI) [![PyPI version](https://badge.fury.io/py/faster-whisper.svg)](https://badge.fury.io/py/faster-whisper)
         
         # Faster Whisper transcription with CTranslate2
```

### Comparing `faster-whisper-0.7.0/README.md` & `faster-whisper-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `faster-whisper-0.7.0/faster_whisper/assets/silero_vad.onnx` & `faster-whisper-0.7.1/faster_whisper/assets/silero_vad.onnx`

 * *Files identical despite different names*

### Comparing `faster-whisper-0.7.0/faster_whisper/audio.py` & `faster-whisper-0.7.1/faster_whisper/audio.py`

 * *Files identical despite different names*

### Comparing `faster-whisper-0.7.0/faster_whisper/feature_extractor.py` & `faster-whisper-0.7.1/faster_whisper/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `faster-whisper-0.7.0/faster_whisper/tokenizer.py` & `faster-whisper-0.7.1/faster_whisper/tokenizer.py`

 * *Files identical despite different names*

### Comparing `faster-whisper-0.7.0/faster_whisper/transcribe.py` & `faster-whisper-0.7.1/faster_whisper/transcribe.py`

 * *Files 2% similar despite different names*

```diff
@@ -418,14 +418,15 @@
                         "No speech threshold is met (%f > %f)",
                         result.no_speech_prob,
                         options.no_speech_threshold,
                     )
 
                     # fast-forward to the next segment boundary
                     seek += segment_size
+                    encoder_output = None
                     continue
 
             tokens = result.sequences_ids[0]
 
             previous_seek = seek
             current_segments = []
 
@@ -574,18 +575,17 @@
     def generate_with_fallback(
         self,
         encoder_output: ctranslate2.StorageView,
         prompt: List[int],
         tokenizer: Tokenizer,
         options: TranscriptionOptions,
     ) -> Tuple[ctranslate2.models.WhisperGenerationResult, float, float, float]:
-        result = None
-        avg_logprob = None
-        final_temperature = None
-        compression_ratio = None
+        decode_result = None
+        all_results = []
+        below_cr_threshold_results = []
 
         max_initial_timestamp_index = int(
             round(options.max_initial_timestamp / self.time_precision)
         )
 
         for temperature in options.temperatures:
             if temperature > 0:
@@ -597,15 +597,14 @@
                 }
             else:
                 kwargs = {
                     "beam_size": options.beam_size,
                     "patience": options.patience,
                 }
 
-            final_temperature = temperature
             result = self.model.generate(
                 encoder_output,
                 [prompt],
                 length_penalty=options.length_penalty,
                 max_length=self.max_length,
                 return_scores=True,
                 return_no_speech_prob=True,
@@ -621,28 +620,36 @@
             seq_len = len(tokens)
             cum_logprob = result.scores[0] * (seq_len**options.length_penalty)
             avg_logprob = cum_logprob / (seq_len + 1)
 
             text = tokenizer.decode(tokens).strip()
             compression_ratio = get_compression_ratio(text)
 
-            needs_fallback = False
+            decode_result = (
+                result,
+                avg_logprob,
+                temperature,
+                compression_ratio,
+            )
+            all_results.append(decode_result)
 
-            if (
-                options.compression_ratio_threshold is not None
-                and compression_ratio > options.compression_ratio_threshold
-            ):
-                needs_fallback = True  # too repetitive
+            needs_fallback = False
 
-                self.logger.debug(
-                    "Compression ratio threshold is not met with temperature %.1f (%f > %f)",
-                    temperature,
-                    compression_ratio,
-                    options.compression_ratio_threshold,
-                )
+            if options.compression_ratio_threshold is not None:
+                if compression_ratio > options.compression_ratio_threshold:
+                    needs_fallback = True  # too repetitive
+
+                    self.logger.debug(
+                        "Compression ratio threshold is not met with temperature %.1f (%f > %f)",
+                        temperature,
+                        compression_ratio,
+                        options.compression_ratio_threshold,
+                    )
+                else:
+                    below_cr_threshold_results.append(decode_result)
 
             if (
                 options.log_prob_threshold is not None
                 and avg_logprob < options.log_prob_threshold
             ):
                 needs_fallback = True  # average log probability is too low
 
@@ -657,16 +664,21 @@
                 options.no_speech_threshold is not None
                 and result.no_speech_prob > options.no_speech_threshold
             ):
                 needs_fallback = False  # silence
 
             if not needs_fallback:
                 break
+        else:
+            # all failed, select the result with the highest average log probability
+            decode_result = max(
+                below_cr_threshold_results or all_results, key=lambda x: x[1]
+            )
 
-        return result, avg_logprob, final_temperature, compression_ratio
+        return decode_result
 
     def get_prompt(
         self,
         tokenizer: Tokenizer,
         previous_tokens: List[int],
         without_timestamps: bool = False,
         prefix: Optional[str] = None,
@@ -718,16 +730,14 @@
         word_durations = word_durations[word_durations.nonzero()]
         median_duration = np.median(word_durations) if len(word_durations) > 0 else 0.0
         max_duration = median_duration * 2
 
         # hack: truncate long words at sentence boundaries.
         # a better segmentation algorithm based on VAD should be able to replace this.
         if len(word_durations) > 0:
-            median_duration = np.median(word_durations)
-            max_duration = median_duration * 2
             sentence_end_marks = ".。!！?？"
             # ensure words at sentence boundaries
             # are not longer than twice the median word duration.
             for i in range(1, len(alignment)):
                 if alignment[i]["end"] - alignment[i]["start"] > max_duration:
                     if alignment[i]["word"] in sentence_end_marks:
                         alignment[i]["end"] = alignment[i]["start"] + max_duration
```

### Comparing `faster-whisper-0.7.0/faster_whisper/utils.py` & `faster-whisper-0.7.1/faster_whisper/utils.py`

 * *Files identical despite different names*

### Comparing `faster-whisper-0.7.0/faster_whisper/vad.py` & `faster-whisper-0.7.1/faster_whisper/vad.py`

 * *Files identical despite different names*

### Comparing `faster-whisper-0.7.0/faster_whisper.egg-info/PKG-INFO` & `faster-whisper-0.7.1/faster_whisper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faster-whisper
-Version: 0.7.0
+Version: 0.7.1
 Summary: Faster Whisper transcription with CTranslate2
 Home-page: https://github.com/guillaumekln/faster-whisper
 Author: Guillaume Klein
 License: MIT
 Description: [![CI](https://github.com/guillaumekln/faster-whisper/workflows/CI/badge.svg)](https://github.com/guillaumekln/faster-whisper/actions?query=workflow%3ACI) [![PyPI version](https://badge.fury.io/py/faster-whisper.svg)](https://badge.fury.io/py/faster-whisper)
         
         # Faster Whisper transcription with CTranslate2
```

### Comparing `faster-whisper-0.7.0/faster_whisper.egg-info/SOURCES.txt` & `faster-whisper-0.7.1/faster_whisper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `faster-whisper-0.7.0/setup.py` & `faster-whisper-0.7.1/setup.py`

 * *Files identical despite different names*

