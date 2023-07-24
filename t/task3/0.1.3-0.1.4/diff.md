# Comparing `tmp/task3-0.1.3.tar.gz` & `tmp/task3-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "task3-0.1.3.tar", max compression
+gzip compressed data, was "task3-0.1.4.tar", max compression
```

## Comparing `task3-0.1.3.tar` & `task3-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      466 2023-07-08 14:31:48.331141 task3-0.1.3/LICENSE
--rw-r--r--   0        0        0      300 2023-07-21 16:40:54.009144 task3-0.1.3/parse_xsv/__init__.py
--rw-r--r--   0        0        0      116 2023-07-12 14:27:57.699438 task3-0.1.3/parse_xsv/__main__.py
--rw-r--r--   0        0        0       23 2023-07-24 19:31:13.468672 task3-0.1.3/parse_xsv/__version__.py
--rw-r--r--   0        0        0      187 2023-07-23 21:21:28.183243 task3-0.1.3/parse_xsv/cli/__init__.py
--rw-r--r--   0        0        0      116 2023-07-12 14:27:57.680442 task3-0.1.3/parse_xsv/cli/__main__.py
--rw-r--r--   0        0        0    17417 2023-07-24 17:14:55.584168 task3-0.1.3/parse_xsv/cli/cli.py
--rw-r--r--   0        0        0    12801 2023-07-24 19:17:27.822641 task3-0.1.3/parse_xsv/parse_xsv.py
--rw-r--r--   0        0        0      113 2023-07-15 09:18:39.572916 task3-0.1.3/parse_xsv/sample_gen/__init__.py
--rw-r--r--   0        0        0      143 2023-07-15 09:18:39.582913 task3-0.1.3/parse_xsv/sample_gen/__main__.py
--rw-r--r--   0        0        0     8102 2023-07-24 12:33:10.476335 task3-0.1.3/parse_xsv/sample_gen/sample_gen.py
--rw-r--r--   0        0        0       97 2023-07-12 14:27:57.666460 task3-0.1.3/parse_xsv/showcase/__init__.py
--rw-r--r--   0        0        0      138 2023-07-12 14:27:57.687500 task3-0.1.3/parse_xsv/showcase/__main__.py
--rw-r--r--   0        0        0    25805 2023-07-24 17:03:10.652441 task3-0.1.3/parse_xsv/showcase/corrupted_sample.csv
--rw-r--r--   0        0        0    29527 2023-07-24 15:54:36.768020 task3-0.1.3/parse_xsv/showcase/sample.csv
--rw-r--r--   0        0        0    29527 2023-07-24 16:01:30.014978 task3-0.1.3/parse_xsv/showcase/sample.tsv
--rw-r--r--   0        0        0    22754 2023-07-24 19:26:22.674171 task3-0.1.3/parse_xsv/showcase/showcase.py
--rw-r--r--   0        0        0      577 2023-07-24 19:31:13.474674 task3-0.1.3/pyproject.toml
--rw-r--r--   0        0        0    17428 2023-07-11 12:14:12.015389 task3-0.1.3/README.md
--rw-r--r--   0        0        0    17733 1970-01-01 00:00:00.000000 task3-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      466 2023-07-08 14:31:48.331141 task3-0.1.4/LICENSE
+-rw-r--r--   0        0        0      300 2023-07-21 16:40:54.009144 task3-0.1.4/parse_xsv/__init__.py
+-rw-r--r--   0        0        0      116 2023-07-12 14:27:57.699438 task3-0.1.4/parse_xsv/__main__.py
+-rw-r--r--   0        0        0       23 2023-07-24 20:01:57.866941 task3-0.1.4/parse_xsv/__version__.py
+-rw-r--r--   0        0        0      187 2023-07-23 21:21:28.183243 task3-0.1.4/parse_xsv/cli/__init__.py
+-rw-r--r--   0        0        0      116 2023-07-12 14:27:57.680442 task3-0.1.4/parse_xsv/cli/__main__.py
+-rw-r--r--   0        0        0    17423 2023-07-24 19:58:50.624510 task3-0.1.4/parse_xsv/cli/cli.py
+-rw-r--r--   0        0        0    12813 2023-07-24 19:56:50.742584 task3-0.1.4/parse_xsv/parse_xsv.py
+-rw-r--r--   0        0        0      113 2023-07-15 09:18:39.572916 task3-0.1.4/parse_xsv/sample_gen/__init__.py
+-rw-r--r--   0        0        0      143 2023-07-15 09:18:39.582913 task3-0.1.4/parse_xsv/sample_gen/__main__.py
+-rw-r--r--   0        0        0     8109 2023-07-24 20:00:04.379744 task3-0.1.4/parse_xsv/sample_gen/sample_gen.py
+-rw-r--r--   0        0        0       97 2023-07-12 14:27:57.666460 task3-0.1.4/parse_xsv/showcase/__init__.py
+-rw-r--r--   0        0        0      138 2023-07-12 14:27:57.687500 task3-0.1.4/parse_xsv/showcase/__main__.py
+-rw-r--r--   0        0        0    25805 2023-07-24 17:03:10.652441 task3-0.1.4/parse_xsv/showcase/corrupted_sample.csv
+-rw-r--r--   0        0        0    29527 2023-07-24 15:54:36.768020 task3-0.1.4/parse_xsv/showcase/sample.csv
+-rw-r--r--   0        0        0    29527 2023-07-24 16:01:30.014978 task3-0.1.4/parse_xsv/showcase/sample.tsv
+-rw-r--r--   0        0        0    22754 2023-07-24 19:26:22.674171 task3-0.1.4/parse_xsv/showcase/showcase.py
+-rw-r--r--   0        0        0      577 2023-07-24 20:01:57.871941 task3-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0    17428 2023-07-11 12:14:12.015389 task3-0.1.4/README.md
+-rw-r--r--   0        0        0    17733 1970-01-01 00:00:00.000000 task3-0.1.4/PKG-INFO
```

### Comparing `task3-0.1.3/parse_xsv/cli/cli.py` & `task3-0.1.4/parse_xsv/cli/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import csv
 import json
 import re
 import sys
 from abc import abstractmethod
 from enum import Enum
 from pathlib import Path
