# Comparing `tmp/mdgpt-0.1.1.tar.gz` & `tmp/mdgpt-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdgpt-0.1.1.tar", max compression
+gzip compressed data, was "mdgpt-0.1.2.tar", max compression
```

## Comparing `mdgpt-0.1.1.tar` & `mdgpt-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1064 2023-07-18 20:46:07.614765 mdgpt-0.1.1/LICENSE
--rw-r--r--   0        0        0      274 2023-07-22 23:02:13.763187 mdgpt-0.1.1/mdgpt/__init__.py
--rw-r--r--   0        0        0     2852 2023-07-23 10:43:22.221126 mdgpt-0.1.1/mdgpt/build.py
--rw-r--r--   0        0        0      502 2023-07-22 23:00:37.776738 mdgpt-0.1.1/mdgpt/misc.py
--rw-r--r--   0        0        0     8884 2023-07-23 10:55:28.885589 mdgpt-0.1.1/mdgpt/translate.py
--rw-r--r--   0        0        0     2479 2023-07-22 23:01:02.240963 mdgpt-0.1.1/mdgpt/utils.py
--rw-r--r--   0        0        0      735 2023-07-23 20:41:52.004138 mdgpt-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1002 2023-07-23 20:41:56.179154 mdgpt-0.1.1/setup.py
--rw-r--r--   0        0        0      634 2023-07-23 20:41:56.179427 mdgpt-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-18 20:46:07.614765 mdgpt-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3723 2023-07-24 00:30:06.355169 mdgpt-0.1.2/README.md
+-rw-r--r--   0        0        0      274 2023-07-22 23:02:13.763187 mdgpt-0.1.2/mdgpt/__init__.py
+-rw-r--r--   0        0        0     2852 2023-07-23 10:43:22.221126 mdgpt-0.1.2/mdgpt/build.py
+-rw-r--r--   0        0        0      448 2023-07-24 10:56:16.849596 mdgpt-0.1.2/mdgpt/misc.py
+-rw-r--r--   0        0        0     8884 2023-07-23 10:55:28.885589 mdgpt-0.1.2/mdgpt/translate.py
+-rw-r--r--   0        0        0     2479 2023-07-22 23:01:02.240963 mdgpt-0.1.2/mdgpt/utils.py
+-rw-r--r--   0        0        0      939 2023-07-24 10:56:01.389335 mdgpt-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4943 2023-07-24 10:57:06.348308 mdgpt-0.1.2/setup.py
+-rw-r--r--   0        0        0     4573 2023-07-24 10:57:06.348687 mdgpt-0.1.2/PKG-INFO
```

### Comparing `mdgpt-0.1.1/LICENSE` & `mdgpt-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mdgpt-0.1.1/mdgpt/build.py` & `mdgpt-0.1.2/mdgpt/build.py`

 * *Files identical despite different names*

### Comparing `mdgpt-0.1.1/mdgpt/translate.py` & `mdgpt-0.1.2/mdgpt/translate.py`

 * *Files identical despite different names*

### Comparing `mdgpt-0.1.1/mdgpt/utils.py` & `mdgpt-0.1.2/mdgpt/utils.py`

 * *Files identical despite different names*

### Comparing `mdgpt-0.1.1/pyproject.toml` & `mdgpt-0.1.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -8,18 +8,22 @@
   | dist
   | venv
 )/
 '''
 
 [tool.poetry]
 name = "mdgpt"
-version = "0.1.1"
-description = "Translate and generate static site from Markdown files using ChatGTP"
+version = "0.1.2"
+description = "Translate markdown files using OpenAI ChatGPT, and generate localized copies of each file."
 authors = ["Jeppe Bårris <jeppe@barris.dk>"]
 license = "MIT"
+readme = "README.md"
+homepage = "https://github.com/Djarnis/mdGPT"
+repository = "https://github.com/Djarnis/mdGPT"
+keywords = ["markdown", "translation", "openai", "chatgpt", "gpt"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 python-frontmatter = "^1.0.0"
 requests = "^2.31.0"
 pycountry = "^22.3.5"
 openai = "^0.27.8"
```

