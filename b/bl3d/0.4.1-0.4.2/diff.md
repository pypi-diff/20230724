# Comparing `tmp/bl3d-0.4.1.tar.gz` & `tmp/bl3d-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bl3d-0.4.1.tar", max compression
+gzip compressed data, was "bl3d-0.4.2.tar", max compression
```

## Comparing `bl3d-0.4.1.tar` & `bl3d-0.4.2.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0    34895 2022-11-09 08:32:45.815575 bl3d-0.4.1/LICENSE.md
--rw-r--r--   0        0        0      182 2022-11-09 07:16:37.084157 bl3d-0.4.1/README.md
--rw-r--r--   0        0        0    12068 2023-06-28 09:40:13.101653 bl3d-0.4.1/bl3d/__init__.py
--rw-r--r--   0        0        0        0 2022-11-09 08:32:45.815575 bl3d-0.4.1/bl3d/py.typed
--rw-r--r--   0        0        0      865 2023-06-28 09:40:13.101653 bl3d-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      746 2023-06-28 09:40:22.446431 bl3d-0.4.1/setup.py
--rw-r--r--   0        0        0      783 2023-06-28 09:40:22.446890 bl3d-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    34895 2022-11-10 07:35:40.853706 bl3d-0.4.2/LICENSE.md
+-rw-r--r--   0        0        0      182 2022-11-10 07:35:40.853706 bl3d-0.4.2/README.md
+-rw-r--r--   0        0        0    12345 2023-07-24 15:19:31.036000 bl3d-0.4.2/bl3d/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-10 07:35:40.853706 bl3d-0.4.2/bl3d/py.typed
+-rw-r--r--   0        0        0      865 2023-07-24 15:19:31.036000 bl3d-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      834 1970-01-01 00:00:00.000000 bl3d-0.4.2/PKG-INFO
```

### Comparing `bl3d-0.4.1/LICENSE.md` & `bl3d-0.4.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bl3d-0.4.1/bl3d/__init__.py` & `bl3d-0.4.2/bl3d/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 import re
+import warnings
 from abc import ABC, abstractmethod, abstractproperty
 from dataclasses import dataclass
 from datetime import date, datetime, timedelta, timezone
 from typing import Any, Optional, Type, TypeVar
 
 import pkg_resources
 
@@ -335,20 +336,28 @@
 @dataclass(frozen=True)
 class DomainEvent(ABC):
     """An event that happened in the domain."""
 
     version: int
 
     @abstractproperty
-    def entity_unique_identifier(self) -> str:
-        """An identifier that uniquely identifies the entity
+    def aggregate_id(self) -> str:
+        """An identifier that uniquely identifies the aggregate
         that emitted the domain event.
         """
         ...
 
+    @property
+    def entity_unique_identifier(self) -> str:
+        """Deprecated. Use `aggregate_id` instead."""
+        warnings.warn(
+            "Deprecated. Use `aggregate_id` instead.", DeprecationWarning, stacklevel=2
+        )
+        return self.aggregate_id
+
 
 @dataclass(frozen=True)
 class EntityState(ABC):
     """The state of an entity.
 
     A new state is created by applying an domain event to it.
     """
```

### Comparing `bl3d-0.4.1/pyproject.toml` & `bl3d-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bl3d"
-version = "0.4.1"
+version = "0.4.2"
 description = "Domain Driven Design library"
 authors = ["Tanguy Le Carrour <tanguy@bioneland.org>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://git.easter-eggs.org/bioneland/bl3d"
 repository = "https://git.easter-eggs.org/bioneland/bl3d"
```

### Comparing `bl3d-0.4.1/PKG-INFO` & `bl3d-0.4.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: bl3d
-Version: 0.4.1
+Version: 0.4.2
 Summary: Domain Driven Design library
 Home-page: https://git.easter-eggs.org/bioneland/bl3d
 License: GPL-3.0-or-later
 Author: Tanguy Le Carrour
 Author-email: tanguy@bioneland.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Project-URL: Repository, https://git.easter-eggs.org/bioneland/bl3d
 Description-Content-Type: text/markdown
 
 # bl3d – A Domain Driven Design library
 
 Bioneland's Domain Driven Design library (bl3d, pronounced */'bled/*) is a collection
 of classes to write domain driven designed software.
```

