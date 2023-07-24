# Comparing `tmp/hassil-1.1.0.tar.gz` & `tmp/hassil-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hassil-1.1.0.tar", last modified: Mon Jul 17 19:55:25 2023, max compression
+gzip compressed data, was "hassil-1.2.0.tar", last modified: Mon Jul 24 20:04:23 2023, max compression
```

## Comparing `hassil-1.1.0.tar` & `hassil-1.2.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-17 19:55:25.475653 hassil-1.1.0/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      689 2023-01-23 19:07:47.000000 hassil-1.1.0/HassILGrammar.g4
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11357 2022-12-05 18:00:35.000000 hassil-1.1.0/LICENSE.md
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      196 2022-12-20 17:37:34.000000 hassil-1.1.0/MANIFEST.in
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4389 2023-07-17 19:55:25.475653 hassil-1.1.0/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3650 2023-05-25 21:44:27.000000 hassil-1.1.0/README.md
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-17 19:55:25.475653 hassil-1.1.0/hassil/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        6 2023-07-17 19:54:35.000000 hassil-1.1.0/hassil/VERSION
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      304 2023-02-01 04:31:35.000000 hassil-1.1.0/hassil/__init__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2552 2023-01-23 19:07:47.000000 hassil-1.1.0/hassil/__main__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      468 2022-12-15 16:06:23.000000 hassil-1.1.0/hassil/_resources.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2279 2023-02-10 20:55:51.000000 hassil-1.1.0/hassil/expression.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    10085 2023-06-15 16:06:29.000000 hassil-1.1.0/hassil/intents.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5388 2023-02-10 20:53:50.000000 hassil-1.1.0/hassil/parse_expression.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7763 2023-02-01 04:31:35.000000 hassil-1.1.0/hassil/parser.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        0 2022-12-15 16:07:59.000000 hassil-1.1.0/hassil/py.typed
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    23303 2023-06-15 16:06:29.000000 hassil-1.1.0/hassil/recognize.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7448 2023-02-10 20:53:57.000000 hassil-1.1.0/hassil/sample.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      783 2023-02-01 04:31:35.000000 hassil-1.1.0/hassil/sample_template.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1725 2023-01-23 19:07:47.000000 hassil-1.1.0/hassil/util.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-17 19:55:25.475653 hassil-1.1.0/hassil.egg-info/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4389 2023-07-17 19:55:25.000000 hassil-1.1.0/hassil.egg-info/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      689 2023-07-17 19:55:25.000000 hassil-1.1.0/hassil.egg-info/SOURCES.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-07-17 19:55:25.000000 hassil-1.1.0/hassil.egg-info/dependency_links.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       48 2023-07-17 19:55:25.000000 hassil-1.1.0/hassil.egg-info/entry_points.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       60 2023-07-17 19:55:25.000000 hassil-1.1.0/hassil.egg-info/requires.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        7 2023-07-17 19:55:25.000000 hassil-1.1.0/hassil.egg-info/top_level.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       15 2023-02-01 04:31:35.000000 hassil-1.1.0/requirements.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       69 2023-07-17 19:53:41.000000 hassil-1.1.0/requirements_dev.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      295 2023-07-17 19:55:25.479653 hassil-1.1.0/setup.cfg
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2069 2023-02-10 21:31:32.000000 hassil-1.1.0/setup.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-17 19:55:25.475653 hassil-1.1.0/tests/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       63 2022-12-07 21:08:40.000000 hassil-1.1.0/tests/__init__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2812 2023-02-01 04:31:35.000000 hassil-1.1.0/tests/test_expression.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4469 2023-02-06 16:37:52.000000 hassil-1.1.0/tests/test_intents.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1755 2023-02-01 04:31:35.000000 hassil-1.1.0/tests/test_parser.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    13434 2023-06-15 16:06:29.000000 hassil-1.1.0/tests/test_recognize.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1906 2023-02-01 04:31:35.000000 hassil-1.1.0/tests/test_sample.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      913 2023-01-23 19:07:47.000000 hassil-1.1.0/tests/test_util.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-24 20:04:23.934606 hassil-1.2.0/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      689 2023-01-23 19:07:47.000000 hassil-1.2.0/HassILGrammar.g4
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11357 2022-12-05 18:00:35.000000 hassil-1.2.0/LICENSE.md
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      196 2022-12-20 17:37:34.000000 hassil-1.2.0/MANIFEST.in
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4426 2023-07-24 20:04:23.934606 hassil-1.2.0/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3687 2023-07-21 19:48:31.000000 hassil-1.2.0/README.md
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-24 20:04:23.934606 hassil-1.2.0/hassil/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        6 2023-07-21 19:48:05.000000 hassil-1.2.0/hassil/VERSION
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      304 2023-02-01 04:31:35.000000 hassil-1.2.0/hassil/__init__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2552 2023-01-23 19:07:47.000000 hassil-1.2.0/hassil/__main__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      468 2022-12-15 16:06:23.000000 hassil-1.2.0/hassil/_resources.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2279 2023-02-10 20:55:51.000000 hassil-1.2.0/hassil/expression.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    10271 2023-07-20 21:44:34.000000 hassil-1.2.0/hassil/intents.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5388 2023-02-10 20:53:50.000000 hassil-1.2.0/hassil/parse_expression.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7763 2023-02-01 04:31:35.000000 hassil-1.2.0/hassil/parser.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        0 2022-12-15 16:07:59.000000 hassil-1.2.0/hassil/py.typed
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    33150 2023-07-24 19:52:55.000000 hassil-1.2.0/hassil/recognize.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7448 2023-02-10 20:53:57.000000 hassil-1.2.0/hassil/sample.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      783 2023-02-01 04:31:35.000000 hassil-1.2.0/hassil/sample_template.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1725 2023-01-23 19:07:47.000000 hassil-1.2.0/hassil/util.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-24 20:04:23.934606 hassil-1.2.0/hassil.egg-info/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4426 2023-07-24 20:04:23.000000 hassil-1.2.0/hassil.egg-info/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      689 2023-07-24 20:04:23.000000 hassil-1.2.0/hassil.egg-info/SOURCES.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-07-24 20:04:23.000000 hassil-1.2.0/hassil.egg-info/dependency_links.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       48 2023-07-24 20:04:23.000000 hassil-1.2.0/hassil.egg-info/entry_points.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       60 2023-07-24 20:04:23.000000 hassil-1.2.0/hassil.egg-info/requires.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        7 2023-07-24 20:04:23.000000 hassil-1.2.0/hassil.egg-info/top_level.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       15 2023-02-01 04:31:35.000000 hassil-1.2.0/requirements.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       69 2023-07-17 19:53:41.000000 hassil-1.2.0/requirements_dev.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      295 2023-07-24 20:04:23.934606 hassil-1.2.0/setup.cfg
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2069 2023-02-10 21:31:32.000000 hassil-1.2.0/setup.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-24 20:04:23.934606 hassil-1.2.0/tests/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       63 2022-12-07 21:08:40.000000 hassil-1.2.0/tests/__init__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2812 2023-02-01 04:31:35.000000 hassil-1.2.0/tests/test_expression.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4469 2023-02-06 16:37:52.000000 hassil-1.2.0/tests/test_intents.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1755 2023-02-01 04:31:35.000000 hassil-1.2.0/tests/test_parser.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    16282 2023-07-21 16:46:01.000000 hassil-1.2.0/tests/test_recognize.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1906 2023-02-01 04:31:35.000000 hassil-1.2.0/tests/test_sample.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      913 2023-01-23 19:07:47.000000 hassil-1.2.0/tests/test_util.py
```

### Comparing `hassil-1.1.0/HassILGrammar.g4` & `hassil-1.2.0/HassILGrammar.g4`

 * *Files identical despite different names*

### Comparing `hassil-1.1.0/LICENSE.md` & `hassil-1.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hassil-1.1.0/PKG-INFO` & `hassil-1.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hassil
-Version: 1.1.0
+Version: 1.2.0
 Summary: The Home Assistant Intent Language parser
 Home-page: http://github.com/home-assistant/hassil
 Author: Michael Hansen
 Author-email: mike@rhasspy.org
 License: Apache-2.0
 Keywords: home assistant intent recognition
 Classifier: Development Status :: 3 - Alpha
