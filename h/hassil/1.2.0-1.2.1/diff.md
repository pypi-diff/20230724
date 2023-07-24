# Comparing `tmp/hassil-1.2.0.tar.gz` & `tmp/hassil-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hassil-1.2.0.tar", last modified: Mon Jul 24 20:04:23 2023, max compression
+gzip compressed data, was "hassil-1.2.1.tar", last modified: Mon Jul 24 21:51:36 2023, max compression
```

## Comparing `hassil-1.2.0.tar` & `hassil-1.2.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-24 20:04:23.934606 hassil-1.2.0/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      689 2023-01-23 19:07:47.000000 hassil-1.2.0/HassILGrammar.g4
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11357 2022-12-05 18:00:35.000000 hassil-1.2.0/LICENSE.md
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      196 2022-12-20 17:37:34.000000 hassil-1.2.0/MANIFEST.in
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4426 2023-07-24 20:04:23.934606 hassil-1.2.0/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3687 2023-07-21 19:48:31.000000 hassil-1.2.0/README.md
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-24 20:04:23.934606 hassil-1.2.0/hassil/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        6 2023-07-21 19:48:05.000000 hassil-1.2.0/hassil/VERSION
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      304 2023-02-01 04:31:35.000000 hassil-1.2.0/hassil/__init__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2552 2023-01-23 19:07:47.000000 hassil-1.2.0/hassil/__main__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      468 2022-12-15 16:06:23.000000 hassil-1.2.0/hassil/_resources.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2279 2023-02-10 20:55:51.000000 hassil-1.2.0/hassil/expression.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    10271 2023-07-20 21:44:34.000000 hassil-1.2.0/hassil/intents.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5388 2023-02-10 20:53:50.000000 hassil-1.2.0/hassil/parse_expression.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7763 2023-02-01 04:31:35.000000 hassil-1.2.0/hassil/parser.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        0 2022-12-15 16:07:59.000000 hassil-1.2.0/hassil/py.typed
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    33150 2023-07-24 19:52:55.000000 hassil-1.2.0/hassil/recognize.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7448 2023-02-10 20:53:57.000000 hassil-1.2.0/hassil/sample.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      783 2023-02-01 04:31:35.000000 hassil-1.2.0/hassil/sample_template.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1725 2023-01-23 19:07:47.000000 hassil-1.2.0/hassil/util.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-24 20:04:23.934606 hassil-1.2.0/hassil.egg-info/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4426 2023-07-24 20:04:23.000000 hassil-1.2.0/hassil.egg-info/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      689 2023-07-24 20:04:23.000000 hassil-1.2.0/hassil.egg-info/SOURCES.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-07-24 20:04:23.000000 hassil-1.2.0/hassil.egg-info/dependency_links.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       48 2023-07-24 20:04:23.000000 hassil-1.2.0/hassil.egg-info/entry_points.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       60 2023-07-24 20:04:23.000000 hassil-1.2.0/hassil.egg-info/requires.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        7 2023-07-24 20:04:23.000000 hassil-1.2.0/hassil.egg-info/top_level.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       15 2023-02-01 04:31:35.000000 hassil-1.2.0/requirements.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       69 2023-07-17 19:53:41.000000 hassil-1.2.0/requirements_dev.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      295 2023-07-24 20:04:23.934606 hassil-1.2.0/setup.cfg
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2069 2023-02-10 21:31:32.000000 hassil-1.2.0/setup.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-24 20:04:23.934606 hassil-1.2.0/tests/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       63 2022-12-07 21:08:40.000000 hassil-1.2.0/tests/__init__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2812 2023-02-01 04:31:35.000000 hassil-1.2.0/tests/test_expression.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4469 2023-02-06 16:37:52.000000 hassil-1.2.0/tests/test_intents.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1755 2023-02-01 04:31:35.000000 hassil-1.2.0/tests/test_parser.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    16282 2023-07-21 16:46:01.000000 hassil-1.2.0/tests/test_recognize.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1906 2023-02-01 04:31:35.000000 hassil-1.2.0/tests/test_sample.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      913 2023-01-23 19:07:47.000000 hassil-1.2.0/tests/test_util.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-24 21:51:36.274543 hassil-1.2.1/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      689 2023-01-23 19:07:47.000000 hassil-1.2.1/HassILGrammar.g4
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11357 2022-12-05 18:00:35.000000 hassil-1.2.1/LICENSE.md
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      196 2022-12-20 17:37:34.000000 hassil-1.2.1/MANIFEST.in
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4547 2023-07-24 21:51:36.274543 hassil-1.2.1/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3808 2023-07-24 20:05:10.000000 hassil-1.2.1/README.md
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-24 21:51:36.274543 hassil-1.2.1/hassil/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        6 2023-07-24 21:46:25.000000 hassil-1.2.1/hassil/VERSION
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      304 2023-02-01 04:31:35.000000 hassil-1.2.1/hassil/__init__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2552 2023-01-23 19:07:47.000000 hassil-1.2.1/hassil/__main__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      468 2022-12-15 16:06:23.000000 hassil-1.2.1/hassil/_resources.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2355 2023-07-24 20:05:10.000000 hassil-1.2.1/hassil/expression.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    10271 2023-07-24 20:05:10.000000 hassil-1.2.1/hassil/intents.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     6797 2023-07-24 20:05:10.000000 hassil-1.2.1/hassil/parse_expression.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     8111 2023-07-24 20:05:10.000000 hassil-1.2.1/hassil/parser.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        0 2022-12-15 16:07:59.000000 hassil-1.2.1/hassil/py.typed
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    34854 2023-07-24 21:50:30.000000 hassil-1.2.1/hassil/recognize.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7448 2023-02-10 20:53:57.000000 hassil-1.2.1/hassil/sample.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      783 2023-02-01 04:31:35.000000 hassil-1.2.1/hassil/sample_template.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1725 2023-01-23 19:07:47.000000 hassil-1.2.1/hassil/util.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-24 21:51:36.274543 hassil-1.2.1/hassil.egg-info/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4547 2023-07-24 21:51:36.000000 hassil-1.2.1/hassil.egg-info/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      689 2023-07-24 21:51:36.000000 hassil-1.2.1/hassil.egg-info/SOURCES.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-07-24 21:51:36.000000 hassil-1.2.1/hassil.egg-info/dependency_links.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       48 2023-07-24 21:51:36.000000 hassil-1.2.1/hassil.egg-info/entry_points.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       60 2023-07-24 21:51:36.000000 hassil-1.2.1/hassil.egg-info/requires.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        7 2023-07-24 21:51:36.000000 hassil-1.2.1/hassil.egg-info/top_level.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       15 2023-02-01 04:31:35.000000 hassil-1.2.1/requirements.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       69 2023-07-17 19:53:41.000000 hassil-1.2.1/requirements_dev.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      295 2023-07-24 21:51:36.274543 hassil-1.2.1/setup.cfg
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2069 2023-02-10 21:31:32.000000 hassil-1.2.1/setup.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-24 21:51:36.274543 hassil-1.2.1/tests/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       63 2022-12-07 21:08:40.000000 hassil-1.2.1/tests/__init__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3500 2023-07-24 20:05:10.000000 hassil-1.2.1/tests/test_expression.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4687 2023-07-24 20:05:10.000000 hassil-1.2.1/tests/test_intents.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1755 2023-02-01 04:31:35.000000 hassil-1.2.1/tests/test_parser.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    17123 2023-07-24 21:50:53.000000 hassil-1.2.1/tests/test_recognize.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1906 2023-02-01 04:31:35.000000 hassil-1.2.1/tests/test_sample.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      913 2023-01-23 19:07:47.000000 hassil-1.2.1/tests/test_util.py
```

### Comparing `hassil-1.2.0/HassILGrammar.g4` & `hassil-1.2.1/HassILGrammar.g4`

 * *Files identical despite different names*

### Comparing `hassil-1.2.0/LICENSE.md` & `hassil-1.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hassil-1.2.0/PKG-INFO` & `hassil-1.2.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hassil
-Version: 1.2.0
+Version: 1.2.1
 Summary: The Home Assistant Intent Language parser
 Home-page: http://github.com/home-assistant/hassil
 Author: Michael Hansen
 Author-email: mike@rhasspy.org
 License: Apache-2.0
 Keywords: home assistant intent recognition
 Classifier: Development Status :: 3 - Alpha
