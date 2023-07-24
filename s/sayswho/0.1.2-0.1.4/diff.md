# Comparing `tmp/sayswho-0.1.2.tar.gz` & `tmp/sayswho-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sayswho-0.1.2.tar", max compression
+gzip compressed data, was "sayswho-0.1.4.tar", max compression
```

## Comparing `sayswho-0.1.2.tar` & `sayswho-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     5267 2023-07-15 21:17:54.348528 sayswho-0.1.2/README.md
--rw-r--r--   0        0        0      523 2023-07-15 20:40:09.241683 sayswho-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     9943 2023-07-16 00:40:03.229641 sayswho-0.1.2/src/sayswho/__init__.py
--rw-r--r--   0        0        0     2540 2023-07-15 20:14:27.794617 sayswho-0.1.2/src/sayswho/constants.py
--rw-r--r--   0        0        0    13743 2023-07-16 00:27:39.870034 sayswho-0.1.2/src/sayswho/helpers.py
--rw-r--r--   0        0        0     7665 2023-07-15 20:59:33.663389 sayswho-0.1.2/src/sayswho/quote_finder.py
--rw-r--r--   0        0        0     1780 2023-07-16 00:32:31.931359 sayswho-0.1.2/src/sayswho/template.html
--rw-r--r--   0        0        0     6097 1970-01-01 00:00:00.000000 sayswho-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     5576 2023-07-24 19:57:47.290495 sayswho-0.1.4/README.md
+-rw-r--r--   0        0        0      523 2023-07-24 20:01:03.198312 sayswho-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0    10886 2023-07-24 19:54:57.763512 sayswho-0.1.4/src/sayswho/__init__.py
+-rw-r--r--   0        0        0     2540 2023-07-15 20:14:27.794617 sayswho-0.1.4/src/sayswho/constants.py
+-rw-r--r--   0        0        0    13752 2023-07-24 19:33:13.901937 sayswho-0.1.4/src/sayswho/helpers.py
+-rw-r--r--   0        0        0     7657 2023-07-24 19:02:19.255908 sayswho-0.1.4/src/sayswho/quote_finder.py
+-rw-r--r--   0        0        0     6406 1970-01-01 00:00:00.000000 sayswho-0.1.4/PKG-INFO
```

### Comparing `sayswho-0.1.2/README.md` & `sayswho-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,24 +6,32 @@
 
 - SaysWho grew out of a larger project for analyzing newspaper articles from Lexis between ~250 and ~2000 words, and it is optimized to navitage the syntax and common errors particular to that text.
 
 - The output of this version is kind of open-ended, and possibly not as useful as it could be. HTML viz is coming, but I'm open to any suggestions about how this could be more useful!
 
 ## Installation
 Install and update using [pip](https://pip.pypa.io/en/stable/):
-
 ```
 $ pip install sayswho
 ```
 
-You will probably need to do this to navigate some versioning issues (see [Notes](#notes))
 
+Install the pre-trained SpaCy coreferencing pipeline.
+```
+$ pip install https://github.com/explosion/spacy-experimental/releases/download/v0.6.1/en_coreference_web_trf-3.4.0a2-py3-none-any.whl
+```
+
+(Optional) If you want to use the most recent version of SpaCy, you will need to update it here. (see [Notes](#notes))
 ```
-$ pip install https://github.com/explosion/spacy-experimental/releases/download/v0.6.0/en_coreference_web_trf-3.4.0a0-py3-none-any.whl
 $ pip install spacy -U
+```
+
+
+Download the SpaCy large english model.
+```
 $ spacy download en_core_web_lg
 ```
 
 ## A Simple Example
 
 ##### Sample text adapted from [here](https://sports.yahoo.com/nets-jacque-vaughn-looking-forward-150705556.html):
 > Nets Coach Jacque Vaughn was optimistic when discussing Ben Simmons's prospects on NBA TV.
@@ -150,9 +158,13 @@
 QUOTE : 3
  DQTriple(speaker=[Vaughn], cue=[told], content=“We’ll continue to see him improve through the offseason.”) 
 
 CLUSTER : 1
  ['Nets Coach Jacque Vaughn', 'Vaughn'] 
 ```
 
-    
+#### Use `.render_to_html()` to output an HTML file with your text, highlighted quotes, and associated clusters.
+
+```
+sw.render_to_html(article_title="My Article Title")
+```
```

### Comparing `sayswho-0.1.2/pyproject.toml` & `sayswho-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sayswho"
-version = "0.1.2"
+version = "0.1.4"
 license = "MIT"
 description = "Quote identification, attribution and resolution."
 authors = ["Andy Friedman <afriedman412@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/afriedman412/sayswho"
 keywords = ["nlp", "natural-language-processing", "spacy"]
```

### Comparing `sayswho-0.1.2/src/sayswho/__init__.py` & `sayswho-0.1.4/src/sayswho/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import numpy as np
 import regex as re
 from .quote_finder import quote_finder
 from . import constants
 from . import helpers
 from jinja2 import Environment, FileSystemLoader
 
+
 class SaysWho:
     """
     Main class for package. Instantiation loads spacy models so they don't have to be loaded again for repeat use.
 
     Input:
         text (str) - if provided, text will be analyzed on instantiation
         coref_nlp (str) - name of coref model
@@ -20,46 +21,46 @@
 
     def __init__(
         self,
         text: str = None,
         coref_nlp: str = "en_coreference_web_trf",
         base_nlp: str = "en_core_web_lg",
         prune: bool = True,
-        prep_text: bool = True
+        prep_text: bool = True,
     ):
-        self.coref_nlp = spacy.load(coref_nlp)
-        self.base_nlp = spacy.load(base_nlp)
+        for v in ["coref_nlp", "base_nlp"]:
+            if not spacy.util.is_package(eval(v)):
+                raise OSError(
+                    f"SpaCy model {v} not installed. See README for instructions on how to install models."
+                )
+            self.__setattr__(v, spacy.load(eval(v)))
         self.prune = prune
         self.prep_text = prep_text
         if text:
             self.attribute(text)
 
     def expand_match(self, match=None):
         """
         Makes QuoteClusterMatch (or a list of QuoteClusterMatches) human-interpretable.
 
         Input:
             match (None, QuoteClusterMatch or list[QuoteClusterMatch]) - the QuoteClusterMatch(s) to be interpreted. Uses self.quote_matches if nothing is proivded.
         """
         if not match:
             match = self.quote_matches
-            
+
         if isinstance(match, list):
             for m in match:
                 self.expand_match(m)
         else:
             for m_ in ["quote", "cluster", "person"]:
                 if getattr(match, f"{m_}_index", None) is not None:
                     i = eval(f"self.{m_}s")
                     v = getattr(match, f"{m_}_index")
-                    data = (
-                        helpers.format_cluster(i[v])
-                        if m_ == "cluster"
-                        else i[v]
-                    )
+                    data = helpers.format_cluster(i[v]) if m_ == "cluster" else i[v]
                     print(m_.upper(), f": {v}" "\n", data, "\n")
         return
 
     def attribute(self, text: str):
         """
         Top level function. Parses text, matches quotes to clusters and gets ent matches.
         Input:
@@ -98,16 +99,16 @@
         # extract coref clusters and clone to doc
         self.clusters = [
             helpers.clone_cluster(cluster, self.doc)
             for k, cluster in self.coref_doc.spans.items()
             if k.startswith("coref")
         ]
         if self.prune:
-            self.clusters = [helpers.prune_cluster_people(cluster)
-                for cluster in self.clusters
+            self.clusters = [
+                helpers.prune_cluster_people(cluster) for cluster in self.clusters
             ]
 
         self.persons = [e for e in self.doc.ents if e.label_ == "PERSON"]
         return
 
     def get_matches(self):
         """
@@ -118,37 +119,39 @@
         """
         pairs_dicto = self.make_pairs()
         arrays = {k: self.make_matrix(k, v) for k, v in pairs_dicto.items()}
 
         big_matrix = np.concatenate(
             (
                 np.transpose(
-                np.nonzero(
-                    arrays["quotes_persons"].dot(
-                        arrays["clusters_persons"].T
+                    np.nonzero(
+                        arrays["quotes_persons"].dot(arrays["clusters_persons"].T)
                     )
-                )
-            ),
-            np.transpose(np.nonzero(arrays["quotes_clusters"])),
+                ),
+                np.transpose(np.nonzero(arrays["quotes_clusters"])),
             )
         )
 
-        results = sorted(list(set(
-            [constants.QuoteClusterMatch(i,j) for i,j in big_matrix]
-            )), key=lambda m: m.quote_index)
+        results = sorted(
+            list(set([constants.QuoteClusterMatch(i, j) for i, j in big_matrix])),
+            key=lambda m: m.quote_index,
+        )
 
         return results
 
     def make_pairs(self) -> dict:
         """
         Creates quote/person, quote/cluster and cluster/person pairs for resolution and cleaning.
 
         TODO: Ensure pronouns aren't being skipped!
         TODO: Make ratio threshold a variable
         """
+        if not all([v in self.__dict__ for v in ["quotes", "clusters", "persons"]]):
+            raise Exception("No text parsed -- run SaysWho.attribute(text).")
+
         pairs_dicto = {
             p: []
             for p in [
                 "quotes_persons",
                 "quotes_clusters",
             ]
         }
@@ -186,56 +189,74 @@
         ]
         return pairs_dicto
 
     def make_matrix(self, key: str, pairs: list[tuple]) -> np.array:
         """
         Convenience function for converting quote/cluster, quote/person and cluster/person pairs into binary matrices.
 
-        Input: 
+        Input:
             key (str) - data types in pairs, connected by "_" (ie "quotes_clusters" means the pairs data is (quote, cluster))
             pairs (list[tuple]) - (data type 1, data type 2) matches
 
         Output:
             m (np.array) - binary matrix of existing data type matches
         """
         x, y = key.split("_")
         m = np.zeros([len(self.__getattribute__(_)) for _ in [x, y]])
         for i, j in pairs:
             m[i, j] = 1
         return m
-    
+
     def print_clusters(self):
         """
         Print clusters with duplicate text removed. For easier interpretation!
         """
         for n, cluster in enumerate(self.clusters):
             print(n, set(t.text for t in cluster))
 
     # VIZ CODE
     def process_quote_for_rendering(self, quote_match):
         quote = {
             "content": self.quotes[quote_match.quote_index].content,
-            "cue": "".join([t.text_with_ws for t in self.quotes[quote_match.quote_index].cue]),
-            "cluster": ', '.join(
-                set([c.text for c in self.clusters[quote_match.cluster_index] if c[0].pos_ !="PRON"])) 
+            "cue": "".join(
+                [t.text_with_ws for t in self.quotes[quote_match.quote_index].cue]
+            ),
+            "cluster": ", ".join(
+                set(
+                    [
+                        c.text
+                        for c in self.clusters[quote_match.cluster_index]
+                        if c[0].pos_ != "PRON"
+                    ]
+                )
+            ),
         }
         return quote
-    
+
     def yield_quotes(self):
         for quote_index in range(len(self.quotes)):
-            for m in (qm for qm in self.quote_matches if qm.quote_index==quote_index):
+            for m in (qm for qm in self.quote_matches if qm.quote_index == quote_index):
                 base_dict = self.process_quote_for_rendering(m)
-                base_dict['cluster_index'] = m.cluster_index
-                base_dict['cluster'] = ', '.join(
-                    set([c.text for c in self.clusters[m.cluster_index] if c[0].pos_ !="PRON"])
+                base_dict["cluster_index"] = m.cluster_index
+                base_dict["cluster"] = ", ".join(
+                    set(
+                        [
+                            c.text
+                            for c in self.clusters[m.cluster_index]
+                            if c[0].pos_ != "PRON"
+                        ]
+                    )
                 )
-            yield(base_dict)
-    
+            yield (base_dict)
+
     def process_text_into_html(self):
-        quote_indexes = [((q.content.start, q.content.end), "QUOTE", n) for n, q in enumerate(self.quotes)]
+        quote_indexes = [
+            ((q.content.start, q.content.end), "QUOTE", n)
+            for n, q in enumerate(self.quotes)
+        ]
         html_output = "<p>"
         color_key = {}
         for token in self.doc:
             coded = False
             if token.text == "\n":
                 token_text = "<br>"
             else:
@@ -247,24 +268,38 @@
                 html_output += helpers.generate_code(n, label, start, color_key)
                 html_output += token_text
             if not coded:
                 html_output += token_text
 
         html_output += "</p>"
         return html_output
-    
-    def render_to_html(self, file_name: str = "temp.html"):
+
+    def render_to_html(
+        self,
+        article_title: str = "My Article",
+        output_path: str = "temp.html",
+        save_file: bool = True,
+    ):
         metadata = {
-            "title": "my article",
+            "title": article_title,
             "bodytext": self.process_text_into_html(),
-            "quotes": list(self.yield_quotes())
+            "quotes": list(self.yield_quotes()),
         }
-        rendered = Environment(
-            loader=FileSystemLoader("./")
-        ).get_template('template.html').render(metadata)
-
-        with open(f"{file_name}.html", "w+") as f:
-            try:
-                f.write(rendered)
-            except UnicodeDecodeError:
-                rendered = re.sub("\u2014", "-", rendered)
-                f.write(rendered)
+        rendered = (
+            Environment(loader=FileSystemLoader("./"))
+            .get_template("template.html")
+            .render(metadata)
+        )
+
+        if save_file:
+            if not output_path.endswith(".html"):
+                output_path = output_path + ".html"
+            with open(output_path, "w+") as f:
+                try:
+                    f.write(rendered)
+                except UnicodeDecodeError:
+                    rendered = re.sub("\u2014", "-", rendered)
+                    f.write(rendered)
+            return
+
+        else:
+            return rendered
```

### Comparing `sayswho-0.1.2/src/sayswho/constants.py` & `sayswho-0.1.4/src/sayswho/constants.py`

 * *Files identical despite different names*

### Comparing `sayswho-0.1.2/src/sayswho/helpers.py` & `sayswho-0.1.4/src/sayswho/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -284,14 +284,15 @@
     return all(
         [
             abs(getattr(s1, attr) - getattr(s2, attr)) < MIN_ENTITY_DIFF
             for attr in ["start", "end"]
         ]
     )
 
+
 def filter_cue_candidates(tok):
     return all([tok.pos == VERB, tok.lemma_ in _reporting_verbs])
 
 
 def filter_speaker_candidates(ch, i, j):
     return all(
         [
@@ -443,22 +444,24 @@
 
 
 def prep_text_for_quote_detection(t, para_char="\n", exp: bool = False):
     return para_char.join(
         [para_quote_fixer(p, exp=exp) for p in t.split(para_char) if p]
     )
 
+
 # VIZ
-def generate_code(
-        n: int, label: str, start: bool=True, color_key: dict={}
-    ) -> str:
+def generate_code(n: int, label: str, start: bool = True, color_key: dict = {}) -> str:
+    if label in color_key:
         color = color_key.get(label)
-        if label.lower()=='quote':
-            if start:
-                return f"<a name=\"quote{n}\"></a><a href=\"#{n}\"><span id=\"QUOTE\" style=\"background-color: {color};\">"
-            else:
-                return "</span></a>"
+    else:
+        color = "PapayaWhip"
+    if label.lower() == "quote":
+        if start:
+            return f'<a name="quote{n}"></a><a href="#{n}"><span id="QUOTE" style="background-color: {color};">'
+        else:
+            return "</span></a>"
+    else:
+        if start:
+            return f'<span id="{label}" style="color: {color};">'
         else:
-            if start:
-                return f"<span id=\"{label}\" style=\"color: {color};\">"
-            else:
-                return "</span>"
+            return "</span>"
```

### Comparing `sayswho-0.1.2/src/sayswho/quote_finder.py` & `sayswho-0.1.4/src/sayswho/quote_finder.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,18 +5,17 @@
 from . import constants
 from operator import attrgetter
 import regex as re
 from typing import Literal, Iterable
 from spacy.tokens import Doc, Token, Span
 from spacy.symbols import VERB, PUNCT
 
+
 def quote_finder(doc: Doc):
-    """
-    
-    """
+    """ """
     qtoks = [tok for tok in doc if tok.is_quote or (re.match(r"\n", tok.text))]
     qtok_idx_pairs = [(-1, -1)]
     for n, q in enumerate(qtoks):
         if (
             not bool(q.whitespace_)
             and q.i not in [q_[1] for q_ in qtok_idx_pairs]
             and q.i > qtok_idx_pairs[-1][1]
```

### Comparing `sayswho-0.1.2/PKG-INFO` & `sayswho-0.1.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sayswho
-Version: 0.1.2
+Version: 0.1.4
 Summary: Quote identification, attribution and resolution.
 Home-page: https://github.com/afriedman412/sayswho
 License: MIT
 Keywords: nlp,natural-language-processing,spacy
 Author: Andy Friedman
 Author-email: afriedman412@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -28,24 +28,32 @@
 
 - SaysWho grew out of a larger project for analyzing newspaper articles from Lexis between ~250 and ~2000 words, and it is optimized to navitage the syntax and common errors particular to that text.
 
 - The output of this version is kind of open-ended, and possibly not as useful as it could be. HTML viz is coming, but I'm open to any suggestions about how this could be more useful!
 
 ## Installation
 Install and update using [pip](https://pip.pypa.io/en/stable/):
-
 ```
 $ pip install sayswho
 ```
 
-You will probably need to do this to navigate some versioning issues (see [Notes](#notes))
 
+Install the pre-trained SpaCy coreferencing pipeline.
+```
+$ pip install https://github.com/explosion/spacy-experimental/releases/download/v0.6.1/en_coreference_web_trf-3.4.0a2-py3-none-any.whl
+```
+
+(Optional) If you want to use the most recent version of SpaCy, you will need to update it here. (see [Notes](#notes))
 ```
-$ pip install https://github.com/explosion/spacy-experimental/releases/download/v0.6.0/en_coreference_web_trf-3.4.0a0-py3-none-any.whl
 $ pip install spacy -U
+```
+
+
+Download the SpaCy large english model.
+```
 $ spacy download en_core_web_lg
 ```
 
 ## A Simple Example
 
 ##### Sample text adapted from [here](https://sports.yahoo.com/nets-jacque-vaughn-looking-forward-150705556.html):
 > Nets Coach Jacque Vaughn was optimistic when discussing Ben Simmons's prospects on NBA TV.
@@ -172,10 +180,14 @@
 QUOTE : 3
  DQTriple(speaker=[Vaughn], cue=[told], content=“We’ll continue to see him improve through the offseason.”) 
 
 CLUSTER : 1
  ['Nets Coach Jacque Vaughn', 'Vaughn'] 
 ```
 
-    
+#### Use `.render_to_html()` to output an HTML file with your text, highlighted quotes, and associated clusters.
+
+```
+sw.render_to_html(article_title="My Article Title")
+```
```

