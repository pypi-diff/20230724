# Comparing `tmp/sib-commit-parser-0.3.4.tar.gz` & `tmp/sib-commit-parser-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sib-commit-parser-0.3.4.tar", last modified: Fri Apr 17 10:46:28 2020, max compression
+gzip compressed data, was "sib-commit-parser-1.0.0.tar", last modified: Mon Jul 24 18:43:27 2023, max compression
```

## Comparing `sib-commit-parser-0.3.4.tar` & `sib-commit-parser-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-17 10:46:28.000000 sib-commit-parser-0.3.4/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-17 10:46:28.000000 sib-commit-parser-0.3.4/sib_commit_parser.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2020-04-17 10:46:28.000000 sib-commit-parser-0.3.4/sib_commit_parser.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2020-04-17 10:46:28.000000 sib-commit-parser-0.3.4/sib_commit_parser.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2020-04-17 10:46:28.000000 sib-commit-parser-0.3.4/sib_commit_parser.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      282 2020-04-17 10:46:28.000000 sib-commit-parser-0.3.4/sib_commit_parser.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     2060 2020-04-17 10:46:28.000000 sib-commit-parser-0.3.4/sib_commit_parser.egg-info/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-17 10:46:28.000000 sib-commit-parser-0.3.4/commit_parser/
--rw-rw-rw-   0 root         (0) root         (0)     2030 2020-04-17 10:46:11.000000 sib-commit-parser-0.3.4/commit_parser/parser.py
--rw-rw-rw-   0 root         (0) root         (0)       73 2020-04-17 10:46:26.000000 sib-commit-parser-0.3.4/commit_parser/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      614 2020-04-17 10:46:28.000000 sib-commit-parser-0.3.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1309 2020-04-17 10:46:11.000000 sib-commit-parser-0.3.4/README.md
--rw-rw-rw-   0 root         (0) root         (0)       61 2020-04-17 10:46:11.000000 sib-commit-parser-0.3.4/setup.py
--rw-r--r--   0 root         (0) root         (0)     2060 2020-04-17 10:46:28.000000 sib-commit-parser-0.3.4/PKG-INFO
+drwxrwxr-x   0 balessan  (1001) balessan  (1001)        0 2023-07-24 18:43:27.904923 sib-commit-parser-1.0.0/
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)     1570 2023-07-24 18:43:27.904923 sib-commit-parser-1.0.0/PKG-INFO
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)     1309 2023-07-24 18:18:30.000000 sib-commit-parser-1.0.0/README.md
+drwxrwxr-x   0 balessan  (1001) balessan  (1001)        0 2023-07-24 18:43:27.904923 sib-commit-parser-1.0.0/commit_parser/
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)       73 2023-07-24 18:43:25.000000 sib-commit-parser-1.0.0/commit_parser/__init__.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)     2599 2023-07-24 18:37:52.000000 sib-commit-parser-1.0.0/commit_parser/parser.py
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)      614 2023-07-24 18:43:27.904923 sib-commit-parser-1.0.0/setup.cfg
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)       61 2023-07-24 18:18:30.000000 sib-commit-parser-1.0.0/setup.py
+drwxrwxr-x   0 balessan  (1001) balessan  (1001)        0 2023-07-24 18:43:27.904923 sib-commit-parser-1.0.0/sib_commit_parser.egg-info/
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)     1570 2023-07-24 18:43:27.000000 sib-commit-parser-1.0.0/sib_commit_parser.egg-info/PKG-INFO
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)      282 2023-07-24 18:43:27.000000 sib-commit-parser-1.0.0/sib_commit_parser.egg-info/SOURCES.txt
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)        1 2023-07-24 18:43:27.000000 sib-commit-parser-1.0.0/sib_commit_parser.egg-info/dependency_links.txt
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)       31 2023-07-24 18:43:27.000000 sib-commit-parser-1.0.0/sib_commit_parser.egg-info/requires.txt
+-rw-rw-r--   0 balessan  (1001) balessan  (1001)       14 2023-07-24 18:43:27.000000 sib-commit-parser-1.0.0/sib_commit_parser.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sib-commit-parser-0.3.4/sib_commit_parser.egg-info/PKG-INFO` & `sib-commit-parser-1.0.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,66 +1,64 @@
 Metadata-Version: 2.1
 Name: sib-commit-parser
-Version: 0.3.4
+Version: 1.0.0
 Summary: Commit parser for StartinBlox packages