@@ -84,14 +84,17 @@
 * Alternative words or phrases
   * `(red | green | blue)`
   * `turn(s | ed | ing)`
 * Optional words or phrases
   * `[the]`
   * `[this | that]`
   * `light[s]`
+* Permutations of words or phrases
+  * `(patience; you must have) my young Padawan`
+  * `is [the] light (on; in <area>)`
 * Slot Lists
   * `{list_name}`
   * `{list_name:slot_name}`
   * Refers to a pre-defined list of values in YAML (`lists`)
 * Expansion Rules
   * `<rule_name>`
   * Refers to a pre-defined expansion rule in YAML (`expansion_rules`), either global or local (particular to the intent to which the sentence refers)
```

### Comparing `hassil-1.2.0/README.md` & `hassil-1.2.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -64,14 +64,17 @@
 * Alternative words or phrases
   * `(red | green | blue)`
   * `turn(s | ed | ing)`
 * Optional words or phrases
   * `[the]`
   * `[this | that]`
   * `light[s]`
+* Permutations of words or phrases
+  * `(patience; you must have) my young Padawan`
+  * `is [the] light (on; in <area>)`
 * Slot Lists
   * `{list_name}`
   * `{list_name:slot_name}`
   * Refers to a pre-defined list of values in YAML (`lists`)
 * Expansion Rules
   * `<rule_name>`
   * Refers to a pre-defined expansion rule in YAML (`expansion_rules`), either global or local (particular to the intent to which the sentence refers)
