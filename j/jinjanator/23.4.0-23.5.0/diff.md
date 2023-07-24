# Comparing `tmp/jinjanator-23.4.0.tar.gz` & `tmp/jinjanator-23.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Mon Jul 24 18:25:45 2023, max compression
+gzip compressed data, last modified: Mon Jul 24 20:08:03 2023, max compression
```

## Comparing `jinjanator-23.4.0.tar` & `jinjanator-23.5.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1830 2023-07-24 18:25:45.000000 jinjanator-23.4.0/CHANGELOG.md
--rw-r--r--   0        0        0     8986 2023-07-24 18:25:45.000000 jinjanator-23.4.0/README.md
--rw-r--r--   0        0        0       81 2023-07-24 18:25:45.000000 jinjanator-23.4.0/src/jinjanator/__init__.py
--rw-r--r--   0        0        0     9612 2023-07-24 18:25:45.000000 jinjanator-23.4.0/src/jinjanator/cli.py
--rw-r--r--   0        0        0      727 2023-07-24 18:25:45.000000 jinjanator-23.4.0/src/jinjanator/context.py
--rw-r--r--   0        0        0     1186 2023-07-24 18:25:45.000000 jinjanator-23.4.0/src/jinjanator/filters.py
--rw-r--r--   0        0        0     3520 2023-07-24 18:25:45.000000 jinjanator-23.4.0/src/jinjanator/formats.py
--rw-r--r--   0        0        0        0 2023-07-24 18:25:45.000000 jinjanator-23.4.0/src/jinjanator/py.typed
--rw-r--r--   0        0        0      162 2023-07-24 18:25:45.000000 jinjanator-23.4.0/src/jinjanator/version.py
--rw-r--r--   0        0        0     1614 2023-07-24 18:25:45.000000 jinjanator-23.4.0/tests/__init__.py
--rw-r--r--   0        0        0      675 2023-07-24 18:25:45.000000 jinjanator-23.4.0/tests/conftest.py
--rw-r--r--   0        0        0     1582 2023-07-24 18:25:45.000000 jinjanator-23.4.0/tests/test_argparse.py
--rw-r--r--   0        0        0     1274 2023-07-24 18:25:45.000000 jinjanator-23.4.0/tests/test_cli.py
--rw-r--r--   0        0        0     2723 2023-07-24 18:25:45.000000 jinjanator-23.4.0/tests/test_env.py
--rw-r--r--   0        0        0      248 2023-07-24 18:25:45.000000 jinjanator-23.4.0/tests/test_extension.py
--rw-r--r--   0        0        0      840 2023-07-24 18:25:45.000000 jinjanator-23.4.0/tests/test_invalid_data.py
--rw-r--r--   0        0        0     3461 2023-07-24 18:25:45.000000 jinjanator-23.4.0/tests/test_nginx_config.py
--rw-r--r--   0        0        0      780 2023-07-24 18:25:45.000000 jinjanator-23.4.0/tests/test_output_file.py
--rw-r--r--   0        0        0      435 2023-07-24 18:25:45.000000 jinjanator-23.4.0/tests/test_template_not_found.py
--rw-r--r--   0        0        0      501 2023-07-24 18:25:45.000000 jinjanator-23.4.0/tests/test_undefined.py
--rw-r--r--   0        0        0      728 2023-07-24 18:25:45.000000 jinjanator-23.4.0/tests/test_unicode.py
--rw-r--r--   0        0        0       58 2023-07-24 18:25:45.000000 jinjanator-23.4.0/.gitignore
--rw-r--r--   0        0        0    35149 2023-07-24 18:25:45.000000 jinjanator-23.4.0/LICENSE.apache-2.0
--rw-r--r--   0        0        0     1321 2023-07-24 18:25:45.000000 jinjanator-23.4.0/LICENSE.bsd-2-clause
--rw-r--r--   0        0        0     6482 2023-07-24 18:25:45.000000 jinjanator-23.4.0/pyproject.toml
--rw-r--r--   0        0        0     7681 2023-07-24 18:25:45.000000 jinjanator-23.4.0/PKG-INFO
+-rw-r--r--   0        0        0     2056 2023-07-24 20:08:03.000000 jinjanator-23.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0     9172 2023-07-24 20:08:03.000000 jinjanator-23.5.0/README.md
+-rw-r--r--   0        0        0       81 2023-07-24 20:08:03.000000 jinjanator-23.5.0/src/jinjanator/__init__.py
+-rw-r--r--   0        0        0     9612 2023-07-24 20:08:03.000000 jinjanator-23.5.0/src/jinjanator/cli.py
+-rw-r--r--   0        0        0      727 2023-07-24 20:08:03.000000 jinjanator-23.5.0/src/jinjanator/context.py
+-rw-r--r--   0        0        0     1186 2023-07-24 20:08:03.000000 jinjanator-23.5.0/src/jinjanator/filters.py
+-rw-r--r--   0        0        0     3520 2023-07-24 20:08:03.000000 jinjanator-23.5.0/src/jinjanator/formats.py
+-rw-r--r--   0        0        0        0 2023-07-24 20:08:03.000000 jinjanator-23.5.0/src/jinjanator/py.typed
+-rw-r--r--   0        0        0      162 2023-07-24 20:08:03.000000 jinjanator-23.5.0/src/jinjanator/version.py
+-rw-r--r--   0        0        0     1614 2023-07-24 20:08:03.000000 jinjanator-23.5.0/tests/__init__.py
+-rw-r--r--   0        0        0      675 2023-07-24 20:08:03.000000 jinjanator-23.5.0/tests/conftest.py
+-rw-r--r--   0        0        0     1582 2023-07-24 20:08:03.000000 jinjanator-23.5.0/tests/test_argparse.py
+-rw-r--r--   0        0        0     1274 2023-07-24 20:08:03.000000 jinjanator-23.5.0/tests/test_cli.py
+-rw-r--r--   0        0        0     2723 2023-07-24 20:08:03.000000 jinjanator-23.5.0/tests/test_env.py
+-rw-r--r--   0        0        0      248 2023-07-24 20:08:03.000000 jinjanator-23.5.0/tests/test_extension.py
+-rw-r--r--   0        0        0      840 2023-07-24 20:08:03.000000 jinjanator-23.5.0/tests/test_invalid_data.py
+-rw-r--r--   0        0        0     3461 2023-07-24 20:08:03.000000 jinjanator-23.5.0/tests/test_nginx_config.py
+-rw-r--r--   0        0        0      780 2023-07-24 20:08:03.000000 jinjanator-23.5.0/tests/test_output_file.py
+-rw-r--r--   0        0        0      435 2023-07-24 20:08:03.000000 jinjanator-23.5.0/tests/test_template_not_found.py
+-rw-r--r--   0        0        0      501 2023-07-24 20:08:03.000000 jinjanator-23.5.0/tests/test_undefined.py
+-rw-r--r--   0        0        0      728 2023-07-24 20:08:03.000000 jinjanator-23.5.0/tests/test_unicode.py
+-rw-r--r--   0        0        0       58 2023-07-24 20:08:03.000000 jinjanator-23.5.0/.gitignore
+-rw-r--r--   0        0        0    11357 2023-07-24 20:08:03.000000 jinjanator-23.5.0/LICENSE.apache-2.0
+-rw-r--r--   0        0        0     1321 2023-07-24 20:08:03.000000 jinjanator-23.5.0/LICENSE.bsd-2-clause
+-rw-r--r--   0        0        0     6482 2023-07-24 20:08:03.000000 jinjanator-23.5.0/pyproject.toml
+-rw-r--r--   0        0        0     7811 2023-07-24 20:08:03.000000 jinjanator-23.5.0/PKG-INFO
```

### Comparing `jinjanator-23.4.0/CHANGELOG.md` & `jinjanator-23.5.0/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -24,14 +24,29 @@
 This changelog is managed by towncrier and is compiled at release time.
 
 See https://github.com/kpfleming/jinjanator/blob/main/.github/CONTRIBUTING.md#changelog for details.
 -->
 
 <!-- towncrier release notes start -->
 