-Home-page: UNKNOWN
 License: MIT
-Description: # StartinBlox commit message parser
-        
-        This pakage implements the releasing policy of SIB project based on commit messages.
-        
-        [See reference](https://git.happy-dev.fr/startinblox/management#commit-messages)
-        
-        ## Setup
-        
-        Add the relevant `semantic_release` section to your `setup.cfg`:
-        ```
-        [semantic_release]
-        version_source = tag
-        version_variable = myapp/__init__.py:__version__
-        commit_parser = commit_parse.parse
-        ```
-        
-        ## Develop the parser
-        
-        Install `python-semantic-release` along with the parser:
-        ```
-        # docker run --rm -v $PWD:/code -w /code -it python:3.6 bash
-        # pip install python-semantic-release
-        # pip install -e .[dev]
-        # export PYTHONPATH=/code/commit_parser/
-        ```
-        
-        Create a dummy project:
-        ```
-        # git init /tmp/test
-        # cd !$
-        ```
-        
-        Add a minimal project:
-        ```
-        # echo 'setup()' > setup.py
-        # echo '__version__ = 0.0.0' > version.py
-        # cat <<EOF > setup.cfg
-        [semantic_release]
-        upload_to_pypi = false
-        version_source = tag
-        version_variable = version.py:__version__
-        commit_parser = commit_parser.parse
-        EOF
-        ```
-        
-        Simulate release:
-        ```
-        # git commit --allow-empty -m 'fix: some stupid message'
-        # semantic-release version --noop
-        Creating new version.
-        Current version: 0.0.0
-        No operation mode. Should have bumped from 0.0.0 to 0.0.1.
-        ```
-        
-        Use `# DEBUG=semantic_release:* semantic-release version --noop` to see debug messages.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Description-Content-Type: text/markdown
+
+# StartinBlox commit message parser
+
+This pakage implements the releasing policy of SIB project based on commit messages.
+
+[See reference](https://git.happy-dev.fr/startinblox/management#commit-messages)
+
+## Setup
+
+Add the relevant `semantic_release` section to your `setup.cfg`:
+```
+[semantic_release]
+version_source = tag
+version_variable = myapp/__init__.py:__version__
+commit_parser = commit_parse.parse
+```
+
+## Develop the parser
+
+Install `python-semantic-release` along with the parser:
+```
+# docker run --rm -v $PWD:/code -w /code -it python:3.6 bash
+# pip install python-semantic-release
+# pip install -e .[dev]
+# export PYTHONPATH=/code/commit_parser/
+```
+
+Create a dummy project:
+```
+# git init /tmp/test
+# cd !$
+```
+
+Add a minimal project:
+```
+# echo 'setup()' > setup.py
+# echo '__version__ = 0.0.0' > version.py
+# cat <<EOF > setup.cfg
+[semantic_release]
+upload_to_pypi = false
+version_source = tag
+version_variable = version.py:__version__
+commit_parser = commit_parser.parse
+EOF
+```
+
+Simulate release:
+```
+# git commit --allow-empty -m 'fix: some stupid message'
+# semantic-release version --noop
+Creating new version.
+Current version: 0.0.0
+No operation mode. Should have bumped from 0.0.0 to 0.0.1.
+```
+
+Use `# DEBUG=semantic_release:* semantic-release version --noop` to see debug messages.
```

### Comparing `sib-commit-parser-0.3.4/commit_parser/parser.py` & `sib-commit-parser-1.0.0/commit_parser/parser.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,32 @@
 """StartinBlox commit style parser"""
 
 import re
 import ndebug
 from typing import Tuple
 from semantic_release.errors import UnknownCommitMessageStyleError
-from semantic_release.history.parser_helpers import ParsedCommit, parse_text_block
+from semantic_release.history.parser_helpers import ParsedCommit
+
+def parse_text_block(text: str) -> Tuple[str, str]:
+    """
+    This will take a text block and return a tuple with body and footer,
+    where footer is defined as the last paragraph.
+
+    :param text: The text string to be divided.
+    :return: A tuple with body and footer,
+    where footer is defined as the last paragraph.
+    """
+    body, footer = '', ''
+    if text:
+        body = text.split('\n\n')[0]
+        if len(text.split('\n\n')) == 2:
+            footer = text.split('\n\n')[1]
+
+    return body.replace('\n', ' '), footer.replace('\n', ' ')
+
 
 debug = ndebug.create(__name__)
 
 re_parser = re.compile(
     r'(?P<type>\w+)'
     r'(?:\((?P<scope>[\w _\-]+)\))?: '
     r'(?P<subject>[^\n]+)'
@@ -70,16 +88,18 @@
             body = ''
             footer = ''
 
     if debug.enabled:
         debug('parse_commit_message -> ({}, {}, {})'.format(
             level_bump,
             _type,
-            (subject, body, footer)
+            (subject, body, footer),
+            ''
         ))
 
     return ParsedCommit(
         level_bump,
         _type,
         '',
-        (subject, body, footer)
-    )
+        (subject, body, footer),
+        ''
+    )
```

### Comparing `sib-commit-parser-0.3.4/setup.cfg` & `sib-commit-parser-1.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `sib-commit-parser-0.3.4/README.md` & `sib-commit-parser-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `sib-commit-parser-0.3.4/PKG-INFO` & `sib-commit-parser-1.0.0/sib_commit_parser.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,66 +1,64 @@
 Metadata-Version: 2.1
 Name: sib-commit-parser
-Version: 0.3.4
+Version: 1.0.0
 Summary: Commit parser for StartinBlox packages
-Home-page: UNKNOWN
 License: MIT
-Description: # StartinBlox commit message parser
-        
-        This pakage implements the releasing policy of SIB project based on commit messages.
-        
-        [See reference](https://git.happy-dev.fr/startinblox/management#commit-messages)
-        
-        ## Setup
-        
-        Add the relevant `semantic_release` section to your `setup.cfg`:
-        ```
-        [semantic_release]
-        version_source = tag
-        version_variable = myapp/__init__.py:__version__
-        commit_parser = commit_parse.parse
-        ```
-        
-        ## Develop the parser
-        
-        Install `python-semantic-release` along with the parser:
-        ```
-        # docker run --rm -v $PWD:/code -w /code -it python:3.6 bash
-        # pip install python-semantic-release
-        # pip install -e .[dev]
-        # export PYTHONPATH=/code/commit_parser/
-        ```
-        
-        Create a dummy project:
-        ```
-        # git init /tmp/test
-        # cd !$
-        ```
-        
-        Add a minimal project:
-        ```
-        # echo 'setup()' > setup.py
-        # echo '__version__ = 0.0.0' > version.py
-        # cat <<EOF > setup.cfg
-        [semantic_release]
-        upload_to_pypi = false
-        version_source = tag
-        version_variable = version.py:__version__
-        commit_parser = commit_parser.parse
-        EOF
-        ```
-        
-        Simulate release:
-        ```
-        # git commit --allow-empty -m 'fix: some stupid message'
-        # semantic-release version --noop
-        Creating new version.
-        Current version: 0.0.0
-        No operation mode. Should have bumped from 0.0.0 to 0.0.1.
-        ```
-        
-        Use `# DEBUG=semantic_release:* semantic-release version --noop` to see debug messages.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Description-Content-Type: text/markdown
+
+# StartinBlox commit message parser
+
+This pakage implements the releasing policy of SIB project based on commit messages.
+
+[See reference](https://git.happy-dev.fr/startinblox/management#commit-messages)
+
+## Setup
+
+Add the relevant `semantic_release` section to your `setup.cfg`:
+```
+[semantic_release]
+version_source = tag
+version_variable = myapp/__init__.py:__version__
+commit_parser = commit_parse.parse
+```
+
+## Develop the parser
+
+Install `python-semantic-release` along with the parser:
+```
+# docker run --rm -v $PWD:/code -w /code -it python:3.6 bash
+# pip install python-semantic-release
+# pip install -e .[dev]
+# export PYTHONPATH=/code/commit_parser/
+```
+
+Create a dummy project:
+```
+# git init /tmp/test
+# cd !$
+```
+
+Add a minimal project:
+```
+# echo 'setup()' > setup.py
+# echo '__version__ = 0.0.0' > version.py
+# cat <<EOF > setup.cfg
+[semantic_release]
+upload_to_pypi = false
+version_source = tag
+version_variable = version.py:__version__
+commit_parser = commit_parser.parse
+EOF
+```
+
+Simulate release:
+```
+# git commit --allow-empty -m 'fix: some stupid message'
+# semantic-release version --noop
+Creating new version.
+Current version: 0.0.0
+No operation mode. Should have bumped from 0.0.0 to 0.0.1.
+```
+
+Use `# DEBUG=semantic_release:* semantic-release version --noop` to see debug messages.
```