```

### Comparing `hassil-1.2.0/hassil/__main__.py` & `hassil-1.2.1/hassil/__main__.py`

 * *Files identical despite different names*

### Comparing `hassil-1.2.0/hassil/expression.py` & `hassil-1.2.1/hassil/expression.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,17 @@
 
     # Sequence of expressions
     GROUP = "group"
 
     # Expressions where only one will be recognized
     ALTERNATIVE = "alternative"
 
+    # Permutations of a set of expressions
+    PERMUTATION = "permutation"
+
 
 @dataclass
 class Sequence(Expression):
     """Ordered sequence of expressions. Supports groups, optionals, and alternatives."""
 
     # Items in the sequence
     items: List[Expression] = field(default_factory=list)
```

### Comparing `hassil-1.2.0/hassil/intents.py` & `hassil-1.2.1/hassil/intents.py`

 * *Files identical despite different names*

### Comparing `hassil-1.2.0/hassil/parse_expression.py` & `hassil-1.2.1/hassil/parse_expression.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from dataclasses import dataclass
-from typing import Optional
+from itertools import permutations
+from typing import List, Optional
 
 from .expression import (
     Expression,
     ListReference,
     RuleReference,
     Sentence,
     Sequence,
@@ -56,15 +57,28 @@
             Sequence(
                 type=SequenceType.GROUP,
                 items=seq.items,
             )
         ]
 
 
-def parse_group_or_alt(
+def ensure_permutation(seq: Sequence):
+    if seq.type != SequenceType.PERMUTATION:
+        seq.type = SequenceType.PERMUTATION
+
+        # Collapse items into a single group
+        seq.items = [
+            Sequence(
+                type=SequenceType.GROUP,
+                items=seq.items,
+            )
+        ]
+
+
+def parse_group_or_alt_or_perm(
     seq_chunk: ParseChunk, metadata: Optional[ParseMetadata] = None
 ) -> Sequence:
     seq = Sequence(type=SequenceType.GROUP)
     if seq_chunk.parse_type == ParseType.GROUP:
         seq_text = remove_delimiters(seq_chunk.text, GROUP_START, GROUP_END)
     elif seq_chunk.parse_type == ParseType.OPT:
         seq_text = remove_delimiters(seq_chunk.text, OPT_START, OPT_END)
@@ -80,15 +94,15 @@
             ParseType.GROUP,
             ParseType.OPT,
             ParseType.LIST,
             ParseType.RULE,
         ):
             item = parse_expression(item_chunk, metadata=metadata)
 
-            if seq.type == SequenceType.ALTERNATIVE:
+            if seq.type in (SequenceType.ALTERNATIVE, SequenceType.PERMUTATION):
                 # Add to most recent group
                 if not seq.items:
                     seq.items.append(Sequence(type=SequenceType.GROUP))
 
                 # Must be group or alternative
                 last_item = seq.items[-1]
                 if not isinstance(last_item, Sequence):
@@ -99,41 +113,57 @@
                 # Add to parent group
                 seq.items.append(item)
         elif item_chunk.parse_type == ParseType.ALT:
             ensure_alternative(seq)
 
             # Begin new group
             seq.items.append(Sequence(type=SequenceType.GROUP))
