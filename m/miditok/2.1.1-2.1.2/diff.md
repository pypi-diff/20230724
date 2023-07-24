# Comparing `tmp/miditok-2.1.1.tar.gz` & `tmp/miditok-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miditok-2.1.1.tar", last modified: Thu Jul  6 13:22:48 2023, max compression
+gzip compressed data, was "miditok-2.1.2.tar", last modified: Mon Jul 24 18:17:36 2023, max compression
```

## Comparing `miditok-2.1.1.tar` & `miditok-2.1.2.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:22:48.044588 miditok-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 13:22:37.000000 miditok-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-07-06 13:22:48.044588 miditok-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-07-06 13:22:37.000000 miditok-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:22:48.040588 miditok-2.1.1/miditok/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-06 13:22:37.000000 miditok-2.1.1/miditok/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16493 2023-07-06 13:22:37.000000 miditok-2.1.1/miditok/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    14950 2023-07-06 13:22:37.000000 miditok-2.1.1/miditok/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:22:48.044588 miditok-2.1.1/miditok/data_augmentation/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-06 13:22:37.000000 miditok-2.1.1/miditok/data_augmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23902 2023-07-06 13:22:37.000000 miditok-2.1.1/miditok/data_augmentation/data_augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    73315 2023-07-06 13:22:37.000000 miditok-2.1.1/miditok/midi_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:22:48.044588 miditok-2.1.1/miditok/tokenizations/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-06 13:22:37.000000 miditok-2.1.1/miditok/tokenizations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22611 2023-07-06 13:22:37.000000 miditok-2.1.1/miditok/tokenizations/cp_word.py
--rw-r--r--   0 runner    (1001) docker     (123)    17837 2023-07-06 13:22:37.000000 miditok-2.1.1/miditok/tokenizations/midi_like.py
--rw-r--r--   0 runner    (1001) docker     (123)    22309 2023-07-06 13:22:37.000000 miditok-2.1.1/miditok/tokenizations/mmm.py
--rw-r--r--   0 runner    (1001) docker     (123)    23063 2023-07-06 13:22:37.000000 miditok-2.1.1/miditok/tokenizations/mumidi.py
--rw-r--r--   0 runner    (1001) docker     (123)    20743 2023-07-06 13:22:37.000000 miditok-2.1.1/miditok/tokenizations/octuple.py
--rw-r--r--   0 runner    (1001) docker     (123)    11982 2023-07-06 13:22:37.000000 miditok-2.1.1/miditok/tokenizations/octuple_mono.py
--rw-r--r--   0 runner    (1001) docker     (123)    16146 2023-07-06 13:22:37.000000 miditok-2.1.1/miditok/tokenizations/remi.py
--rw-r--r--   0 runner    (1001) docker     (123)    26784 2023-07-06 13:22:37.000000 miditok-2.1.1/miditok/tokenizations/remi_plus.py
--rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-07-06 13:22:37.000000 miditok-2.1.1/miditok/tokenizations/structured.py
--rw-r--r--   0 runner    (1001) docker     (123)    20996 2023-07-06 13:22:37.000000 miditok-2.1.1/miditok/tokenizations/tsd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:22:48.044588 miditok-2.1.1/miditok/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-06 13:22:37.000000 miditok-2.1.1/miditok/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15771 2023-07-06 13:22:37.000000 miditok-2.1.1/miditok/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:22:48.044588 miditok-2.1.1/miditok.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-07-06 13:22:48.000000 miditok-2.1.1/miditok.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-06 13:22:48.000000 miditok-2.1.1/miditok.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 13:22:48.000000 miditok-2.1.1/miditok.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-06 13:22:48.000000 miditok-2.1.1/miditok.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 13:22:48.000000 miditok-2.1.1/miditok.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 13:22:48.044588 miditok-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-06 13:22:37.000000 miditok-2.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:22:48.044588 miditok-2.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-07-06 13:22:37.000000 miditok-2.1.1/tests/test_bpe.py
--rw-r--r--   0 runner    (1001) docker     (123)    11182 2023-07-06 13:22:37.000000 miditok-2.1.1/tests/test_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     8316 2023-07-06 13:22:37.000000 miditok-2.1.1/tests/test_multitrack.py
--rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-07-06 13:22:37.000000 miditok-2.1.1/tests/test_one_track.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-06 13:22:37.000000 miditok-2.1.1/tests/test_saving_loading_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-06 13:22:37.000000 miditok-2.1.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-07-06 13:22:37.000000 miditok-2.1.1/tests/tests_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:17:36.077942 miditok-2.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-24 18:17:20.000000 miditok-2.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-07-24 18:17:36.077942 miditok-2.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-07-24 18:17:20.000000 miditok-2.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:17:36.073942 miditok-2.1.2/miditok/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-24 18:17:20.000000 miditok-2.1.2/miditok/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16493 2023-07-24 18:17:20.000000 miditok-2.1.2/miditok/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14950 2023-07-24 18:17:20.000000 miditok-2.1.2/miditok/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:17:36.073942 miditok-2.1.2/miditok/data_augmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-24 18:17:20.000000 miditok-2.1.2/miditok/data_augmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23930 2023-07-24 18:17:20.000000 miditok-2.1.2/miditok/data_augmentation/data_augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76693 2023-07-24 18:17:20.000000 miditok-2.1.2/miditok/midi_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:17:36.077942 miditok-2.1.2/miditok/tokenizations/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-24 18:17:20.000000 miditok-2.1.2/miditok/tokenizations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22751 2023-07-24 18:17:20.000000 miditok-2.1.2/miditok/tokenizations/cp_word.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17978 2023-07-24 18:17:20.000000 miditok-2.1.2/miditok/tokenizations/midi_like.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22279 2023-07-24 18:17:20.000000 miditok-2.1.2/miditok/tokenizations/mmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22628 2023-07-24 18:17:20.000000 miditok-2.1.2/miditok/tokenizations/mumidi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19855 2023-07-24 18:17:20.000000 miditok-2.1.2/miditok/tokenizations/octuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12123 2023-07-24 18:17:20.000000 miditok-2.1.2/miditok/tokenizations/octuple_mono.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16074 2023-07-24 18:17:20.000000 miditok-2.1.2/miditok/tokenizations/remi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26758 2023-07-24 18:17:20.000000 miditok-2.1.2/miditok/tokenizations/remi_plus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9570 2023-07-24 18:17:20.000000 miditok-2.1.2/miditok/tokenizations/structured.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21427 2023-07-24 18:17:20.000000 miditok-2.1.2/miditok/tokenizations/tsd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:17:36.077942 miditok-2.1.2/miditok/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-24 18:17:20.000000 miditok-2.1.2/miditok/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15771 2023-07-24 18:17:20.000000 miditok-2.1.2/miditok/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:17:36.073942 miditok-2.1.2/miditok.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-07-24 18:17:36.000000 miditok-2.1.2/miditok.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-24 18:17:36.000000 miditok-2.1.2/miditok.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:17:36.000000 miditok-2.1.2/miditok.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-24 18:17:36.000000 miditok-2.1.2/miditok.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-24 18:17:36.000000 miditok-2.1.2/miditok.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 18:17:36.077942 miditok-2.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-24 18:17:20.000000 miditok-2.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:17:36.077942 miditok-2.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-07-24 18:17:20.000000 miditok-2.1.2/tests/test_bpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-07-24 18:17:20.000000 miditok-2.1.2/tests/test_io_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-24 18:17:20.000000 miditok-2.1.2/tests/test_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-07-24 18:17:20.000000 miditok-2.1.2/tests/test_multitrack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-07-24 18:17:20.000000 miditok-2.1.2/tests/test_one_track.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-24 18:17:20.000000 miditok-2.1.2/tests/test_saving_loading_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-24 18:17:20.000000 miditok-2.1.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-07-24 18:17:20.000000 miditok-2.1.2/tests/tests_utils.py
```

### Comparing `miditok-2.1.1/LICENSE` & `miditok-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `miditok-2.1.1/PKG-INFO` & `miditok-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miditok
-Version: 2.1.1
+Version: 2.1.2
 Summary: A convenient MIDI tokenizer for Deep Learning networks, with multiple encoding strategies
 Home-page: https://github.com/Natooz/MidiTok
 Author: Nathan Fradet
 License: MIT
 Keywords: artificial intelligence,deep learning,transformer,midi,tokenization,music,mir
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `miditok-2.1.1/README.md` & `miditok-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `miditok-2.1.1/miditok/classes.py` & `miditok-2.1.2/miditok/classes.py`

 * *Files identical despite different names*

