# Comparing `tmp/datawords-0.6.2.tar.gz` & `tmp/datawords-0.7.0.tar.gz`

## Comparing `datawords-0.6.2.tar` & `datawords-0.7.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0    20849 2020-02-02 00:00:00.000000 datawords-0.6.2/.pylintrc
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 datawords-0.6.2/Makefile
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 datawords-0.6.2/mypy.ini
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 datawords-0.6.2/readthedocs.yml
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 datawords-0.6.2/datawords/__about__.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 datawords-0.6.2/datawords/__init__.py
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 datawords-0.6.2/datawords/_utils.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 datawords-0.6.2/datawords/constants.py
--rw-r--r--   0        0        0    12398 2020-02-02 00:00:00.000000 datawords-0.6.2/datawords/indexes.py
--rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 datawords-0.6.2/datawords/install_pytorch.py
--rw-r--r--   0        0        0     5994 2020-02-02 00:00:00.000000 datawords-0.6.2/datawords/models.py
--rw-r--r--   0        0        0    14532 2020-02-02 00:00:00.000000 datawords-0.6.2/datawords/parsers.py
--rw-r--r--   0        0        0     7034 2020-02-02 00:00:00.000000 datawords-0.6.2/datawords/ranking.py
--rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 datawords-0.6.2/datawords/utils.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 datawords-0.6.2/datawords/deepnlp/__init__.py
--rw-r--r--   0        0        0     3387 2020-02-02 00:00:00.000000 datawords-0.6.2/datawords/deepnlp/core.py
--rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 datawords-0.6.2/datawords/deepnlp/translators.py
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 datawords-0.6.2/datawords/deepnlp/translators2.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 datawords-0.6.2/datawords/deepnlp/utils.py
--rw-r--r--   0        0        0     6276 2020-02-02 00:00:00.000000 datawords-0.6.2/datawords/files/stop_en.txt
--rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 datawords-0.6.2/datawords/files/stop_es.txt
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 datawords-0.6.2/datawords/files/stop_pt.txt
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 datawords-0.6.2/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 datawords-0.6.2/docs/make.bat
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 datawords-0.6.2/docs/source/api_reference.rst
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 datawords-0.6.2/docs/source/conf.py
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 datawords-0.6.2/docs/source/index.rst
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 datawords-0.6.2/docs/source/introduction.rst
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 datawords-0.6.2/docs/source/api/deepnlp.rst
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 datawords-0.6.2/docs/source/api/indexes.rst
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 datawords-0.6.2/docs/source/api/models.rst
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 datawords-0.6.2/docs/source/api/parsers.rst
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 datawords-0.6.2/docs/source/api/ranking.rst
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 datawords-0.6.2/tests/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 datawords-0.6.2/tests/shared.py
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 datawords-0.6.2/tests/test_indexes.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 datawords-0.6.2/tests/test_models.py
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 datawords-0.6.2/tests/test_parsers.py
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 datawords-0.6.2/tests/test_rankings.py
--rw-r--r--   0        0        0    21956 2020-02-02 00:00:00.000000 datawords-0.6.2/tests/texts.txt
--rw-r--r--   0        0        0     7876 2020-02-02 00:00:00.000000 datawords-0.6.2/.gitignore
--rw-r--r--   0        0        0    15977 2020-02-02 00:00:00.000000 datawords-0.6.2/LICENSE
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 datawords-0.6.2/NOTICE.md
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 datawords-0.6.2/README.md
--rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 datawords-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 datawords-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0    20849 2020-02-02 00:00:00.000000 datawords-0.7.0/.pylintrc
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 datawords-0.7.0/Makefile
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 datawords-0.7.0/mypy.ini
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 datawords-0.7.0/readthedocs.yml
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 datawords-0.7.0/datawords/__about__.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 datawords-0.7.0/datawords/__init__.py
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 datawords-0.7.0/datawords/_utils.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 datawords-0.7.0/datawords/constants.py
+-rw-r--r--   0        0        0    13515 2020-02-02 00:00:00.000000 datawords-0.7.0/datawords/indexes.py
+-rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 datawords-0.7.0/datawords/install_pytorch.py
+-rw-r--r--   0        0        0     5994 2020-02-02 00:00:00.000000 datawords-0.7.0/datawords/models.py
+-rw-r--r--   0        0        0    14532 2020-02-02 00:00:00.000000 datawords-0.7.0/datawords/parsers.py
+-rw-r--r--   0        0        0     7034 2020-02-02 00:00:00.000000 datawords-0.7.0/datawords/ranking.py
+-rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 datawords-0.7.0/datawords/utils.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 datawords-0.7.0/datawords/deepnlp/__init__.py
+-rw-r--r--   0        0        0     3387 2020-02-02 00:00:00.000000 datawords-0.7.0/datawords/deepnlp/core.py
+-rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 datawords-0.7.0/datawords/deepnlp/translators.py
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 datawords-0.7.0/datawords/deepnlp/translators2.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 datawords-0.7.0/datawords/deepnlp/utils.py
+-rw-r--r--   0        0        0     6276 2020-02-02 00:00:00.000000 datawords-0.7.0/datawords/files/stop_en.txt
+-rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 datawords-0.7.0/datawords/files/stop_es.txt
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 datawords-0.7.0/datawords/files/stop_pt.txt
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 datawords-0.7.0/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 datawords-0.7.0/docs/make.bat
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 datawords-0.7.0/docs/source/api_reference.rst
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 datawords-0.7.0/docs/source/conf.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 datawords-0.7.0/docs/source/index.rst
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 datawords-0.7.0/docs/source/introduction.rst
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 datawords-0.7.0/docs/source/api/deepnlp.rst
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 datawords-0.7.0/docs/source/api/indexes.rst
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 datawords-0.7.0/docs/source/api/models.rst
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 datawords-0.7.0/docs/source/api/parsers.rst
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 datawords-0.7.0/docs/source/api/ranking.rst
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 datawords-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 datawords-0.7.0/tests/shared.py
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 datawords-0.7.0/tests/test_indexes.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 datawords-0.7.0/tests/test_models.py
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 datawords-0.7.0/tests/test_parsers.py
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 datawords-0.7.0/tests/test_rankings.py
+-rw-r--r--   0        0        0    21956 2020-02-02 00:00:00.000000 datawords-0.7.0/tests/texts.txt
+-rw-r--r--   0        0        0     7876 2020-02-02 00:00:00.000000 datawords-0.7.0/.gitignore
+-rw-r--r--   0        0        0    15977 2020-02-02 00:00:00.000000 datawords-0.7.0/LICENSE
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 datawords-0.7.0/NOTICE.md
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 datawords-0.7.0/README.md
+-rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 datawords-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 datawords-0.7.0/PKG-INFO
```

### Comparing `datawords-0.6.2/.pylintrc` & `datawords-0.7.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `datawords-0.6.2/Makefile` & `datawords-0.7.0/Makefile`

 * *Files identical despite different names*