+        elif item_chunk.parse_type == ParseType.PERM:
+            ensure_permutation(seq)
+
+            # Begin new group
+            seq.items.append(Sequence(type=SequenceType.GROUP))
         else:
             raise ParseExpressionError(seq_chunk, metadata=metadata)
 
         # Next chunk
         seq_text = seq_text[item_chunk.end_index :]
 
         if seq_text == last_seq_text:
             # No change, unable to proceed
             raise ParseExpressionError(seq_chunk, metadata=metadata)
 
         item_chunk = next_chunk(seq_text)
         last_seq_text = seq_text
 
+    if seq.type == SequenceType.PERMUTATION:
+        permuted_items: List[Expression] = []
+
+        for permutation in permutations(seq.items):
+            permutation_with_spaces = add_spaces_between_items(list(permutation))
+            permuted_items.append(
+                Sequence(type=SequenceType.GROUP, items=permutation_with_spaces)
+            )
+
+        seq = Sequence(type=SequenceType.ALTERNATIVE, items=permuted_items)
+
     return seq
 
 
 def parse_expression(
     chunk: ParseChunk, metadata: Optional[ParseMetadata] = None
 ) -> Expression:
     if chunk.parse_type == ParseType.WORD:
         return TextChunk(text=normalize_text(chunk.text), original_text=chunk.text)
 
     if chunk.parse_type == ParseType.GROUP:
-        return parse_group_or_alt(chunk, metadata=metadata)
+        return parse_group_or_alt_or_perm(chunk, metadata=metadata)
 
     if chunk.parse_type == ParseType.OPT:
-        seq = parse_group_or_alt(chunk, metadata=metadata)
+        seq = parse_group_or_alt_or_perm(chunk, metadata=metadata)
         ensure_alternative(seq)
         seq.items.append(TextChunk(text=""))
         return seq
 
     if chunk.parse_type == ParseType.LIST:
         return ListReference(
             list_name=remove_delimiters(chunk.text, LIST_START, LIST_END),
@@ -183,7 +213,21 @@
         first_item = seq.items[0]
         if isinstance(first_item, Sequence):
             seq = first_item
 
     return Sentence(
         type=seq.type, items=seq.items, text=original_text if keep_text else None
     )
+
+
+def add_spaces_between_items(items: List[Expression]) -> List[Expression]:
+    """Add spaces between each 2 items of a sequence, used for permutations"""
+
+    spaced_items: List[Expression] = []
+
+    for item in items:
+        spaced_items = spaced_items + [TextChunk(text=" ")] + [item]
+
+    spaced_items.append(TextChunk(text=" "))
+    items = spaced_items
+
+    return items
```

### Comparing `hassil-1.2.0/hassil/parser.py` & `hassil-1.2.1/hassil/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,23 +19,25 @@
     RULE_START: RULE_END,
 }
 DELIM_START = tuple(DELIM.keys())
 DELIM_END = tuple(DELIM.values())
 
 WORD_SEP = " "
 ALT_SEP = "|"
+PERM_SEP = ";"
 ESCAPE_CHAR = "\\"
 
 
 class ParseType(Enum):
     """Parse chunk types."""
 
     GROUP = auto()
     OPT = auto()
     ALT = auto()
+    PERM = auto()
     RULE = auto()
     LIST = auto()
     WORD = auto()
     END = auto()
 
 
 @dataclass
@@ -100,15 +102,15 @@
             separator_found = True
             continue
 
         if separator_found and (c != WORD_SEP):
             # Start of next word
             return start_index + i
 
-        if (c == ALT_SEP) or (c in DELIM_START) or (c in DELIM_END):
+        if (c == ALT_SEP) or (c == PERM_SEP) or (c in DELIM_START) or (c in DELIM_END):
             return start_index + i
 
     if text:
         # Entire text is a word
         return start_index + len(text)
 
     return None
@@ -125,14 +127,17 @@
 
     if c == OPT_START:
         return ParseType.OPT
 
     if c == ALT_SEP:
         return ParseType.ALT
 
+    if c == PERM_SEP:
+        return ParseType.PERM
+
     if c == LIST_START:
         return ParseType.LIST
 
     if c == RULE_START:
         return ParseType.RULE
 
     return ParseType.WORD
@@ -270,14 +275,22 @@
         return ParseChunk(
             text=text[start_index : start_index + 1],
             start_index=start_index,
             end_index=start_index + 1,
             parse_type=ParseType.ALT,
         )
 