### Comparing `miditok-2.1.1/miditok/constants.py` & `miditok-2.1.2/miditok/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Constants for data encoding
 
 """
 
-CURRENT_VERSION_PACKAGE = "2.1.1"  # used when saving the config of a tokenizer
+CURRENT_VERSION_PACKAGE = "2.1.2"  # used when saving the config of a tokenizer
 
 MIDI_FILES_EXTENSIONS = [".mid", ".midi", ".MID", ".MIDI"]
 
 # Starting id of chr() method for BPE, as the 5 (0 to 4 included) firsts are ignored by 🤗tokenize
 # We also skip the 32nd (0x20) (space) as it causes issues when loading a BPE model with spaces in merged
 # Issue for reference: https://github.com/huggingface/tokenizers/issues/566
 # List of unicode characters: https://www.fileformat.info/info/charset/UTF-8/list.htm
```

### Comparing `miditok-2.1.1/miditok/data_augmentation/data_augmentation.py` & `miditok-2.1.2/miditok/data_augmentation/data_augmentation.py`

 * *Files 8% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     nb_augmentations, nb_tracks_augmented = 0, 0
     for file_path in tqdm(files_paths, desc="Performing data augmentation"):
         if as_tokens:
             with open(file_path) as json_file:
                 file = json.load(json_file)
                 ids, programs = file["ids"], file["programs"]
 
-            if tokenizer.unique_track:
+            if tokenizer.one_token_stream:
                 ids = [ids]
 
             # Perform data augmentation for each track
             offsets = get_offsets(
                 tokenizer,
                 nb_octave_offset,
                 nb_vel_offset,
@@ -87,17 +87,17 @@
                 ids=ids,
             )
             augmented_tokens: Dict[
                 Tuple[int, int, int], List[Union[int, List[int]]]
             ] = {}
             for track, (_, is_drum) in zip(ids, programs):
                 # we dont augment drums
-                if not tokenizer.unique_track and is_drum:
+                if not tokenizer.one_token_stream and is_drum:
                     continue
-                elif tokenizer.unique_track and all(p[1] for p in programs):
+                elif tokenizer.one_token_stream and all(p[1] for p in programs):
                     continue
                 corrected_offsets = deepcopy(offsets)
                 vel_dim = int(128 / len(tokenizer.velocities))
                 corrected_offsets[1] = [
                     int(off / vel_dim) for off in corrected_offsets[1]
                 ]
                 aug = data_augmentation_tokens(
@@ -105,22 +105,22 @@
                     tokenizer,
                     *corrected_offsets,
                     all_offset_combinations=all_offset_combinations,
                 )
                 if len(aug) == 0:
                     continue
                 for aug_offsets, seq in aug:
-                    if tokenizer.unique_track:
+                    if tokenizer.one_token_stream:
                         augmented_tokens[aug_offsets] = seq
                         continue
                     try:
                         augmented_tokens[aug_offsets].append(seq)
                     except KeyError:
                         augmented_tokens[aug_offsets] = [seq]
-            if not tokenizer.unique_track:
+            if not tokenizer.one_token_stream:
                 for i, (track, (_, is_drum)) in enumerate(
                     zip(ids, programs)
                 ):  # adding drums to all already augmented
                     if is_drum:
                         for aug_offsets in augmented_tokens:
                             augmented_tokens[aug_offsets].insert(i, track)
 
@@ -138,15 +138,15 @@
                 saving_path = (
                     file_path.parent if out_path is None else out_path
                 ) / f"{file_path.stem}{suffix}.json"
                 tokenizer.save_tokens(tracks_seq, saving_path, programs)
                 nb_augmentations += 1
                 nb_tracks_augmented += len(tracks_seq)
             if copy_original_in_new_location and out_path is not None:
-                if tokenizer.unique_track:
+                if tokenizer.one_token_stream:
                     ids = ids[0]
                 tokenizer.save_tokens(
                     ids, out_path / f"{file_path.stem}.json", programs
                 )
 
         else:  # as midi
             try:
@@ -451,15 +451,15 @@
             pitch_tokens = np.array(
                 tokenizer.token_ids_of_type("Pitch")
                 + tokenizer.token_ids_of_type("NoteOn")
             )
             note_off_tokens = np.array(tokenizer.token_ids_of_type("NoteOff"))
             mask_pitch = np.isin(tokens, pitch_tokens)
             # If applicable, removes drum notes from the mask
-            if tokenizer.unique_track:
+            if tokenizer.one_token_stream:
                 for idx, is_note in enumerate(mask_pitch):
                     if (
                         is_note
                         and idx > 0
                         and tokenizer[tokens[idx - 1]] == "Program_-1"
                     ):
                         mask_pitch[idx] = False
```

### Comparing `miditok-2.1.1/miditok/midi_tokenizer.py` & `miditok-2.1.2/miditok/midi_tokenizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,97 +28,155 @@
     CHR_ID_START,
     PITCH_CLASSES,
     UNKNOWN_CHORD_PREFIX,
     MIDI_FILES_EXTENSIONS,
 )
 
 
+def convert_sequence_to_tokseq(
+        tokenizer,
+        input_seq,
+        complete_seq: bool = True,
+        decode_bpe: bool = True
+) -> Union[TokSequence, List[TokSequence]]:
+    r"""Converts a sequence into a :class:`miditok.TokSequence` or list of :class:`miditok.TokSequence`
+    objects with the appropriate format of the tokenizer being used.
+
+    :param tokenizer: tokenizer being used with the sequence.
+    :param input_seq: sequence to convert. It can be a list of ids (integers), tokens (string) or events (Event).
+        It can also be a Pytorch or TensorFlow tensor, or Numpy array representing ids.
+    :param complete_seq: will complete the output sequence(s). (default: True)
+    :param decode_bpe: if the input sequence contains ids, and that they contain BPE tokens, these tokens will
+        be decoded. (default: True)
+    :return:
+    """
+    # Deduce the type of data (ids/tokens/events)
+    try:
+        arg = ("ids", convert_ids_tensors_to_list(input_seq))
+    except (AttributeError, ValueError, TypeError, IndexError):
+        if isinstance(input_seq[0], str) or (
+                isinstance(input_seq[0], list) and isinstance(input_seq[0][0], str)
+        ):
+            arg = ("tokens", input_seq)
+        else:  # list of Event, but unlikely
+            arg = ("events", input_seq)
+
+    # Deduce nb of subscripts / dims
+    nb_io_dims = len(tokenizer.io_format)
+    nb_seq_dims = 1
+    if isinstance(arg[1][0], list):
+        nb_seq_dims += 1
+        if isinstance(arg[1][0][0], list):
+            nb_seq_dims += 1
+
+    # Check the number of dimensions is good
+    # In case of no one_token_stream and one dimension short --> unsqueeze
+    if not tokenizer.one_token_stream and nb_seq_dims == nb_io_dims - 1:
+        print(f"The input sequence has one dimension less than expected ({nb_seq_dims} instead of "
+              f"{nb_io_dims}). It is being unsqueezed to conform with the tokenizer's i/o format "
+              f"({tokenizer.io_format})")
+        arg = (arg[0], [arg[1]])
+
+    elif nb_seq_dims != nb_io_dims:
+        raise ValueError(f"The input sequence does not have the expected dimension "
+                         f"({nb_seq_dims} instead of {nb_io_dims}).")
+
+    # Convert to TokSequence
+    if not tokenizer.one_token_stream and nb_io_dims == nb_seq_dims:
+        seq = []
+        for obj in arg[1]:
+            kwarg = {arg[0]: obj}
+            seq.append(TokSequence(**kwarg))
+            if not tokenizer.is_multi_voc:
+                seq[-1].ids_bpe_encoded = tokenizer._are_ids_bpe_encoded(
+                    seq[-1].ids
+                )
+    else:  # 1 subscript, one_token_stream and no multi-voc
+        kwarg = {arg[0]: arg[1]}
+        seq = TokSequence(**kwarg)
+        if not tokenizer.is_multi_voc:
+            seq.ids_bpe_encoded = tokenizer._are_ids_bpe_encoded(seq.ids)
+
+    # decode BPE and complete the output sequence(s) if requested
+    if tokenizer.has_bpe and decode_bpe:
+        tokenizer.decode_bpe(seq)
+    if complete_seq:
+        if isinstance(seq, TokSequence):
+            tokenizer.complete_sequence(seq)
+        else:
+            for seq_ in seq:
+                tokenizer.complete_sequence(seq_)
+
+    return seq
+
+
 def _in_as_seq(complete: bool = True, decode_bpe: bool = True):
-    """Decorator creating if necessary and completing a TokSequence object before that the function is called.
-    This decorator is used by the :py:meth:`miditok.MIDITokenizer.track_to_tokens` method.
+    r"""Decorator creating if necessary and completing a :class:`miditok.TokSequence` object before that the function
+    is called. This decorator is made to be used by the :py:meth:`miditok.MIDITokenizer.tokens_to_midi` method.
 
     :param complete: will complete the sequence, i.e. complete its ``ids`` , ``tokens`` and ``events`` .
     :param decode_bpe: will decode BPE, if applicable. This step is performed before completing the sequence.
     """
 
     def decorator(function: Callable = None):
         def wrapper(*args, **kwargs):
-            self = args[0]
+            tokenizer = args[0]
             seq = args[1]
             if not isinstance(seq, TokSequence) and not all(
                 isinstance(seq_, TokSequence) for seq_ in seq
             ):
