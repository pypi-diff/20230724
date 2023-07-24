# Comparing `tmp/yamlwrap-2.1.0.tar.gz` & `tmp/yamlwrap-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yamlwrap-2.1.0.tar", last modified: Sun Aug 15 11:19:30 2021, max compression
+gzip compressed data, was "yamlwrap-2.1.1.tar", last modified: Mon Jul 24 05:41:21 2023, max compression
```

## Comparing `yamlwrap-2.1.0.tar` & `yamlwrap-2.1.1.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxrwxr-x   0 eikman    (1000) eikman    (1000)        0 2021-08-15 11:19:30.220990 yamlwrap-2.1.0/
--rw-rw-r--   0 eikman    (1000) eikman    (1000)    35149 2021-04-19 16:14:35.000000 yamlwrap-2.1.0/LICENSE
--rw-rw-r--   0 eikman    (1000) eikman    (1000)     2819 2021-08-15 11:19:30.220990 yamlwrap-2.1.0/PKG-INFO
--rw-rw-r--   0 eikman    (1000) eikman    (1000)     1952 2021-08-14 09:55:21.000000 yamlwrap-2.1.0/README.md
--rw-r--r--   0 eikman    (1000) eikman    (1000)     1040 2021-08-15 11:19:30.220990 yamlwrap-2.1.0/setup.cfg
-drwxrwxr-x   0 eikman    (1000) eikman    (1000)        0 2021-08-15 11:19:30.220990 yamlwrap-2.1.0/src/
-drwxrwxr-x   0 eikman    (1000) eikman    (1000)        0 2021-08-15 11:19:30.220990 yamlwrap-2.1.0/src/yamlwrap/
--rw-rw-r--   0 eikman    (1000) eikman    (1000)     6885 2021-08-15 11:15:37.000000 yamlwrap-2.1.0/src/yamlwrap/__init__.py
--rw-rw-r--   0 eikman    (1000) eikman    (1000)     4723 2021-05-19 18:00:14.000000 yamlwrap-2.1.0/src/yamlwrap/__main__.py
-drwxrwxr-x   0 eikman    (1000) eikman    (1000)        0 2021-08-15 11:19:30.220990 yamlwrap-2.1.0/src/yamlwrap.egg-info/
--rw-rw-r--   0 eikman    (1000) eikman    (1000)     2819 2021-08-15 11:19:30.000000 yamlwrap-2.1.0/src/yamlwrap.egg-info/PKG-INFO
--rw-rw-r--   0 eikman    (1000) eikman    (1000)      256 2021-08-15 11:19:30.000000 yamlwrap-2.1.0/src/yamlwrap.egg-info/SOURCES.txt
--rw-rw-r--   0 eikman    (1000) eikman    (1000)        1 2021-08-15 11:19:30.000000 yamlwrap-2.1.0/src/yamlwrap.egg-info/dependency_links.txt
--rw-rw-r--   0 eikman    (1000) eikman    (1000)       21 2021-08-15 11:19:30.000000 yamlwrap-2.1.0/src/yamlwrap.egg-info/requires.txt
--rw-rw-r--   0 eikman    (1000) eikman    (1000)        9 2021-08-15 11:19:30.000000 yamlwrap-2.1.0/src/yamlwrap.egg-info/top_level.txt
+drwxrwxr-x   0 eikman    (1000) eikman    (1000)        0 2023-07-24 05:41:21.973646 yamlwrap-2.1.1/
+-rw-rw-r--   0 eikman    (1000) eikman    (1000)    35149 2021-04-19 16:14:35.000000 yamlwrap-2.1.1/LICENSE
+-rw-rw-r--   0 eikman    (1000) eikman    (1000)     3137 2023-07-24 05:41:21.973646 yamlwrap-2.1.1/PKG-INFO
+-rw-rw-r--   0 eikman    (1000) eikman    (1000)     2260 2023-07-24 05:38:31.000000 yamlwrap-2.1.1/README.md
+-rw-rw-r--   0 eikman    (1000) eikman    (1000)     1419 2023-07-22 20:12:55.000000 yamlwrap-2.1.1/pyproject.toml
+-rw-rw-r--   0 eikman    (1000) eikman    (1000)       38 2023-07-24 05:41:21.973646 yamlwrap-2.1.1/setup.cfg
+drwxrwxr-x   0 eikman    (1000) eikman    (1000)        0 2023-07-24 05:41:21.969646 yamlwrap-2.1.1/src/
+drwxrwxr-x   0 eikman    (1000) eikman    (1000)        0 2023-07-24 05:41:21.973646 yamlwrap-2.1.1/src/yamlwrap/
+-rw-rw-r--   0 eikman    (1000) eikman    (1000)     6864 2023-07-24 05:40:09.000000 yamlwrap-2.1.1/src/yamlwrap/__init__.py
+-rw-rw-r--   0 eikman    (1000) eikman    (1000)     4824 2023-07-22 20:17:37.000000 yamlwrap-2.1.1/src/yamlwrap/__main__.py
+drwxrwxr-x   0 eikman    (1000) eikman    (1000)        0 2023-07-24 05:41:21.973646 yamlwrap-2.1.1/src/yamlwrap.egg-info/
+-rw-rw-r--   0 eikman    (1000) eikman    (1000)     3137 2023-07-24 05:41:21.000000 yamlwrap-2.1.1/src/yamlwrap.egg-info/PKG-INFO
+-rw-rw-r--   0 eikman    (1000) eikman    (1000)      303 2023-07-24 05:41:21.000000 yamlwrap-2.1.1/src/yamlwrap.egg-info/SOURCES.txt
+-rw-rw-r--   0 eikman    (1000) eikman    (1000)        1 2023-07-24 05:41:21.000000 yamlwrap-2.1.1/src/yamlwrap.egg-info/dependency_links.txt
+-rw-rw-r--   0 eikman    (1000) eikman    (1000)       39 2023-07-24 05:41:21.000000 yamlwrap-2.1.1/src/yamlwrap.egg-info/requires.txt
+-rw-rw-r--   0 eikman    (1000) eikman    (1000)        9 2023-07-24 05:41:21.000000 yamlwrap-2.1.1/src/yamlwrap.egg-info/top_level.txt
+drwxrwxr-x   0 eikman    (1000) eikman    (1000)        0 2023-07-24 05:41:21.973646 yamlwrap-2.1.1/tests/
+-rw-r--r--   0 eikman    (1000) eikman    (1000)     3414 2023-07-23 15:31:40.000000 yamlwrap-2.1.1/tests/test_upstream.py
+-rw-rw-r--   0 eikman    (1000) eikman    (1000)     8945 2023-07-23 19:56:56.000000 yamlwrap-2.1.1/tests/test_wrap.py
```

### Comparing `yamlwrap-2.1.0/LICENSE` & `yamlwrap-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yamlwrap-2.1.0/PKG-INFO` & `yamlwrap-2.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 Metadata-Version: 2.1
 Name: yamlwrap
