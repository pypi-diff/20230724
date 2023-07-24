# Comparing `tmp/openlrc-0.2.1.tar.gz` & `tmp/openlrc-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlrc-0.2.1.tar", max compression
+gzip compressed data, was "openlrc-0.2.2.tar", max compression
```

## Comparing `openlrc-0.2.1.tar` & `openlrc-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1083 2023-05-10 10:20:06.659160 openlrc-0.2.1/LICENSE
--rw-r--r--   0        0        0      106 2023-06-09 13:01:57.605311 openlrc-0.2.1/openlrc/__init__.py
--rw-r--r--   0        0        0     6643 2023-07-14 13:02:05.768264 openlrc-0.2.1/openlrc/chatbot.py
--rw-r--r--   0        0        0     2761 2023-07-12 18:58:48.074505 openlrc-0.2.1/openlrc/context.py
--rw-r--r--   0        0        0     2164 2023-07-13 10:41:08.371996 openlrc-0.2.1/openlrc/defaults.py
--rw-r--r--   0        0        0      966 2023-07-05 20:31:15.832362 openlrc-0.2.1/openlrc/exceptions.py
--rw-r--r--   0        0        0      597 2023-06-15 20:08:22.292558 openlrc-0.2.1/openlrc/logger.py
--rw-r--r--   0        0        0    13617 2023-07-17 08:20:23.713740 openlrc-0.2.1/openlrc/openlrc.py
--rw-r--r--   0        0        0     5147 2023-07-16 07:28:45.850524 openlrc-0.2.1/openlrc/opt.py
--rw-r--r--   0        0        0     3920 2023-07-17 08:05:53.681548 openlrc-0.2.1/openlrc/preprocess.py
--rw-r--r--   0        0        0     7702 2023-07-12 18:58:48.076743 openlrc-0.2.1/openlrc/prompter.py
--rw-r--r--   0        0        0     6736 2023-07-16 07:46:51.494326 openlrc-0.2.1/openlrc/subtitle.py
--rw-r--r--   0        0        0     6614 2023-07-13 15:11:24.766191 openlrc-0.2.1/openlrc/transcribe.py
--rw-r--r--   0        0        0     5867 2023-07-17 07:58:32.297546 openlrc-0.2.1/openlrc/translate.py
--rw-r--r--   0        0        0     7332 2023-07-14 03:29:48.721545 openlrc-0.2.1/openlrc/utils.py
--rw-r--r--   0        0        0     1733 2023-07-17 08:24:48.610852 openlrc-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     5712 2023-07-17 08:30:54.378527 openlrc-0.2.1/README.md
--rw-r--r--   0        0        0     7296 1970-01-01 00:00:00.000000 openlrc-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-05-10 10:20:06.659160 openlrc-0.2.2/LICENSE
+-rw-r--r--   0        0        0      106 2023-06-09 13:01:57.605311 openlrc-0.2.2/openlrc/__init__.py
+-rw-r--r--   0        0        0     6643 2023-07-14 13:02:05.768264 openlrc-0.2.2/openlrc/chatbot.py
+-rw-r--r--   0        0        0     2761 2023-07-12 18:58:48.074505 openlrc-0.2.2/openlrc/context.py
+-rw-r--r--   0        0        0     2164 2023-07-13 10:41:08.371996 openlrc-0.2.2/openlrc/defaults.py
+-rw-r--r--   0        0        0      966 2023-07-05 20:31:15.832362 openlrc-0.2.2/openlrc/exceptions.py
+-rw-r--r--   0        0        0      597 2023-06-15 20:08:22.292558 openlrc-0.2.2/openlrc/logger.py
+-rw-r--r--   0        0        0    13635 2023-07-24 13:15:39.297332 openlrc-0.2.2/openlrc/openlrc.py
+-rw-r--r--   0        0        0     5147 2023-07-16 07:28:45.850524 openlrc-0.2.2/openlrc/opt.py
+-rw-r--r--   0        0        0     4565 2023-07-24 13:43:23.138403 openlrc-0.2.2/openlrc/preprocess.py
+-rw-r--r--   0        0        0     7806 2023-07-20 07:34:11.090837 openlrc-0.2.2/openlrc/prompter.py
+-rw-r--r--   0        0        0     6736 2023-07-16 07:46:51.494326 openlrc-0.2.2/openlrc/subtitle.py
+-rw-r--r--   0        0        0     6614 2023-07-13 15:11:24.766191 openlrc-0.2.2/openlrc/transcribe.py
+-rw-r--r--   0        0        0     5867 2023-07-17 07:58:32.297546 openlrc-0.2.2/openlrc/translate.py
+-rw-r--r--   0        0        0     7424 2023-07-17 09:59:41.106278 openlrc-0.2.2/openlrc/utils.py
+-rw-r--r--   0        0        0     1753 2023-07-24 13:57:19.898830 openlrc-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     5712 2023-07-17 08:30:54.378527 openlrc-0.2.2/README.md
+-rw-r--r--   0        0        0     7336 1970-01-01 00:00:00.000000 openlrc-0.2.2/PKG-INFO
```

### Comparing `openlrc-0.2.1/LICENSE` & `openlrc-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openlrc-0.2.1/openlrc/chatbot.py` & `openlrc-0.2.2/openlrc/chatbot.py`

 * *Files identical despite different names*

### Comparing `openlrc-0.2.1/openlrc/context.py` & `openlrc-0.2.2/openlrc/context.py`

 * *Files identical despite different names*

### Comparing `openlrc-0.2.1/openlrc/defaults.py` & `openlrc-0.2.2/openlrc/defaults.py`

 * *Files identical despite different names*

### Comparing `openlrc-0.2.1/openlrc/exceptions.py` & `openlrc-0.2.2/openlrc/exceptions.py`

 * *Files identical despite different names*

### Comparing `openlrc-0.2.1/openlrc/logger.py` & `openlrc-0.2.2/openlrc/logger.py`

 * *Files identical despite different names*

### Comparing `openlrc-0.2.1/openlrc/openlrc.py` & `openlrc-0.2.2/openlrc/openlrc.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,15 +270,15 @@
         for i, path in enumerate(paths):
             if not path.exists() or not path.is_file():
                 raise FileNotFoundError(f'File not found: {path}')
 
             paths[i] = extract_audio(path)
 
             if get_file_type(path) == 'video':