-                try:
-                    arg = ("ids", convert_ids_tensors_to_list(seq))
-                except (AttributeError, ValueError, TypeError, IndexError):
-                    if isinstance(seq[0], str) or (
-                        isinstance(seq[0], str) and isinstance(seq[0][0], str)
-                    ):
-                        arg = ("tokens", seq)
-                    else:  # list of Event, very unlikely
-                        arg = ("events", seq)
-
-                if isinstance(arg[1][0], list):
-                    seq = []
-                    for obj in arg[1]:
-                        kwarg = {arg[0]: obj}
-                        seq.append(TokSequence(**kwarg))
-                        seq[-1].ids_bpe_encoded = self._are_ids_bpe_encoded(seq[-1].ids)
-                else:
-                    kwarg = {arg[0]: arg[1]}
-                    seq = TokSequence(**kwarg)
-                    seq.ids_bpe_encoded = self._are_ids_bpe_encoded(seq.ids)
-
-            if self.has_bpe and decode_bpe:
-                self.decode_bpe(seq)
-            if complete:
-                if isinstance(seq, TokSequence):
-                    self.complete_sequence(seq)
-                else:
-                    for seq_ in seq:
-                        self.complete_sequence(seq_)
+                seq = convert_sequence_to_tokseq(tokenizer, seq, complete, decode_bpe)
+            else:
+                if tokenizer.has_bpe and decode_bpe:
+                    tokenizer.decode_bpe(seq)
+                if complete:
+                    if isinstance(seq, TokSequence):
+                        tokenizer.complete_sequence(seq)
+                    else:
+                        for seq_ in seq:
+                            tokenizer.complete_sequence(seq_)
 
             args = list(args)
             args[1] = seq
             return function(*args, **kwargs)
 
         return wrapper
 
     return decorator
 
 
 def _out_as_complete_seq(function: Callable):
-    """Decorator completing an output Sequence object."""
+    r"""Decorator completing an output :class:`miditok.TokSequence` object."""
 
     def wrapper(*args, **kwargs):
         self = args[0]
         res = function(*args, **kwargs)
         self.complete_sequence(res)
         return res
 
     return wrapper
 
 
 class MIDITokenizer(ABC):
     r"""MIDI tokenizer base class, containing common methods and attributes for all tokenizers.
 
     :param tokenizer_config: the tokenizer's configuration, as a :class:`miditok.classes.TokenizerConfig` object.
-    :param unique_track: set to True if the tokenizer works only with a unique track.
-            Tokens will be saved as a single track. This applies to representations that natively handle
-            multiple tracks such as Octuple, resulting in a single "stream" of tokens for all tracks.
+    :param one_token_stream: give True if the tokenizer handle all the tracks of a MIDI as a single sequence of tokens.
+            Tokens will be saved as a single sequence. This applies to representations that natively handle
+            multiple tracks such as Octuple or REMIPlus, resulting in a single "stream" of tokens per MIDI.
             This attribute will be saved in config files of the tokenizer. (default: False)
     :param params: path to a tokenizer config file. This will override other arguments and
             load the tokenizer based on the config file. This is particularly useful if the
             tokenizer learned Byte Pair Encoding. (default: None)
     """
 
     def __init__(
         self,
         tokenizer_config: TokenizerConfig = None,
-        unique_track: bool = False,
+        one_token_stream: bool = False,
         params: Union[str, Path] = None,
     ):
         # Initialize params
         self.config = deepcopy(tokenizer_config)
         # vocab of prime tokens, can be viewed as unique char / bytes
         self._vocab_base = {}
         # the other way, to decode id (int) -> token (str)
@@ -143,15 +201,15 @@
                 self.config = TokenizerConfig()
             assert (
                 self.config.pitch_range[0] >= 0 and self.config.pitch_range[1] <= 128
             ), "You must specify a pitch_range between 0 and 127 (included, i.e. range.stop at 128)"
             assert (
                 0 < self.config.nb_velocities < 128
             ), "You must specify a nb_velocities between 1 and 127 (included)"
-            self.unique_track = unique_track
+            self.one_token_stream = one_token_stream
 
         # Tweak the tokenizer's configuration and / or attributes before creating the vocabulary
         # This method is intended to be overridden by inheriting tokenizer classes
         self._tweak_config_before_creating_voc()
 
         # Init duration and velocity values
         self.durations = self.__create_durations_tuples()
@@ -438,15 +496,15 @@
         This method returns a list of :class:`miditok.TokSequence`.
 
         If you are implementing your own tokenization by subclassing this class, **override the
         ``_midi_to_tokens`` method**. This method implement necessary MIDI preprocessing.
 
         :param midi: the MIDI object to convert.
         :param apply_bpe_if_possible: will apply BPE if the tokenizer's vocabulary was learned with.
-        :return: a :class:`miditok.TokSequence` if `tokenizer.unique_track` is true, else a list of
+        :return: a :class:`miditok.TokSequence` if `tokenizer.one_token_stream` is true, else a list of
                 :class:`miditok.TokSequence` objects.
         """
         # Check if the durations values have been calculated before for this time division
         if midi.ticks_per_beat not in self._durations_ticks:
             self._durations_ticks[midi.ticks_per_beat] = np.array(
                 [
                     (beat * res + pos) * midi.ticks_per_beat // res
@@ -585,36 +643,37 @@
         tokens = []
         for byte_ in bytes_:
             token_str = self._vocab_bpe_bytes_to_tokens[byte_]
             tokens.append(token_str if as_str else Event(*token_str.split("_")))
         tokens = [tok for toks in tokens for tok in toks]  # flatten
         return tokens
 
+    @_in_as_seq()
     def tokens_to_midi(
         self,
         tokens: Union[TokSequence, List, np.ndarray, Any],
         programs: Optional[List[Tuple[int, bool]]] = None,
         output_path: Optional[str] = None,
         time_division: Optional[int] = TIME_DIVISION,
     ) -> MidiFile:
         r"""Converts multiple sequences of tokens (:class:`miditok.TokSequence`) into a MIDI and saves it.
         **NOTE:** With Remi, MIDI-Like, CP Word or other tokenization that processes tracks
         independently, only the tempo changes of the first track in tokens will be used.
 
         :param tokens: tokens to convert. Can be either a list of :class:`miditok.TokSequence`,
                 a Tensor (PyTorch and Tensorflow are supported), a numpy array or a Python list of ints.
                 The first dimension represents tracks, unless the tokenizer handle tracks altogether as a
-                single token sequence (e.g. Octuple, MuMIDI): tokenizer.unique_track == True.
+                single token sequence (e.g. Octuple, MuMIDI): tokenizer.one_token_stream == True.
         :param programs: programs of the tracks. If none is given, will default to piano, program 0. (default: None)
         :param output_path: path to save the file. (default: None)
         :param time_division: MIDI time division / resolution, in ticks/beat (of the MIDI to create).
         :return: the midi object (miditoolkit.MidiFile).
         """
         midi = MidiFile(ticks_per_beat=time_division)
-        # if self.unique_track:
+        # if self.one_token_stream:
         #    tokens = [tokens]
         for i, track_tokens in enumerate(tokens):
             if programs is not None:
                 track, tempo_changes = self.tokens_to_track(
                     track_tokens, time_division, programs[i]
                 )
             else:
@@ -635,15 +694,15 @@
             Path(output_path).mkdir(parents=True, exist_ok=True)
             midi.dump(output_path)
         return midi
 
     @abstractmethod
     def tokens_to_track(
         self,
-        tokens: Union[TokSequence, List, np.ndarray, Any],
+        tokens: TokSequence,
         time_division: Optional[int] = TIME_DIVISION,
         program: Optional[Tuple[int, bool]] = (0, False),
     ) -> Tuple[Instrument, List[TempoChange]]:
         r"""Converts a sequence of tokens into a track object.
         This method is unimplemented and need to be overridden by inheriting classes.
         This method should be decorated with _in_as_complete_seq to receive any type of input.
 