@@ -135,14 +135,16 @@
         context:
           <name>: <value>
   <range_name>
     range:
       type: "number"
       from: 0
       to: 100  # inclusive
+  <wildcard_name>
+    wildcard: true
 
 # Optional rules that are expanded in sentence templates
 expansion_rules:
   # Referenced as <rule_name>
   <rule_name>: "<sentence template>"
 
 # Optional words that the intent recognizer can skip during recognition
```

### Comparing `hassil-1.1.0/README.md` & `hassil-1.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -115,14 +115,16 @@
         context:
           <name>: <value>
   <range_name>
     range:
       type: "number"
       from: 0
       to: 100  # inclusive
+  <wildcard_name>
+    wildcard: true
 
 # Optional rules that are expanded in sentence templates
 expansion_rules:
   # Referenced as <rule_name>
   <rule_name>: "<sentence template>"
 
 # Optional words that the intent recognizer can skip during recognition
```

### Comparing `hassil-1.1.0/hassil/__main__.py` & `hassil-1.2.0/hassil/__main__.py`

 * *Files identical despite different names*

### Comparing `hassil-1.1.0/hassil/expression.py` & `hassil-1.2.0/hassil/expression.py`

 * *Files identical despite different names*

### Comparing `hassil-1.1.0/hassil/intents.py` & `hassil-1.2.0/hassil/intents.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,14 +158,19 @@
                 TextSlotValue.from_tuple(value_tuple, allow_template)
                 for value_tuple in tuples
             ],
         )
 
 
 @dataclass