-Version: 2.1.0
+Version: 2.1.1
 Summary: VCS-friendly documents in YAML
-Home-page: https://github.com/veikman/yamlwrap
-Author: Viktor Eikman
-Author-email: viktor.eikman@gmail.com
+Author-email: Viktor Eikman <viktor.eikman@gmail.com>
 License: GPL-3.0-only
-Platform: UNKNOWN
+Project-URL: Homepage, https://github.com/veikman/yamlwrap
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Version Control
 Classifier: Topic :: Text Editors
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8
+Provides-Extra: testing
 License-File: LICENSE
 
-# `yamlwrap`: VCS-friendly documents in YAML
+`yamlwrap` is a Python module for keeping content ready for the web while
+under effective version control.
 
-This is a Python module for maintaining arbitrarily long Markdown documents in
-YAML mappings, under version control and subject to other text-based tools.
-
-`yamlwrap` serves this purpose by adding YAML support to
-`[punwrap](https://github.com/veikman/punwrap)`, a Rust extension for wrapping
-Markdown.
+[![PyPI version](https://badge.fury.io/py/yamlwrap.svg)](https://badge.fury.io/py/yamlwrap)
 
 ## Audience
 
-`yamlwrap` is for people who maintain the contents of statically built web
-sites as YAML and prefer off-line text editors over SQL and plutonian web-based
-administrative interfaces. It won’t do much good for configuration files.
+Do you use YAML just for configuration files? Then you don’t need `yamlwrap`.
+
+Do you maintain a statically built web site? Do you want to keep even long
+documents with complex internal markup in plain-text files, but always ready
+for the ORM? Do you want automatic rewrapping (reflowing) of text for short
+lines and neat Git diffs? Do you want to use YAML everywhere, for quick,
+unambiguous, syntax-checked conversion to JSON or SQL for publication? Then
+`yamlwrap` is for you.
+
+Stop using plutonian web-based administrative interfaces. Use `yamlwrap` and
+your favourite text editor.
 
 ## Usage
 
-This is primarily a function library. Its main interface is
+This project is primarily a function library. Its highest-level interface is
 `yamlwrap.transform`, which takes and returns serialized YAML, along with
 keyword parameters for how to change that YAML. `yamlwrap.unwrap`, which takes
 a block of text as one string, is a suitable preprocessor for
 line-break-sensitive markup resolution.
 
 The package also comes with a CLI that works on a file level and can produce
 diffs or new files from simple transformations.
@@ -57,22 +60,22 @@
 ## Development
 
 This project is managed using PyInvoke. Run `inv -l` for a list of common
 tasks.
 
 ## History
 
-`yamlwrap` was originally part of `django-yamldoc`, when that project was
-called `vedm`. It became its own module (v1.0.0) in 2021. Later that year,
-internal logic based on Python regexes was stripped out in favour of `punwrap`,
-resulting in a more narrow focus (Markdown instead of arbitrary markup) and
-substantial behavioural changes (v2.0.0).
+`yamlwrap` was originally part of
+[`django-yamldoc`](https://github.com/veikman/django-yamldoc), when that
+project was called `vedm`. It became its own module (v1.0.0) in 2021. Later
+that year, internal logic based on Python regexes was stripped out in favour of
+[`punwrap`](https://github.com/veikman/punwrap), resulting in a more narrow
+focus (Markdown instead of arbitrary markup) and substantial behavioural
+changes (v2.0.0).
 
 Later changes are described in the [change log](CHANGELOG.md).
 
 ## Legal
 
-Copyright 2016–2021 Viktor Eikman
+Copyright 2016–2023 Viktor Eikman
 
 `yamlwrap` is licensed as detailed in the accompanying file LICENSE.
-
-
```

### Comparing `yamlwrap-2.1.0/README.md` & `yamlwrap-2.1.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,29 @@
-# `yamlwrap`: VCS-friendly documents in YAML
+`yamlwrap` is a Python module for keeping content ready for the web while
+under effective version control.
 
-This is a Python module for maintaining arbitrarily long Markdown documents in
-YAML mappings, under version control and subject to other text-based tools.
-
-`yamlwrap` serves this purpose by adding YAML support to
-`[punwrap](https://github.com/veikman/punwrap)`, a Rust extension for wrapping
-Markdown.
+[![PyPI version](https://badge.fury.io/py/yamlwrap.svg)](https://badge.fury.io/py/yamlwrap)
 
 ## Audience
 
-`yamlwrap` is for people who maintain the contents of statically built web
-sites as YAML and prefer off-line text editors over SQL and plutonian web-based
-administrative interfaces. It won’t do much good for configuration files.
+Do you use YAML just for configuration files? Then you don’t need `yamlwrap`.
+
+Do you maintain a statically built web site? Do you want to keep even long
+documents with complex internal markup in plain-text files, but always ready
+for the ORM? Do you want automatic rewrapping (reflowing) of text for short
+lines and neat Git diffs? Do you want to use YAML everywhere, for quick,
+unambiguous, syntax-checked conversion to JSON or SQL for publication? Then
+`yamlwrap` is for you.
+
+Stop using plutonian web-based administrative interfaces. Use `yamlwrap` and
+your favourite text editor.
 
 ## Usage
 
-This is primarily a function library. Its main interface is
+This project is primarily a function library. Its highest-level interface is
 `yamlwrap.transform`, which takes and returns serialized YAML, along with
 keyword parameters for how to change that YAML. `yamlwrap.unwrap`, which takes
 a block of text as one string, is a suitable preprocessor for
 line-break-sensitive markup resolution.
 
 The package also comes with a CLI that works on a file level and can produce
 diffs or new files from simple transformations.
@@ -34,20 +38,22 @@
 ## Development
 
 This project is managed using PyInvoke. Run `inv -l` for a list of common
 tasks.
 
 ## History
 
-`yamlwrap` was originally part of `django-yamldoc`, when that project was
-called `vedm`. It became its own module (v1.0.0) in 2021. Later that year,
-internal logic based on Python regexes was stripped out in favour of `punwrap`,
-resulting in a more narrow focus (Markdown instead of arbitrary markup) and
-substantial behavioural changes (v2.0.0).
+`yamlwrap` was originally part of
+[`django-yamldoc`](https://github.com/veikman/django-yamldoc), when that
+project was called `vedm`. It became its own module (v1.0.0) in 2021. Later
+that year, internal logic based on Python regexes was stripped out in favour of
+[`punwrap`](https://github.com/veikman/punwrap), resulting in a more narrow
+focus (Markdown instead of arbitrary markup) and substantial behavioural
+changes (v2.0.0).
 
 Later changes are described in the [change log](CHANGELOG.md).
 
 ## Legal
 
-Copyright 2016–2021 Viktor Eikman
+Copyright 2016–2023 Viktor Eikman
 
 `yamlwrap` is licensed as detailed in the accompanying file LICENSE.
```

### Comparing `yamlwrap-2.1.0/src/yamlwrap/__init__.py` & `yamlwrap-2.1.1/src/yamlwrap/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,20 +40,22 @@
 import yaml  # PyPI: PyYAML.
 
 #############
 # CONSTANTS #
 #############
 
 
-__version__ = '2.1.0'
+__version__ = '2.1.1'
 
 
 # Unicode space ranges.
-_NONPRINTABLE = re.compile(r'[^\x09\x0A\x0D\x20-\x7E\x85\xA0-'
-                           r'\uD7FF\uE000-\uFFFD\U00010000-\U0010FFFF]')
+_NONPRINTABLE = re.compile(
+    r'[^\x09\x0A\x0D\x20-\x7E\x85\xA0-'
+    r'\uD7FF\uE000-\uFFFD\U00010000-\U0010FFFF]'
+)
 
 
 WIDTH_DEFAULT = 70
 WIDTH_DUMP = 160
 
 
 ###########
@@ -65,22 +67,22 @@
 
 
 #######################
 # INTERFACE FUNCTIONS #
 #######################
 
 
-def dump(data, sort_dicts=False, width=WIDTH_DUMP, **kwargs) -> str:
+def dump(data, sort_keys=False, width=WIDTH_DUMP, **kwargs) -> str:
     """Serialize passed data structure as YAML.
 
     The main job of this function is to preserve the order of mappings for
     readability.
 
     """
-    return pyaml.dump(data, sort_dicts=sort_dicts, width=width, **kwargs)
+    return pyaml.dump(data, sort_keys=sort_keys, width=width, **kwargs)
 
 
 def load(data: str):
     """Parse passed string as YAML.
 
     The main job of this function is to work around the lack of support for
     SMP Unicode characters in PyYaml 3.13. A future release of PyYaml may fix
@@ -88,18 +90,25 @@
     PyYaml in this back end.
 
     """
     yaml.reader.Reader.NON_PRINTABLE = _NONPRINTABLE
     return yaml.safe_load(data)
 
 
-def transform(raw: str, twopass=True, unwrap=False, wrap=False,
-              loader=load, dumper=dump,
-              lint_fn: Optional[Callable[[str], None]] = None,
-              map_fn=lambda x: x, postdescent_fn=lambda x: x) -> Optional[str]:
+def transform(
+    raw: str,
+    twopass=True,
+    unwrap=False,
+    wrap=False,
+    loader=load,
+    dumper=dump,
+    lint_fn: Optional[Callable[[str], None]] = None,
+    map_fn=lambda x: x,
+    postdescent_fn=lambda x: x,
+) -> Optional[str]:
     """Modify a serialized YAML string if needed.
 
     Return a string if changes are suggested, else return None.
 
     This is a crude high-level API that deserializes YAML, walks through an
     arbitrarily complex data structure inside, and round-trips back to
     serialized data. Not all options for lower-level functions conditionally
@@ -126,17 +135,19 @@
     else:
         if unwrap:
             string_fns.append(_unwrap)
         if wrap:
             string_fns.append(_wrap)
 
     if lint_fn is not None:
+
         def lint(r: str) -> str:
             lint_fn(r)  # type: ignore[misc]
             return r
+
         string_fns.append(lint)
 
     _descend(data, map_fn, string_fns)
 
     postdescent_fn(data)
 
     cooked = dumper(data, **dump_args)
@@ -195,16 +206,17 @@
 _rewrap = rewrap
 _unwrap = unwrap
 _wrap = wrap
 
 
 def _is_listlike(object_: Any) -> bool:
     """Return True if object_ is an iterable container."""
-    if (isinstance(object_, collections.abc.Iterable) and
-            not isinstance(object_, str)):
+    if isinstance(object_, collections.abc.Iterable) and not isinstance(
+        object_, str
+    ):
         return True
     return False
 
 
 def _descend(object_: Any, map_fn, string_fns, **kwargs):
     """Walk down through mutable containers, applying functions."""
     if isinstance(object_, collections.abc.Mapping):
```

### Comparing `yamlwrap-2.1.0/src/yamlwrap.egg-info/PKG-INFO` & `yamlwrap-2.1.1/src/yamlwrap.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 Metadata-Version: 2.1
 Name: yamlwrap
-Version: 2.1.0
+Version: 2.1.1
 Summary: VCS-friendly documents in YAML
-Home-page: https://github.com/veikman/yamlwrap
-Author: Viktor Eikman
-Author-email: viktor.eikman@gmail.com
+Author-email: Viktor Eikman <viktor.eikman@gmail.com>
 License: GPL-3.0-only
-Platform: UNKNOWN
+Project-URL: Homepage, https://github.com/veikman/yamlwrap
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Version Control
 Classifier: Topic :: Text Editors
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8
+Provides-Extra: testing
 License-File: LICENSE
 
-# `yamlwrap`: VCS-friendly documents in YAML
+`yamlwrap` is a Python module for keeping content ready for the web while
+under effective version control.
 
-This is a Python module for maintaining arbitrarily long Markdown documents in
-YAML mappings, under version control and subject to other text-based tools.
-
-`yamlwrap` serves this purpose by adding YAML support to
-`[punwrap](https://github.com/veikman/punwrap)`, a Rust extension for wrapping
-Markdown.
+[![PyPI version](https://badge.fury.io/py/yamlwrap.svg)](https://badge.fury.io/py/yamlwrap)
 
 ## Audience
 
-`yamlwrap` is for people who maintain the contents of statically built web
-sites as YAML and prefer off-line text editors over SQL and plutonian web-based
-administrative interfaces. It won’t do much good for configuration files.
+Do you use YAML just for configuration files? Then you don’t need `yamlwrap`.
+
+Do you maintain a statically built web site? Do you want to keep even long
+documents with complex internal markup in plain-text files, but always ready
+for the ORM? Do you want automatic rewrapping (reflowing) of text for short
+lines and neat Git diffs? Do you want to use YAML everywhere, for quick,
+unambiguous, syntax-checked conversion to JSON or SQL for publication? Then
+`yamlwrap` is for you.
+
+Stop using plutonian web-based administrative interfaces. Use `yamlwrap` and
+your favourite text editor.
 
 ## Usage
 
-This is primarily a function library. Its main interface is
+This project is primarily a function library. Its highest-level interface is
 `yamlwrap.transform`, which takes and returns serialized YAML, along with
 keyword parameters for how to change that YAML. `yamlwrap.unwrap`, which takes
 a block of text as one string, is a suitable preprocessor for
 line-break-sensitive markup resolution.
 
 The package also comes with a CLI that works on a file level and can produce
 diffs or new files from simple transformations.
@@ -57,22 +60,22 @@
 ## Development
 
 This project is managed using PyInvoke. Run `inv -l` for a list of common
 tasks.
 
 ## History
 
-`yamlwrap` was originally part of `django-yamldoc`, when that project was
-called `vedm`. It became its own module (v1.0.0) in 2021. Later that year,
-internal logic based on Python regexes was stripped out in favour of `punwrap`,
-resulting in a more narrow focus (Markdown instead of arbitrary markup) and
-substantial behavioural changes (v2.0.0).
+`yamlwrap` was originally part of
+[`django-yamldoc`](https://github.com/veikman/django-yamldoc), when that
+project was called `vedm`. It became its own module (v1.0.0) in 2021. Later
+that year, internal logic based on Python regexes was stripped out in favour of
+[`punwrap`](https://github.com/veikman/punwrap), resulting in a more narrow
+focus (Markdown instead of arbitrary markup) and substantial behavioural
+changes (v2.0.0).
 
 Later changes are described in the [change log](CHANGELOG.md).
 
 ## Legal
 
-Copyright 2016–2021 Viktor Eikman
+Copyright 2016–2023 Viktor Eikman
 
 `yamlwrap` is licensed as detailed in the accompanying file LICENSE.
-
-
```

