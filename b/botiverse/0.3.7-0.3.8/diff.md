# Comparing `tmp/botiverse-0.3.7.tar.gz` & `tmp/botiverse-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botiverse-0.3.7.tar", last modified: Mon Jul 24 17:02:45 2023, max compression
+gzip compressed data, was "botiverse-0.3.8.tar", last modified: Mon Jul 24 17:19:02 2023, max compression
```

## Comparing `botiverse-0.3.7.tar` & `botiverse-0.3.8.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:02:45.610345 botiverse-0.3.7/
--rw-r--r--   0 essam      (501) staff       (20)     1192 2023-07-24 17:02:45.610120 botiverse-0.3.7/PKG-INFO
--rw-r--r--   0 essam      (501) staff       (20)      440 2023-01-31 16:00:25.000000 botiverse-0.3.7/README.md
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:02:45.591718 botiverse-0.3.7/botiverse/
--rw-r--r--   0 essam      (501) staff       (20)       84 2023-07-24 15:57:44.000000 botiverse-0.3.7/botiverse/__init__.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:02:45.593058 botiverse-0.3.7/botiverse/bots/
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:02:45.593572 botiverse-0.3.7/botiverse/bots/BasicBot/
--rw-r--r--   0 essam      (501) staff       (20)     7769 2023-07-24 14:11:30.000000 botiverse-0.3.7/botiverse/bots/BasicBot/BasicBot.py
--rw-r--r--   0 essam      (501) staff       (20)        0 2023-01-31 14:19:10.000000 botiverse-0.3.7/botiverse/bots/BasicBot/__init__.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:02:45.593992 botiverse-0.3.7/botiverse/bots/ConverseBot/
--rw-r--r--   0 essam      (501) staff       (20)     6760 2023-07-24 15:08:00.000000 botiverse-0.3.7/botiverse/bots/ConverseBot/ConverseBot.py
--rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-10 23:47:13.000000 botiverse-0.3.7/botiverse/bots/ConverseBot/__init__.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:02:45.594680 botiverse-0.3.7/botiverse/bots/VoiceBot/
--rw-r--r--   0 essam      (501) staff       (20)     4025 2023-07-24 13:43:59.000000 botiverse-0.3.7/botiverse/bots/VoiceBot/SpeechClassifier.py
--rw-r--r--   0 essam      (501) staff       (20)     3473 2023-07-24 13:43:43.000000 botiverse-0.3.7/botiverse/bots/VoiceBot/VoiceBot.py
--rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-06 20:19:05.000000 botiverse-0.3.7/botiverse/bots/VoiceBot/__init__.py
--rw-r--r--   0 essam      (501) staff       (20)     1758 2023-07-24 13:20:58.000000 botiverse-0.3.7/botiverse/bots/VoiceBot/utils.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:02:45.595594 botiverse-0.3.7/botiverse/bots/WhizBot/
--rw-r--r--   0 essam      (501) staff       (20)     2691 2023-07-24 14:25:02.000000 botiverse-0.3.7/botiverse/bots/WhizBot/WhizBot.py
--rw-r--r--   0 essam      (501) staff       (20)     5084 2023-07-24 15:08:20.000000 botiverse-0.3.7/botiverse/bots/WhizBot/WhizBot_BERT.py
--rw-r--r--   0 essam      (501) staff       (20)     5309 2023-07-24 15:08:14.000000 botiverse-0.3.7/botiverse/bots/WhizBot/WhizBot_GRU.py
--rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-10 23:47:13.000000 botiverse-0.3.7/botiverse/bots/WhizBot/__init__.py
--rw-r--r--   0 essam      (501) staff       (20)      407 2023-07-24 16:36:12.000000 botiverse-0.3.7/botiverse/bots/__init__.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:02:45.596392 botiverse-0.3.7/botiverse/bots/basic_TODS/
--rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-06 20:16:45.000000 botiverse-0.3.7/botiverse/bots/basic_TODS/__init__.py
--rw-r--r--   0 essam      (501) staff       (20)     4076 2023-07-24 07:57:53.000000 botiverse-0.3.7/botiverse/bots/basic_TODS/basic_TODS.py
--rw-r--r--   0 essam      (501) staff       (20)     1387 2023-07-10 06:53:03.000000 botiverse-0.3.7/botiverse/bots/basic_TODS/tods_example.py
--rw-r--r--   0 essam      (501) staff       (20)     7368 2023-07-10 06:53:03.000000 botiverse-0.3.7/botiverse/bots/basic_TODS/utils.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:02:45.597088 botiverse-0.3.7/botiverse/bots/deep_TODS/
--rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-06 20:16:45.000000 botiverse-0.3.7/botiverse/bots/deep_TODS/__init__.py
--rw-r--r--   0 essam      (501) staff       (20)     5990 2023-07-24 07:57:53.000000 botiverse-0.3.7/botiverse/bots/deep_TODS/deep_TODS.py
--rw-r--r--   0 essam      (501) staff       (20)     5169 2023-07-10 06:53:03.000000 botiverse-0.3.7/botiverse/bots/deep_TODS/utils.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:02:45.597613 botiverse-0.3.7/botiverse/gui/
--rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-02 09:46:31.000000 botiverse-0.3.7/botiverse/gui/__init__.py
--rw-r--r--   0 essam      (501) staff       (20)     1004 2023-07-24 13:02:01.000000 botiverse-0.3.7/botiverse/gui/gui.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:02:45.597879 botiverse-0.3.7/botiverse/models/
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:02:45.598810 botiverse-0.3.7/botiverse/models/BERT/
--rw-r--r--   0 essam      (501) staff       (20)    11321 2023-07-10 06:53:03.000000 botiverse-0.3.7/botiverse/models/BERT/BERT.py
--rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-10 06:53:03.000000 botiverse-0.3.7/botiverse/models/BERT/__init__.py
--rw-r--r--   0 essam      (501) staff       (20)     1878 2023-07-10 06:53:03.000000 botiverse-0.3.7/botiverse/models/BERT/config.py
--rw-r--r--   0 essam      (501) staff       (20)     3282 2023-07-10 06:53:03.000000 botiverse-0.3.7/botiverse/models/BERT/utils.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:02:45.599461 botiverse-0.3.7/botiverse/models/FastSpeech1/
--rw-r--r--   0 essam      (501) staff       (20)    28410 2023-07-02 10:31:31.000000 botiverse-0.3.7/botiverse/models/FastSpeech1/FastSpeech.py
--rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-01 08:08:36.000000 botiverse-0.3.7/botiverse/models/FastSpeech1/__init__.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:02:45.599895 botiverse-0.3.7/botiverse/models/GRUClassifier/
--rw-r--r--   0 essam      (501) staff       (20)     4483 2023-07-10 23:47:13.000000 botiverse-0.3.7/botiverse/models/GRUClassifier/GRUClassifier.py
--rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-10 23:47:13.000000 botiverse-0.3.7/botiverse/models/GRUClassifier/__init__.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:02:45.600269 botiverse-0.3.7/botiverse/models/LSTM/
--rw-r--r--   0 essam      (501) staff       (20)    11718 2023-07-09 13:09:18.000000 botiverse-0.3.7/botiverse/models/LSTM/LSTM.py
--rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-03 13:16:35.000000 botiverse-0.3.7/botiverse/models/LSTM/__init__.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:02:45.600704 botiverse-0.3.7/botiverse/models/LinearClassifier/
--rw-r--r--   0 essam      (501) staff       (20)     1214 2023-07-10 23:47:13.000000 botiverse-0.3.7/botiverse/models/LinearClassifier/LinearClassifier.py
--rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-10 23:47:13.000000 botiverse-0.3.7/botiverse/models/LinearClassifier/__init__.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:02:45.601288 botiverse-0.3.7/botiverse/models/NN/
--rw-r--r--   0 essam      (501) staff       (20)    13533 2023-07-08 17:02:04.000000 botiverse-0.3.7/botiverse/models/NN/NN.py
--rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-01 08:08:27.000000 botiverse-0.3.7/botiverse/models/NN/__init__.py
--rw-r--r--   0 essam      (501) staff       (20)     1358 2023-07-07 09:30:15.000000 botiverse-0.3.7/botiverse/models/NN/utils.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:02:45.601765 botiverse-0.3.7/botiverse/models/SVM/
--rw-r--r--   0 essam      (501) staff       (20)     9087 2023-07-07 09:30:15.000000 botiverse-0.3.7/botiverse/models/SVM/SVM.py
--rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-01 08:08:33.000000 botiverse-0.3.7/botiverse/models/SVM/__init__.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:02:45.602295 botiverse-0.3.7/botiverse/models/T5Model/
--rw-r--r--   0 essam      (501) staff       (20)    30038 2023-07-19 06:34:34.000000 botiverse-0.3.7/botiverse/models/T5Model/T5Model.py
--rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-10 23:47:13.000000 botiverse-0.3.7/botiverse/models/T5Model/__init__.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:02:45.604650 botiverse-0.3.7/botiverse/models/TRIPPY/
--rw-r--r--   0 essam      (501) staff       (20)     5185 2023-07-10 23:47:13.000000 botiverse-0.3.7/botiverse/models/TRIPPY/TRIPPY.py
--rw-r--r--   0 essam      (501) staff       (20)     9192 2023-07-24 07:57:53.000000 botiverse-0.3.7/botiverse/models/TRIPPY/TRIPPY_DST.py
--rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-10 06:53:03.000000 botiverse-0.3.7/botiverse/models/TRIPPY/__init__.py
--rw-r--r--   0 essam      (501) staff       (20)     3302 2023-07-10 23:47:13.000000 botiverse-0.3.7/botiverse/models/TRIPPY/config.py
--rw-r--r--   0 essam      (501) staff       (20)    21274 2023-07-24 07:57:53.000000 botiverse-0.3.7/botiverse/models/TRIPPY/data.py
--rw-r--r--   0 essam      (501) staff       (20)     9398 2023-07-10 23:47:13.000000 botiverse-0.3.7/botiverse/models/TRIPPY/evaluate.py
--rw-r--r--   0 essam      (501) staff       (20)     4778 2023-07-10 06:53:03.000000 botiverse-0.3.7/botiverse/models/TRIPPY/infer.py
--rw-r--r--   0 essam      (501) staff       (20)     6225 2023-07-10 23:47:13.000000 botiverse-0.3.7/botiverse/models/TRIPPY/run.py
--rw-r--r--   0 essam      (501) staff       (20)     5068 2023-07-10 06:53:03.000000 botiverse-0.3.7/botiverse/models/TRIPPY/train.py
--rw-r--r--   0 essam      (501) staff       (20)    12849 2023-07-10 23:47:13.000000 botiverse-0.3.7/botiverse/models/TRIPPY/utils.py
--rw-r--r--   0 essam      (501) staff       (20)      559 2023-07-10 23:47:13.000000 botiverse-0.3.7/botiverse/models/__init__.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:02:45.604904 botiverse-0.3.7/botiverse/preprocessors/
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:02:45.605467 botiverse-0.3.7/botiverse/preprocessors/BertEmbeddings/
--rw-r--r--   0 essam      (501) staff       (20)     3958 2023-07-24 06:57:48.000000 botiverse-0.3.7/botiverse/preprocessors/BertEmbeddings/BertEmbeddings.py
--rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-06 20:19:05.000000 botiverse-0.3.7/botiverse/preprocessors/BertEmbeddings/__init__.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:02:45.605895 botiverse-0.3.7/botiverse/preprocessors/BoW/
--rw-r--r--   0 essam      (501) staff       (20)     1671 2023-07-08 15:48:43.000000 botiverse-0.3.7/botiverse/preprocessors/BoW/BoW.py
--rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-08 15:48:15.000000 botiverse-0.3.7/botiverse/preprocessors/BoW/__init__.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:02:45.606306 botiverse-0.3.7/botiverse/preprocessors/Frequency/
--rw-r--r--   0 essam      (501) staff       (20)     9916 2023-07-09 10:07:24.000000 botiverse-0.3.7/botiverse/preprocessors/Frequency/Frequency.py
--rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-04 18:04:01.000000 botiverse-0.3.7/botiverse/preprocessors/Frequency/__init__.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:02:45.606680 botiverse-0.3.7/botiverse/preprocessors/GloVe/
--rw-r--r--   0 essam      (501) staff       (20)     2995 2023-07-04 19:50:45.000000 botiverse-0.3.7/botiverse/preprocessors/GloVe/GloVe.py
--rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-03 13:47:23.000000 botiverse-0.3.7/botiverse/preprocessors/GloVe/__init__.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:02:45.590322 botiverse-0.3.7/botiverse/preprocessors/Special/
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:02:45.607209 botiverse-0.3.7/botiverse/preprocessors/Special/ConverseBot_Preprocessor/
--rw-r--r--   0 essam      (501) staff       (20)     5317 2023-07-23 14:29:14.000000 botiverse-0.3.7/botiverse/preprocessors/Special/ConverseBot_Preprocessor/ConverseBot_Preprocessor.py
--rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-10 23:47:13.000000 botiverse-0.3.7/botiverse/preprocessors/Special/ConverseBot_Preprocessor/__init__.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:02:45.607735 botiverse-0.3.7/botiverse/preprocessors/Special/WhizBot_BERT_Preprocessor/
--rw-r--r--   0 essam      (501) staff       (20)     5445 2023-07-10 23:47:13.000000 botiverse-0.3.7/botiverse/preprocessors/Special/WhizBot_BERT_Preprocessor/WhizBot_BERT_Preprocessor.py
--rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-10 23:47:13.000000 botiverse-0.3.7/botiverse/preprocessors/Special/WhizBot_BERT_Preprocessor/__init__.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:02:45.608174 botiverse-0.3.7/botiverse/preprocessors/Special/WhizBot_GRU_Preprocessor/
--rw-r--r--   0 essam      (501) staff       (20)     5515 2023-07-10 23:47:13.000000 botiverse-0.3.7/botiverse/preprocessors/Special/WhizBot_GRU_Preprocessor/WhizBot_GRU_Preprocessor.py
--rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-10 23:47:13.000000 botiverse-0.3.7/botiverse/preprocessors/Special/WhizBot_GRU_Preprocessor/__init__.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:02:45.608590 botiverse-0.3.7/botiverse/preprocessors/TF_IDF/
--rw-r--r--   0 essam      (501) staff       (20)     2493 2023-07-08 19:06:06.000000 botiverse-0.3.7/botiverse/preprocessors/TF_IDF/TF_IDF.py
--rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-03 13:47:16.000000 botiverse-0.3.7/botiverse/preprocessors/TF_IDF/__init__.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:02:45.608985 botiverse-0.3.7/botiverse/preprocessors/TF_IDF_GLOVE/
--rw-r--r--   0 essam      (501) staff       (20)     2763 2023-07-04 19:53:43.000000 botiverse-0.3.7/botiverse/preprocessors/TF_IDF_GLOVE/TF_IDF_GLOVE.py
--rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-03 13:47:12.000000 botiverse-0.3.7/botiverse/preprocessors/TF_IDF_GLOVE/__init__.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:02:45.609404 botiverse-0.3.7/botiverse/preprocessors/Vocalize/
--rw-r--r--   0 essam      (501) staff       (20)     5322 2023-07-07 09:30:15.000000 botiverse-0.3.7/botiverse/preprocessors/Vocalize/Vocalize.py
--rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-04 17:46:59.000000 botiverse-0.3.7/botiverse/preprocessors/Vocalize/__init__.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:02:45.609794 botiverse-0.3.7/botiverse/preprocessors/Wav2Vec/
--rw-r--r--   0 essam      (501) staff       (20)     6846 2023-07-24 07:58:06.000000 botiverse-0.3.7/botiverse/preprocessors/Wav2Vec/Wav2Vec.py
--rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-03 13:47:08.000000 botiverse-0.3.7/botiverse/preprocessors/Wav2Vec/__init__.py
--rw-r--r--   0 essam      (501) staff       (20)      584 2023-07-24 06:37:23.000000 botiverse-0.3.7/botiverse/preprocessors/__init__.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:02:45.592817 botiverse-0.3.7/botiverse.egg-info/
--rw-r--r--   0 essam      (501) staff       (20)     1192 2023-07-24 17:02:45.000000 botiverse-0.3.7/botiverse.egg-info/PKG-INFO
--rw-r--r--   0 essam      (501) staff       (20)     3267 2023-07-24 17:02:45.000000 botiverse-0.3.7/botiverse.egg-info/SOURCES.txt
--rw-r--r--   0 essam      (501) staff       (20)        1 2023-07-24 17:02:45.000000 botiverse-0.3.7/botiverse.egg-info/dependency_links.txt
--rw-r--r--   0 essam      (501) staff       (20)       12 2023-07-24 17:02:45.000000 botiverse-0.3.7/botiverse.egg-info/requires.txt
--rw-r--r--   0 essam      (501) staff       (20)       10 2023-07-24 17:02:45.000000 botiverse-0.3.7/botiverse.egg-info/top_level.txt
--rw-r--r--   0 essam      (501) staff       (20)       38 2023-07-24 17:02:45.610458 botiverse-0.3.7/setup.cfg
--rw-r--r--   0 essam      (501) staff       (20)     3642 2023-07-24 17:02:30.000000 botiverse-0.3.7/setup.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:19:02.639289 botiverse-0.3.8/
+-rw-r--r--   0 essam      (501) staff       (20)     1192 2023-07-24 17:19:02.639055 botiverse-0.3.8/PKG-INFO
+-rw-r--r--   0 essam      (501) staff       (20)      440 2023-01-31 16:00:25.000000 botiverse-0.3.8/README.md
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:19:02.606219 botiverse-0.3.8/botiverse/
+-rw-r--r--   0 essam      (501) staff       (20)       84 2023-07-24 15:57:44.000000 botiverse-0.3.8/botiverse/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:19:02.607508 botiverse-0.3.8/botiverse/bots/
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:19:02.608549 botiverse-0.3.8/botiverse/bots/BasicBot/
+-rw-r--r--   0 essam      (501) staff       (20)     7769 2023-07-24 14:11:30.000000 botiverse-0.3.8/botiverse/bots/BasicBot/BasicBot.py
+-rw-r--r--   0 essam      (501) staff       (20)        0 2023-01-31 14:19:10.000000 botiverse-0.3.8/botiverse/bots/BasicBot/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:19:02.609186 botiverse-0.3.8/botiverse/bots/ConverseBot/
+-rw-r--r--   0 essam      (501) staff       (20)     6760 2023-07-24 15:08:00.000000 botiverse-0.3.8/botiverse/bots/ConverseBot/ConverseBot.py
+-rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-10 23:47:13.000000 botiverse-0.3.8/botiverse/bots/ConverseBot/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:19:02.610386 botiverse-0.3.8/botiverse/bots/VoiceBot/
+-rw-r--r--   0 essam      (501) staff       (20)     4025 2023-07-24 13:43:59.000000 botiverse-0.3.8/botiverse/bots/VoiceBot/SpeechClassifier.py
+-rw-r--r--   0 essam      (501) staff       (20)     3473 2023-07-24 13:43:43.000000 botiverse-0.3.8/botiverse/bots/VoiceBot/VoiceBot.py
+-rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-06 20:19:05.000000 botiverse-0.3.8/botiverse/bots/VoiceBot/__init__.py
+-rw-r--r--   0 essam      (501) staff       (20)     1758 2023-07-24 13:20:58.000000 botiverse-0.3.8/botiverse/bots/VoiceBot/utils.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:19:02.612172 botiverse-0.3.8/botiverse/bots/WhizBot/
+-rw-r--r--   0 essam      (501) staff       (20)     2691 2023-07-24 14:25:02.000000 botiverse-0.3.8/botiverse/bots/WhizBot/WhizBot.py
+-rw-r--r--   0 essam      (501) staff       (20)     5084 2023-07-24 15:08:20.000000 botiverse-0.3.8/botiverse/bots/WhizBot/WhizBot_BERT.py
+-rw-r--r--   0 essam      (501) staff       (20)     5309 2023-07-24 15:08:14.000000 botiverse-0.3.8/botiverse/bots/WhizBot/WhizBot_GRU.py
+-rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-10 23:47:13.000000 botiverse-0.3.8/botiverse/bots/WhizBot/__init__.py
+-rw-r--r--   0 essam      (501) staff       (20)      407 2023-07-24 16:36:12.000000 botiverse-0.3.8/botiverse/bots/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:19:02.613180 botiverse-0.3.8/botiverse/bots/basic_TODS/
+-rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-06 20:16:45.000000 botiverse-0.3.8/botiverse/bots/basic_TODS/__init__.py
+-rw-r--r--   0 essam      (501) staff       (20)     4076 2023-07-24 07:57:53.000000 botiverse-0.3.8/botiverse/bots/basic_TODS/basic_TODS.py
+-rw-r--r--   0 essam      (501) staff       (20)     1387 2023-07-10 06:53:03.000000 botiverse-0.3.8/botiverse/bots/basic_TODS/tods_example.py
+-rw-r--r--   0 essam      (501) staff       (20)     7368 2023-07-10 06:53:03.000000 botiverse-0.3.8/botiverse/bots/basic_TODS/utils.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:19:02.619221 botiverse-0.3.8/botiverse/bots/deep_TODS/
+-rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-06 20:16:45.000000 botiverse-0.3.8/botiverse/bots/deep_TODS/__init__.py
+-rw-r--r--   0 essam      (501) staff       (20)     5990 2023-07-24 07:57:53.000000 botiverse-0.3.8/botiverse/bots/deep_TODS/deep_TODS.py
+-rw-r--r--   0 essam      (501) staff       (20)     5169 2023-07-10 06:53:03.000000 botiverse-0.3.8/botiverse/bots/deep_TODS/utils.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:19:02.619704 botiverse-0.3.8/botiverse/gui/
+-rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-02 09:46:31.000000 botiverse-0.3.8/botiverse/gui/__init__.py
+-rw-r--r--   0 essam      (501) staff       (20)     1004 2023-07-24 13:02:01.000000 botiverse-0.3.8/botiverse/gui/gui.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:19:02.620271 botiverse-0.3.8/botiverse/models/
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:19:02.621358 botiverse-0.3.8/botiverse/models/BERT/
+-rw-r--r--   0 essam      (501) staff       (20)    11321 2023-07-10 06:53:03.000000 botiverse-0.3.8/botiverse/models/BERT/BERT.py
+-rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-10 06:53:03.000000 botiverse-0.3.8/botiverse/models/BERT/__init__.py
+-rw-r--r--   0 essam      (501) staff       (20)     1878 2023-07-10 06:53:03.000000 botiverse-0.3.8/botiverse/models/BERT/config.py
+-rw-r--r--   0 essam      (501) staff       (20)     3282 2023-07-10 06:53:03.000000 botiverse-0.3.8/botiverse/models/BERT/utils.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:19:02.622832 botiverse-0.3.8/botiverse/models/FastSpeech1/
+-rw-r--r--   0 essam      (501) staff       (20)    28410 2023-07-02 10:31:31.000000 botiverse-0.3.8/botiverse/models/FastSpeech1/FastSpeech.py
+-rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-01 08:08:36.000000 botiverse-0.3.8/botiverse/models/FastSpeech1/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:19:02.623710 botiverse-0.3.8/botiverse/models/GRUClassifier/
+-rw-r--r--   0 essam      (501) staff       (20)     4483 2023-07-10 23:47:13.000000 botiverse-0.3.8/botiverse/models/GRUClassifier/GRUClassifier.py
+-rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-10 23:47:13.000000 botiverse-0.3.8/botiverse/models/GRUClassifier/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:19:02.624422 botiverse-0.3.8/botiverse/models/LSTM/
+-rw-r--r--   0 essam      (501) staff       (20)    11718 2023-07-09 13:09:18.000000 botiverse-0.3.8/botiverse/models/LSTM/LSTM.py
+-rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-03 13:16:35.000000 botiverse-0.3.8/botiverse/models/LSTM/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:19:02.625002 botiverse-0.3.8/botiverse/models/LinearClassifier/
+-rw-r--r--   0 essam      (501) staff       (20)     1214 2023-07-10 23:47:13.000000 botiverse-0.3.8/botiverse/models/LinearClassifier/LinearClassifier.py
+-rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-10 23:47:13.000000 botiverse-0.3.8/botiverse/models/LinearClassifier/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:19:02.625934 botiverse-0.3.8/botiverse/models/NN/
+-rw-r--r--   0 essam      (501) staff       (20)    13533 2023-07-08 17:02:04.000000 botiverse-0.3.8/botiverse/models/NN/NN.py
+-rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-01 08:08:27.000000 botiverse-0.3.8/botiverse/models/NN/__init__.py
+-rw-r--r--   0 essam      (501) staff       (20)     1358 2023-07-07 09:30:15.000000 botiverse-0.3.8/botiverse/models/NN/utils.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:19:02.626724 botiverse-0.3.8/botiverse/models/SVM/
+-rw-r--r--   0 essam      (501) staff       (20)     9087 2023-07-07 09:30:15.000000 botiverse-0.3.8/botiverse/models/SVM/SVM.py
+-rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-01 08:08:33.000000 botiverse-0.3.8/botiverse/models/SVM/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:19:02.627486 botiverse-0.3.8/botiverse/models/T5Model/
+-rw-r--r--   0 essam      (501) staff       (20)    30038 2023-07-19 06:34:34.000000 botiverse-0.3.8/botiverse/models/T5Model/T5Model.py
+-rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-10 23:47:13.000000 botiverse-0.3.8/botiverse/models/T5Model/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:19:02.631468 botiverse-0.3.8/botiverse/models/TRIPPY/
+-rw-r--r--   0 essam      (501) staff       (20)     5185 2023-07-10 23:47:13.000000 botiverse-0.3.8/botiverse/models/TRIPPY/TRIPPY.py
+-rw-r--r--   0 essam      (501) staff       (20)     9192 2023-07-24 07:57:53.000000 botiverse-0.3.8/botiverse/models/TRIPPY/TRIPPY_DST.py
+-rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-10 06:53:03.000000 botiverse-0.3.8/botiverse/models/TRIPPY/__init__.py
+-rw-r--r--   0 essam      (501) staff       (20)     3302 2023-07-10 23:47:13.000000 botiverse-0.3.8/botiverse/models/TRIPPY/config.py
+-rw-r--r--   0 essam      (501) staff       (20)    21274 2023-07-24 07:57:53.000000 botiverse-0.3.8/botiverse/models/TRIPPY/data.py
+-rw-r--r--   0 essam      (501) staff       (20)     9398 2023-07-10 23:47:13.000000 botiverse-0.3.8/botiverse/models/TRIPPY/evaluate.py
+-rw-r--r--   0 essam      (501) staff       (20)     4778 2023-07-10 06:53:03.000000 botiverse-0.3.8/botiverse/models/TRIPPY/infer.py
+-rw-r--r--   0 essam      (501) staff       (20)     6225 2023-07-10 23:47:13.000000 botiverse-0.3.8/botiverse/models/TRIPPY/run.py
+-rw-r--r--   0 essam      (501) staff       (20)     5068 2023-07-10 06:53:03.000000 botiverse-0.3.8/botiverse/models/TRIPPY/train.py
+-rw-r--r--   0 essam      (501) staff       (20)    12849 2023-07-10 23:47:13.000000 botiverse-0.3.8/botiverse/models/TRIPPY/utils.py
+-rw-r--r--   0 essam      (501) staff       (20)      559 2023-07-10 23:47:13.000000 botiverse-0.3.8/botiverse/models/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:19:02.631840 botiverse-0.3.8/botiverse/preprocessors/
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:19:02.632709 botiverse-0.3.8/botiverse/preprocessors/BertEmbeddings/
+-rw-r--r--   0 essam      (501) staff       (20)     3958 2023-07-24 06:57:48.000000 botiverse-0.3.8/botiverse/preprocessors/BertEmbeddings/BertEmbeddings.py
+-rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-06 20:19:05.000000 botiverse-0.3.8/botiverse/preprocessors/BertEmbeddings/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:19:02.633222 botiverse-0.3.8/botiverse/preprocessors/BoW/
+-rw-r--r--   0 essam      (501) staff       (20)     1671 2023-07-08 15:48:43.000000 botiverse-0.3.8/botiverse/preprocessors/BoW/BoW.py
+-rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-08 15:48:15.000000 botiverse-0.3.8/botiverse/preprocessors/BoW/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:19:02.633875 botiverse-0.3.8/botiverse/preprocessors/Frequency/
+-rw-r--r--   0 essam      (501) staff       (20)     9916 2023-07-09 10:07:24.000000 botiverse-0.3.8/botiverse/preprocessors/Frequency/Frequency.py
+-rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-04 18:04:01.000000 botiverse-0.3.8/botiverse/preprocessors/Frequency/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:19:02.634550 botiverse-0.3.8/botiverse/preprocessors/GloVe/
+-rw-r--r--   0 essam      (501) staff       (20)     2995 2023-07-04 19:50:45.000000 botiverse-0.3.8/botiverse/preprocessors/GloVe/GloVe.py
+-rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-03 13:47:23.000000 botiverse-0.3.8/botiverse/preprocessors/GloVe/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:19:02.604341 botiverse-0.3.8/botiverse/preprocessors/Special/
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:19:02.635118 botiverse-0.3.8/botiverse/preprocessors/Special/ConverseBot_Preprocessor/
+-rw-r--r--   0 essam      (501) staff       (20)     5317 2023-07-23 14:29:14.000000 botiverse-0.3.8/botiverse/preprocessors/Special/ConverseBot_Preprocessor/ConverseBot_Preprocessor.py
+-rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-10 23:47:13.000000 botiverse-0.3.8/botiverse/preprocessors/Special/ConverseBot_Preprocessor/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:19:02.635682 botiverse-0.3.8/botiverse/preprocessors/Special/WhizBot_BERT_Preprocessor/
+-rw-r--r--   0 essam      (501) staff       (20)     5445 2023-07-10 23:47:13.000000 botiverse-0.3.8/botiverse/preprocessors/Special/WhizBot_BERT_Preprocessor/WhizBot_BERT_Preprocessor.py
+-rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-10 23:47:13.000000 botiverse-0.3.8/botiverse/preprocessors/Special/WhizBot_BERT_Preprocessor/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:19:02.636246 botiverse-0.3.8/botiverse/preprocessors/Special/WhizBot_GRU_Preprocessor/
+-rw-r--r--   0 essam      (501) staff       (20)     5515 2023-07-10 23:47:13.000000 botiverse-0.3.8/botiverse/preprocessors/Special/WhizBot_GRU_Preprocessor/WhizBot_GRU_Preprocessor.py
+-rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-10 23:47:13.000000 botiverse-0.3.8/botiverse/preprocessors/Special/WhizBot_GRU_Preprocessor/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:19:02.636752 botiverse-0.3.8/botiverse/preprocessors/TF_IDF/
+-rw-r--r--   0 essam      (501) staff       (20)     2493 2023-07-08 19:06:06.000000 botiverse-0.3.8/botiverse/preprocessors/TF_IDF/TF_IDF.py
+-rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-03 13:47:16.000000 botiverse-0.3.8/botiverse/preprocessors/TF_IDF/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:19:02.637329 botiverse-0.3.8/botiverse/preprocessors/TF_IDF_GLOVE/
+-rw-r--r--   0 essam      (501) staff       (20)     2763 2023-07-04 19:53:43.000000 botiverse-0.3.8/botiverse/preprocessors/TF_IDF_GLOVE/TF_IDF_GLOVE.py
+-rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-03 13:47:12.000000 botiverse-0.3.8/botiverse/preprocessors/TF_IDF_GLOVE/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:19:02.637908 botiverse-0.3.8/botiverse/preprocessors/Vocalize/
+-rw-r--r--   0 essam      (501) staff       (20)     5322 2023-07-07 09:30:15.000000 botiverse-0.3.8/botiverse/preprocessors/Vocalize/Vocalize.py
+-rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-04 17:46:59.000000 botiverse-0.3.8/botiverse/preprocessors/Vocalize/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:19:02.638724 botiverse-0.3.8/botiverse/preprocessors/Wav2Vec/
+-rw-r--r--   0 essam      (501) staff       (20)     6846 2023-07-24 07:58:06.000000 botiverse-0.3.8/botiverse/preprocessors/Wav2Vec/Wav2Vec.py
+-rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-03 13:47:08.000000 botiverse-0.3.8/botiverse/preprocessors/Wav2Vec/__init__.py
+-rw-r--r--   0 essam      (501) staff       (20)      584 2023-07-24 06:37:23.000000 botiverse-0.3.8/botiverse/preprocessors/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 17:19:02.607322 botiverse-0.3.8/botiverse.egg-info/
+-rw-r--r--   0 essam      (501) staff       (20)     1192 2023-07-24 17:19:02.000000 botiverse-0.3.8/botiverse.egg-info/PKG-INFO
+-rw-r--r--   0 essam      (501) staff       (20)     3267 2023-07-24 17:19:02.000000 botiverse-0.3.8/botiverse.egg-info/SOURCES.txt
+-rw-r--r--   0 essam      (501) staff       (20)        1 2023-07-24 17:19:02.000000 botiverse-0.3.8/botiverse.egg-info/dependency_links.txt
+-rw-r--r--   0 essam      (501) staff       (20)       12 2023-07-24 17:19:02.000000 botiverse-0.3.8/botiverse.egg-info/requires.txt
+-rw-r--r--   0 essam      (501) staff       (20)       10 2023-07-24 17:19:02.000000 botiverse-0.3.8/botiverse.egg-info/top_level.txt
+-rw-r--r--   0 essam      (501) staff       (20)       38 2023-07-24 17:19:02.639365 botiverse-0.3.8/setup.cfg
+-rw-r--r--   0 essam      (501) staff       (20)     3698 2023-07-24 17:18:42.000000 botiverse-0.3.8/setup.py
```

### Comparing `botiverse-0.3.7/PKG-INFO` & `botiverse-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botiverse
-Version: 0.3.7
+Version: 0.3.8
 Summary: botiverse is a chatbot library that offers a high-level API to
 Home-page: https://botiverse.readthedocs.io/
 Author: Essam W., Mohamed Saad, Yousef Atef, Karim Taha
 Author-email: essamwisam@outlook.com
 License: GPLv3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `botiverse-0.3.7/botiverse/bots/BasicBot/BasicBot.py` & `botiverse-0.3.8/botiverse/bots/BasicBot/BasicBot.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/botiverse/bots/ConverseBot/ConverseBot.py` & `botiverse-0.3.8/botiverse/bots/ConverseBot/ConverseBot.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/botiverse/bots/VoiceBot/SpeechClassifier.py` & `botiverse-0.3.8/botiverse/bots/VoiceBot/SpeechClassifier.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/botiverse/bots/VoiceBot/VoiceBot.py` & `botiverse-0.3.8/botiverse/bots/VoiceBot/VoiceBot.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/botiverse/bots/VoiceBot/utils.py` & `botiverse-0.3.8/botiverse/bots/VoiceBot/utils.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/botiverse/bots/WhizBot/WhizBot.py` & `botiverse-0.3.8/botiverse/bots/WhizBot/WhizBot.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/botiverse/bots/WhizBot/WhizBot_BERT.py` & `botiverse-0.3.8/botiverse/bots/WhizBot/WhizBot_BERT.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/botiverse/bots/WhizBot/WhizBot_GRU.py` & `botiverse-0.3.8/botiverse/bots/WhizBot/WhizBot_GRU.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/botiverse/bots/basic_TODS/basic_TODS.py` & `botiverse-0.3.8/botiverse/bots/basic_TODS/basic_TODS.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/botiverse/bots/basic_TODS/tods_example.py` & `botiverse-0.3.8/botiverse/bots/basic_TODS/tods_example.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/botiverse/bots/basic_TODS/utils.py` & `botiverse-0.3.8/botiverse/bots/basic_TODS/utils.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/botiverse/bots/deep_TODS/deep_TODS.py` & `botiverse-0.3.8/botiverse/bots/deep_TODS/deep_TODS.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/botiverse/bots/deep_TODS/utils.py` & `botiverse-0.3.8/botiverse/bots/deep_TODS/utils.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/botiverse/gui/gui.py` & `botiverse-0.3.8/botiverse/gui/gui.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/botiverse/models/BERT/BERT.py` & `botiverse-0.3.8/botiverse/models/BERT/BERT.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/botiverse/models/BERT/config.py` & `botiverse-0.3.8/botiverse/models/BERT/config.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/botiverse/models/BERT/utils.py` & `botiverse-0.3.8/botiverse/models/BERT/utils.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/botiverse/models/FastSpeech1/FastSpeech.py` & `botiverse-0.3.8/botiverse/models/FastSpeech1/FastSpeech.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/botiverse/models/GRUClassifier/GRUClassifier.py` & `botiverse-0.3.8/botiverse/models/GRUClassifier/GRUClassifier.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/botiverse/models/LSTM/LSTM.py` & `botiverse-0.3.8/botiverse/models/LSTM/LSTM.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/botiverse/models/LinearClassifier/LinearClassifier.py` & `botiverse-0.3.8/botiverse/models/LinearClassifier/LinearClassifier.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/botiverse/models/NN/NN.py` & `botiverse-0.3.8/botiverse/models/NN/NN.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/botiverse/models/NN/utils.py` & `botiverse-0.3.8/botiverse/models/NN/utils.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/botiverse/models/SVM/SVM.py` & `botiverse-0.3.8/botiverse/models/SVM/SVM.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/botiverse/models/T5Model/T5Model.py` & `botiverse-0.3.8/botiverse/models/T5Model/T5Model.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/botiverse/models/TRIPPY/TRIPPY.py` & `botiverse-0.3.8/botiverse/models/TRIPPY/TRIPPY.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/botiverse/models/TRIPPY/TRIPPY_DST.py` & `botiverse-0.3.8/botiverse/models/TRIPPY/TRIPPY_DST.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/botiverse/models/TRIPPY/config.py` & `botiverse-0.3.8/botiverse/models/TRIPPY/config.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/botiverse/models/TRIPPY/data.py` & `botiverse-0.3.8/botiverse/models/TRIPPY/data.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/botiverse/models/TRIPPY/evaluate.py` & `botiverse-0.3.8/botiverse/models/TRIPPY/evaluate.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/botiverse/models/TRIPPY/infer.py` & `botiverse-0.3.8/botiverse/models/TRIPPY/infer.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/botiverse/models/TRIPPY/run.py` & `botiverse-0.3.8/botiverse/models/TRIPPY/run.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/botiverse/models/TRIPPY/train.py` & `botiverse-0.3.8/botiverse/models/TRIPPY/train.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/botiverse/models/TRIPPY/utils.py` & `botiverse-0.3.8/botiverse/models/TRIPPY/utils.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/botiverse/models/__init__.py` & `botiverse-0.3.8/botiverse/models/__init__.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/botiverse/preprocessors/BertEmbeddings/BertEmbeddings.py` & `botiverse-0.3.8/botiverse/preprocessors/BertEmbeddings/BertEmbeddings.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/botiverse/preprocessors/BoW/BoW.py` & `botiverse-0.3.8/botiverse/preprocessors/BoW/BoW.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/botiverse/preprocessors/Frequency/Frequency.py` & `botiverse-0.3.8/botiverse/preprocessors/Frequency/Frequency.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/botiverse/preprocessors/GloVe/GloVe.py` & `botiverse-0.3.8/botiverse/preprocessors/GloVe/GloVe.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/botiverse/preprocessors/Special/ConverseBot_Preprocessor/ConverseBot_Preprocessor.py` & `botiverse-0.3.8/botiverse/preprocessors/Special/ConverseBot_Preprocessor/ConverseBot_Preprocessor.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/botiverse/preprocessors/Special/WhizBot_BERT_Preprocessor/WhizBot_BERT_Preprocessor.py` & `botiverse-0.3.8/botiverse/preprocessors/Special/WhizBot_BERT_Preprocessor/WhizBot_BERT_Preprocessor.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/botiverse/preprocessors/Special/WhizBot_GRU_Preprocessor/WhizBot_GRU_Preprocessor.py` & `botiverse-0.3.8/botiverse/preprocessors/Special/WhizBot_GRU_Preprocessor/WhizBot_GRU_Preprocessor.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/botiverse/preprocessors/TF_IDF/TF_IDF.py` & `botiverse-0.3.8/botiverse/preprocessors/TF_IDF/TF_IDF.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/botiverse/preprocessors/TF_IDF_GLOVE/TF_IDF_GLOVE.py` & `botiverse-0.3.8/botiverse/preprocessors/TF_IDF_GLOVE/TF_IDF_GLOVE.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/botiverse/preprocessors/Vocalize/Vocalize.py` & `botiverse-0.3.8/botiverse/preprocessors/Vocalize/Vocalize.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/botiverse/preprocessors/Wav2Vec/Wav2Vec.py` & `botiverse-0.3.8/botiverse/preprocessors/Wav2Vec/Wav2Vec.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/botiverse/preprocessors/__init__.py` & `botiverse-0.3.8/botiverse/preprocessors/__init__.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/botiverse.egg-info/PKG-INFO` & `botiverse-0.3.8/botiverse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botiverse
-Version: 0.3.7
+Version: 0.3.8
 Summary: botiverse is a chatbot library that offers a high-level API to
 Home-page: https://botiverse.readthedocs.io/
 Author: Essam W., Mohamed Saad, Yousef Atef, Karim Taha
 Author-email: essamwisam@outlook.com
 License: GPLv3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `botiverse-0.3.7/botiverse.egg-info/SOURCES.txt` & `botiverse-0.3.8/botiverse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.7/setup.py` & `botiverse-0.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     readme = f.read()
 
 # This call to setup() does all the work
 setup(
     name="botiverse",
-    version="0.3.7",
+    version="0.3.8",
     description='''botiverse is a chatbot library that offers a high-level API to
     access a diverse set of chatbot models''',
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://botiverse.readthedocs.io/",
     author="Essam W., Mohamed Saad, Yousef Atef, Karim Taha",
     author_email="essamwisam@outlook.com",
@@ -77,14 +77,15 @@
               "botiverse.preprocessors.Special.WhizBot_GRU_Preprocessor",
               "botiverse.preprocessors.GloVe",    
               "botiverse.preprocessors.TF_IDF",
               "botiverse.preprocessors.TF_IDF_GLOVE",
               "botiverse.preprocessors.Vocalize",
               "botiverse.preprocessors.Wav2Vec",
               ],
+    package_data={'botiverse/models/TRIPPY':['*.txt']},
     include_package_data=True,
     install_requires=["numpy", "torch"]            # just as was in requirements.txt
 )
 
 
 # Steps to upload to PyPI
 # 0 - Increment the version number in setup.py
```