+## [23.5.0](https://github.com/kpfleming/jinjanator/tree/23.5.0) - 2023-07-24
+
+### Additions
+
+- Added link to Ansible plugin.
+  
+
+
+### Fixes
+
+- Corrected content of LICENSE file.
+  
+- Corrected formatting of README on PyPI.
+
+
 ## [23.4.0](https://github.com/kpfleming/jinjanator/tree/23.4.0) - 2023-07-24
 
 ### Backwards-incompatible Changes
 
 - Moved plugin API to the jinjanator-plugins package.
   [#12](https://github.com/kpfleming/jinjanator/issues/12)
```

### Comparing `jinjanator-23.4.0/README.md` & `jinjanator-23.5.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,20 @@
 
 ## Installation
 
 ```
 pip install jinjanator
 ```
 
+## Available Plugins
+
+* [jinjanator-plugin-ansible](https://pypi.org/project/jinjanator-plugin-ansible) -
+  makes Ansible's 'core' filters and tests available during template
+  rendering
+
 ## Tutorial
 
 Suppose you have an NGINX configuration file template, `nginx.j2`:
 
 ```jinja2
 server {
   listen 80;
@@ -301,15 +307,15 @@
 ```jinja2
 User: {{ user_login }}
 Pass: {{ env("USER_PASSWORD") }}
 ```
 
 Notice that there must be quotes around the environment variable name
 when it is a literal string.
-"<!-- fancy-readme end -->"
+<!-- fancy-readme end -->
 
 ## Chat
 
 If you'd like to chat with the Jinjanator community, join us on
 [Matrix](https://matrix.to/#/#jinjanator:km6g.us)!
 
 ## Credits
```

#### html2text {}

```diff
@@ -16,48 +16,50 @@
 pallets/jinja/) templates. It is a fork of `j2cli`, which itself was a fork of
 `jinja2-cli`, both of which are no longer actively maintained. Open Source
 software: [Apache License 2.0](https://spdx.org/licenses/Apache-2.0.html) ##  
 Features: * Jinja2 templating * INI, YAML, JSON data sources supported *
 Environment variables can be used with or without data files * Plugins can
 provide additional formats, filters, tests, and global functions (see
 [jinjanator-plugins](https://github.com/kpfleming/jinjanator-plugins) for
-details) ## Installation ``` pip install jinjanator ``` ## Tutorial Suppose you
-have an NGINX configuration file template, `nginx.j2`: ```jinja2 server
-{ listen 80; server_name {{ nginx.hostname }}; root {{ nginx.webroot }}; index
-index.htm; } ``` And you have a JSON file with the data, `nginx.json`: ```json
-{ "nginx":{ "hostname": "localhost", "webroot": "/var/www/project" } } ``` This
-is how you render it into a working configuration file: ```bash $ jinjanate
-nginx.j2 nginx.json > nginx.conf ``` The output is saved to `nginx.conf`: ```
-server { listen 80; server_name localhost; root /var/www/project; index
-index.htm; } ``` Alternatively, you can use the `-o nginx.conf` or `--output-
-file nginx.conf`options to write directly to the file. ## Tutorial with
-environment variables Suppose, you have a very simple template,
-`person.xml.j2`: ```jinja2 {{ name }}{{ age }} ``` What is the easiest way to
-use jinjanator here? Use environment variables in your Bash script: ```bash $
-export name=Andrew $ export age=31 $ jinjanate /tmp/person.xml.j2 Andrew31 ```
-## Using environment variables Even when you use a data file as the data
-source, you can always access environment variables using the `env()` function:
-```jinja2 Username: {{ login }} Password: {{ env("APP_PASSWORD") }} ``` Or, if
-you prefer, as a filter: ```jinja2 Username: {{ login }} Password: {
-{ "APP_PASSWORD" | env }} ``` ## CLI Reference `jinjanate` accepts the
-following arguments: * `template`: Jinja2 template file to render * `data`:
-(optional) path to the data used for rendering. The default is `-`: use stdin.
-Options: * `--format FMT, -f FMT`: format for the data file. The default is
-`?`: guess from file extension. Supported formats are YAML (.yaml or .yml),
-JSON (.json), INI (.ini), and dotenv (.env), plus any formats provided by
-plugins you have installed. * `--format-option OPT`: option to be passed to the
-parser for the data format selected with `--format` (or auto-selected). This
-can be specified multiple times. Refer to the documentation for the format
-itself to learn whether it supports any options. * `--help, -h`: generates a
-help message describing usage of the tool. * `--import-env VAR, -e VAR`: import
-all environment variables into the template as `VAR`. To import environment
-variables into the global scope, give it an empty string: `--import-env=`.
-(This will overwrite any existing variables with the same names!) * `--output-
-file OUTFILE, -o OUTFILE`: Write rendered template to a file. * `--quiet`:
-Avoid generating any output on stderr. * `--undefined`: Allow undefined
+details) ## Installation ``` pip install jinjanator ``` ## Available Plugins *
+[jinjanator-plugin-ansible](https://pypi.org/project/jinjanator-plugin-ansible)
+- makes Ansible's 'core' filters and tests available during template rendering
+## Tutorial Suppose you have an NGINX configuration file template, `nginx.j2`:
+```jinja2 server { listen 80; server_name {{ nginx.hostname }}; root {
+{ nginx.webroot }}; index index.htm; } ``` And you have a JSON file with the
+data, `nginx.json`: ```json { "nginx":{ "hostname": "localhost", "webroot": "/
+var/www/project" } } ``` This is how you render it into a working configuration
+file: ```bash $ jinjanate nginx.j2 nginx.json > nginx.conf ``` The output is
+saved to `nginx.conf`: ``` server { listen 80; server_name localhost; root /
+var/www/project; index index.htm; } ``` Alternatively, you can use the `-
+o nginx.conf` or `--output-file nginx.conf`options to write directly to the
+file. ## Tutorial with environment variables Suppose, you have a very simple
+template, `person.xml.j2`: ```jinja2 {{ name }}{{ age }} ``` What is the
+easiest way to use jinjanator here? Use environment variables in your Bash
+script: ```bash $ export name=Andrew $ export age=31 $ jinjanate /tmp/
+person.xml.j2 Andrew31 ``` ## Using environment variables Even when you use a
+data file as the data source, you can always access environment variables using
+the `env()` function: ```jinja2 Username: {{ login }} Password: {{ env
+("APP_PASSWORD") }} ``` Or, if you prefer, as a filter: ```jinja2 Username: {
+{ login }} Password: {{ "APP_PASSWORD" | env }} ``` ## CLI Reference
+`jinjanate` accepts the following arguments: * `template`: Jinja2 template file
+to render * `data`: (optional) path to the data used for rendering. The default
+is `-`: use stdin. Options: * `--format FMT, -f FMT`: format for the data file.
+The default is `?`: guess from file extension. Supported formats are YAML
+(.yaml or .yml), JSON (.json), INI (.ini), and dotenv (.env), plus any formats
+provided by plugins you have installed. * `--format-option OPT`: option to be
+passed to the parser for the data format selected with `--format` (or auto-
+selected). This can be specified multiple times. Refer to the documentation for
+the format itself to learn whether it supports any options. * `--help, -h`:
+generates a help message describing usage of the tool. * `--import-env VAR, -
+e VAR`: import all environment variables into the template as `VAR`. To import
+environment variables into the global scope, give it an empty string: `--
+import-env=`. (This will overwrite any existing variables with the same names!)
+* `--output-file OUTFILE, -o OUTFILE`: Write rendered template to a file. * `--
+quiet`: Avoid generating any output on stderr. * `--undefined`: Allow undefined
 variables to be used in templates (no error will be raised). * `--version`:
 prints the version of the tool and the Jinja2 package installed. There is some
 special behavior with environment variables: * When `data` is not provided
 (data is `-`), `--format` defaults to `env` and thus reads environment
 variables. ## Usage Examples Render a template using INI-file data source: $
 jinjanate config.j2 data.ini Render using JSON data source: $ jinjanate
 config.j2 data.json Render using YAML data source: $ jinjanate config.j2
@@ -87,15 +89,15 @@
 `env(varname, default=None)` Use an environment variable's value in the
 template. This filter is available even when your data source is something
 other than the environment. Example: ```jinja2 User: {{ user_login }} Pass: {
 { "USER_PASSWORD" | env }} ``` You can provide a default value: ```jinja2 Pass:
 {{ "USER_PASSWORD" | env("-none-") }} ``` For your convenience, it's also
 available as a global function: ```jinja2 User: {{ user_login }} Pass: {{ env
 ("USER_PASSWORD") }} ``` Notice that there must be quotes around the
-environment variable name when it is a literal string. "" ## Chat If you'd like
+environment variable name when it is a literal string.  ## Chat If you'd like
 to chat with the Jinjanator community, join us on [Matrix](https://matrix.to/#/
 #jinjanator:km6g.us)! ## Credits This tool was created from [j2cli](https://
 github.com/kolypto/j2cli), which itself was created from [jinja2-cli](https://
 github.com/mattrobenolt/jinja2-cli). It was created to bring the project up to
 'modern' Python coding, packaging, and project-management standards, and to
 support plugins to provide extensibility. ["Standing on the shoulders of
 giants"](https://en.wikipedia.org/wiki/Standing_on_the_shoulders_of_giants)
```

### Comparing `jinjanator-23.4.0/src/jinjanator/cli.py` & `jinjanator-23.5.0/src/jinjanator/cli.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.4.0/src/jinjanator/context.py` & `jinjanator-23.5.0/src/jinjanator/context.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.4.0/src/jinjanator/filters.py` & `jinjanator-23.5.0/src/jinjanator/filters.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.4.0/src/jinjanator/formats.py` & `jinjanator-23.5.0/src/jinjanator/formats.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.4.0/tests/__init__.py` & `jinjanator-23.5.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.4.0/tests/conftest.py` & `jinjanator-23.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.4.0/tests/test_argparse.py` & `jinjanator-23.5.0/tests/test_argparse.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.4.0/tests/test_cli.py` & `jinjanator-23.5.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.4.0/tests/test_env.py` & `jinjanator-23.5.0/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.4.0/tests/test_invalid_data.py` & `jinjanator-23.5.0/tests/test_invalid_data.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.4.0/tests/test_nginx_config.py` & `jinjanator-23.5.0/tests/test_nginx_config.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.4.0/tests/test_output_file.py` & `jinjanator-23.5.0/tests/test_output_file.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.4.0/tests/test_unicode.py` & `jinjanator-23.5.0/tests/test_unicode.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.4.0/LICENSE.bsd-2-clause` & `jinjanator-23.5.0/LICENSE.bsd-2-clause`

 * *Files identical despite different names*

### Comparing `jinjanator-23.4.0/pyproject.toml` & `jinjanator-23.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jinjanator-23.4.0/PKG-INFO` & `jinjanator-23.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jinjanator
-Version: 23.4.0
+Version: 23.5.0
 Summary: Command-line interface to Jinja2 for templating in shell scripts.
 Project-URL: Bug Tracker, https://github.com/kpfleming/jinjanator/issues
 Project-URL: Homepage, https://github.com/kpfleming/jinjanator
 Author-email: "Kevin P. Fleming" <jinjanator@kevin.km6g.us>, Mark Vartanyan <kolypto@gmail.com>
 License: Apache-2.0
 License-File: LICENSE.apache-2.0
 License-File: LICENSE.bsd-2-clause
@@ -43,14 +43,20 @@
 
 ## Installation
 
 ```
 pip install jinjanator
 ```
 
+## Available Plugins
+
+* [jinjanator-plugin-ansible](https://pypi.org/project/jinjanator-plugin-ansible) -
+  makes Ansible's 'core' filters and tests available during template
+  rendering
+
 ## Tutorial
 
 Suppose you have an NGINX configuration file template, `nginx.j2`:
 
 ```jinja2
 server {
   listen 80;
@@ -312,16 +318,23 @@
 ```jinja2
 User: {{ user_login }}
 Pass: {{ env("USER_PASSWORD") }}
 ```
 
 Notice that there must be quotes around the environment variable name
 when it is a literal string.
-"## Release Information
-### Backwards-incompatible Changes
+## Release Information
+### Additions
+
+- Added link to Ansible plugin.
+  
+
+
+### Fixes
 
-- Moved plugin API to the jinjanator-plugins package.
-  [[#12](https://github.com/kpfleming/jinjanator/issues/12)](https://github.com/kpfleming/jinjanator/issues/12)
+- Corrected content of LICENSE file.
+  
+- Corrected formatting of README on PyPI.
 
 
 ---
 [→ Full Changelog](https://github.com/kpfleming/jinjanator/blob/main/CHANGELOG.md)
```