### Comparing `datawords-0.6.2/datawords/_utils.py` & `datawords-0.7.0/datawords/_utils.py`

 * *Files identical despite different names*

### Comparing `datawords-0.6.2/datawords/constants.py` & `datawords-0.7.0/datawords/constants.py`

 * *Files identical despite different names*

### Comparing `datawords-0.6.2/datawords/indexes.py` & `datawords-0.7.0/datawords/indexes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import json
 import os
 import sqlite3
-from typing import Any, Callable, Dict, List, Union
+from typing import Any, Callable, Dict, Iterable, List, Optional, Union
 
 import numpy as np
 from annoy import AnnoyIndex
-from attrs import define, asdict
+from attrs import asdict, define
+from tqdm import tqdm
 
 from datawords import _utils, parsers
 from datawords.models import Word2VecHelper
 
 
 @define
 class LiteDoc:
     """
-    Used by :class:`SQLiteIndex`
+    Represents a document indexed in the :class:`SQLiteIndex`
     """
 
     id: str
     text: str
 
+
 @define
 class TextIndexMeta:
     name: str
     words_model_path: str
     vector_size: int = 100
     ann_trees: int = 10
     distance_metric: str = "angular"
@@ -101,22 +103,24 @@
         else:
             res = [self.id_mapper[_v] for _v in vectors]
         return res
 
     @classmethod
     def build(
         cls,
-        ids: List[Any],
+        ids: Iterable,
         *,
         getter: Callable,
-        words_model_path: str = None,
-        words_model: Word2VecHelper = None,
+        words_model_path: Optional[str] = None,
+        words_model: Optional[Word2VecHelper] = None,
         distance_metric: str = "angular",
         ann_trees: int = 10,
         n_jobs: int = -1,
+        progress_bar=True,
+        total_ids=None,
     ) -> "TextIndex":
         """
         Build the TextIndex . Use as follows:
 
         .. code-block:: python
 
             def getter(id_: str) -> str:
@@ -154,15 +158,15 @@
         :rtype: TextIndex
 
         """
         if not words_model:
             words_model = Word2VecHelper.load(words_model_path, keyed_vectors=True)
         ix = AnnoyIndex(words_model.vector_size, distance_metric)
         id_mapper = {}