@@ -1021,15 +1080,15 @@
             iterator = []  # list of lists of one string (bytes)
             for file_path in tqdm(tokens_paths, desc="Loading token files"):
                 sample = self.load_tokens(file_path)
                 bytes_ = self._ids_to_bytes(
                     sample["ids"], as_one_str=True
                 )  # list of str (bytes)
                 iterator += (
-                    [[byte_] for byte_ in bytes_] if not self.unique_track else [bytes_]
+                    [[byte_] for byte_ in bytes_] if not self.one_token_stream else [bytes_]
                 )
 
             # This doesn't seem to work, the trainer pre-processes the sequences, but then no word remains
             """def it_gen():
                 for file_path_ in tqdm(tokens_paths, desc="Loading token files"):
                     sample_ = self.load_tokens(file_path_)
                     yield self._ids_to_bytes(sample_["ids"], as_one_str=True)
@@ -1158,15 +1217,15 @@
             return
 
         files_paths = list(Path(dataset_path).glob("**/*.json"))
         for path in tqdm(files_paths, desc="Applying BPE to dataset"):
             sample = self.load_tokens(path)
             seq = (
                 TokSequence(ids=sample["ids"])
-                if self.unique_track
+                if self.one_token_stream
                 else [TokSequence(ids=track) for track in sample["ids"]]
             )
             self.apply_bpe(seq)
 
             out_ = (
                 Path(out_path) / path.relative_to(dataset_path)
                 if out_path is not None
@@ -1287,26 +1346,30 @@
 
         if apply_bpe and self.has_bpe:
             self.apply_bpe_to_dataset(out_dir)
 
     @_in_as_seq(complete=False, decode_bpe=False)
     def tokens_errors(
         self, tokens: Union[TokSequence, List[Union[int, List[int]]]]
-    ) -> float:
+    ) -> Union[float, List[float]]:
         r"""Checks if a sequence of tokens is made of good token types
         successions and returns the error ratio (lower is better).
         The common implementation in MIDITokenizer class will check token types,
         duplicated notes and time errors. It works for REMI, TSD and Structured.
         Other tokenizations override this method to include other errors
         (like no NoteOff / NoteOn for MIDILike and embedding pooling).
         Overridden methods must call decompose_bpe at the beginning if BPE is used!
 
         :param tokens: sequence of tokens to check.
         :return: the error ratio (lower is better).
         """
+        # If list of TokSequence -> recursive
+        if isinstance(tokens, list):
+            return [self.tokens_errors(tok_seq) for tok_seq in tokens]
+
         nb_tok_predicted = len(tokens)  # used to norm the score
         if self.has_bpe:
             self.decode_bpe(tokens)
         self.complete_sequence(tokens)
 
         # Override from here
         tokens = tokens.tokens
@@ -1436,15 +1499,15 @@
 
         dict_config = self.config.to_dict(serialize=True)
         dict_config["beat_res"] = {
             f"{k1}_{k2}": v for (k1, k2), v in dict_config["beat_res"].items()
         }
         params = {
             "config": dict_config,
-            "unique_track": self.unique_track,
+            "one_token_stream": self.one_token_stream,
             "has_bpe": self.has_bpe,
             "tokenization": self.__class__.__name__,
             "miditok_version": CURRENT_VERSION_PACKAGE,
             **additional_attributes,
         }
 
         out_path = Path(out_path)
@@ -1508,26 +1571,40 @@
                         for beat_range, res in value.items()
                     }
                 # Convert old attribute from < v2.1.0 to new for TokenizerConfig
                 elif key in old_add_tokens_attr:
                     key = old_add_tokens_attr[key]
                 setattr(self.config, key, value)
                 continue
+            elif key == "unique_track":
+                # For config files <= v2.1.1 before the attribute is renamed
+                self.one_token_stream = value
 
             setattr(self, key, value)
 
     @property
     def is_multi_voc(self) -> bool:
         """Returns a bool indicating if the tokenizer uses embedding
         pooling, and so have multiple vocabularies.
 
         :return: True is the tokenizer uses embedding pooling else False.
         """
         return isinstance(self._vocab_base, list)
 
+    @property
+    def io_format(self) -> Tuple[str]:
+        format_ = []
+        if not self.one_token_stream:
+            format_.append("I")
+        format_.append("T")
+        if self.is_multi_voc:
+            format_.append("C")
+
+        return tuple(d for d in format_)
+
     def __call__(self, obj: Any, *args, **kwargs):
         r"""Calling a tokenizer allows to directly convert a MIDI to tokens or the other way around.
         The method automatically detects MIDI and token objects, as well as paths and can directly load
         MIDI or token json files before converting them.
         This will call the :py:func:`miditok.MIDITokenizer.midi_to_tokens` if you provide a MIDI object
         or path to a MIDI file, or the :py:func:`miditok.MIDITokenizer.tokens_to_midi` method otherwise.
 
@@ -1575,21 +1652,30 @@
         to get the sum of the lengths.
 
         :return: length of the vocabulary.
         """
         return [len(v) for v in self.vocab] if self.is_multi_voc else len(self)
 
     def __repr__(self):
-        out_str = f"{self.len} tokens"
+        out_str = f"{self.len} tokens with {self.io_format} io format"
+
+        # one_token_stream / multi-voc
+        tmp = []
+        if self.one_token_stream:
+            tmp.append("one token stream")
         if self.is_multi_voc:
-            out_str += " (multi-voc)"
+            tmp.append("multi-voc")
+        if len(tmp) > 0:
+            out_str += f"({', '.join(tmp)})"
+
+        # BPE
         if self.has_bpe:
-            out_str += " with BPE"
+            out_str += ", with BPE"
         else:
-            out_str += " without BPE"
+            out_str += ", without BPE"
         return out_str
 
     def __getitem__(
         self, item: Union[int, str, Tuple[int, Union[int, str]]]
     ) -> Union[str, int, List[int]]:
         r"""Convert a token (int) to an event (str), or vice-versa.
```

### Comparing `miditok-2.1.1/miditok/tokenizations/cp_word.py` & `miditok-2.1.2/miditok/tokenizations/cp_word.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,18 +281,17 @@
             if program is not None:
                 cp_token_template[
                     self.vocab_types_idx["Program"]
                 ] = f"Program_{program}"
 
         return cp_token_template
 
-    @_in_as_seq()
     def tokens_to_track(
         self,
-        tokens: Union[TokSequence, List, np.ndarray, Any],
+        tokens: TokSequence,
         time_division: Optional[int] = TIME_DIVISION,
         program: Optional[Tuple[int, bool]] = (0, False),
     ) -> Tuple[Instrument, List[TempoChange]]:
         r"""Converts a sequence of tokens into a track object
 
         :param tokens: sequence of tokens to convert. Can be either a Tensor (PyTorch and Tensorflow are supported),
                 a numpy array, a Python list or a TokSequence.
@@ -461,24 +460,29 @@
         for key in dic:
             dic[key].append("Ignore")
         dic["Ignore"] = list(dic.keys())
 
         return dic
 
     @_in_as_seq()
-    def tokens_errors(self, tokens: Union[TokSequence, List, np.ndarray, Any]) -> float:
+    def tokens_errors(
+        self, tokens: Union[TokSequence, List, np.ndarray, Any]
+    ) -> Union[float, List[float]]:
         r"""Checks if a sequence of tokens is made of good token types
         successions and returns the error ratio (lower is better).
         The Pitch and Position values are also analyzed:
             - a position token cannot have a value <= to the current position (it would go back in time)
             - a pitch token should not be present if the same pitch is already played at the current position
 
         :param tokens: sequence of tokens to check
         :return: the error ratio (lower is better)
         """
+        # If list of TokSequence -> recursive
+        if isinstance(tokens, list):
+            return [self.tokens_errors(tok_seq) for tok_seq in tokens]
 
         def cp_token_type(tok: List[int]) -> List[str]:
             family = self[0, tok[0]].split("_")[1]
             if family == "Note":
                 return self[2, tok[2]].split("_")
             elif family == "Metric":
                 bar_pos = self[1, tok[1]].split("_")
```

### Comparing `miditok-2.1.1/miditok/tokenizations/midi_like.py` & `miditok-2.1.2/miditok/tokenizations/midi_like.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,18 +174,17 @@
                 unknown_chords_nb_notes_range=self.config.chord_unknown,
             )
 
         events.sort(key=lambda x: (x.time, self._order(x)))
 
         return TokSequence(events=events)
 
-    @_in_as_seq()
     def tokens_to_track(
         self,
-        tokens: Union[TokSequence, List, np.ndarray, Any],
+        tokens: TokSequence,
         time_division: Optional[int] = TIME_DIVISION,
         program: Optional[Tuple[int, bool]] = (0, False),
         default_duration: int = None,
     ) -> Tuple[Instrument, List[TempoChange]]:
         r"""Converts a sequence of tokens into a track object
 
         :param tokens: sequence of tokens to convert. Can be either a Tensor (PyTorch and Tensorflow are supported),
@@ -347,24 +346,30 @@
             if self.config.use_chords:
                 dic["Rest"] += ["Chord"]
             dic["NoteOff"] += ["Rest"]
 
         return dic
 
     @_in_as_seq(complete=False, decode_bpe=False)
-    def tokens_errors(self, tokens: Union[TokSequence, List, np.ndarray, Any]) -> float:
+    def tokens_errors(
+        self, tokens: Union[TokSequence, List, np.ndarray, Any]
+    ) -> Union[float, List[float]]:
         r"""Checks if a sequence of tokens is made of good token types
         successions and returns the error ratio (lower is better).
         The Pitch and Position values are also analyzed:
             - a NoteOn token should not be present if the same pitch is already being played
             - a NoteOff token should not be present the note is not being played
 
         :param tokens: sequence of tokens to check
         :return: the error ratio (lower is better)
         """
+        # If list of TokSequence -> recursive
+        if isinstance(tokens, list):
+            return [self.tokens_errors(tok_seq) for tok_seq in tokens]
+
         nb_tok_predicted = len(tokens)  # used to norm the score
         if self.has_bpe:
             self.decode_bpe(tokens)
         self.complete_sequence(tokens)
 
         # Override from here
```

### Comparing `miditok-2.1.1/miditok/tokenizations/mmm.py` & `miditok-2.1.2/miditok/tokenizations/mmm.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,15 +212,15 @@
             Event("Bar", "End", events[-1].time + 1),
             Event("Track", "End", events[-1].time + 1),
         ]
         return events
 
     def tokens_to_track(
         self,
-        tokens: Union[TokSequence, List, np.ndarray, Any],
+        tokens: TokSequence,
         time_division: Optional[int] = TIME_DIVISION,
         program: Optional[Tuple[int, bool]] = (0, False),
     ) -> None:
         r"""NOT RELEVANT / IMPLEMENTED FOR MMM, use tokens_to_midi instead
 
         :param tokens: sequence of tokens to convert. Can be either a Tensor (PyTorch and Tensorflow are supported),
                 a numpy array, a Python list or a TokSequence.
```

### Comparing `miditok-2.1.1/miditok/tokenizations/mumidi.py` & `miditok-2.1.2/miditok/tokenizations/mumidi.py`

 * *Files 7% similar despite different names*

```diff
@@ -63,15 +63,15 @@
                 # this attribute might increase over tokenizations, if the tokenizer encounter longer MIDIs
                 tokenizer_config.additional_params["max_bar_embedding"] = 60
         super().__init__(tokenizer_config, True, params=params)
 
     def _tweak_config_before_creating_voc(self):
         self.config.use_rests = False
         self.config.use_time_signatures = False
-        # self.unique_track = True
+        # self.one_token_stream = True
 
         self.vocab_types_idx = {
             "Pitch": 0,
             "DrumPitch": 0,
             "Position": 0,
             "Bar": 0,
             "Program": 0,
@@ -97,35 +97,14 @@
         * (-3 / 3: Tempo)
         * -2: Velocity
         * -1: Duration
 
         :param midi: the MIDI object to convert
         :return: sequences of tokens
         """