+class WildcardSlotList(SlotList):
+    """Matches as much text as possible."""
+
+
+@dataclass
 class IntentsSettings:
     """Settings for intents."""
 
     ignore_whitespace: bool = False
     """True if whitespace should be ignored during matching."""
 
 
@@ -302,14 +307,18 @@
         return RangeSlotList(
             type=RangeType(range_dict.get("type", "number")),
             start=int(range_dict["from"]),
             stop=int(range_dict["to"]),
             step=int(range_dict.get("step", 1)),
         )
 
+    if list_dict.get("wildcard", False):
+        # Wildcard
+        return WildcardSlotList()
+
     raise ValueError(f"Unknown slot list type: {list_dict}")
 
 
 def _parse_settings(settings_dict: dict[str, Any]) -> IntentsSettings:
     """Parse intent settings."""
     return IntentsSettings(
         ignore_whitespace=settings_dict.get("ignore_whitespace", False)
```

### Comparing `hassil-1.1.0/hassil/parse_expression.py` & `hassil-1.2.0/hassil/parse_expression.py`

 * *Files identical despite different names*

### Comparing `hassil-1.1.0/hassil/parser.py` & `hassil-1.2.0/hassil/parser.py`

 * *Files identical despite different names*

### Comparing `hassil-1.1.0/hassil/sample.py` & `hassil-1.2.0/hassil/sample.py`

 * *Files identical despite different names*

### Comparing `hassil-1.1.0/hassil/sample_template.py` & `hassil-1.2.0/hassil/sample_template.py`

 * *Files identical despite different names*

### Comparing `hassil-1.1.0/hassil/util.py` & `hassil-1.2.0/hassil/util.py`

 * *Files identical despite different names*

### Comparing `hassil-1.1.0/hassil.egg-info/PKG-INFO` & `hassil-1.2.0/hassil.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hassil
-Version: 1.1.0
+Version: 1.2.0
 Summary: The Home Assistant Intent Language parser
 Home-page: http://github.com/home-assistant/hassil
 Author: Michael Hansen
 Author-email: mike@rhasspy.org
 License: Apache-2.0
 Keywords: home assistant intent recognition
 Classifier: Development Status :: 3 - Alpha
@@ -135,14 +135,16 @@
         context:
           <name>: <value>
   <range_name>
     range:
       type: "number"
       from: 0
       to: 100  # inclusive
+  <wildcard_name>
+    wildcard: true
 
 # Optional rules that are expanded in sentence templates
 expansion_rules:
   # Referenced as <rule_name>
   <rule_name>: "<sentence template>"
 
 # Optional words that the intent recognizer can skip during recognition
```

### Comparing `hassil-1.1.0/hassil.egg-info/SOURCES.txt` & `hassil-1.2.0/hassil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hassil-1.1.0/setup.py` & `hassil-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `hassil-1.1.0/tests/test_expression.py` & `hassil-1.2.0/tests/test_expression.py`

 * *Files identical despite different names*

### Comparing `hassil-1.1.0/tests/test_intents.py` & `hassil-1.2.0/tests/test_intents.py`

 * *Files identical despite different names*

### Comparing `hassil-1.1.0/tests/test_parser.py` & `hassil-1.2.0/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `hassil-1.1.0/tests/test_recognize.py` & `hassil-1.2.0/tests/test_recognize.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import cast
 
 import pytest
 
 from hassil import Intents, recognize, recognize_all
 from hassil.expression import TextChunk
 from hassil.intents import TextSlotList
+from hassil.recognize import UnmatchedRangeEntity, UnmatchedTextEntity
 
 TEST_YAML = """
 language: "en"
 intents:
   TurnOnTV:
     data:
       - sentences:
@@ -509,7 +510,97 @@
     for sentence in (
         "are the lights on in the kitchen",
         "are the lights in the kitchen on",
     ):
         result = recognize(sentence, intents)
         assert result is not None, sentence
         assert result.intent.name == "GetSmokeState"
+
+
+def test_unmatched_entity() -> None:
+    """Test allow_unmatched_entities option to provide better feedback."""
+    yaml_text = """
+    language: "en"
+    intents:
+      Test:
+        data:
+          - sentences:
+              - "set [all] {domain} in {area} to {percent}[%] now"
+    lists:
+      area:
+        values:
+          - kitchen
+          - bedroom
+      domain:
+        values:
+          - lights
+      percent:
+        range:
+          type: percentage
+          from: 0
+          to: 100
+    """
+
+    with io.StringIO(yaml_text) as test_file:
+        intents = Intents.from_yaml(test_file)
+
+    sentence = "set fans in living room to 101% now"
+
+    # Should fail without unmatched entities enabled
+    result = recognize(sentence, intents, allow_unmatched_entities=False)
+    assert result is None, f"{sentence} should not match"
+
+    # Should succeed now
+    result = recognize(sentence, intents, allow_unmatched_entities=True)
+    assert result is not None, f"{sentence} should match"
+    assert set(result.unmatched_entities.keys()) == {"domain", "area", "percent"}
+    domain = result.unmatched_entities["domain"]
+    assert isinstance(domain, UnmatchedTextEntity)
+    assert domain.text == "fans "
+
+    area = result.unmatched_entities["area"]
+    assert isinstance(area, UnmatchedTextEntity)
+    assert area.text == "living room "
+
+    percent = result.unmatched_entities["percent"]
+    assert isinstance(percent, UnmatchedRangeEntity)
+    assert percent.value == 101
+
+    sentence = "set all lights in kitchen to blah blah blah now"
+    result = recognize(sentence, intents, allow_unmatched_entities=True)
+    assert result is not None, f"{sentence} should match"
+    assert set(result.unmatched_entities.keys()) == {"percent"}
+
+    percent = result.unmatched_entities["percent"]
+    assert isinstance(percent, UnmatchedTextEntity)
+    assert percent.text == "blah blah blah "
+
+
+def test_wildcard() -> None:
+    """Test wildcard slot lists/entities."""
+    yaml_text = """
+    language: "en"
+    intents:
+      Test:
+        data:
+          - sentences:
+              - "play {album} by {artist} [please] now"
+    lists:
+      album:
+        wildcard: true
+      artist:
+        wildcard: true
+    """
+
+    with io.StringIO(yaml_text) as test_file:
+        intents = Intents.from_yaml(test_file)
+
+    sentence = "play the white album by the beatles please now"
+    result = recognize(sentence, intents)
+    assert result is not None, f"{sentence} should match"
+    assert result.entities["album"].value == "the white album "
+    assert result.entities["artist"].value == "the beatles "
+
+    # Wildcards cannot be empty
+    sentence = "play by please now"
+    result = recognize(sentence, intents)
+    assert result is None, f"{sentence} should not match"
```

### Comparing `hassil-1.1.0/tests/test_sample.py` & `hassil-1.2.0/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `hassil-1.1.0/tests/test_util.py` & `hassil-1.2.0/tests/test_util.py`

 * *Files identical despite different names*