-        for _ix, _id in enumerate(ids):
+        for _ix, _id in tqdm(enumerate(ids), disable=not progress_bar, total=total_ids):
             data = getter(_id)
             v = words_model.encode(data)
             ix.add_item(_ix, v)
             id_mapper[_ix] = _id
         ix.build(ann_trees, n_jobs=n_jobs)
         obj = cls(
             words_model=words_model,
@@ -171,15 +175,15 @@
             distance_metric=distance_metric,
             ix=ix,
         )
         return obj
 
     @classmethod
     def load(
-        cls, fp: Union[str, os.PathLike], words_model: Word2VecHelper = None
+        cls, fp: Union[str, os.PathLike], words_model: Optional[Word2VecHelper] = None
     ) -> "TextIndex":
         """loads the TextIndex model.
 
         :param fp: The path to the index. Each model is stored in a folder.
         The path should be to that folder.
         :type fp: Union[str, os.PathLike]
         :param words_model: Optional, the words model to be used.
@@ -315,14 +319,50 @@
             pass
         except sqlite3.OperationalError:
             pass
 
         cur.close()
         return added
 
+    @classmethod
+    def build(
+        cls,
+        ids: Iterable,
+        *,
+        getter: Callable,
+        stopwords=set(),
+        progress_bar=True,
+        total_ids=None,
+        sqlite: str = ":memory:",
+    ) -> "SQLiteIndex":
+        obj = cls(sqlite, stopwords)
+        cur = obj.db.cursor()
+        tracking = []
+        for _id in tqdm(ids, disable=not progress_bar, total=total_ids):
+            data = getter(_id)
+            doc = LiteDoc(
+                id=_id,
+                text=data
+            )
+            try:
+                obj._insert(cur, doc)
+                tracking.append(True)
+            except sqlite3.IntegrityError:
+                tracking.append(False)
+        obj.db.commit()
+        cur.close()
+        return obj
+
+    @classmethod
+    def load(
+        cls, sqlite: str, stopwords=set()
+    ) -> "SQLiteIndex":
+        obj = cls(sqlite, stopwords)
+        return obj
+
     def add_batch(self, docs: List[LiteDoc]) -> List[bool]:
         """
         Add documents in batch.
 
         :param docs: A list of documents
         :type docs: List[LiteDoc]
         :return: True if it was stored or false if not.
@@ -365,15 +405,15 @@
     def total(self) -> int:
         """Returns the total of documents stored in the index."""
         cur = self.db.cursor()
         res = cur.execute("select count(*) from search_index;").fetchone()
         cur.close()
         return res[0]
 