+    if next_type == ParseType.PERM:
+        return ParseChunk(
+            text=text[start_index : start_index + 1],
+            start_index=start_index,
+            end_index=start_index + 1,
+            parse_type=ParseType.PERM,
+        )
+
     return None
 
 
 def remove_delimiters(
     text: str, start_char: str, end_char: Optional[str] = None
 ) -> str:
     """Removes the surrounding delimiters in text."""
```

### Comparing `hassil-1.2.0/hassil/recognize.py` & `hassil-1.2.1/hassil/recognize.py`

 * *Files 2% similar despite different names*

```diff
@@ -369,14 +369,45 @@
                     text=text,
                     intent_context=intent_context,
                 )
                 maybe_match_contexts = match_expression(
                     local_settings, match_context, intent_sentence
                 )
                 for maybe_match_context in maybe_match_contexts:
+                    # Close any open wildcards or unmatched entities
+                    final_text = maybe_match_context.text.strip()
+                    if final_text:
+                        if (
+                            maybe_match_context.unmatched_entities
+                            and isinstance(
+                                maybe_match_context.unmatched_entities[-1],
+                                UnmatchedTextEntity,
+                            )
+                            and maybe_match_context.unmatched_entities[-1].is_open
+                        ):
+                            # Consume the rest of the text (unmatched entity)
+                            unmatched_entity = cast(
+                                UnmatchedTextEntity,
+                                maybe_match_context.unmatched_entities[-1],
+                            )
+                            unmatched_entity.text += final_text
+                            unmatched_entity.is_open = False
+                            maybe_match_context.text = ""
+                        elif (
+                            maybe_match_context.entities
+                            and maybe_match_context.entities[-1].is_wildcard
+                            and maybe_match_context.entities[-1].is_wildcard_open
+                        ):
+                            # Consume the rest of the text (wildcard)
+                            wildcard = maybe_match_context.entities[-1]
+                            wildcard.text += final_text
+                            wildcard.value = wildcard.text
+                            wildcard.is_wildcard_open = False
+                            maybe_match_context.text = ""
+
                     if not maybe_match_context.is_match:
                         # Incomplete match with text still left at the end
                         continue
 
                     skip_match = False
 
                     # Verify excluded context
```

### Comparing `hassil-1.2.0/hassil/sample.py` & `hassil-1.2.1/hassil/sample.py`

 * *Files identical despite different names*

### Comparing `hassil-1.2.0/hassil/sample_template.py` & `hassil-1.2.1/hassil/sample_template.py`

 * *Files identical despite different names*

### Comparing `hassil-1.2.0/hassil/util.py` & `hassil-1.2.1/hassil/util.py`

 * *Files identical despite different names*

### Comparing `hassil-1.2.0/hassil.egg-info/PKG-INFO` & `hassil-1.2.1/hassil.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hassil
-Version: 1.2.0
+Version: 1.2.1
 Summary: The Home Assistant Intent Language parser
 Home-page: http://github.com/home-assistant/hassil
 Author: Michael Hansen
 Author-email: mike@rhasspy.org
 License: Apache-2.0
 Keywords: home assistant intent recognition
 Classifier: Development Status :: 3 - Alpha
@@ -84,14 +84,17 @@
 * Alternative words or phrases
   * `(red | green | blue)`
   * `turn(s | ed | ing)`
 * Optional words or phrases
   * `[the]`
   * `[this | that]`
   * `light[s]`
+* Permutations of words or phrases
+  * `(patience; you must have) my young Padawan`
+  * `is [the] light (on; in <area>)`
 * Slot Lists
   * `{list_name}`
   * `{list_name:slot_name}`
   * Refers to a pre-defined list of values in YAML (`lists`)
 * Expansion Rules
   * `<rule_name>`
   * Refers to a pre-defined expansion rule in YAML (`expansion_rules`), either global or local (particular to the intent to which the sentence refers)
```

### Comparing `hassil-1.2.0/hassil.egg-info/SOURCES.txt` & `hassil-1.2.1/hassil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hassil-1.2.0/setup.py` & `hassil-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `hassil-1.2.0/tests/test_expression.py` & `hassil-1.2.1/tests/test_expression.py`

 * *Files 26% similar despite different names*

