# Comparing `tmp/whisper-at-0.2.tar.gz` & `tmp/whisper-at-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper-at-0.2.tar", last modified: Thu Jul  6 19:56:42 2023, max compression
+gzip compressed data, was "whisper-at-0.4.tar", last modified: Mon Jul 24 03:09:02 2023, max compression
```

## Comparing `whisper-at-0.2.tar` & `whisper-at-0.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwsr-x   0 yuangong (25758) sls       (1226)        0 2023-07-06 19:56:42.297318 whisper-at-0.2/
--rw-r--r--   0 yuangong (25758) sls       (1226)     1298 2023-07-06 19:49:21.000000 whisper-at-0.2/LICENSE
--rw-r--r--   0 yuangong (25758) sls       (1226)     1063 2023-05-05 07:31:35.000000 whisper-at-0.2/LICENSE_OpenAI_Whisper
--rw-r--r--   0 yuangong (25758) sls       (1226)      131 2023-06-03 09:13:21.000000 whisper-at-0.2/MANIFEST.in
--rw-rw-r--   0 yuangong (25758) sls       (1226)    17901 2023-07-06 19:56:42.295793 whisper-at-0.2/PKG-INFO
--rw-r--r--   0 yuangong (25758) sls       (1226)    17563 2023-07-06 19:54:21.000000 whisper-at-0.2/README.md
--rw-r--r--   0 yuangong (25758) sls       (1226)      115 2023-05-05 07:31:35.000000 whisper-at-0.2/pyproject.toml
--rw-r--r--   0 yuangong (25758) sls       (1226)       54 2023-05-05 07:31:35.000000 whisper-at-0.2/requirements.txt
--rw-rw-r--   0 yuangong (25758) sls       (1226)       38 2023-07-06 19:56:42.297945 whisper-at-0.2/setup.cfg
--rw-r--r--   0 yuangong (25758) sls       (1226)     1097 2023-07-06 19:51:10.000000 whisper-at-0.2/setup.py
-drwxrwsr-x   0 yuangong (25758) sls       (1226)        0 2023-07-06 19:56:42.149217 whisper-at-0.2/whisper_at/
--rw-r--r--   0 yuangong (25758) sls       (1226)     8905 2023-06-16 23:12:55.000000 whisper-at-0.2/whisper_at/__init__.py
--rw-r--r--   0 yuangong (25758) sls       (1226)       35 2023-05-05 07:31:35.000000 whisper-at-0.2/whisper_at/__main__.py
-drwxrwsr-x   0 yuangong (25758) sls       (1226)        0 2023-07-06 19:56:42.257680 whisper-at-0.2/whisper_at/assets/
--rw-r--r--   0 yuangong (25758) sls       (1226)    14675 2023-06-06 05:36:29.000000 whisper-at-0.2/whisper_at/assets/class_labels_indices.csv
--rw-r--r--   0 yuangong (25758) sls       (1226)   835554 2023-05-05 07:31:35.000000 whisper-at-0.2/whisper_at/assets/gpt2.tiktoken
--rw-r--r--   0 yuangong (25758) sls       (1226)  2728075 2023-06-03 19:35:16.000000 whisper-at-0.2/whisper_at/assets/label_name_dict.json
--rw-r--r--   0 yuangong (25758) sls       (1226)     2048 2023-05-05 07:31:35.000000 whisper-at-0.2/whisper_at/assets/mel_filters.npz
--rw-r--r--   0 yuangong (25758) sls       (1226)   816730 2023-05-05 07:31:35.000000 whisper-at-0.2/whisper_at/assets/multilingual.tiktoken
--rw-r--r--   0 yuangong (25758) sls       (1226)     2920 2023-06-04 08:50:38.000000 whisper-at-0.2/whisper_at/at_post_processing.py
--rw-r--r--   0 yuangong (25758) sls       (1226)     4837 2023-05-05 07:31:35.000000 whisper-at-0.2/whisper_at/audio.py
--rw-r--r--   0 yuangong (25758) sls       (1226)    32120 2023-06-01 08:27:38.000000 whisper-at-0.2/whisper_at/decoding.py
--rw-r--r--   0 yuangong (25758) sls       (1226)    14807 2023-06-04 20:07:06.000000 whisper-at-0.2/whisper_at/model.py
-drwxrwsr-x   0 yuangong (25758) sls       (1226)        0 2023-07-06 19:56:42.291713 whisper-at-0.2/whisper_at/normalizers/
--rw-r--r--   0 yuangong (25758) sls       (1226)      130 2023-05-05 07:31:35.000000 whisper-at-0.2/whisper_at/normalizers/__init__.py
--rw-r--r--   0 yuangong (25758) sls       (1226)     1936 2023-05-05 07:31:35.000000 whisper-at-0.2/whisper_at/normalizers/basic.py
--rw-r--r--   0 yuangong (25758) sls       (1226)    56128 2023-05-05 07:31:35.000000 whisper-at-0.2/whisper_at/normalizers/english.json
--rw-r--r--   0 yuangong (25758) sls       (1226)    20868 2023-05-05 07:31:35.000000 whisper-at-0.2/whisper_at/normalizers/english.py
--rw-r--r--   0 yuangong (25758) sls       (1226)    11431 2023-05-05 07:31:35.000000 whisper-at-0.2/whisper_at/timing.py
--rw-r--r--   0 yuangong (25758) sls       (1226)    11981 2023-05-05 07:31:35.000000 whisper-at-0.2/whisper_at/tokenizer.py
--rw-r--r--   0 yuangong (25758) sls       (1226)    23967 2023-06-01 22:56:11.000000 whisper-at-0.2/whisper_at/transcribe.py
--rw-r--r--   0 yuangong (25758) sls       (1226)     3474 2023-05-05 07:31:35.000000 whisper-at-0.2/whisper_at/triton_ops.py
--rw-r--r--   0 yuangong (25758) sls       (1226)     9428 2023-05-05 07:31:35.000000 whisper-at-0.2/whisper_at/utils.py
--rw-r--r--   0 yuangong (25758) sls       (1226)       20 2023-07-06 19:50:35.000000 whisper-at-0.2/whisper_at/version.py
-drwxrwsr-x   0 yuangong (25758) sls       (1226)        0 2023-07-06 19:56:42.166847 whisper-at-0.2/whisper_at.egg-info/
--rw-rw-r--   0 yuangong (25758) sls       (1226)    17901 2023-07-06 19:56:42.000000 whisper-at-0.2/whisper_at.egg-info/PKG-INFO
--rw-rw-r--   0 yuangong (25758) sls       (1226)      903 2023-07-06 19:56:42.000000 whisper-at-0.2/whisper_at.egg-info/SOURCES.txt
--rw-rw-r--   0 yuangong (25758) sls       (1226)        1 2023-07-06 19:56:42.000000 whisper-at-0.2/whisper_at.egg-info/dependency_links.txt
--rw-rw-r--   0 yuangong (25758) sls       (1226)       51 2023-07-06 19:56:42.000000 whisper-at-0.2/whisper_at.egg-info/entry_points.txt
--rw-rw-r--   0 yuangong (25758) sls       (1226)      107 2023-07-06 19:56:42.000000 whisper-at-0.2/whisper_at.egg-info/requires.txt
--rw-rw-r--   0 yuangong (25758) sls       (1226)       11 2023-07-06 19:56:42.000000 whisper-at-0.2/whisper_at.egg-info/top_level.txt
+drwxrwsr-x   0 yuangong (25758) sls       (1226)        0 2023-07-24 03:09:02.617278 whisper-at-0.4/
+-rw-r--r--   0 yuangong (25758) sls       (1226)     1298 2023-07-06 19:49:21.000000 whisper-at-0.4/LICENSE
+-rw-r--r--   0 yuangong (25758) sls       (1226)     1063 2023-05-05 07:31:35.000000 whisper-at-0.4/LICENSE_OpenAI_Whisper
+-rw-r--r--   0 yuangong (25758) sls       (1226)      131 2023-06-03 09:13:21.000000 whisper-at-0.4/MANIFEST.in
+-rw-rw-r--   0 yuangong (25758) sls       (1226)    19916 2023-07-24 03:09:02.616117 whisper-at-0.4/PKG-INFO
+-rw-r--r--   0 yuangong (25758) sls       (1226)    19578 2023-07-19 23:54:51.000000 whisper-at-0.4/README.md
+-rw-r--r--   0 yuangong (25758) sls       (1226)      115 2023-05-05 07:31:35.000000 whisper-at-0.4/pyproject.toml
+-rw-r--r--   0 yuangong (25758) sls       (1226)       53 2023-07-19 23:37:00.000000 whisper-at-0.4/requirements.txt
+-rw-rw-r--   0 yuangong (25758) sls       (1226)       38 2023-07-24 03:09:02.617615 whisper-at-0.4/setup.cfg
+-rw-r--r--   0 yuangong (25758) sls       (1226)     1097 2023-07-24 03:08:43.000000 whisper-at-0.4/setup.py
+drwxrwsr-x   0 yuangong (25758) sls       (1226)        0 2023-07-24 03:09:02.541009 whisper-at-0.4/whisper_at/
+-rw-r--r--   0 yuangong (25758) sls       (1226)     8961 2023-07-24 03:05:42.000000 whisper-at-0.4/whisper_at/__init__.py
+-rw-r--r--   0 yuangong (25758) sls       (1226)       35 2023-05-05 07:31:35.000000 whisper-at-0.4/whisper_at/__main__.py
+drwxrwsr-x   0 yuangong (25758) sls       (1226)        0 2023-07-24 03:09:02.597315 whisper-at-0.4/whisper_at/assets/
+-rw-r--r--   0 yuangong (25758) sls       (1226)    14675 2023-06-06 05:36:29.000000 whisper-at-0.4/whisper_at/assets/class_labels_indices.csv
+-rw-r--r--   0 yuangong (25758) sls       (1226)   835554 2023-05-05 07:31:35.000000 whisper-at-0.4/whisper_at/assets/gpt2.tiktoken
+-rw-r--r--   0 yuangong (25758) sls       (1226)  2728075 2023-06-03 19:35:16.000000 whisper-at-0.4/whisper_at/assets/label_name_dict.json
+-rw-r--r--   0 yuangong (25758) sls       (1226)     2048 2023-05-05 07:31:35.000000 whisper-at-0.4/whisper_at/assets/mel_filters.npz
+-rw-r--r--   0 yuangong (25758) sls       (1226)   816730 2023-05-05 07:31:35.000000 whisper-at-0.4/whisper_at/assets/multilingual.tiktoken
+-rw-r--r--   0 yuangong (25758) sls       (1226)     2920 2023-06-04 08:50:38.000000 whisper-at-0.4/whisper_at/at_post_processing.py
+-rw-r--r--   0 yuangong (25758) sls       (1226)     4837 2023-05-05 07:31:35.000000 whisper-at-0.4/whisper_at/audio.py
+-rw-r--r--   0 yuangong (25758) sls       (1226)    32120 2023-06-01 08:27:38.000000 whisper-at-0.4/whisper_at/decoding.py
+-rw-r--r--   0 yuangong (25758) sls       (1226)    14807 2023-06-04 20:07:06.000000 whisper-at-0.4/whisper_at/model.py
+drwxrwsr-x   0 yuangong (25758) sls       (1226)        0 2023-07-24 03:09:02.613632 whisper-at-0.4/whisper_at/normalizers/
+-rw-r--r--   0 yuangong (25758) sls       (1226)      130 2023-05-05 07:31:35.000000 whisper-at-0.4/whisper_at/normalizers/__init__.py
+-rw-r--r--   0 yuangong (25758) sls       (1226)     1936 2023-05-05 07:31:35.000000 whisper-at-0.4/whisper_at/normalizers/basic.py
+-rw-r--r--   0 yuangong (25758) sls       (1226)    56128 2023-05-05 07:31:35.000000 whisper-at-0.4/whisper_at/normalizers/english.json
+-rw-r--r--   0 yuangong (25758) sls       (1226)    20868 2023-05-05 07:31:35.000000 whisper-at-0.4/whisper_at/normalizers/english.py
+-rw-r--r--   0 yuangong (25758) sls       (1226)    11431 2023-05-05 07:31:35.000000 whisper-at-0.4/whisper_at/timing.py
+-rw-r--r--   0 yuangong (25758) sls       (1226)    11981 2023-05-05 07:31:35.000000 whisper-at-0.4/whisper_at/tokenizer.py
+-rw-r--r--   0 yuangong (25758) sls       (1226)    23967 2023-06-01 22:56:11.000000 whisper-at-0.4/whisper_at/transcribe.py
+-rw-r--r--   0 yuangong (25758) sls       (1226)     3474 2023-05-05 07:31:35.000000 whisper-at-0.4/whisper_at/triton_ops.py
+-rw-r--r--   0 yuangong (25758) sls       (1226)     9428 2023-05-05 07:31:35.000000 whisper-at-0.4/whisper_at/utils.py
+-rw-r--r--   0 yuangong (25758) sls       (1226)       20 2023-07-24 03:08:36.000000 whisper-at-0.4/whisper_at/version.py
+drwxrwsr-x   0 yuangong (25758) sls       (1226)        0 2023-07-24 03:09:02.551436 whisper-at-0.4/whisper_at.egg-info/
+-rw-rw-r--   0 yuangong (25758) sls       (1226)    19916 2023-07-24 03:09:02.000000 whisper-at-0.4/whisper_at.egg-info/PKG-INFO
+-rw-rw-r--   0 yuangong (25758) sls       (1226)      903 2023-07-24 03:09:02.000000 whisper-at-0.4/whisper_at.egg-info/SOURCES.txt
+-rw-rw-r--   0 yuangong (25758) sls       (1226)        1 2023-07-24 03:09:02.000000 whisper-at-0.4/whisper_at.egg-info/dependency_links.txt
+-rw-rw-r--   0 yuangong (25758) sls       (1226)       51 2023-07-24 03:09:02.000000 whisper-at-0.4/whisper_at.egg-info/entry_points.txt
+-rw-rw-r--   0 yuangong (25758) sls       (1226)      107 2023-07-24 03:09:02.000000 whisper-at-0.4/whisper_at.egg-info/requires.txt
+-rw-rw-r--   0 yuangong (25758) sls       (1226)       11 2023-07-24 03:09:02.000000 whisper-at-0.4/whisper_at.egg-info/top_level.txt
```

### Comparing `whisper-at-0.2/LICENSE` & `whisper-at-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper-at-0.2/LICENSE_OpenAI_Whisper` & `whisper-at-0.4/LICENSE_OpenAI_Whisper`

 * *Files identical despite different names*

### Comparing `whisper-at-0.2/PKG-INFO` & `whisper-at-0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,73 +1,111 @@
-Metadata-Version: 2.1
-Name: whisper-at
-Version: 0.2
-Summary: Joint speech recognition and audio tagging model.
-Home-page: https://github.com/YuanGongND/whisper-at
-Author: Yuan Gong
-License: BSD
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-License-File: LICENSE_OpenAI_Whisper
-
-# Whisper-AT
+# Whisper-AT: Noise-Robust Automatic Speech Recognizers are Also Strong Audio Event Taggers
 
 - [Introduction](#introduction)
 - [Citation](#citation)
 - [For Applications](#for-applications)
 - [For Research](#for-research)
 - [Available Models and Audio Tagging Performance](#available-models-and-audio-tagging-performance)
 - [License](#license)
 - [Contact](#contact)
 
 ## Introduction
 
-[**[Paper]**]()
+[**[Paper]**](https://arxiv.org/pdf/2307.03183.pdf)
+
+[**[HuggingFace Space]**](https://huggingface.co/spaces/yuangongfdu/whisper-at) (Try Whisper-AT without Coding!)
+
 [**[Colab Demo]**](https://colab.research.google.com/drive/1BbOGWCMjkOlOY5PbEMGk5RomRSqMcy_Q?usp=sharing)
 
+[**[Local Notebook Demo]**(for user without Colab access)](https://github.com/YuanGongND/whisper-at/blob/main/sample/whisper_at_demo.ipynb)
+
 <p align="center"><img src="https://github.com/YuanGongND/whisper-at/blob/main/tltr.png?raw=true" alt="Illustration of Whisper-AT." width="800"/></p>
 
+<div align="center">
+  (Please turn on audio to listen to the sounds)
+  <video src="https://github.com/YuanGongND/whisper-at/assets/17163494/b479320a-b7f7-4bfc-acba-087b447623bd" width="400" />
+</div>
+
 Whisper-AT is a joint audio tagging and speech recognition model. It inherits strong speech recognition ability from [OpenAI Whisper](https://github.com/openai/whisper), and its ASR performance is exactly the same as the original Whisper. 
 The API interface and usage are also identical to the original OpenAI Whisper, so users can seamlessly switch from the original Whisper to Whisper-AT.
 
 The advantage of Whisper-AT is that with minimal (less than 1%**) additional computational cost, Whisper-AT outputs general audio event labels ([527-class AudioSet labels](https://github.com/YuanGongND/whisper-at/blob/main/audioset_label.csv)) in desired temporal resolution in addition to the ASR transcripts. This makes audio tagging much easier and faster than using a standalone audio tagging model.
 
 Internally, Whisper-AT freezes all original Whisper parameters, and trains a Time- and Layer-wise Transformer (TL-TR) on top of the Whisper encoder representations for the audio tagging task.
 
 To help better understand the pros and cons of this work, we have attached the anonymous reviews and our responses [[here]](https://github.com/YuanGongND/whisper-at/tree/main/review). We thank the anonymous reviewers' invaluable comments.
 
 ** *Not for all models, see the paper for details.*
 
+<hr style="border: 0; height: 1px; background-color: #e0e0e0;">
+
+***Quick Start (Run in 8 lines of code)***
+
+In shell, 
+```
+pip install whisper-at
+```
+
+For Mac users, there is a known bug, please use the following workaround:
+```bash
+# install all dependencies except triton, this will break when it tries to install triton
+pip install whisper-at 
+# install whisper-at without any dependency
+pip install --no-deps whisper-at  
+```
+Then, in Python,
+```python3
+import whisper_at as whisper
+
+audio_tagging_time_resolution = 10
+model = whisper.load_model("large-v1")
+result = model.transcribe("audio.mp3", at_time_res=audio_tagging_time_resolution)
+# ASR Results
+print(result["text"])
+# Audio Tagging Results
+audio_tag_result = whisper.parse_at_label(result, language='follow_asr', top_k=5, p_threshold=-1, include_class_list=list(range(527)))
+print(audio_tag_result)
+```
+
 ## Citation
 Please cite our Interspeech 2023 paper if you find this repository useful. 
 ```  
 @inproceedings{gong_whisperat,
   author={Gong, Yuan and Khurana, Sameer and Karlinsky, Leonid and Glass, James},
   title={Whisper-AT: Noise-Robust Automatic Speech Recognizers are Also Strong Audio Event Taggers},
   year=2023,
   booktitle={Proc. Interspeech 2023}
 }
 ```
 
 ## For Applications
 
-**The best way to learn how to use Whisper-AT is this [Colab Tutorial](https://colab.research.google.com/drive/1BbOGWCMjkOlOY5PbEMGk5RomRSqMcy_Q?usp=sharing). You can skip all below if you read it.**
+**The best way to learn how to use Whisper-AT is this [[**Colab Tutorial**]](https://colab.research.google.com/drive/1BbOGWCMjkOlOY5PbEMGk5RomRSqMcy_Q?usp=sharing). You can skip all below if you read it.**
+If you don't have Google Colab access (uncommon), you can use this [[Local Notebook]](https://github.com/YuanGongND/whisper-at/blob/main/sample/whisper_at_demo.ipynb) as a substitution.
+
+<hr style="border: 0; height: 1px; background-color: #e0e0e0;">
 
 If you do not care how Whisper-AT is implemented, but just want to use it, you only need to read this section. This will be very simple.
 
 ### Step 1. Install Whisper-AT
 
 We intentionally do not any additional dependencies to the original Whisper. So if your environment can run the original Whisper, it can also run Whisper-AT.
 
 Whisper-AT can be installed simply by:
 
     pip install whisper-at
 
+For Mac users, there is a known bug, please use the following workaround:
+```bash
+# install all dependencies except triton, this will break when it tries to install triton
+pip install whisper-at 
+# install whisper-at without any dependency
+pip install --no-deps whisper-at  
+```
+
 Note that following original Whisper, it also requires the command-line tool [`ffmpeg`](https://ffmpeg.org/) to be installed on your system. Please check OpenAI Whisper repo for details.
 
 ### Step 2. Use as the Original Whisper
 
 ```python3
 # note this is whisper"_"at not whisper-at
 import whisper_at as whisper
@@ -119,15 +157,15 @@
 **Return:** A dictionary of audio tagging results.
 
 This makes the audio tagging result human-readable, in specified language. If not specified, `whisepr.parse_at_label` output label names in the same language with the ASR output.
 That's it!
 
 ## For Research
 
-If you are interested in the findings and experiments in our Interspeech paper *[Whisper-AT: Noise-Robust Automatic Speech Recognizers are Also Strong Audio Event Taggers]()*, please check this section.
+If you are interested in the findings and experiments in our Interspeech paper *[Whisper-AT: Noise-Robust Automatic Speech Recognizers are Also Strong Audio Event Taggers](https://arxiv.org/pdf/2307.03183.pdf)*, please check this section.
 We provide our code to reproduce the experiments in the paper. 
 
 The paper mainly contains two contributions:
 - First we report an interesting and surprising finding that while Whisper is very robust against real-world background sounds (e.g., music), its audio representation is actually **NOT noise-invariant**, but is instead highly correlated to non-speech sounds, indicating that Whisper recognizes speech **conditioned** on the noise type. 
 - Second, with the above finding, we build a unified audio tagging and speech recognition model Whisper-AT by freezing the backbone of Whisper, and training a novel audio tagging model called **Time and Layer-wise Transformer (TL-TR)** on top of it. With  <1% extra computational cost, Whisper-AT can recognize audio events, in addition to spoken text, in a single forward pass.
 
 <hr style="border: 0; height: 1px; background-color: #e0e0e0;">
@@ -237,8 +275,8 @@
 - Whisper-AT supports all Whisper models. The script downloads the original OpenAI Whisper model and our AT model automatically.
 - All results reported in the paper are based on `large-v1`, `medium.en`, `small.en`, `base.en`, and `tiny.en`. `large-v2` and multi-lingual models are trained after the paper is finished.
 
 ## License
 Whisper-AT's code and model weights are released under a BSD license, which is similar with the original OpenAI Whisper's MIT license. Commercial use is welcome. 
 
 ## Contact
-If you have a question, please create a Github issue (preferred) or send me an email [yuangong@mit.edu](yuangong@mit.edu).
+If you have a question, please create a Github issue (preferred) or send me an email [yuangong@mit.edu](yuangong@mit.edu).
```

### Comparing `whisper-at-0.2/README.md` & `whisper-at-0.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,60 +1,124 @@
-# Whisper-AT
+Metadata-Version: 2.1
+Name: whisper-at
+Version: 0.4
+Summary: Joint speech recognition and audio tagging model.
+Home-page: https://github.com/YuanGongND/whisper-at
+Author: Yuan Gong
+License: BSD
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+License-File: LICENSE_OpenAI_Whisper
+
+# Whisper-AT: Noise-Robust Automatic Speech Recognizers are Also Strong Audio Event Taggers
 
 - [Introduction](#introduction)
 - [Citation](#citation)
 - [For Applications](#for-applications)
 - [For Research](#for-research)
 - [Available Models and Audio Tagging Performance](#available-models-and-audio-tagging-performance)
 - [License](#license)
 - [Contact](#contact)
 
 ## Introduction
 
-[**[Paper]**]()
+[**[Paper]**](https://arxiv.org/pdf/2307.03183.pdf)
+
+[**[HuggingFace Space]**](https://huggingface.co/spaces/yuangongfdu/whisper-at) (Try Whisper-AT without Coding!)
+
 [**[Colab Demo]**](https://colab.research.google.com/drive/1BbOGWCMjkOlOY5PbEMGk5RomRSqMcy_Q?usp=sharing)
 
+[**[Local Notebook Demo]**(for user without Colab access)](https://github.com/YuanGongND/whisper-at/blob/main/sample/whisper_at_demo.ipynb)
+
 <p align="center"><img src="https://github.com/YuanGongND/whisper-at/blob/main/tltr.png?raw=true" alt="Illustration of Whisper-AT." width="800"/></p>
 
+<div align="center">
+  (Please turn on audio to listen to the sounds)
+  <video src="https://github.com/YuanGongND/whisper-at/assets/17163494/b479320a-b7f7-4bfc-acba-087b447623bd" width="400" />
+</div>
+
 Whisper-AT is a joint audio tagging and speech recognition model. It inherits strong speech recognition ability from [OpenAI Whisper](https://github.com/openai/whisper), and its ASR performance is exactly the same as the original Whisper. 
 The API interface and usage are also identical to the original OpenAI Whisper, so users can seamlessly switch from the original Whisper to Whisper-AT.
 
 The advantage of Whisper-AT is that with minimal (less than 1%**) additional computational cost, Whisper-AT outputs general audio event labels ([527-class AudioSet labels](https://github.com/YuanGongND/whisper-at/blob/main/audioset_label.csv)) in desired temporal resolution in addition to the ASR transcripts. This makes audio tagging much easier and faster than using a standalone audio tagging model.
 
 Internally, Whisper-AT freezes all original Whisper parameters, and trains a Time- and Layer-wise Transformer (TL-TR) on top of the Whisper encoder representations for the audio tagging task.
 
 To help better understand the pros and cons of this work, we have attached the anonymous reviews and our responses [[here]](https://github.com/YuanGongND/whisper-at/tree/main/review). We thank the anonymous reviewers' invaluable comments.
 
 ** *Not for all models, see the paper for details.*
 
+<hr style="border: 0; height: 1px; background-color: #e0e0e0;">
+
+***Quick Start (Run in 8 lines of code)***
+
+In shell, 
+```
+pip install whisper-at
+```
+
+For Mac users, there is a known bug, please use the following workaround:
+```bash
+# install all dependencies except triton, this will break when it tries to install triton
+pip install whisper-at 
+# install whisper-at without any dependency
+pip install --no-deps whisper-at  
+```
+Then, in Python,
+```python3
+import whisper_at as whisper
+
+audio_tagging_time_resolution = 10
+model = whisper.load_model("large-v1")
+result = model.transcribe("audio.mp3", at_time_res=audio_tagging_time_resolution)
+# ASR Results
+print(result["text"])
+# Audio Tagging Results
+audio_tag_result = whisper.parse_at_label(result, language='follow_asr', top_k=5, p_threshold=-1, include_class_list=list(range(527)))
+print(audio_tag_result)
+```
+
 ## Citation
 Please cite our Interspeech 2023 paper if you find this repository useful. 
 ```  
 @inproceedings{gong_whisperat,
   author={Gong, Yuan and Khurana, Sameer and Karlinsky, Leonid and Glass, James},
   title={Whisper-AT: Noise-Robust Automatic Speech Recognizers are Also Strong Audio Event Taggers},
   year=2023,
   booktitle={Proc. Interspeech 2023}
 }
 ```
 
 ## For Applications
 
-**The best way to learn how to use Whisper-AT is this [Colab Tutorial](https://colab.research.google.com/drive/1BbOGWCMjkOlOY5PbEMGk5RomRSqMcy_Q?usp=sharing). You can skip all below if you read it.**
+**The best way to learn how to use Whisper-AT is this [[**Colab Tutorial**]](https://colab.research.google.com/drive/1BbOGWCMjkOlOY5PbEMGk5RomRSqMcy_Q?usp=sharing). You can skip all below if you read it.**
+If you don't have Google Colab access (uncommon), you can use this [[Local Notebook]](https://github.com/YuanGongND/whisper-at/blob/main/sample/whisper_at_demo.ipynb) as a substitution.
+
+<hr style="border: 0; height: 1px; background-color: #e0e0e0;">
 
 If you do not care how Whisper-AT is implemented, but just want to use it, you only need to read this section. This will be very simple.
 
 ### Step 1. Install Whisper-AT
 
 We intentionally do not any additional dependencies to the original Whisper. So if your environment can run the original Whisper, it can also run Whisper-AT.
 
 Whisper-AT can be installed simply by:
 
     pip install whisper-at
 
+For Mac users, there is a known bug, please use the following workaround:
+```bash
+# install all dependencies except triton, this will break when it tries to install triton
+pip install whisper-at 
+# install whisper-at without any dependency
+pip install --no-deps whisper-at  
+```
+
 Note that following original Whisper, it also requires the command-line tool [`ffmpeg`](https://ffmpeg.org/) to be installed on your system. Please check OpenAI Whisper repo for details.
 
 ### Step 2. Use as the Original Whisper
 
 ```python3
 # note this is whisper"_"at not whisper-at
 import whisper_at as whisper
@@ -106,15 +170,15 @@
 **Return:** A dictionary of audio tagging results.
 
 This makes the audio tagging result human-readable, in specified language. If not specified, `whisepr.parse_at_label` output label names in the same language with the ASR output.
 That's it!
 
 ## For Research
 
-If you are interested in the findings and experiments in our Interspeech paper *[Whisper-AT: Noise-Robust Automatic Speech Recognizers are Also Strong Audio Event Taggers]()*, please check this section.
+If you are interested in the findings and experiments in our Interspeech paper *[Whisper-AT: Noise-Robust Automatic Speech Recognizers are Also Strong Audio Event Taggers](https://arxiv.org/pdf/2307.03183.pdf)*, please check this section.
 We provide our code to reproduce the experiments in the paper. 
 
 The paper mainly contains two contributions:
 - First we report an interesting and surprising finding that while Whisper is very robust against real-world background sounds (e.g., music), its audio representation is actually **NOT noise-invariant**, but is instead highly correlated to non-speech sounds, indicating that Whisper recognizes speech **conditioned** on the noise type. 
 - Second, with the above finding, we build a unified audio tagging and speech recognition model Whisper-AT by freezing the backbone of Whisper, and training a novel audio tagging model called **Time and Layer-wise Transformer (TL-TR)** on top of it. With  <1% extra computational cost, Whisper-AT can recognize audio events, in addition to spoken text, in a single forward pass.
 
 <hr style="border: 0; height: 1px; background-color: #e0e0e0;">
@@ -224,8 +288,8 @@
 - Whisper-AT supports all Whisper models. The script downloads the original OpenAI Whisper model and our AT model automatically.
 - All results reported in the paper are based on `large-v1`, `medium.en`, `small.en`, `base.en`, and `tiny.en`. `large-v2` and multi-lingual models are trained after the paper is finished.
 
 ## License
 Whisper-AT's code and model weights are released under a BSD license, which is similar with the original OpenAI Whisper's MIT license. Commercial use is welcome. 
 
 ## Contact
-If you have a question, please create a Github issue (preferred) or send me an email [yuangong@mit.edu](yuangong@mit.edu).
+If you have a question, please create a Github issue (preferred) or send me an email [yuangong@mit.edu](yuangong@mit.edu).
```

### Comparing `whisper-at-0.2/setup.py` & `whisper-at-0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 requirements = []
 if sys.platform.startswith("linux") and platform.machine() == "x86_64":
     requirements.append("triton==2.0.0")
 
 setup(
     name="whisper-at",
     py_modules=["whisper_at"],
-    version=0.2,
+    version=0.4,
     description="Joint speech recognition and audio tagging model.",
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     readme="README.md",
     python_requires=">=3.8",
     author="Yuan Gong",
     url="https://github.com/YuanGongND/whisper-at",
```

### Comparing `whisper-at-0.2/whisper_at/__init__.py` & `whisper-at-0.4/whisper_at/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,16 @@
 }
 
 
 def _download(url: str, root: str, in_memory: bool) -> Union[bytes, str]:
     os.makedirs(root, exist_ok=True)
 
     expected_sha256 = url.split("/")[-2]
-    download_target = os.path.join(root, os.path.basename(url))
+    parsed_url = urllib.parse.urlparse(url).path
+    download_target = os.path.join(root, os.path.basename(parsed_url))
 
     if os.path.exists(download_target) and not os.path.isfile(download_target):
         raise RuntimeError(f"{download_target} exists and is not a regular file")
 
     if os.path.isfile(download_target):
         with open(download_target, "rb") as f:
             model_bytes = f.read()
```

### Comparing `whisper-at-0.2/whisper_at/assets/class_labels_indices.csv` & `whisper-at-0.4/whisper_at/assets/class_labels_indices.csv`

 * *Files identical despite different names*

### Comparing `whisper-at-0.2/whisper_at/assets/gpt2.tiktoken` & `whisper-at-0.4/whisper_at/assets/gpt2.tiktoken`

 * *Files identical despite different names*

### Comparing `whisper-at-0.2/whisper_at/assets/label_name_dict.json` & `whisper-at-0.4/whisper_at/assets/label_name_dict.json`

 * *Files identical despite different names*

### Comparing `whisper-at-0.2/whisper_at/assets/mel_filters.npz` & `whisper-at-0.4/whisper_at/assets/mel_filters.npz`

 * *Files identical despite different names*

### Comparing `whisper-at-0.2/whisper_at/assets/multilingual.tiktoken` & `whisper-at-0.4/whisper_at/assets/multilingual.tiktoken`

 * *Files identical despite different names*

### Comparing `whisper-at-0.2/whisper_at/at_post_processing.py` & `whisper-at-0.4/whisper_at/at_post_processing.py`

 * *Files identical despite different names*

### Comparing `whisper-at-0.2/whisper_at/audio.py` & `whisper-at-0.4/whisper_at/audio.py`

 * *Files identical despite different names*

### Comparing `whisper-at-0.2/whisper_at/decoding.py` & `whisper-at-0.4/whisper_at/decoding.py`

 * *Files identical despite different names*

### Comparing `whisper-at-0.2/whisper_at/model.py` & `whisper-at-0.4/whisper_at/model.py`

 * *Files identical despite different names*

### Comparing `whisper-at-0.2/whisper_at/normalizers/basic.py` & `whisper-at-0.4/whisper_at/normalizers/basic.py`

 * *Files identical despite different names*

### Comparing `whisper-at-0.2/whisper_at/normalizers/english.json` & `whisper-at-0.4/whisper_at/normalizers/english.json`

 * *Files identical despite different names*

### Comparing `whisper-at-0.2/whisper_at/normalizers/english.py` & `whisper-at-0.4/whisper_at/normalizers/english.py`

 * *Files identical despite different names*

### Comparing `whisper-at-0.2/whisper_at/timing.py` & `whisper-at-0.4/whisper_at/timing.py`

 * *Files identical despite different names*

### Comparing `whisper-at-0.2/whisper_at/tokenizer.py` & `whisper-at-0.4/whisper_at/tokenizer.py`

 * *Files identical despite different names*

### Comparing `whisper-at-0.2/whisper_at/transcribe.py` & `whisper-at-0.4/whisper_at/transcribe.py`

 * *Files identical despite different names*

### Comparing `whisper-at-0.2/whisper_at/triton_ops.py` & `whisper-at-0.4/whisper_at/triton_ops.py`

 * *Files identical despite different names*

### Comparing `whisper-at-0.2/whisper_at/utils.py` & `whisper-at-0.4/whisper_at/utils.py`

 * *Files identical despite different names*

### Comparing `whisper-at-0.2/whisper_at.egg-info/PKG-INFO` & `whisper-at-0.4/whisper_at.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,73 +1,124 @@
 Metadata-Version: 2.1
 Name: whisper-at
-Version: 0.2
+Version: 0.4
 Summary: Joint speech recognition and audio tagging model.
 Home-page: https://github.com/YuanGongND/whisper-at
 Author: Yuan Gong
 License: BSD
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 License-File: LICENSE_OpenAI_Whisper
 
-# Whisper-AT
+# Whisper-AT: Noise-Robust Automatic Speech Recognizers are Also Strong Audio Event Taggers
 
 - [Introduction](#introduction)
 - [Citation](#citation)
 - [For Applications](#for-applications)
 - [For Research](#for-research)
 - [Available Models and Audio Tagging Performance](#available-models-and-audio-tagging-performance)
 - [License](#license)
 - [Contact](#contact)
 
 ## Introduction
 
-[**[Paper]**]()
+[**[Paper]**](https://arxiv.org/pdf/2307.03183.pdf)
+
+[**[HuggingFace Space]**](https://huggingface.co/spaces/yuangongfdu/whisper-at) (Try Whisper-AT without Coding!)
+
 [**[Colab Demo]**](https://colab.research.google.com/drive/1BbOGWCMjkOlOY5PbEMGk5RomRSqMcy_Q?usp=sharing)
 
+[**[Local Notebook Demo]**(for user without Colab access)](https://github.com/YuanGongND/whisper-at/blob/main/sample/whisper_at_demo.ipynb)
+
 <p align="center"><img src="https://github.com/YuanGongND/whisper-at/blob/main/tltr.png?raw=true" alt="Illustration of Whisper-AT." width="800"/></p>
 
+<div align="center">
+  (Please turn on audio to listen to the sounds)
+  <video src="https://github.com/YuanGongND/whisper-at/assets/17163494/b479320a-b7f7-4bfc-acba-087b447623bd" width="400" />
+</div>
+
 Whisper-AT is a joint audio tagging and speech recognition model. It inherits strong speech recognition ability from [OpenAI Whisper](https://github.com/openai/whisper), and its ASR performance is exactly the same as the original Whisper. 
 The API interface and usage are also identical to the original OpenAI Whisper, so users can seamlessly switch from the original Whisper to Whisper-AT.
 
 The advantage of Whisper-AT is that with minimal (less than 1%**) additional computational cost, Whisper-AT outputs general audio event labels ([527-class AudioSet labels](https://github.com/YuanGongND/whisper-at/blob/main/audioset_label.csv)) in desired temporal resolution in addition to the ASR transcripts. This makes audio tagging much easier and faster than using a standalone audio tagging model.
 
 Internally, Whisper-AT freezes all original Whisper parameters, and trains a Time- and Layer-wise Transformer (TL-TR) on top of the Whisper encoder representations for the audio tagging task.
 
 To help better understand the pros and cons of this work, we have attached the anonymous reviews and our responses [[here]](https://github.com/YuanGongND/whisper-at/tree/main/review). We thank the anonymous reviewers' invaluable comments.
 
 ** *Not for all models, see the paper for details.*
 
+<hr style="border: 0; height: 1px; background-color: #e0e0e0;">
+
+***Quick Start (Run in 8 lines of code)***
+
+In shell, 
+```
+pip install whisper-at
+```
+
+For Mac users, there is a known bug, please use the following workaround:
+```bash
+# install all dependencies except triton, this will break when it tries to install triton
+pip install whisper-at 
+# install whisper-at without any dependency
+pip install --no-deps whisper-at  
+```
+Then, in Python,
+```python3
+import whisper_at as whisper
+
+audio_tagging_time_resolution = 10
+model = whisper.load_model("large-v1")
+result = model.transcribe("audio.mp3", at_time_res=audio_tagging_time_resolution)
+# ASR Results
+print(result["text"])
+# Audio Tagging Results
+audio_tag_result = whisper.parse_at_label(result, language='follow_asr', top_k=5, p_threshold=-1, include_class_list=list(range(527)))
+print(audio_tag_result)
+```
+
 ## Citation
 Please cite our Interspeech 2023 paper if you find this repository useful. 
 ```  
 @inproceedings{gong_whisperat,
   author={Gong, Yuan and Khurana, Sameer and Karlinsky, Leonid and Glass, James},
   title={Whisper-AT: Noise-Robust Automatic Speech Recognizers are Also Strong Audio Event Taggers},
   year=2023,
   booktitle={Proc. Interspeech 2023}
 }
 ```
 
 ## For Applications
 
-**The best way to learn how to use Whisper-AT is this [Colab Tutorial](https://colab.research.google.com/drive/1BbOGWCMjkOlOY5PbEMGk5RomRSqMcy_Q?usp=sharing). You can skip all below if you read it.**
+**The best way to learn how to use Whisper-AT is this [[**Colab Tutorial**]](https://colab.research.google.com/drive/1BbOGWCMjkOlOY5PbEMGk5RomRSqMcy_Q?usp=sharing). You can skip all below if you read it.**
+If you don't have Google Colab access (uncommon), you can use this [[Local Notebook]](https://github.com/YuanGongND/whisper-at/blob/main/sample/whisper_at_demo.ipynb) as a substitution.
+
+<hr style="border: 0; height: 1px; background-color: #e0e0e0;">
 
 If you do not care how Whisper-AT is implemented, but just want to use it, you only need to read this section. This will be very simple.
 
 ### Step 1. Install Whisper-AT
 
 We intentionally do not any additional dependencies to the original Whisper. So if your environment can run the original Whisper, it can also run Whisper-AT.
 
 Whisper-AT can be installed simply by:
 
     pip install whisper-at
 
+For Mac users, there is a known bug, please use the following workaround:
+```bash
+# install all dependencies except triton, this will break when it tries to install triton
+pip install whisper-at 
+# install whisper-at without any dependency
+pip install --no-deps whisper-at  
+```
+
 Note that following original Whisper, it also requires the command-line tool [`ffmpeg`](https://ffmpeg.org/) to be installed on your system. Please check OpenAI Whisper repo for details.
 
 ### Step 2. Use as the Original Whisper
 
 ```python3
 # note this is whisper"_"at not whisper-at
 import whisper_at as whisper
@@ -119,15 +170,15 @@
 **Return:** A dictionary of audio tagging results.
 
 This makes the audio tagging result human-readable, in specified language. If not specified, `whisepr.parse_at_label` output label names in the same language with the ASR output.
 That's it!
 
 ## For Research
 
-If you are interested in the findings and experiments in our Interspeech paper *[Whisper-AT: Noise-Robust Automatic Speech Recognizers are Also Strong Audio Event Taggers]()*, please check this section.
+If you are interested in the findings and experiments in our Interspeech paper *[Whisper-AT: Noise-Robust Automatic Speech Recognizers are Also Strong Audio Event Taggers](https://arxiv.org/pdf/2307.03183.pdf)*, please check this section.
 We provide our code to reproduce the experiments in the paper. 
 
 The paper mainly contains two contributions:
 - First we report an interesting and surprising finding that while Whisper is very robust against real-world background sounds (e.g., music), its audio representation is actually **NOT noise-invariant**, but is instead highly correlated to non-speech sounds, indicating that Whisper recognizes speech **conditioned** on the noise type. 
 - Second, with the above finding, we build a unified audio tagging and speech recognition model Whisper-AT by freezing the backbone of Whisper, and training a novel audio tagging model called **Time and Layer-wise Transformer (TL-TR)** on top of it. With  <1% extra computational cost, Whisper-AT can recognize audio events, in addition to spoken text, in a single forward pass.
 
 <hr style="border: 0; height: 1px; background-color: #e0e0e0;">
```

### Comparing `whisper-at-0.2/whisper_at.egg-info/SOURCES.txt` & `whisper-at-0.4/whisper_at.egg-info/SOURCES.txt`

 * *Files identical despite different names*

