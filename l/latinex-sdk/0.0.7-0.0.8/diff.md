# Comparing `tmp/latinex_sdk-0.0.7.tar.gz` & `tmp/latinex-sdk-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latinex_sdk-0.0.7.tar", last modified: Tue Jun  6 06:11:32 2023, max compression
+gzip compressed data, was "latinex-sdk-0.0.8.tar", last modified: Mon Jul 24 06:53:21 2023, max compression
```

## Comparing `latinex_sdk-0.0.7.tar` & `latinex-sdk-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 06:11:32.397264 latinex_sdk-0.0.7/
--rw-rw-rw-   0        0        0     1365 2023-06-06 06:11:32.396248 latinex_sdk-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      696 2023-06-04 19:13:24.000000 latinex_sdk-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 06:11:32.378246 latinex_sdk-0.0.7/latinex_sdk/
--rw-rw-rw-   0        0        0        0 2023-06-04 18:53:05.000000 latinex_sdk-0.0.7/latinex_sdk/__init__.py
--rw-rw-rw-   0        0        0     2888 2023-06-06 06:08:01.000000 latinex_sdk-0.0.7/latinex_sdk/generic_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-06 06:11:32.394249 latinex_sdk-0.0.7/latinex_sdk.egg-info/
--rw-rw-rw-   0        0        0     1365 2023-06-06 06:11:32.000000 latinex_sdk-0.0.7/latinex_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-06-06 06:11:32.000000 latinex_sdk-0.0.7/latinex_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 06:11:32.000000 latinex_sdk-0.0.7/latinex_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-06-06 06:11:32.000000 latinex_sdk-0.0.7/latinex_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-06 06:11:32.000000 latinex_sdk-0.0.7/latinex_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 06:11:32.397264 latinex_sdk-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1328 2023-06-06 06:10:48.000000 latinex_sdk-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:53:21.613918 latinex-sdk-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-24 06:53:12.000000 latinex-sdk-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-24 06:53:21.613918 latinex-sdk-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-24 06:53:12.000000 latinex-sdk-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:53:21.613918 latinex-sdk-0.0.8/latinex-sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-24 06:53:12.000000 latinex-sdk-0.0.8/latinex-sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-07-24 06:53:12.000000 latinex-sdk-0.0.8/latinex-sdk/generic_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:53:21.613918 latinex-sdk-0.0.8/latinex_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-24 06:53:21.000000 latinex-sdk-0.0.8/latinex_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-24 06:53:21.000000 latinex-sdk-0.0.8/latinex_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 06:53:21.000000 latinex-sdk-0.0.8/latinex_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 06:53:21.000000 latinex-sdk-0.0.8/latinex_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-24 06:53:21.000000 latinex-sdk-0.0.8/latinex_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 06:53:21.617918 latinex-sdk-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-24 06:53:12.000000 latinex-sdk-0.0.8/setup.py
```

### Comparing `latinex_sdk-0.0.7/PKG-INFO` & `latinex-sdk-0.0.8/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,52 @@
-Metadata-Version: 2.1
-Name: latinex_sdk
-Version: 0.0.7
-Summary: Software Development Kit for Latinex (https://www.latinexbolsa.com)
-Author: Blasser Analytica (Rodolfo Blasser)
-Author-email: <rodolfoblasser@gmail.com>
-Keywords: python,panama,finance,stocks,fixed income,data,api,market data,latinex
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-
-
-# latinex_sdk
-Python SDK for basic interactions with the Latinex API
-
-# Developed by Rodolfo Blasser 
-https://www.linkedin.com/in/rodblasser/
-
-## Usage
-This is a prototype SDK and it's not being currently maintained.
-
-## Example
-```python
-from latinex_sdk.generic_utils import Utilities as utils
-
-# Test Connectivity
-test = utils.whois()
-print(test)
-
-# Welcome
-greetings = utils.welcome()
-print(greetings)
-
-# Register (get an API Key)
-email = "example1@mail.com"
-get_key = utils.register(email)
-print(get_key)
-
-# Params
-fecha_inicio = "2023-05-28"
-fecha_fin = "2023-06-28"
-tipo_emision = "BONOS"
-key = get_key[1]
-
-# Query
-data = utils.get_historic(key, fecha_inicio, fecha_fin, tipo_emision)
-```
+Metadata-Version: 2.1
+Name: latinex-sdk
+Version: 0.0.8
+Summary: Software Development Kit for Latinex (https://www.latinexbolsa.com)
+Author: Blasser Analytica (Rodolfo Blasser)
+Author-email: <rodolfoblasser@gmail.com>
+Keywords: python,panama,finance,stocks,fixed income,data,api,market data,latinex
+Classifier: Development Status :: 1 - Planning
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# latinex_sdk
+Python SDK for basic interactions with the Latinex API
+
+# Developed by Rodolfo Blasser 
+https://www.linkedin.com/in/rodblasser/
+
+## Usage
+This is a prototype SDK and it's not being currently maintained.
+
+## Example
+```python
+from latinex_sdk.generic_utils import Utilities as utils
+
+# Test Connectivity
+test = utils.whois()
+print(test)
+
+# Welcome
+greetings = utils.welcome()
+print(greetings)
+
+# Register (get an API Key)
+email = "example1@mail.com"
+get_key = utils.register(email)
+print(get_key)
+
+# Params
+fecha_inicio = "2023-05-28"
+fecha_fin = "2023-06-28"
+tipo_emision = "BONOS"
+key = get_key[1]
+
+# Query
+data = utils.get_historic(key, fecha_inicio, fecha_fin, tipo_emision)
+```
```

### Comparing `latinex_sdk-0.0.7/README.md` & `latinex-sdk-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `latinex_sdk-0.0.7/latinex_sdk.egg-info/PKG-INFO` & `latinex-sdk-0.0.8/latinex_sdk.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,52 @@
-Metadata-Version: 2.1
-Name: latinex-sdk
-Version: 0.0.7
-Summary: Software Development Kit for Latinex (https://www.latinexbolsa.com)
-Author: Blasser Analytica (Rodolfo Blasser)
-Author-email: <rodolfoblasser@gmail.com>
-Keywords: python,panama,finance,stocks,fixed income,data,api,market data,latinex
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-
-
-# latinex_sdk
-Python SDK for basic interactions with the Latinex API
-
-# Developed by Rodolfo Blasser 
-https://www.linkedin.com/in/rodblasser/
-
-## Usage
-This is a prototype SDK and it's not being currently maintained.
-
-## Example
-```python
-from latinex_sdk.generic_utils import Utilities as utils
-
-# Test Connectivity
-test = utils.whois()
-print(test)
-
-# Welcome
-greetings = utils.welcome()
-print(greetings)
-
-# Register (get an API Key)
-email = "example1@mail.com"
-get_key = utils.register(email)
-print(get_key)
-
-# Params
-fecha_inicio = "2023-05-28"
-fecha_fin = "2023-06-28"
-tipo_emision = "BONOS"
-key = get_key[1]
-
-# Query
-data = utils.get_historic(key, fecha_inicio, fecha_fin, tipo_emision)
-```
+Metadata-Version: 2.1
+Name: latinex-sdk
+Version: 0.0.8
+Summary: Software Development Kit for Latinex (https://www.latinexbolsa.com)
+Author: Blasser Analytica (Rodolfo Blasser)
+Author-email: <rodolfoblasser@gmail.com>
+Keywords: python,panama,finance,stocks,fixed income,data,api,market data,latinex
+Classifier: Development Status :: 1 - Planning
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# latinex_sdk
+Python SDK for basic interactions with the Latinex API
+
+# Developed by Rodolfo Blasser 
+https://www.linkedin.com/in/rodblasser/
+
+## Usage
+This is a prototype SDK and it's not being currently maintained.
+
+## Example
+```python
+from latinex_sdk.generic_utils import Utilities as utils
+
+# Test Connectivity
+test = utils.whois()
+print(test)
+
+# Welcome
+greetings = utils.welcome()
+print(greetings)
+
+# Register (get an API Key)
+email = "example1@mail.com"
+get_key = utils.register(email)
+print(get_key)
+
+# Params
+fecha_inicio = "2023-05-28"
+fecha_fin = "2023-06-28"
+tipo_emision = "BONOS"
+key = get_key[1]
+
+# Query
+data = utils.get_historic(key, fecha_inicio, fecha_fin, tipo_emision)
+```
```

### Comparing `latinex_sdk-0.0.7/setup.py` & `latinex-sdk-0.0.8/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,32 +3,32 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 DESCRIPTION = 'Software Development Kit for Latinex (https://www.latinexbolsa.com)'
 LONG_DESCRIPTION = 'This SKD facilitates the use of the Latinex REST API, it allows the user to register (getting an API Key) and to fetch data in a friction-less manner'
 
 # Setting up
 setup(
-    name="latinex_sdk",
+    name="latinex-sdk",
     version=VERSION,
     author="Blasser Analytica (Rodolfo Blasser)",
     author_email="<rodolfoblasser@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=['requests', 'pandas', 'urllib3', 'pytz'],
+    install_requires=['requests', 'pandas', 'urllib3'],
     keywords=['python', 'panama', 'finance', 'stocks', 'fixed income', 'data', 'api', 'market data', 'latinex'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
-)
+)
```