-        # Check if the durations values have been calculated before for this time division
-        if midi.ticks_per_beat not in self._durations_ticks:
-            self._durations_ticks[midi.ticks_per_beat] = np.array(
-                [
-                    (beat * res + pos) * midi.ticks_per_beat // res
-                    for beat, pos, res in self.durations
-                ]
-            )
-        # Preprocess the MIDI file
-        self.preprocess_midi(midi)
-
-        # Register MIDI metadata
-        self.current_midi_metadata = {
-            "time_division": midi.ticks_per_beat,
-            "tempo_changes": midi.tempo_changes,
-            "time_sig_changes": midi.time_signature_changes,
-            "key_sig_changes": midi.key_signature_changes,
-        }
-
-        # **************** OVERRIDE FROM HERE, KEEP THE LINES ABOVE IN YOUR METHOD ****************
-
         # Check bar embedding limit, update if needed
         nb_bars = ceil(midi.max_tick / (midi.ticks_per_beat * 4))
         if self.config.additional_params["max_bar_embedding"] < nb_bars:
             for i in range(self.config.additional_params["max_bar_embedding"], nb_bars):
                 self.add_to_vocab(f"BarPosEnc_{i}", 1)
             self.config.additional_params["max_bar_embedding"] = nb_bars
 
@@ -144,26 +123,26 @@
         tokens = []
 
         current_tick = -1
         current_bar = -1
         current_pos = -1
         current_track = -2  # because -2 doesn't exist
         current_tempo_idx = 0