```diff
@@ -35,14 +35,39 @@
 
 def test_group_alternative():
     assert parse_expression(next_chunk("(test | test2)")) == alt(
         items=[group(items=[t(text="test ")]), group(items=[t(text=" test2")])],
     )
 
 
+def test_group_permutation():
+    assert parse_expression(next_chunk("(test; test2)")) == alt(
+        items=[
+            group(
+                items=[
+                    t(text=" "),
+                    group(items=[t(text="test")]),
+                    t(text=" "),
+                    group(items=[t(text=" test2")]),
+                    t(text=" "),
+                ]
+            ),
+            group(
+                items=[
+                    t(text=" "),
+                    group(items=[t(text=" test2")]),
+                    t(text=" "),
+                    group(items=[t(text="test")]),
+                    t(text=" "),
+                ]
+            ),
+        ],
+    )
+
+
 def test_slot_reference():
     assert parse_expression(next_chunk("{test}")) == ListReference(list_name="test")
 
 
 def test_rule_reference():
     assert parse_expression(next_chunk("<test>")) == RuleReference(rule_name="test")
```

### Comparing `hassil-1.2.0/tests/test_intents.py` & `hassil-1.2.1/tests/test_intents.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,20 @@
 
 
 def test_no_whitespace_fails():
     sentence = parse_sentence("this is a test")
     assert not is_match("thisisatest", sentence)
 
 
+def test_permutations():
+    sentence = parse_sentence("(in the kitchen;is there smoke)")
+    assert is_match("in the kitchen is there smoke", sentence)
+    assert is_match("is there smoke in the kitchen", sentence)
+
+
 def test_nl_optional_whitespace():
     sentence = parse_sentence(
         "[<doe>] (alle|in) <area>[ ]<lamp> aan [willen | kunnen] [<doe>]"
     )
     slot_lists = {
         "area": TextSlotList.from_strings(["Keuken", "Woonkamer"], allow_template=False)
     }
```

### Comparing `hassil-1.2.0/tests/test_parser.py` & `hassil-1.2.1/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `hassil-1.2.0/tests/test_recognize.py` & `hassil-1.2.1/tests/test_recognize.py`

 * *Files 2% similar despite different names*

```diff
@@ -521,14 +521,15 @@
     yaml_text = """
     language: "en"
     intents:
       Test:
         data:
           - sentences:
               - "set [all] {domain} in {area} to {percent}[%] now"
+              - "set {area} {domain} to {percent}"
     lists:
       area:
         values:
           - kitchen
           - bedroom
       domain:
         values:
@@ -570,24 +571,35 @@
     assert result is not None, f"{sentence} should match"
     assert set(result.unmatched_entities.keys()) == {"percent"}
 
     percent = result.unmatched_entities["percent"]
     assert isinstance(percent, UnmatchedTextEntity)
     assert percent.text == "blah blah blah "
 
+    # Test with unmatched entity at end of sentence
+    sentence = "set kitchen lights to fifty"
+    result = recognize(sentence, intents, allow_unmatched_entities=True)
+    assert result is not None, f"{sentence} should match"
+    assert set(result.unmatched_entities.keys()) == {"percent"}
+
+    percent = result.unmatched_entities["percent"]
+    assert isinstance(percent, UnmatchedTextEntity)
+    assert percent.text == "fifty"
+
 
 def test_wildcard() -> None:
     """Test wildcard slot lists/entities."""
     yaml_text = """
     language: "en"
     intents:
       Test:
         data:
           - sentences:
               - "play {album} by {artist} [please] now"
+              - "start {album} by {artist}"
     lists:
       album:
         wildcard: true
       artist:
         wildcard: true
     """
 
@@ -600,7 +612,14 @@
     assert result.entities["album"].value == "the white album "
     assert result.entities["artist"].value == "the beatles "
 
     # Wildcards cannot be empty
     sentence = "play by please now"
     result = recognize(sentence, intents)
     assert result is None, f"{sentence} should not match"
+
+    # Test without text at the end
+    sentence = "start the white album by the beatles"
+    result = recognize(sentence, intents)
+    assert result is not None, f"{sentence} should match"
+    assert result.entities["album"].value == "the white album "
+    assert result.entities["artist"].value == "the beatles"
```

### Comparing `hassil-1.2.0/tests/test_sample.py` & `hassil-1.2.1/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `hassil-1.2.0/tests/test_util.py` & `hassil-1.2.1/tests/test_util.py`

 * *Files identical despite different names*