-                self.from_video.add(path.name)
+                self.from_video.add(path.name + '_preprocessed')
 
         # Audio-based process
         preprocessor = Preprocessor(paths)
         paths = preprocessor.run(noise_suppress)
 
         return paths
```

### Comparing `openlrc-0.2.1/openlrc/opt.py` & `openlrc-0.2.2/openlrc/opt.py`

 * *Files identical despite different names*

### Comparing `openlrc-0.2.1/openlrc/preprocess.py` & `openlrc-0.2.2/openlrc/preprocess.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 #  Copyright (C) 2023. Hao Zheng
 #  All rights reserved.
 import logging
 from pathlib import Path
 from typing import List, Union
 
+import torch
 from df.enhance import enhance, init_df, load_audio, save_audio
 from ffmpeg_normalize import FFmpegNormalize
+from tqdm import tqdm
 
 from openlrc.logger import logger
 from openlrc.utils import release_memory
 
 
 class Preprocessor:
     """
@@ -26,30 +28,43 @@
             if not path.exists():
                 path.mkdir()
 
     def noise_suppression(self, audio_paths: Union[str, Path, List[str], List[Path]], atten_lim_db=15):
         """
         Supress noise in audio.
         """
-        logger.info('Noise suppressing...')
+        if not audio_paths:
+            return []
 
         model, df_state, _ = init_df()
 
         ns_audio_paths = []
         for audio_path, output_path in zip(audio_paths, self.output_paths):
             audio_name = audio_path.stem
             ns_path = output_path / f'{audio_name}_ns.wav'
 
             if not ns_path.exists():
-                audio, _ = load_audio(audio_path, sr=df_state.sr())
-                enhanced = enhance(model, df_state, audio, atten_lim_db=atten_lim_db)
+                audio, info = load_audio(audio_path, sr=df_state.sr())
+
+                # Split audio into 10min chunks
+                audio_chunks = [audio[:, i:i + 600 * info.sample_rate]
+                                for i in range(0, audio.shape[1], 600 * info.sample_rate)]
+
+                enhanced_chunks = []
+                for ac in tqdm(audio_chunks, desc='Noise suppressing...'):
+                    enhanced_chunks.append(enhance(model, df_state, ac, atten_lim_db=atten_lim_db))
+
+                enhanced = torch.cat(enhanced_chunks, dim=1)
+
+                assert enhanced.shape == audio.shape, 'Enhanced audio shape does not match original audio shape.'
 
                 save_audio(ns_path, enhanced, sr=df_state.sr())
 
             ns_audio_paths.append(ns_path)
+            logger.debug(f'Noise suppressed audio saved to {ns_path}')
 
         release_memory(model)
 
         return ns_audio_paths
 
     def loudness_normalization(self, audio_paths: Union[str, Path, List[str], List[Path]]):
         """
```

### Comparing `openlrc-0.2.1/openlrc/prompter.py` & `openlrc-0.2.2/openlrc/prompter.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 
 from langcodes import Language
 from lingua import LanguageDetectorBuilder
 
 from openlrc.logger import logger
 
 # instruction prompt modified from https://github.com/machinewrapped/gpt-subtrans