-        current_tempo = self.current_midi_metadata["tempo_changes"][
+        current_tempo = self._current_midi_metadata["tempo_changes"][
             current_tempo_idx
         ].tempo
         for note_token in note_tokens:
             # (Tempo) update tempo values current_tempo
             if self.config.use_tempos:
                 # If the current tempo is not the last one
                 if current_tempo_idx + 1 < len(
-                    self.current_midi_metadata["tempo_changes"]
+                    self._current_midi_metadata["tempo_changes"]
                 ):
                     # Will loop over incoming tempo changes
-                    for tempo_change in self.current_midi_metadata["tempo_changes"][
+                    for tempo_change in self._current_midi_metadata["tempo_changes"][
                         current_tempo_idx + 1 :
                     ]:
                         # If this tempo change happened before the current moment
                         if tempo_change.time <= note_token[0].time:
                             current_tempo = tempo_change.tempo
                             current_tempo_idx += (
                                 1  # update tempo value (might not change) and index
@@ -228,15 +207,15 @@
         * 2: Duration
 
         :param track: track object to convert.
         :return: sequence of corresponding tokens.
         """
         # Make sure the notes are sorted first by their onset (start) times, second by pitch
         # notes.sort(key=lambda x: (x.start, x.pitch))  # done in midi_to_tokens
-        dur_bins = self._durations_ticks[self.current_midi_metadata["time_division"]]
+        dur_bins = self._durations_ticks[self._current_midi_metadata["time_division"]]
 
         tokens = []
         for note in track.notes:
             # Note
             duration = note.end - note.start
             dur_idx = np.argmin(np.abs(dur_bins - duration))
             if not track.is_drum:
@@ -315,17 +294,23 @@
         :param time_division: MIDI time division / resolution, in ticks/beat (of the MIDI to create)
         :return: the midi object (miditoolkit.MidiFile)
         """
         assert (
             time_division % max(self.config.beat_res.values()) == 0
         ), f"Invalid time division, please give one divisible by {max(self.config.beat_res.values())}"
         midi = MidiFile(ticks_per_beat=time_division)
-        midi.tempo_changes.append(TempoChange(TEMPO, 0))
-        ticks_per_sample = time_division // max(self.config.beat_res.values())
 
+        # Tempos
+        if self.config.use_tempos:
+            first_tempo = int(tokens.tokens[0][3].split("_")[1])
+        else:
+            first_tempo = TEMPO
+        midi.tempo_changes.append(TempoChange(first_tempo, 0))
+
+        ticks_per_sample = time_division // max(self.config.beat_res.values())
         tracks = {}
         current_tick = 0
         current_bar = -1
         current_track = 0  # default set to piano
         for time_step in tokens.tokens:
             tok_type, tok_val = time_step[0].split("_")
             if tok_type == "Bar":
@@ -353,14 +338,20 @@
                 vel = int(vel)
                 duration = self._token_duration_to_ticks(duration, time_division)
 
                 tracks[current_track].append(
                     Note(vel, pitch, current_tick, current_tick + duration)
                 )
 
+            # Decode tempo if required
+            if self.config.use_tempos:
+                tempo_val = int(time_step[3].split("_")[1])
+                if tempo_val != midi.tempo_changes[-1].tempo:
+                    midi.tempo_changes.append(TempoChange(tempo_val, current_tick))
+
         # Appends created notes to MIDI object
         for program, notes in tracks.items():
             if int(program) == -1:
                 midi.instruments.append(Instrument(0, True, "Drums"))
             else:
                 midi.instruments.append(
                     Instrument(
@@ -373,15 +364,15 @@
         if output_path:
             Path(output_path).mkdir(parents=True, exist_ok=True)
             midi.dump(output_path)
         return midi
 
     def tokens_to_track(
         self,
-        tokens: Union[TokSequence, List, np.ndarray, Any],
+        tokens: TokSequence,
         time_division: Optional[int] = TIME_DIVISION,
         program: Optional[Tuple[int, bool]] = (0, False),
     ):
         r"""Not relevant / implemented for MuMIDI. Use :py:meth:`miditok.MuMIDI.tokens_to_midi` instead.
 
         :param tokens: sequence of tokens to convert. Can be either a Tensor (PyTorch and Tensorflow are supported),
                 a numpy array, a Python list or a TokSequence.
```

### Comparing `miditok-2.1.1/miditok/tokenizations/octuple.py` & `miditok-2.1.2/miditok/tokenizations/octuple.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     * Tokens are first sorted by time, then track, then pitch values.
     * Tracks with the same *Program* will be merged.
     """
 
     def _tweak_config_before_creating_voc(self):
         self.config.use_chords = False
         self.config.use_rests = False
-        self.unique_track = True
+        self.one_token_stream = True
 
         # used in place of positional encoding
         # This attribute might increase over tokenizations, if the tokenizer encounter longer MIDIs
         if "max_bar_embedding" not in self.config.additional_params:
             self.config.additional_params["max_bar_embedding"] = 60
 
         token_types = ["Pitch", "Velocity", "Duration", "Program", "Position", "Bar"]
@@ -74,36 +74,14 @@
             5: Bar
             (6: Tempo)
             (7: TimeSignature)
 
         :param midi: the MIDI object to convert
         :return: sequences of tokens
         """
-        # Check if the durations values have been calculated before for this time division
-        if midi.ticks_per_beat not in self._durations_ticks:
-            self._durations_ticks[midi.ticks_per_beat] = np.array(
-                [
-                    (beat * res + pos) * midi.ticks_per_beat // res
-                    for beat, pos, res in self.durations
-                ]
-            )
-
-        # Preprocess the MIDI file
-        self.preprocess_midi(midi)
-
-        # Register MIDI metadata
-        self.current_midi_metadata = {
-            "time_division": midi.ticks_per_beat,
-            "tempo_changes": midi.tempo_changes,
-            "time_sig_changes": midi.time_signature_changes,
-            "key_sig_changes": midi.key_signature_changes,
-        }
-
-        # **************** OVERRIDE FROM HERE, KEEP THE LINES ABOVE IN YOUR METHOD ****************
-
         # Check bar embedding limit, update if needed
         nb_bars = ceil(midi.max_tick / (midi.ticks_per_beat * 4))
         if self.config.additional_params["max_bar_embedding"] < nb_bars:
             for i in range(self.config.additional_params["max_bar_embedding"], nb_bars):
                 self.add_to_vocab(f"Bar_{i}", 5)
             self.config.additional_params["max_bar_embedding"] = nb_bars
 
@@ -137,30 +115,30 @@
             (7: TimeSignature)
 
         :param track: track object to convert
         :return: sequence of corresponding tokens
         """
         # Make sure the notes are sorted first by their onset (start) times, second by pitch
         # notes.sort(key=lambda x: (x.start, x.pitch))  # done in midi_to_tokens
-        time_division = self.current_midi_metadata["time_division"]
+        time_division = self._current_midi_metadata["time_division"]
         ticks_per_sample = time_division / max(self.config.beat_res.values())
         dur_bins = self._durations_ticks[time_division]
 
         tokens = []
         current_tick = -1
         current_bar = -1
         current_pos = -1
         current_tempo_idx = 0
-        current_tempo = self.current_midi_metadata["tempo_changes"][
+        current_tempo = self._current_midi_metadata["tempo_changes"][
             current_tempo_idx
         ].tempo
         current_time_sig_idx = 0
         current_time_sig_tick = 0
         current_time_sig_bar = 0
-        time_sig_change = self.current_midi_metadata["time_sig_changes"][
+        time_sig_change = self._current_midi_metadata["time_sig_changes"][
             current_time_sig_idx
         ]
         current_time_sig = self._reduce_time_signature(
             time_sig_change.numerator, time_sig_change.denominator
         )
         ticks_per_bar = time_division * current_time_sig[0]
 
@@ -195,18 +173,18 @@
                 f"Bar_{current_bar}",
             ]
 
             # (Tempo)
             if self.config.use_tempos:
                 # If the current tempo is not the last one
                 if current_tempo_idx + 1 < len(
-                    self.current_midi_metadata["tempo_changes"]
+                    self._current_midi_metadata["tempo_changes"]
                 ):
                     # Will loop over incoming tempo changes
-                    for tempo_change in self.current_midi_metadata["tempo_changes"][
+                    for tempo_change in self._current_midi_metadata["tempo_changes"][
                         current_tempo_idx + 1 :
                     ]:
                         # If this tempo change happened before the current moment
                         if tempo_change.time <= note.start:
                             current_tempo = tempo_change.tempo
                             current_tempo_idx += (
                                 1  # update tempo value (might not change) and index
@@ -215,18 +193,18 @@
                             break  # this tempo change is beyond the current time step, we break the loop
                 token.append(f"Tempo_{current_tempo}")
 
             # (TimeSignature)
             if self.config.use_time_signatures:
                 # If the current time signature is not the last one
                 if current_time_sig_idx + 1 < len(
-                    self.current_midi_metadata["time_sig_changes"]
+                    self._current_midi_metadata["time_sig_changes"]
                 ):
                     # Will loop over incoming time signature changes
-                    for time_sig_change in self.current_midi_metadata[
+                    for time_sig_change in self._current_midi_metadata[
                         "time_sig_changes"
                     ][current_time_sig_idx + 1 :]:
                         # If this time signature change happened before the current moment
                         if time_sig_change.time <= note.start:
                             current_time_sig = self._reduce_time_signature(
                                 time_sig_change.numerator, time_sig_change.denominator
                             )
@@ -377,15 +355,15 @@
         if output_path:
             Path(output_path).mkdir(parents=True, exist_ok=True)
             midi.dump(output_path)
         return midi
 
     def tokens_to_track(
         self,
-        tokens: Union[TokSequence, List, np.ndarray, Any],
+        tokens: TokSequence,
         time_division: Optional[int] = TIME_DIVISION,
         program: Optional[Tuple[int, bool]] = (0, False),
     ) -> Tuple[Instrument, List[TempoChange]]:
         r"""NOT RELEVANT / IMPLEMENTED FOR OCTUPLE
         Use tokens_to_midi instead
 
         :param tokens: sequence of tokens to convert. Can be either a Tensor (PyTorch and Tensorflow are supported),
```

### Comparing `miditok-2.1.1/miditok/tokenizations/octuple_mono.py` & `miditok-2.1.2/miditok/tokenizations/octuple_mono.py`

 * *Files 3% similar despite different names*

```diff
@@ -126,18 +126,17 @@
                             break  # this tempo change is beyond the current time step, we break the loop
                 token_ts.append(f"Tempo_{current_tempo}")
 
             tokens.append(token_ts)
 
         return TokSequence(tokens=tokens)
 
-    @_in_as_seq()
     def tokens_to_track(
         self,
-        tokens: Union[TokSequence, List, np.ndarray, Any],
+        tokens: TokSequence,
         time_division: Optional[int] = TIME_DIVISION,
         program: Optional[Tuple[int, bool]] = (0, False),
     ) -> Tuple[Instrument, List[TempoChange]]:
         r"""Converts a sequence of tokens into a track object
         A time step is a list of tokens where:
             (list index: token type)
             0: Pitch
@@ -247,26 +246,32 @@
         Not relevant for Octuple.
 
         :return: the token types transitions dictionary
         """
         return {}  # not relevant for this encoding
 
     @_in_as_seq()
-    def tokens_errors(self, tokens: Union[TokSequence, List, np.ndarray, Any]) -> float:
+    def tokens_errors(
+        self, tokens: Union[TokSequence, List, np.ndarray, Any]
+    ) -> Union[float, List[float]]:
         r"""Checks if a sequence of tokens is made of good token values and
         returns the error ratio (lower is better).
         The token types are always the same in Octuple so this method only checks
         if their values are correct:
             - a bar token value cannot be < to the current bar (it would go back in time)
             - same for positions
             - a pitch token should not be present if the same pitch is already played at the current position
 
         :param tokens: sequence of tokens to check
         :return: the error ratio (lower is better)
         """
+        # If list of TokSequence -> recursive
+        if isinstance(tokens, list):
+            return [self.tokens_errors(tok_seq) for tok_seq in tokens]
+
         err = 0
         current_bar = current_pos = -1
         current_pitches = []
 
         for token in tokens.tokens:
             if any(tok.split("_")[1] == "None" for tok in token):
                 err += 1
```

### Comparing `miditok-2.1.1/miditok/tokenizations/remi.py` & `miditok-2.1.2/miditok/tokenizations/remi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from typing import List, Tuple, Dict, Optional, Union, Any
+from typing import List, Tuple, Dict, Optional
 
 import numpy as np
 from miditoolkit import Instrument, Note, TempoChange
 
-from ..midi_tokenizer import MIDITokenizer, _in_as_seq, _out_as_complete_seq
+from ..midi_tokenizer import MIDITokenizer, _out_as_complete_seq
 from ..classes import TokSequence, Event
 from ..utils import detect_chords
 from ..constants import (
     TIME_DIVISION,
     TEMPO,
     MIDI_INSTRUMENTS,
 )
@@ -198,18 +198,17 @@
                 unknown_chords_nb_notes_range=self.config.chord_unknown,
             )
 
         events.sort(key=lambda x: (x.time, self._order(x)))
 
         return TokSequence(events=events)
 
-    @_in_as_seq()
     def tokens_to_track(
         self,
-        tokens: Union[TokSequence, List, np.ndarray, Any],
+        tokens: TokSequence,
         time_division: Optional[int] = TIME_DIVISION,
         program: Optional[Tuple[int, bool]] = (0, False),
     ) -> Tuple[Instrument, List[TempoChange]]:
         r"""Converts a sequence of tokens into a track object
 
         :param tokens: sequence of tokens to convert. Can be either a Tensor (PyTorch and Tensorflow are supported),
                 a numpy array, a Python list or a TokSequence.
```

### Comparing `miditok-2.1.1/miditok/tokenizations/remi_plus.py` & `miditok-2.1.2/miditok/tokenizations/remi_plus.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             tokenizer_config.additional_params["max_bar_embedding"] = max_bar_embedding
         super().__init__(tokenizer_config, True, params)
 
     def _tweak_config_before_creating_voc(self):
         self.config.use_programs = True
         # code handling rest decoding is writen, but not for detection (encoding)
         self.config.use_rests = False
-        # self.unique_track = True
+        # self.one_token_stream = True
 
         # In case the tokenizer has been created without specifying any config or params file path
         if "max_bar_embedding" not in self.config.additional_params:
             # If used, this attribute might increase over tokenizations, if the tokenizer encounter longer MIDIs
             self.config.additional_params["max_bar_embedding"] = None
 
     def __notes_to_events(self, tracks: List[Instrument]) -> List[Event]:
@@ -288,15 +288,15 @@
         :return: :class:`miditok.TokSequence` of corresponding tokens.
         """
         events = self.__notes_to_events([track])
         return TokSequence(events=events)  # type: ignore
 
     def tokens_to_track(
         self,
-        tokens: Union[TokSequence, List, np.ndarray, Any],
+        tokens: TokSequence,
         time_division: Optional[int] = TIME_DIVISION,
         program: Optional[Tuple[int, bool]] = (0, False),
     ) -> None:
         r"""NOT RELEVANT / IMPLEMENTED FOR REMIPlus
         Use tokens_to_midi instead
 
         :param tokens: sequence of tokens to convert. Can be either a Tensor (PyTorch and Tensorflow are supported),
```

### Comparing `miditok-2.1.1/miditok/tokenizations/structured.py` & `miditok-2.1.2/miditok/tokenizations/structured.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,18 +132,17 @@
                 )
             )
 
         events.sort(key=lambda x: x.time)
 
         return TokSequence(events=events)
 
-    @_in_as_seq()
     def tokens_to_track(
         self,
-        tokens: Union[TokSequence, List, np.ndarray, Any],
+        tokens: TokSequence,
         time_division: Optional[int] = TIME_DIVISION,
         program: Optional[Tuple[int, bool]] = (0, False),
     ) -> Tuple[Instrument, List[TempoChange]]:
         r"""Converts a sequence of tokens into a track object.
 
         :param tokens: sequence of tokens to convert. Can be either a Tensor (PyTorch and Tensorflow are supported),
                 a numpy array, a Python list or a TokSequence.
```

### Comparing `miditok-2.1.1/miditok/tokenizations/tsd.py` & `miditok-2.1.2/miditok/tokenizations/tsd.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     note, it could be unsuited for tracks with long pauses. In such case, the
     maximum *TimeShift* value will be used.
     """
 
     def _tweak_config_before_creating_voc(self):
         self.config.use_time_signatures = False
         if self.config.use_programs:
-            self.unique_track = True
+            self.one_token_stream = True
 
     def __notes_to_events(self, track: Instrument) -> List[Event]:
         r"""Converts notes of a track (``miditoolkit.Instrument``) into a sequence of `Event` objects.
 
         :param track: MIDI track to convert
         :return: sequence of corresponding Events
         """
@@ -197,24 +197,24 @@
 
     def _midi_to_tokens(
         self, midi: MidiFile, *args, **kwargs
     ) -> Union[TokSequence, List[TokSequence]]:
         r"""Converts a preprocessed MIDI object to a sequence of tokens.
 
         :param midi: the MIDI objet to convert.
-        :return: a :class:`miditok.TokSequence` if `tokenizer.unique_track` is true, else a list of
+        :return: a :class:`miditok.TokSequence` if `tokenizer.one_token_stream` is true, else a list of
                 :class:`miditok.TokSequence` objects.
         """
         # Convert each track to tokens
         all_events = []
 
         # Adds note tokens
         for track in midi.instruments:
             note_events = self.__notes_to_events(track)
-            if self.unique_track:
+            if self.one_token_stream:
                 all_events += note_events
             else:
                 all_events.append(note_events)
         # Adds tempo events if specified
         if self.config.use_tempos:
             tempo_events = []
             for tempo_change in self._current_midi_metadata["tempo_changes"]:
@@ -222,22 +222,22 @@
                     Event(
                         type="Tempo",
                         value=tempo_change.tempo,
                         time=tempo_change.time,
                         desc=tempo_change.tempo,
                     )
                 )
-            if self.unique_track:
+            if self.one_token_stream:
                 all_events += tempo_events
             else:
                 for i in range(len(all_events)):
                     all_events[i] += tempo_events
 
         # Add time events
-        if self.unique_track:
+        if self.one_token_stream:
             all_events.sort(key=lambda x: x.time)
             all_events = self.__add_time_note_events(all_events)
             tok_sequence = TokSequence(events=all_events)
             self.complete_sequence(tok_sequence)
         else:
             tok_sequence = []
             for i in range(len(all_events)):
@@ -246,15 +246,15 @@
                 tok_sequence.append(TokSequence(events=all_events[i]))
                 self.complete_sequence(tok_sequence[-1])
 
         return tok_sequence
 
     def tokens_to_track(
         self,
-        tokens: Union[TokSequence, List, np.ndarray, Any],
+        tokens: TokSequence,
         time_division: Optional[int] = TIME_DIVISION,
         program: Optional[Tuple[int, bool]] = (0, False),
     ) -> Tuple[Instrument, List[TempoChange]]:
         pass
 
     def track_to_tokens(self, track: Instrument) -> TokSequence:
         pass
@@ -262,28 +262,28 @@
     @_in_as_seq()
     def tokens_to_midi(
         self,
         tokens: Union[
             Union[TokSequence, List, np.ndarray, Any],
             List[Union[TokSequence, List, np.ndarray, Any]],
         ],
-        _=None,
+        programs: Optional[List[Tuple[int, bool]]] = None,
         output_path: Optional[str] = None,
         time_division: int = TIME_DIVISION,
     ) -> MidiFile:
         r"""Converts tokens (:class:`miditok.TokSequence`) into a MIDI and saves it.
 
         :param tokens: tokens to convert. Can be either a list of :class:`miditok.TokSequence`,
-        :param _: unused, to match parent method signature
+        :param programs: programs of the tracks. If none is given, will default to piano, program 0. (default: None)
         :param output_path: path to save the file. (default: None)
         :param time_division: MIDI time division / resolution, in ticks/beat (of the MIDI to create).
         :return: the midi object (:class:`miditoolkit.MidiFile`).
         """
-        # Unsqueeze tokens in case of unique_track
-        if self.unique_track:  # ie single token seq
+        # Unsqueeze tokens in case of one_token_stream
+        if self.one_token_stream:  # ie single token seq
             tokens = [tokens]
         for i in range(len(tokens)):
             tokens[i] = tokens[i].tokens
         midi = MidiFile(ticks_per_beat=time_division)
         assert (
             time_division % max(self.config.beat_res.values()) == 0
         ), f"Invalid time division, please give one divisible by {max(self.config.beat_res.values())}"
@@ -293,15 +293,23 @@
         instruments: Dict[int, Instrument] = {}
         tempo_changes = [TempoChange(TEMPO, -1)]
         time_signature_changes = [TimeSignature(*TIME_SIGNATURE, 0)]
 
         current_tick = 0
         current_program = 0
         previous_note_end = 0
-        for seq in tokens:
+        for si, seq in enumerate(tokens):
+            # Set track / sequence program if needed
+            if not self.one_token_stream:
+                current_tick = 0
+                previous_note_end = 0
+                if programs is not None:
+                    current_program = -1 if programs[si][1] else programs[si][0]
+
+            # Decode tokens
             for ti, token in enumerate(seq):
                 if token.split("_")[0] == "TimeShift":
                     current_tick += self._token_duration_to_ticks(
                         token.split("_")[1], time_division
                     )
                 elif token.split("_")[0] == "Rest":
                     beat, pos = map(int, seq[ti].split("_")[1].split("."))
```

### Comparing `miditok-2.1.1/miditok/utils/utils.py` & `miditok-2.1.2/miditok/utils/utils.py`

 * *Files identical despite different names*

### Comparing `miditok-2.1.1/miditok.egg-info/PKG-INFO` & `miditok-2.1.2/miditok.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miditok
-Version: 2.1.1
+Version: 2.1.2
 Summary: A convenient MIDI tokenizer for Deep Learning networks, with multiple encoding strategies
 Home-page: https://github.com/Natooz/MidiTok
 Author: Nathan Fradet
 License: MIT
 Keywords: artificial intelligence,deep learning,transformer,midi,tokenization,music,mir
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `miditok-2.1.1/miditok.egg-info/SOURCES.txt` & `miditok-2.1.2/miditok.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -22,13 +22,14 @@
 miditok/tokenizations/remi.py
 miditok/tokenizations/remi_plus.py
 miditok/tokenizations/structured.py
 miditok/tokenizations/tsd.py
 miditok/utils/__init__.py
 miditok/utils/utils.py
 tests/test_bpe.py
+tests/test_io_formats.py
 tests/test_methods.py
 tests/test_multitrack.py
 tests/test_one_track.py
 tests/test_saving_loading_config.py
 tests/test_utils.py
 tests/tests_utils.py
```

### Comparing `miditok-2.1.1/setup.py` & `miditok-2.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setup(
     name="miditok",
     author="Nathan Fradet",
     url="https://github.com/Natooz/MidiTok",
     packages=find_packages(exclude=("tests",)),
-    version="2.1.1",
+    version="2.1.2",
     license="MIT",
     description="A convenient MIDI tokenizer for Deep Learning networks, with multiple encoding strategies",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=[
         "artificial intelligence",
         "deep learning",
```

### Comparing `miditok-2.1.1/tests/test_bpe.py` & `miditok-2.1.2/tests/test_bpe.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         vocab_inv = {v: k for k, v in tokenizer._vocab_base.items()}
         assert (
             test_id_to_token == vocab_inv
         ), "Vocabulary inversion failed, something might be wrong with the way they are built"
 
         for file_path in files:
             tokens = tokenizer(file_path, apply_bpe_if_possible=False)
-            if not tokenizer.unique_track:
+            if not tokenizer.one_token_stream:
                 tokens = tokens[0]
             to_tok = tokenizer._bytes_to_tokens(tokens.bytes)
             to_id = tokenizer._tokens_to_ids(to_tok)
             to_by = tokenizer._ids_to_bytes(to_id, as_one_str=True)
             assert all(
                 [to_by == tokens.bytes, to_tok == tokens.tokens, to_id == tokens.ids]
             ), "Conversion between tokens / bytes / ids failed, something might be wrong in vocabularies"
@@ -108,15 +108,15 @@
     at_least_one_error = False
     tok_times = []
     for i, file_path in enumerate(tqdm(files, desc="Testing BPE unbatched")):
         midi = MidiFile(file_path)
 
         for tokenization, tokenizer in zip(tokenizations, tokenizers):
             tokens_no_bpe = tokenizer(deepcopy(midi), apply_bpe_if_possible=False)
-            if not tokenizer.unique_track:
+            if not tokenizer.one_token_stream:
                 tokens_no_bpe = tokens_no_bpe[0]
             tokens_bpe = deepcopy(tokens_no_bpe)  # with BPE
 
             t0 = time()
             tokenizer.apply_bpe(tokens_bpe)
             tok_times.append(time() - t0)
 
@@ -140,15 +140,15 @@
     at_least_one_error = False
     tok_times = []
     for tokenization, tokenizer in zip(tokenizations, tokenizers):
         samples_no_bpe = []
         for i, file_path in enumerate(tqdm(files, desc="Testing BPE batched")):
             # Reads the midi
             midi = MidiFile(file_path)
-            if not tokenizer.unique_track:
+            if not tokenizer.one_token_stream:
                 samples_no_bpe.append(tokenizer(midi, apply_bpe_if_possible=False)[0])
             else:
                 samples_no_bpe.append(tokenizer(midi, apply_bpe_if_possible=False))
 
         t0 = time()
         samples_bpe = deepcopy(samples_no_bpe)
         tokenizer.apply_bpe(samples_bpe)
```

### Comparing `miditok-2.1.1/tests/test_methods.py` & `miditok-2.1.2/tests/test_methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,27 +203,33 @@
                 file = json.load(json_file)
                 aug_tokens, aug_programs = file["ids"], file["programs"]
             with open(tokens_path / f"{original_stem}.json") as json_file:
                 file = json.load(json_file)
                 original_tokens, original_programs = file["ids"], file["programs"]
 
             # Compare them
-            if tokenizer.unique_track:
+            if tokenizer.one_token_stream:
                 original_tokens, aug_tokens = [original_tokens], [aug_tokens]
             for original_track, aug_track, (_, is_drum) in zip(
                 original_tokens, aug_tokens, original_programs
             ):
                 if is_drum:
                     continue
-                for idx, (original_token, aug_token) in enumerate(zip(original_track, aug_track)):
+                for idx, (original_token, aug_token) in enumerate(
+                    zip(original_track, aug_track)
+                ):
                     if not tokenizer.is_multi_voc:
                         if original_token in pitch_tokens:
                             pitch_offset = offsets[0]
                             # no offset for drum pitches
-                            if tokenizer.unique_track and idx > 0 and tokenizer[original_track[idx - 1]] == "Program_-1":
+                            if (
+                                tokenizer.one_token_stream
+                                and idx > 0
+                                and tokenizer[original_track[idx - 1]] == "Program_-1"
+                            ):
                                 pitch_offset = 0
                             assert aug_token == original_token + pitch_offset
                         elif original_token in vel_tokens:
                             assert aug_token in [
                                 original_token + offsets[1],
                                 tok_vel_min,
                                 tok_vel_max,
```

### Comparing `miditok-2.1.1/tests/test_multitrack.py` & `miditok-2.1.2/tests/test_multitrack.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,22 +101,19 @@
             for track in midi_to_compare.instruments:
                 if track.is_drum:
                     track.program = (
                         0  # need to be done before sorting tracks per program
                     )
 
             # Sort and merge tracks if needed
-            # MIDI produced with Octuple contains tracks ordered by program
-            if tokenizer.unique_track:
-                miditok.utils.merge_same_program_tracks(
-                    midi_to_compare.instruments
-                )  # merge tracks
-            for (
-                track
-            ) in midi_to_compare.instruments:  # reduce the duration of notes to long
+            # MIDI produced with one_token_stream contains tracks with different orders
+            if tokenizer.one_token_stream:
+                miditok.utils.merge_same_program_tracks(midi_to_compare.instruments)
+            # reduce the duration of notes to long
+            for track in midi_to_compare.instruments:
                 reduce_note_durations(
                     track.notes,
                     max(tu[1] for tu in BEAT_RES_TEST) * midi_to_compare.ticks_per_beat,
                 )
                 miditok.utils.remove_duplicated_notes(track.notes)
             if tokenization in ["Octuple", "REMIPlus"]:  # needed
                 adapt_tempo_changes_times(
@@ -133,15 +130,15 @@
                 miditok.utils.get_midi_programs(midi_to_compare),
                 time_division=midi_to_compare.ticks_per_beat,
             )
             new_midi.instruments.sort(key=lambda x: (x.program, x.is_drum))
 
             # Checks types and values conformity following the rules
             tokens_types = tokenizer.tokens_errors(
-                tokens[0] if not tokenizer.unique_track else tokens
+                tokens[0] if not tokenizer.one_token_stream else tokens
             )
             if tokens_types != 0.0:
                 print(
                     f"Validation of tokens types / values successions failed with {tokenization}: {tokens_types:.2f}"
                 )
 
             # Checks notes
```

### Comparing `miditok-2.1.1/tests/test_one_track.py` & `miditok-2.1.2/tests/test_one_track.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,17 +15,19 @@
 from typing import Union
 
 import miditok
 from miditoolkit import MidiFile, Marker
 from tqdm import tqdm
 
 from .tests_utils import (
+    ALL_TOKENIZATIONS,
     track_equals,
     tempo_changes_equals,
     time_signature_changes_equals,
+    adapt_tempo_changes_times,
 )
 
 # Special beat res for test, up to 64 beats so the duration and time-shift values are
 # long enough for MIDI-Like and Structured encodings, and with a single beat resolution
 BEAT_RES_TEST = {(0, 64): 8}
 TOKENIZER_PARAMS = {
     "beat_res": BEAT_RES_TEST,
@@ -51,36 +53,25 @@
     r"""Reads a few MIDI files, convert them into token sequences, convert them back to MIDI files.
     The converted back MIDI files should identical to original one, expect with note starting and ending
     times quantized, and maybe a some duplicated notes removed
 
     :param data_path: root path to the data to test
     :param saving_erroneous_midis: will save MIDIs converted back with errors, to be used to debug
     """
-    tokenizations = [
-        "MIDILike",
-        "TSD",
-        "Structured",
-        "REMI",
-        "REMIPlus",
-        "CPWord",
-        "Octuple",
-        "OctupleMono",
-        "MuMIDI",
-        "MMM",
-    ]
     files = list(Path(data_path).glob("**/*.mid"))
     at_least_one_error = False
 
     for i, file_path in enumerate(tqdm(files, desc="Testing One Track")):
         # Reads the midi
         midi = MidiFile(file_path)
+        adapt_tempo_changes_times(midi.instruments, midi.tempo_changes)
         tracks = [deepcopy(midi.instruments[0])]
         has_errors = False
 
-        for tokenization in tokenizations:
+        for tokenization in ALL_TOKENIZATIONS:
             tokenizer_config = miditok.TokenizerConfig(**TOKENIZER_PARAMS)
             # Increase the number of rest just to cover very long pauses / rests in test examples
             if tokenization in ["MIDILike", "TSD"]:
                 tokenizer_config.rest_range = (
                     tokenizer_config.rest_range[0],
                     max(t[1] for t in BEAT_RES_TEST),
                 )
@@ -89,43 +80,35 @@
             )
 
             # printing the tokenizer shouldn't fail
             _ = str(tokenizer)
 
             # Convert the track in tokens
             tokens = tokenizer(midi)
-            if (
-                not tokenizer.unique_track or tokenization == "TSD"
-            ):  # or isinstance list
+            if not tokenizer.one_token_stream:
                 tokens = tokens[0]
 
             # Checks types and values conformity following the rules
             tokens_types = tokenizer.tokens_errors(tokens)
             if tokens_types != 0.0:
                 print(
                     f"Validation of tokens types / values successions failed with {tokenization}: {tokens_types:.2f}"
                 )
 
             # Convert back tokens into a track object
-            tempo_changes = None
+            if not tokenizer.one_token_stream:
+                tokens = [tokens]
+            new_midi = tokenizer.tokens_to_midi(
+                tokens, time_division=midi.ticks_per_beat
+            )
+            track = new_midi.instruments[0]
+            tempo_changes = new_midi.tempo_changes
             time_sig_changes = None
-            if tokenizer.unique_track or tokenization == "TSD":
-                if tokenization == "TSD":
-                    tokens = [tokens]
-                new_midi = tokenizer.tokens_to_midi(
-                    tokens, time_division=midi.ticks_per_beat
-                )
-                track = new_midi.instruments[0]
-                if tokenization == "Octuple":
-                    tempo_changes = new_midi.tempo_changes
-                    time_sig_changes = new_midi.time_signature_changes
-            else:
-                track, tempo_changes = tokenizer.tokens_to_track(
-                    tokens, midi.ticks_per_beat
-                )
+            if tokenization == "Octuple":
+                time_sig_changes = new_midi.time_signature_changes
 
             # Checks its good
             errors = track_equals(midi.instruments[0], track)
             if len(errors) > 0:
                 has_errors = True
                 if errors[0][0] != "len":
                     for err, note, exp in errors:
```

### Comparing `miditok-2.1.1/tests/test_saving_loading_config.py` & `miditok-2.1.2/tests/test_saving_loading_config.py`

 * *Files identical despite different names*

### Comparing `miditok-2.1.1/tests/test_utils.py` & `miditok-2.1.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `miditok-2.1.1/tests/tests_utils.py` & `miditok-2.1.2/tests/tests_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,28 @@
 """
 
 from typing import Tuple, List, Union
 
 from miditoolkit import MidiFile, Instrument, Note, TempoChange, TimeSignature
 
 
+ALL_TOKENIZATIONS = [
+    "MIDILike",
+    "TSD",
+    "Structured",
+    "REMI",
+    "REMIPlus",
+    "CPWord",
+    "Octuple",
+    "OctupleMono",
+    "MuMIDI",
+    "MMM",
+]
+
+
 def midis_equals(
     midi1: MidiFile, midi2: MidiFile
 ) -> List[Tuple[int, str, List[Tuple[str, Union[Note, int], int]]]]:
     errors = []
     for track1, track2 in zip(midi1.instruments, midi2.instruments):
         track_errors = track_equals(track1, track2)
         if len(track_errors) > 0:
```

