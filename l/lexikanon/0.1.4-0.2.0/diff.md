# Comparing `tmp/lexikanon-0.1.4.tar.gz` & `tmp/lexikanon-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lexikanon-0.1.4.tar", max compression
+gzip compressed data, was "lexikanon-0.2.0.tar", max compression
```

## Comparing `lexikanon-0.1.4.tar` & `lexikanon-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,42 @@
--rw-r--r--   0        0        0     1071 2023-07-24 07:39:52.669796 lexikanon-0.1.4/LICENSE
--rw-r--r--   0        0        0     2129 2023-07-24 07:39:52.669796 lexikanon-0.1.4/README.md
--rw-r--r--   0        0        0     2881 2023-07-24 07:40:20.670040 lexikanon-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      184 2023-07-24 07:39:52.673796 lexikanon-0.1.4/src/lexikanon/__cli__.py
--rw-r--r--   0        0        0      464 2023-07-24 07:39:52.673796 lexikanon-0.1.4/src/lexikanon/__init__.py
--rw-r--r--   0        0        0       22 2023-07-24 07:40:20.614040 lexikanon-0.1.4/src/lexikanon/_version.py
--rw-r--r--   0        0        0        0 2023-07-24 07:39:52.673796 lexikanon-0.1.4/src/lexikanon/conf/__init__.py
--rw-r--r--   0        0        0      177 2023-07-24 07:39:52.673796 lexikanon-0.1.4/src/lexikanon/conf/about/lexikanon.yaml
--rw-r--r--   0        0        0      195 2023-07-24 07:39:52.673796 lexikanon-0.1.4/src/lexikanon/project.toml
--rw-r--r--   0        0        0        0 2023-07-24 07:39:52.673796 lexikanon-0.1.4/src/lexikanon/py.typed
--rw-r--r--   0        0        0     2806 1970-01-01 00:00:00.000000 lexikanon-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-24 09:29:24.392688 lexikanon-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2129 2023-07-24 09:29:24.392688 lexikanon-0.2.0/README.md
+-rw-r--r--   0        0        0     2932 2023-07-24 09:30:10.645084 lexikanon-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      184 2023-07-24 09:29:24.396689 lexikanon-0.2.0/src/lexikanon/__cli__.py
+-rw-r--r--   0        0        0      464 2023-07-24 09:29:24.396689 lexikanon-0.2.0/src/lexikanon/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-24 09:30:10.577083 lexikanon-0.2.0/src/lexikanon/_version.py
+-rw-r--r--   0        0        0        0 2023-07-24 09:29:24.396689 lexikanon-0.2.0/src/lexikanon/conf/__init__.py
+-rw-r--r--   0        0        0      177 2023-07-24 09:29:24.396689 lexikanon-0.2.0/src/lexikanon/conf/about/lexikanon.yaml
+-rw-r--r--   0        0        0      169 2023-07-24 09:29:24.396689 lexikanon-0.2.0/src/lexikanon/conf/normalizer/__init__.yaml
+-rw-r--r--   0        0        0       54 2023-07-24 09:29:24.396689 lexikanon-0.2.0/src/lexikanon/conf/normalizer/formal_en.yaml
+-rw-r--r--   0        0        0       77 2023-07-24 09:29:24.396689 lexikanon-0.2.0/src/lexikanon/conf/normalizer/formal_en_parantheses.yaml
+-rw-r--r--   0        0        0       43 2023-07-24 09:29:24.396689 lexikanon-0.2.0/src/lexikanon/conf/normalizer/formal_ko.yaml
+-rw-r--r--   0        0        0      363 2023-07-24 09:29:24.396689 lexikanon-0.2.0/src/lexikanon/conf/normalizer/ftfy/__init__.yaml
+-rw-r--r--   0        0        0       67 2023-07-24 09:29:24.396689 lexikanon-0.2.0/src/lexikanon/conf/normalizer/informal_ko.yaml
+-rw-r--r--   0        0        0      102 2023-07-24 09:29:24.396689 lexikanon-0.2.0/src/lexikanon/conf/normalizer/spaces/__init__.yaml
+-rw-r--r--   0        0        0      151 2023-07-24 09:29:24.396689 lexikanon-0.2.0/src/lexikanon/conf/normalizer/special_characters/__init__.yaml
+-rw-r--r--   0        0        0      143 2023-07-24 09:29:24.396689 lexikanon-0.2.0/src/lexikanon/conf/stopwords/__init__.yaml
+-rw-r--r--   0        0        0      491 2023-07-24 09:29:24.396689 lexikanon-0.2.0/src/lexikanon/conf/tokenizer/__init__.yaml
+-rw-r--r--   0        0        0      238 2023-07-24 09:29:24.396689 lexikanon-0.2.0/src/lexikanon/conf/tokenizer/mecab.yaml
+-rw-r--r--   0        0        0      151 2023-07-24 09:29:24.396689 lexikanon-0.2.0/src/lexikanon/conf/tokenizer/nltk.yaml
+-rw-r--r--   0        0        0       84 2023-07-24 09:29:24.396689 lexikanon-0.2.0/src/lexikanon/conf/tokenizer/simple.yaml
+-rw-r--r--   0        0        0       88 2023-07-24 09:29:24.396689 lexikanon-0.2.0/src/lexikanon/conf/tokenizer/tagger/mecab.yaml
+-rw-r--r--   0        0        0      125 2023-07-24 09:29:24.396689 lexikanon-0.2.0/src/lexikanon/conf/tokenizer/tagger/nltk.yaml
+-rw-r--r--   0        0        0       61 2023-07-24 09:29:24.396689 lexikanon-0.2.0/src/lexikanon/normalizers/__init__.py
+-rw-r--r--   0        0        0    10196 2023-07-24 09:29:24.396689 lexikanon-0.2.0/src/lexikanon/normalizers/normalizer.py
+-rw-r--r--   0        0        0      195 2023-07-24 09:29:24.396689 lexikanon-0.2.0/src/lexikanon/project.toml
+-rw-r--r--   0        0        0        0 2023-07-24 09:29:24.396689 lexikanon-0.2.0/src/lexikanon/py.typed
+-rw-r--r--   0        0        0  2355775 2023-07-24 09:29:24.412689 lexikanon-0.2.0/src/lexikanon/resources/dictionaries/mecab/ekon_v1.dic
+-rw-r--r--   0        0        0       58 2023-07-24 09:29:24.412689 lexikanon-0.2.0/src/lexikanon/stopwords/__init__.py
+-rw-r--r--   0        0        0     2803 2023-07-24 09:29:24.412689 lexikanon-0.2.0/src/lexikanon/stopwords/stopwords.py
+-rw-r--r--   0        0        0      181 2023-07-24 09:29:24.412689 lexikanon-0.2.0/src/lexikanon/tokenizers/__init__.py
+-rw-r--r--   0        0        0     9219 2023-07-24 09:29:24.412689 lexikanon-0.2.0/src/lexikanon/tokenizers/base.py
+-rw-r--r--   0        0        0      732 2023-07-24 09:29:24.412689 lexikanon-0.2.0/src/lexikanon/tokenizers/mecab.py
+-rw-r--r--   0        0        0     3074 2023-07-24 09:29:24.412689 lexikanon-0.2.0/src/lexikanon/tokenizers/nltk.py
+-rw-r--r--   0        0        0    14339 2023-07-24 09:29:24.412689 lexikanon-0.2.0/src/lexikanon/utils/__init__.py
+-rw-r--r--   0        0        0     8294 2023-07-24 09:29:24.412689 lexikanon-0.2.0/src/lexikanon/utils/hangle.py
+-rw-r--r--   0        0        0      255 2023-07-24 09:29:24.412689 lexikanon-0.2.0/src/lexikanon/utils/hanja/__init__.py
+-rw-r--r--   0        0        0     2123 2023-07-24 09:29:24.412689 lexikanon-0.2.0/src/lexikanon/utils/hanja/hangul.py
+-rw-r--r--   0        0        0     2813 2023-07-24 09:29:24.412689 lexikanon-0.2.0/src/lexikanon/utils/hanja/impl.py
+-rw-r--r--   0        0        0      427 2023-07-24 09:29:24.412689 lexikanon-0.2.0/src/lexikanon/utils/hanja/table.py
+-rw-r--r--   0        0        0   522443 2023-07-24 09:29:24.412689 lexikanon-0.2.0/src/lexikanon/utils/hanja/table.yml
+-rw-r--r--   0        0        0     2920 1970-01-01 00:00:00.000000 lexikanon-0.2.0/PKG-INFO
```

### Comparing `lexikanon-0.1.4/LICENSE` & `lexikanon-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lexikanon-0.1.4/README.md` & `lexikanon-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `lexikanon-0.1.4/pyproject.toml` & `lexikanon-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lexikanon"
-version = "0.1.4"
+version = "0.2.0"
 description = "A Python Library for Tokenizers"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://lexikanon.entelecheia.ai"
 repository = "https://github.com/entelecheia/lexikanon"
 readme = "README.md"
 packages = [{ include = "lexikanon", from = "src" }]
@@ -12,14 +12,17 @@
 [tool.poetry.scripts]
 lexikanon = 'lexikanon.__cli__:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
 click = "^8.1.3"
 hyfi = "^1.8.3"
+ftfy = "^6.1.1"
+nltk = "^3.8.1"
+ekonlpy = "^2.0.1"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
 isort = "^5.12.0"
```

### Comparing `lexikanon-0.1.4/PKG-INFO` & `lexikanon-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: lexikanon
-Version: 0.1.4
+Version: 0.2.0
 Summary: A Python Library for Tokenizers
 Home-page: https://lexikanon.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: ekonlpy (>=2.0.1,<3.0.0)
+Requires-Dist: ftfy (>=6.1.1,<7.0.0)
 Requires-Dist: hyfi (>=1.8.3,<2.0.0)
+Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Project-URL: Repository, https://github.com/entelecheia/lexikanon
 Description-Content-Type: text/markdown
 
 # Lexikanon
 
 [![pypi-image]][pypi-url]
 [![version-image]][release-url]
```