-    def search(self, text: str, limit: int = 1) -> List[LiteDoc]:
+    def search(self, text: str, top_n: int = 5) -> List[LiteDoc]:
         """
         Performs a search in the index.
 
         :param text: text to search.
         :type text: str
         :param limit: how many results retrieve.
         :type limit: int
@@ -382,14 +422,14 @@
         """
         tokens = self._parse(text)
         words = " ".join(tokens)
         cur = self.db.cursor()
         try:
             result = cur.execute(
                 f"""select * from search_docs where text MATCH '"{words}" *'
-                                    limit {limit}"""
+                                    limit {top_n}"""
             ).fetchall()
 
         except sqlite3.OperationalError:
             result = []
         cur.close()
         return [LiteDoc(id=r[0], text=r[1]) for r in result]
```

### Comparing `datawords-0.6.2/datawords/install_pytorch.py` & `datawords-0.7.0/datawords/install_pytorch.py`

 * *Files identical despite different names*

### Comparing `datawords-0.6.2/datawords/models.py` & `datawords-0.7.0/datawords/models.py`

 * *Files identical despite different names*

### Comparing `datawords-0.6.2/datawords/parsers.py` & `datawords-0.7.0/datawords/parsers.py`

 * *Files identical despite different names*

### Comparing `datawords-0.6.2/datawords/ranking.py` & `datawords-0.7.0/datawords/ranking.py`

 * *Files identical despite different names*

### Comparing `datawords-0.6.2/datawords/utils.py` & `datawords-0.7.0/datawords/utils.py`

 * *Files identical despite different names*

### Comparing `datawords-0.6.2/datawords/deepnlp/core.py` & `datawords-0.7.0/datawords/deepnlp/core.py`

 * *Files identical despite different names*

### Comparing `datawords-0.6.2/datawords/deepnlp/translators.py` & `datawords-0.7.0/datawords/deepnlp/translators.py`

 * *Files identical despite different names*

### Comparing `datawords-0.6.2/datawords/deepnlp/translators2.py` & `datawords-0.7.0/datawords/deepnlp/translators2.py`

 * *Files identical despite different names*

### Comparing `datawords-0.6.2/datawords/files/stop_en.txt` & `datawords-0.7.0/datawords/files/stop_en.txt`

 * *Files identical despite different names*

### Comparing `datawords-0.6.2/datawords/files/stop_es.txt` & `datawords-0.7.0/datawords/files/stop_es.txt`

 * *Files identical despite different names*

### Comparing `datawords-0.6.2/datawords/files/stop_pt.txt` & `datawords-0.7.0/datawords/files/stop_pt.txt`

 * *Files identical despite different names*

### Comparing `datawords-0.6.2/docs/Makefile` & `datawords-0.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `datawords-0.6.2/docs/make.bat` & `datawords-0.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `datawords-0.6.2/docs/source/conf.py` & `datawords-0.7.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `datawords-0.6.2/docs/source/index.rst` & `datawords-0.7.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `datawords-0.6.2/docs/source/introduction.rst` & `datawords-0.7.0/docs/source/introduction.rst`

 * *Files identical despite different names*

### Comparing `datawords-0.6.2/docs/source/api/deepnlp.rst` & `datawords-0.7.0/docs/source/api/deepnlp.rst`

 * *Files identical despite different names*

### Comparing `datawords-0.6.2/docs/source/api/parsers.rst` & `datawords-0.7.0/docs/source/api/parsers.rst`

 * *Files identical despite different names*

### Comparing `datawords-0.6.2/tests/test_models.py` & `datawords-0.7.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `datawords-0.6.2/tests/test_parsers.py` & `datawords-0.7.0/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `datawords-0.6.2/tests/test_rankings.py` & `datawords-0.7.0/tests/test_rankings.py`

 * *Files identical despite different names*

### Comparing `datawords-0.6.2/tests/texts.txt` & `datawords-0.7.0/tests/texts.txt`

 * *Files identical despite different names*

### Comparing `datawords-0.6.2/.gitignore` & `datawords-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `datawords-0.6.2/LICENSE` & `datawords-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datawords-0.6.2/README.md` & `datawords-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `datawords-0.6.2/pyproject.toml` & `datawords-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datawords-0.6.2/PKG-INFO` & `datawords-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datawords
-Version: 0.6.2
+Version: 0.7.0
 Summary: A library to work with text data
 Project-URL: Documentation, https://github.com/unknown/datawords#readme
 Project-URL: Issues, https://github.com/unknown/datawords/issues
 Project-URL: Source, https://github.com/unknown/datawords
 Author-email: Xavier Petit <nuxion@gmail.com>
 License-Expression: MPL-2.0
 License-File: LICENSE
```