-base_instruction = f'''You are a translator, your task is to accurately revise and translate subtitles into a target language.
-The input are transcribed from audio, so there may be errors in the transcription. Please correct any errors you find in the sentences first, based on their context. Then translate them to target language according to the revised sentences.
+base_instruction = f'''You are a translator tasked with revising and translating subtitles into a target language. Your goal is to ensure accurate, concise, and natural-sounding translations for each line of dialogue. The input consists of transcribed audio, which may contain transcription errors. Your task is to first correct any errors you find in the sentences based on their context, and then translate them to the target language according to the revised sentences.
 The user will provide a chunk of lines, you should respond with an accurate, concise, and natural-sounding translation for the dialogue. 
 The user may provide additional context, such as background, description or title of the source material, a summary of the current scene, or a list of character names. Use this information to improve the quality of your translation.
 Your response will be processed by an automated system, so it is imperative that you adhere to the required output format.
 
 Example input (Japanese to Chinese):
 
 #200
```

### Comparing `openlrc-0.2.1/openlrc/subtitle.py` & `openlrc-0.2.2/openlrc/subtitle.py`

 * *Files identical despite different names*

### Comparing `openlrc-0.2.1/openlrc/transcribe.py` & `openlrc-0.2.2/openlrc/transcribe.py`

 * *Files identical despite different names*

### Comparing `openlrc-0.2.1/openlrc/translate.py` & `openlrc-0.2.2/openlrc/translate.py`

 * *Files identical despite different names*

### Comparing `openlrc-0.2.1/openlrc/utils.py` & `openlrc-0.2.2/openlrc/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,14 +127,18 @@
         self._stop = time.perf_counter()
         logger.info(f'{self.task} Elapsed: {self._elapsed:.2f}s')
 
     @property
     def _elapsed(self):
         return self._stop - self._start
 
+    @property
+    def duration(self):
+        return time.perf_counter() - self._start
+
     def __enter__(self):
         self.start()
         return self
 
     def __exit__(self, *args):
         self.stop()
```

### Comparing `openlrc-0.2.1/pyproject.toml` & `openlrc-0.2.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [virtualenvs]
 create = true
 in-project = true
 
 [tool.poetry]
 name = "openlrc"
-version = "0.2.1"
+version = "0.2.2"
 description = "Transcribe (whisper) and translate (gpt) voice into LRC file."
 license = "MIT"
 authors = [
     "Hao Zheng <zhenghaosustc@gmail.com>"
 ]
 readme = "README.md"
 homepage = "https://github.com/zh-plus/Open-Lyrics"
@@ -47,18 +47,19 @@
 ffmpeg-python = "^0.2.0"
 lingua-language-detector = "^1.3.2"
 pandas = "^2.0.2"
 filetype = "^1.2.0"
 jaconvV2 = "^0.4"
 spacy = "^3.5.4"
 pysbd = "^0.3.4"
-faster-whisper = "^0.6.0"
+faster-whisper = "^0.7.1"
 soundfile = "^0.12.1"
 ffmpeg-normalize = "^1.27.5"
 deepfilternet = "^0.5.3"
+aiohttp = "^3.8.5"
 #torch = { version = "2.0.1", source = "torch" }
 #torchaudio = { version = "2.0.2", source = "torch" }
 #torchvision = { version = "0.15.2", source = "torch" }
 
 
 [[tool.poetry.source]]
 name = "PyPI"
```

### Comparing `openlrc-0.2.1/README.md` & `openlrc-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `openlrc-0.2.1/PKG-INFO` & `openlrc-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlrc
-Version: 0.2.1
+Version: 0.2.2
 Summary: Transcribe (whisper) and translate (gpt) voice into LRC file.
 Home-page: https://github.com/zh-plus/Open-Lyrics
 License: MIT
 Keywords: openai-gpt3,whisper,voice transcribe,lrc
 Author: Hao Zheng
 Author-email: zhenghaosustc@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -13,18 +13,19 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
+Requires-Dist: aiohttp (>=3.8.5,<4.0.0)
 Requires-Dist: audioread (>=3.0.0,<4.0.0)
 Requires-Dist: colorlog (>=6.7.0,<7.0.0)
 Requires-Dist: deepfilternet (>=0.5.3,<0.6.0)
-Requires-Dist: faster-whisper (>=0.6.0,<0.7.0)
+Requires-Dist: faster-whisper (>=0.7.1,<0.8.0)
 Requires-Dist: ffmpeg-normalize (>=1.27.5,<2.0.0)
 Requires-Dist: ffmpeg-python (>=0.2.0,<0.3.0)
 Requires-Dist: filetype (>=1.2.0,<2.0.0)
 Requires-Dist: jaconvV2 (>=0.4,<0.5)
 Requires-Dist: langcodes (>=3.3.0,<4.0.0)
 Requires-Dist: language-data (>=1.1,<2.0)
 Requires-Dist: lingua-language-detector (>=1.3.2,<2.0.0)
```