-from typing import Optional
+from typing import Optional, List
 
 from parse_xsv.parse_xsv import set_log_level, logger, packet_version, QuotingTypes, ReaderXSV
 
 
 class RegexPatterns(Enum):
     IP4 = \
         re.compile(r'\b(?:(?:25[0-5]|2[0-4]\d|[01]?\d\d?)\.){3}'
@@ -153,28 +153,28 @@
         self.args = args
         self.kwargs = kwargs
 
 
 class Group:
     def __init__(self, title, description: str = None,
                  required: bool = False,
-                 arguments: list[Argument] = None):
+                 arguments: List[Argument] = None):
         self.title = title
         self.description = description
         self.required = required
         self.arguments = arguments
 
 
 class Command:
     def __init__(self, prog_name: str = None,
                  help_epilog: str = None,
                  help_formatter=argparse.RawDescriptionHelpFormatter,
-                 base_arg: list[Argument] = None,
-                 groups: list[Group] = None,
-                 mutually_groups: list[Group] = None,
+                 base_arg: List[Argument] = None,
+                 groups: List[Group] = None,
+                 mutually_groups: List[Group] = None,
                  argv: Optional[str] = None) -> None:
         self.argv = argv or sys.argv[:]
         self.prog_name = prog_name if prog_name else Path(self.argv[0]).name
 
         base_arg = base_arg if base_arg else []
         groups = groups if groups else []
         mutually_groups = mutually_groups if mutually_groups else []
@@ -182,17 +182,17 @@
         self.arguments = self.__parse_args(epilog=help_epilog,
                                            formatter=help_formatter,
                                            base_arg=base_arg,
                                            groups=groups,
                                            mutually_groups=mutually_groups)
 
     def __parse_args(self, epilog, formatter,
-                     base_arg: list[Argument],
-                     groups: list[Group],
-                     mutually_groups: list[Group]) -> argparse.Namespace:
+                     base_arg: List[Argument],
+                     groups: List[Group],
+                     mutually_groups: List[Group]) -> argparse.Namespace:
         parser = argparse.ArgumentParser(
             prog=self.prog_name,
             description=f"{self.prog_name} version {packet_version()}",
             epilog=epilog,
             formatter_class=formatter
         )
```

### Comparing `task3-0.1.3/parse_xsv/parse_xsv.py` & `task3-0.1.4/parse_xsv/parse_xsv.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import csv
 import logging
 from _csv import QUOTE_MINIMAL, QUOTE_NONE
 from collections import Counter
 from enum import Enum
-from typing import Pattern, List
+from typing import Pattern, List, Tuple, Set
 
 from typing.io import TextIO
 
 from parse_xsv.__version__ import __version__
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.ERROR)
@@ -28,17 +28,17 @@
 class ReaderXSV(csv.DictReader):
     def __init__(self,
                  io: TextIO,
                  pure: bool = False,
                  no_header: bool = False,
                  search_string: str = None,
                  search_regex: Pattern[str] = None,
-                 column_regex: list[tuple] = None,
-                 rows: list[str] = None,
-                 columns: list[str] = None,
+                 column_regex: List[Tuple] = None,
+                 rows: List[str] = None,
+                 columns: List[str] = None,
                  json: bool = False,
                  *args, **kwargs):
         super().__init__(io, *args, **kwargs)
 
         self.search_string = search_string
         self.search_regex = search_regex
         self.column_regex = column_regex if column_regex else []
@@ -84,15 +84,15 @@
             elif not self.json and not any([val for key, val in enumerate(line)
                                             if key + 1 in ind_lst and el[1].search(str(val))]):
                 return False
 
         return True
 
     # noinspection PyMethodMayBeStatic
-    def __transform_indexes__(self, lst: list[str], max_index: int) -> set[int]:
+    def __transform_indexes__(self, lst: List[str], max_index: int) -> Set[int]:
         ret = set()
         for index in lst:
             if index.find('-', 1, len(index) - 1) != -1:
                 rng = [int(part) for part in index.split('-')]
                 if len(rng) != 2:
                     raise Exception(f'Wrong index range was passed {index}')
```

### Comparing `task3-0.1.3/parse_xsv/sample_gen/sample_gen.py` & `task3-0.1.4/parse_xsv/sample_gen/sample_gen.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import csv
 import random
 import sys
-from typing import List, Optional
+from typing import List, Optional, Tuple
 
 from faker import Faker, documentor, exceptions
 
 from parse_xsv import QuotingTypes
 from parse_xsv.cli.cli import Argument, Command
 from parse_xsv.parse_xsv import packet_version, set_log_level, logger
 
 
 class CommandGenCLI(Command):
-    __faker_methods__: list[str] = None
+    __faker_methods__: List[str] = None
 
     @staticmethod
     def __get_faker_methods__() -> List[str]:
         """Generate a method list of Faker library methods"""
         fake = Faker()
         doc = documentor.Documentor(fake)
 
@@ -29,22 +29,22 @@
                 break
 
         return [''.join(el.replace('fake.', '').split('(')[:1])
                 for _, fmt in formatters
                 for el in fmt if el.find('fake.') != -1]
 
     @classmethod
-    def faker_methods(cls) -> list[str]:
+    def faker_methods(cls) -> List[str]:
         """Getter/setter-initializer for the private static cache class argument __faker_methods__"""
         if cls.__faker_methods__ is None:
             cls.__faker_methods__ = cls.__get_faker_methods__()
 
         return cls.__faker_methods__
 
-    def __parse_structure_arg__(self) -> list[tuple]:
+    def __parse_structure_arg__(self) -> List[Tuple]:
         """It parses a name,val string to the tuple of (name, val).
         If name was missed, the index is added instead of name (index, val)."""
 
         splitted = [str(val).split(',') for ind, val in enumerate(self.arguments.structure)]
 
         if any(er_el := [el for el in splitted if len(el) == 0 or len(el) > 2]):
             raise Exception(f'Wrong structure element(s) were passed: {er_el}')
@@ -54,15 +54,15 @@
                 (
                     str(index) if len(spl_lst) == 1 else spl_lst[0],
                     spl_lst[0] if len(spl_lst) == 1 else spl_lst[1],
                 )
                 for index, spl_lst in enumerate(splitted)
             ]
 
-    def __broke_lines__(self, list_to_be_broken: list[list]) -> list[list]:
+    def __broke_lines__(self, list_to_be_broken: List[List]) -> List[List]:
         """1. Randomly selects lines to be damaged.
         2. Randomly selects whether add or skip line elements (if line is short only add).
         3. If it needs to be added, Faker's random methods are utilized to add a random amount of data.
         4. If it needs to be skipped, a random number of line elements is skipped."""
 
         fake = Faker()
         ret = []
```

### Comparing `task3-0.1.3/parse_xsv/showcase/corrupted_sample.csv` & `task3-0.1.4/parse_xsv/showcase/corrupted_sample.csv`

 * *Files identical despite different names*

### Comparing `task3-0.1.3/parse_xsv/showcase/sample.csv` & `task3-0.1.4/parse_xsv/showcase/sample.csv`

 * *Files identical despite different names*

### Comparing `task3-0.1.3/parse_xsv/showcase/sample.tsv` & `task3-0.1.4/parse_xsv/showcase/sample.tsv`

 * *Files identical despite different names*

### Comparing `task3-0.1.3/parse_xsv/showcase/showcase.py` & `task3-0.1.4/parse_xsv/showcase/showcase.py`

 * *Files identical despite different names*

### Comparing `task3-0.1.3/pyproject.toml` & `task3-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "task3"
-version = "0.1.3"
+version = "0.1.4"
 description = "xSV file parser CLI and library"
 authors = ["Bill.Avramenko <billavramenko@gmail.com>"]
 readme = "README.md"
 packages = [{include = "parse_xsv"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `task3-0.1.3/README.md` & `task3-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `task3-0.1.3/PKG-INFO` & `task3-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: task3
-Version: 0.1.3
+Version: 0.1.4
 Summary: xSV file parser CLI and library
 Author: Bill.Avramenko
 Author-email: billavramenko@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: task3 Version: 0.1.3 Summary: xSV file parser CLI
+Metadata-Version: 2.1 Name: task3 Version: 0.1.4 Summary: xSV file parser CLI
 and library Author: Bill.Avramenko Author-email: billavramenko@gmail.com
 Requires-Python: >=3.8,<4.0 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: faker
 (>=19.2.0,<20.0.0) Requires-Dist: questionary (>=1.10.0,<2.0.0) Description-
 Content-Type: text/markdown
```

