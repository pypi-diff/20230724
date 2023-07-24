# Comparing `tmp/jinjanator-23.3.0.tar.gz` & `tmp/jinjanator-23.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sat Jul 22 21:49:54 2023, max compression
+gzip compressed data, last modified: Mon Jul 24 18:25:45 2023, max compression
```

## Comparing `jinjanator-23.3.0.tar` & `jinjanator-23.4.0.tar`

### file list

```diff
@@ -1,31 +1,26 @@
--rw-r--r--   0        0        0     1600 2023-07-22 21:49:54.000000 jinjanator-23.3.0/CHANGELOG.md
--rw-r--r--   0        0        0     5925 2023-07-22 21:49:54.000000 jinjanator-23.3.0/PLUGINS.md
--rw-r--r--   0        0        0     8755 2023-07-22 21:49:54.000000 jinjanator-23.3.0/README.md
--rw-r--r--   0        0        0     1120 2023-07-22 21:49:54.000000 jinjanator-23.3.0/plugin_example/jinjanator_plugin_example.py
--rw-r--r--   0        0        0      591 2023-07-22 21:49:54.000000 jinjanator-23.3.0/plugin_example/pyproject.toml
--rw-r--r--   0        0        0     1747 2023-07-22 21:49:54.000000 jinjanator-23.3.0/plugin_example/tests/test_plugin.py
--rw-r--r--   0        0        0       81 2023-07-22 21:49:54.000000 jinjanator-23.3.0/src/jinjanator/__init__.py
--rw-r--r--   0        0        0     9522 2023-07-22 21:49:54.000000 jinjanator-23.3.0/src/jinjanator/cli.py
--rw-r--r--   0        0        0      716 2023-07-22 21:49:54.000000 jinjanator-23.3.0/src/jinjanator/context.py
--rw-r--r--   0        0        0     1154 2023-07-22 21:49:54.000000 jinjanator-23.3.0/src/jinjanator/filters.py
--rw-r--r--   0        0        0     3509 2023-07-22 21:49:54.000000 jinjanator-23.3.0/src/jinjanator/formats.py
--rw-r--r--   0        0        0     2456 2023-07-22 21:49:54.000000 jinjanator-23.3.0/src/jinjanator/plugin.py
--rw-r--r--   0        0        0        0 2023-07-22 21:49:54.000000 jinjanator-23.3.0/src/jinjanator/py.typed
--rw-r--r--   0        0        0      162 2023-07-22 21:49:54.000000 jinjanator-23.3.0/src/jinjanator/version.py
--rw-r--r--   0        0        0     1614 2023-07-22 21:49:54.000000 jinjanator-23.3.0/tests/__init__.py
--rw-r--r--   0        0        0      675 2023-07-22 21:49:54.000000 jinjanator-23.3.0/tests/conftest.py
--rw-r--r--   0        0        0     1580 2023-07-22 21:49:54.000000 jinjanator-23.3.0/tests/test_argparse.py
--rw-r--r--   0        0        0     1284 2023-07-22 21:49:54.000000 jinjanator-23.3.0/tests/test_cli.py
--rw-r--r--   0        0        0     2723 2023-07-22 21:49:54.000000 jinjanator-23.3.0/tests/test_env.py
--rw-r--r--   0        0        0      248 2023-07-22 21:49:54.000000 jinjanator-23.3.0/tests/test_extension.py
--rw-r--r--   0        0        0      840 2023-07-22 21:49:54.000000 jinjanator-23.3.0/tests/test_invalid_data.py
--rw-r--r--   0        0        0     3749 2023-07-22 21:49:54.000000 jinjanator-23.3.0/tests/test_nginx_config.py
--rw-r--r--   0        0        0      780 2023-07-22 21:49:54.000000 jinjanator-23.3.0/tests/test_output_file.py
--rw-r--r--   0        0        0      435 2023-07-22 21:49:54.000000 jinjanator-23.3.0/tests/test_template_not_found.py
--rw-r--r--   0        0        0      501 2023-07-22 21:49:54.000000 jinjanator-23.3.0/tests/test_undefined.py
--rw-r--r--   0        0        0      731 2023-07-22 21:49:54.000000 jinjanator-23.3.0/tests/test_unicode.py
--rw-r--r--   0        0        0       58 2023-07-22 21:49:54.000000 jinjanator-23.3.0/.gitignore
--rw-r--r--   0        0        0    35149 2023-07-22 21:49:54.000000 jinjanator-23.3.0/LICENSE.apache-2.0
--rw-r--r--   0        0        0     1321 2023-07-22 21:49:54.000000 jinjanator-23.3.0/LICENSE.bsd-2-clause
--rw-r--r--   0        0        0     6908 2023-07-22 21:49:54.000000 jinjanator-23.3.0/pyproject.toml
--rw-r--r--   0        0        0     7820 2023-07-22 21:49:54.000000 jinjanator-23.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1830 2023-07-24 18:25:45.000000 jinjanator-23.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0     8986 2023-07-24 18:25:45.000000 jinjanator-23.4.0/README.md
+-rw-r--r--   0        0        0       81 2023-07-24 18:25:45.000000 jinjanator-23.4.0/src/jinjanator/__init__.py
+-rw-r--r--   0        0        0     9612 2023-07-24 18:25:45.000000 jinjanator-23.4.0/src/jinjanator/cli.py
+-rw-r--r--   0        0        0      727 2023-07-24 18:25:45.000000 jinjanator-23.4.0/src/jinjanator/context.py
+-rw-r--r--   0        0        0     1186 2023-07-24 18:25:45.000000 jinjanator-23.4.0/src/jinjanator/filters.py
+-rw-r--r--   0        0        0     3520 2023-07-24 18:25:45.000000 jinjanator-23.4.0/src/jinjanator/formats.py
+-rw-r--r--   0        0        0        0 2023-07-24 18:25:45.000000 jinjanator-23.4.0/src/jinjanator/py.typed
+-rw-r--r--   0        0        0      162 2023-07-24 18:25:45.000000 jinjanator-23.4.0/src/jinjanator/version.py
+-rw-r--r--   0        0        0     1614 2023-07-24 18:25:45.000000 jinjanator-23.4.0/tests/__init__.py
+-rw-r--r--   0        0        0      675 2023-07-24 18:25:45.000000 jinjanator-23.4.0/tests/conftest.py
+-rw-r--r--   0        0        0     1582 2023-07-24 18:25:45.000000 jinjanator-23.4.0/tests/test_argparse.py
+-rw-r--r--   0        0        0     1274 2023-07-24 18:25:45.000000 jinjanator-23.4.0/tests/test_cli.py
+-rw-r--r--   0        0        0     2723 2023-07-24 18:25:45.000000 jinjanator-23.4.0/tests/test_env.py
+-rw-r--r--   0        0        0      248 2023-07-24 18:25:45.000000 jinjanator-23.4.0/tests/test_extension.py
+-rw-r--r--   0        0        0      840 2023-07-24 18:25:45.000000 jinjanator-23.4.0/tests/test_invalid_data.py
+-rw-r--r--   0        0        0     3461 2023-07-24 18:25:45.000000 jinjanator-23.4.0/tests/test_nginx_config.py
+-rw-r--r--   0        0        0      780 2023-07-24 18:25:45.000000 jinjanator-23.4.0/tests/test_output_file.py
+-rw-r--r--   0        0        0      435 2023-07-24 18:25:45.000000 jinjanator-23.4.0/tests/test_template_not_found.py
+-rw-r--r--   0        0        0      501 2023-07-24 18:25:45.000000 jinjanator-23.4.0/tests/test_undefined.py
+-rw-r--r--   0        0        0      728 2023-07-24 18:25:45.000000 jinjanator-23.4.0/tests/test_unicode.py
+-rw-r--r--   0        0        0       58 2023-07-24 18:25:45.000000 jinjanator-23.4.0/.gitignore
+-rw-r--r--   0        0        0    35149 2023-07-24 18:25:45.000000 jinjanator-23.4.0/LICENSE.apache-2.0
+-rw-r--r--   0        0        0     1321 2023-07-24 18:25:45.000000 jinjanator-23.4.0/LICENSE.bsd-2-clause
+-rw-r--r--   0        0        0     6482 2023-07-24 18:25:45.000000 jinjanator-23.4.0/pyproject.toml
+-rw-r--r--   0        0        0     7681 2023-07-24 18:25:45.000000 jinjanator-23.4.0/PKG-INFO
```

### Comparing `jinjanator-23.3.0/CHANGELOG.md` & `jinjanator-23.4.0/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -24,14 +24,22 @@
 This changelog is managed by towncrier and is compiled at release time.
 
 See https://github.com/kpfleming/jinjanator/blob/main/.github/CONTRIBUTING.md#changelog for details.
 -->
 
 <!-- towncrier release notes start -->
 
+## [23.4.0](https://github.com/kpfleming/jinjanator/tree/23.4.0) - 2023-07-24
+
+### Backwards-incompatible Changes
+
+- Moved plugin API to the jinjanator-plugins package.
+  [#12](https://github.com/kpfleming/jinjanator/issues/12)
+
+
 ## [23.3.0](https://github.com/kpfleming/jinjanator/tree/23.3.0) - 2023-07-22
 
 ### Fixes
 
 - Disabled Jinja2 'autoescape' feature since it can produce incorrect output.
   [#8](https://github.com/kpfleming/jinjanator/issues/8)
 - Add missing 'attrs' package to project dependencies.
```

### Comparing `jinjanator-23.3.0/README.md` & `jinjanator-23.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,31 +15,34 @@
 `j2cli`, which itself was a fork of `jinja2-cli`, both of which are no
 longer actively maintained.
 
 Open Source software: [Apache License 2.0](https://spdx.org/licenses/Apache-2.0.html)
 
 ## &nbsp;
 
+<!-- fancy-readme start -->
 Features:
 
 * Jinja2 templating
 * INI, YAML, JSON data sources supported
 * Environment variables can be used with or without data files
 * Plugins can provide additional formats, filters, tests, and global
-  functions (see [Plugins](PLUGINS.md) for details).
+  functions (see
+  [jinjanator-plugins](https://github.com/kpfleming/jinjanator-plugins)
+  for details)
 
 ## Installation
 
 ```
 pip install jinjanator
 ```
 
 ## Tutorial
 
-Suppose, you have an NGINX configuration file template, `nginx.j2`:
+Suppose you have an NGINX configuration file template, `nginx.j2`:
 
 ```jinja2
 server {
   listen 80;
   server_name {{ nginx.hostname }};
 
   root {{ nginx.webroot }};
@@ -298,14 +301,20 @@
 ```jinja2
 User: {{ user_login }}
 Pass: {{ env("USER_PASSWORD") }}
 ```
 
 Notice that there must be quotes around the environment variable name
 when it is a literal string.
+"<!-- fancy-readme end -->"
+
+## Chat
+
+If you'd like to chat with the Jinjanator community, join us on
+[Matrix](https://matrix.to/#/#jinjanator:km6g.us)!
 
 ## Credits
 
 This tool was created from [j2cli](https://github.com/kolypto/j2cli),
 which itself was created from
 [jinja2-cli](https://github.com/mattrobenolt/jinja2-cli). It was
 created to bring the project up to 'modern' Python coding, packaging,
```

#### html2text {}

```diff
@@ -14,49 +14,50 @@
 Testing-Pytest-orange.svg)](https://github.com/pytest-dev/pytest) This repo
 contains `jinjanator`, a CLI tool to render [Jinja2](https://github.com/
 pallets/jinja/) templates. It is a fork of `j2cli`, which itself was a fork of
 `jinja2-cli`, both of which are no longer actively maintained. Open Source
 software: [Apache License 2.0](https://spdx.org/licenses/Apache-2.0.html) ##  
 Features: * Jinja2 templating * INI, YAML, JSON data sources supported *
 Environment variables can be used with or without data files * Plugins can
-provide additional formats, filters, tests, and global functions (see [Plugins]
-(PLUGINS.md) for details). ## Installation ``` pip install jinjanator ``` ##
-Tutorial Suppose, you have an NGINX configuration file template, `nginx.j2`:
-```jinja2 server { listen 80; server_name {{ nginx.hostname }}; root {
-{ nginx.webroot }}; index index.htm; } ``` And you have a JSON file with the
-data, `nginx.json`: ```json { "nginx":{ "hostname": "localhost", "webroot": "/
-var/www/project" } } ``` This is how you render it into a working configuration
-file: ```bash $ jinjanate nginx.j2 nginx.json > nginx.conf ``` The output is
-saved to `nginx.conf`: ``` server { listen 80; server_name localhost; root /
-var/www/project; index index.htm; } ``` Alternatively, you can use the `-
-o nginx.conf` or `--output-file nginx.conf`options to write directly to the
-file. ## Tutorial with environment variables Suppose, you have a very simple
-template, `person.xml.j2`: ```jinja2 {{ name }}{{ age }} ``` What is the
-easiest way to use jinjanator here? Use environment variables in your Bash
-script: ```bash $ export name=Andrew $ export age=31 $ jinjanate /tmp/
-person.xml.j2 Andrew31 ``` ## Using environment variables Even when you use a
-data file as the data source, you can always access environment variables using
-the `env()` function: ```jinja2 Username: {{ login }} Password: {{ env
-("APP_PASSWORD") }} ``` Or, if you prefer, as a filter: ```jinja2 Username: {
-{ login }} Password: {{ "APP_PASSWORD" | env }} ``` ## CLI Reference
-`jinjanate` accepts the following arguments: * `template`: Jinja2 template file
-to render * `data`: (optional) path to the data used for rendering. The default
-is `-`: use stdin. Options: * `--format FMT, -f FMT`: format for the data file.
-The default is `?`: guess from file extension. Supported formats are YAML
-(.yaml or .yml), JSON (.json), INI (.ini), and dotenv (.env), plus any formats
-provided by plugins you have installed. * `--format-option OPT`: option to be
-passed to the parser for the data format selected with `--format` (or auto-
-selected). This can be specified multiple times. Refer to the documentation for
-the format itself to learn whether it supports any options. * `--help, -h`:
-generates a help message describing usage of the tool. * `--import-env VAR, -
-e VAR`: import all environment variables into the template as `VAR`. To import
-environment variables into the global scope, give it an empty string: `--
-import-env=`. (This will overwrite any existing variables with the same names!)
-* `--output-file OUTFILE, -o OUTFILE`: Write rendered template to a file. * `--
-quiet`: Avoid generating any output on stderr. * `--undefined`: Allow undefined
+provide additional formats, filters, tests, and global functions (see
+[jinjanator-plugins](https://github.com/kpfleming/jinjanator-plugins) for
+details) ## Installation ``` pip install jinjanator ``` ## Tutorial Suppose you
+have an NGINX configuration file template, `nginx.j2`: ```jinja2 server
+{ listen 80; server_name {{ nginx.hostname }}; root {{ nginx.webroot }}; index
+index.htm; } ``` And you have a JSON file with the data, `nginx.json`: ```json
+{ "nginx":{ "hostname": "localhost", "webroot": "/var/www/project" } } ``` This
+is how you render it into a working configuration file: ```bash $ jinjanate
+nginx.j2 nginx.json > nginx.conf ``` The output is saved to `nginx.conf`: ```
+server { listen 80; server_name localhost; root /var/www/project; index
+index.htm; } ``` Alternatively, you can use the `-o nginx.conf` or `--output-
+file nginx.conf`options to write directly to the file. ## Tutorial with
+environment variables Suppose, you have a very simple template,
+`person.xml.j2`: ```jinja2 {{ name }}{{ age }} ``` What is the easiest way to
+use jinjanator here? Use environment variables in your Bash script: ```bash $
+export name=Andrew $ export age=31 $ jinjanate /tmp/person.xml.j2 Andrew31 ```
+## Using environment variables Even when you use a data file as the data
+source, you can always access environment variables using the `env()` function:
+```jinja2 Username: {{ login }} Password: {{ env("APP_PASSWORD") }} ``` Or, if
+you prefer, as a filter: ```jinja2 Username: {{ login }} Password: {
+{ "APP_PASSWORD" | env }} ``` ## CLI Reference `jinjanate` accepts the
+following arguments: * `template`: Jinja2 template file to render * `data`:
+(optional) path to the data used for rendering. The default is `-`: use stdin.
+Options: * `--format FMT, -f FMT`: format for the data file. The default is
+`?`: guess from file extension. Supported formats are YAML (.yaml or .yml),
+JSON (.json), INI (.ini), and dotenv (.env), plus any formats provided by
+plugins you have installed. * `--format-option OPT`: option to be passed to the
+parser for the data format selected with `--format` (or auto-selected). This
+can be specified multiple times. Refer to the documentation for the format
+itself to learn whether it supports any options. * `--help, -h`: generates a
+help message describing usage of the tool. * `--import-env VAR, -e VAR`: import
+all environment variables into the template as `VAR`. To import environment
+variables into the global scope, give it an empty string: `--import-env=`.
+(This will overwrite any existing variables with the same names!) * `--output-
+file OUTFILE, -o OUTFILE`: Write rendered template to a file. * `--quiet`:
+Avoid generating any output on stderr. * `--undefined`: Allow undefined
 variables to be used in templates (no error will be raised). * `--version`:
 prints the version of the tool and the Jinja2 package installed. There is some
 special behavior with environment variables: * When `data` is not provided
 (data is `-`), `--format` defaults to `env` and thus reads environment
 variables. ## Usage Examples Render a template using INI-file data source: $
 jinjanate config.j2 data.ini Render using JSON data source: $ jinjanate
 config.j2 data.json Render using YAML data source: $ jinjanate config.j2
@@ -86,24 +87,26 @@
 `env(varname, default=None)` Use an environment variable's value in the
 template. This filter is available even when your data source is something
 other than the environment. Example: ```jinja2 User: {{ user_login }} Pass: {
 { "USER_PASSWORD" | env }} ``` You can provide a default value: ```jinja2 Pass:
 {{ "USER_PASSWORD" | env("-none-") }} ``` For your convenience, it's also
 available as a global function: ```jinja2 User: {{ user_login }} Pass: {{ env
 ("USER_PASSWORD") }} ``` Notice that there must be quotes around the
-environment variable name when it is a literal string. ## Credits This tool was
-created from [j2cli](https://github.com/kolypto/j2cli), which itself was
-created from [jinja2-cli](https://github.com/mattrobenolt/jinja2-cli). It was
-created to bring the project up to 'modern' Python coding, packaging, and
-project-management standards, and to support plugins to provide extensibility.
-["Standing on the shoulders of giants"](https://en.wikipedia.org/wiki/
-Standing_on_the_shoulders_of_giants) could not be more true than it is in the
-Python community; this project relies on many wonderful tools and libraries
-produced by the global open source software community, in addition to Python
-itself. I've listed many of them below, but if I've overlooked any please do
-not be offended :-) * [Attrs](https://github.com/python-attrs/attrs) * [Black]
-(https://github.com/psf/black) * [Hatch-Fancy-PyPI-Readme](https://github.com/
-hynek/hatch-fancy-pypi-readme) * [Hatch](https://github.com/pypa/hatch) *
-[Jinja2](https://github.com/pallets/jinja/) * [Mypy](https://github.com/python/
-mypy) * [Pluggy](https://github.com/pytest-dev/pluggy) * [Pytest](https://
-github.com/pytest-dev/pytest) * [Ruff](https://github.com/astral-sh/ruff) *
-[Towncrier](https://github.com/twisted/towncrier)
+environment variable name when it is a literal string. "" ## Chat If you'd like
+to chat with the Jinjanator community, join us on [Matrix](https://matrix.to/#/
+#jinjanator:km6g.us)! ## Credits This tool was created from [j2cli](https://
+github.com/kolypto/j2cli), which itself was created from [jinja2-cli](https://
+github.com/mattrobenolt/jinja2-cli). It was created to bring the project up to
+'modern' Python coding, packaging, and project-management standards, and to
+support plugins to provide extensibility. ["Standing on the shoulders of
+giants"](https://en.wikipedia.org/wiki/Standing_on_the_shoulders_of_giants)
+could not be more true than it is in the Python community; this project relies
+on many wonderful tools and libraries produced by the global open source
+software community, in addition to Python itself. I've listed many of them
+below, but if I've overlooked any please do not be offended :-) * [Attrs]
+(https://github.com/python-attrs/attrs) * [Black](https://github.com/psf/black)
+* [Hatch-Fancy-PyPI-Readme](https://github.com/hynek/hatch-fancy-pypi-readme) *
+[Hatch](https://github.com/pypa/hatch) * [Jinja2](https://github.com/pallets/
+jinja/) * [Mypy](https://github.com/python/mypy) * [Pluggy](https://github.com/
+pytest-dev/pluggy) * [Pytest](https://github.com/pytest-dev/pytest) * [Ruff]
+(https://github.com/astral-sh/ruff) * [Towncrier](https://github.com/twisted/
+towncrier)
```

### Comparing `jinjanator-23.3.0/src/jinjanator/cli.py` & `jinjanator-23.4.0/src/jinjanator/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,17 +11,18 @@
     Mapping,
     Sequence,
     TextIO,
     cast,
 )
 
 import jinja2
+import jinjanator_plugins
 import pluggy  # type: ignore[import]
 
-from . import filters, formats, plugin, version
+from . import filters, formats, version
 from .context import read_context_data
 
 
 class FilePathLoader(jinja2.BaseLoader):
     def __init__(self, cwd: Path, encoding: str = "utf-8"):
         self.cwd = cwd
         self.encoding = encoding
@@ -56,15 +57,15 @@
     )
 
     def __init__(
         self,
         cwd: Path,
         allow_undefined: bool,  # noqa: FBT001
         j2_env_params: dict[str, Any],
-        plugin_hook_callers: plugin.PluginHookCallers,
+        plugin_hook_callers: jinjanator_plugins.PluginHookCallers,
     ):
         j2_env_params.setdefault("keep_trailing_newline", True)
         j2_env_params.setdefault(
             "undefined",
             jinja2.Undefined if allow_undefined else jinja2.StrictUndefined,
         )
         j2_env_params.setdefault("extensions", self.ENABLED_EXTENSIONS)
@@ -102,15 +103,15 @@
         if self.already_seen and option_string:
             parser.error(option_string + " cannot be specified more than once.")
         setattr(namespace, self.dest, values)
         self.already_seen = True
 
 
 def parse_args(
-    formats: Mapping[str, plugin.Format],
+    formats: Mapping[str, jinjanator_plugins.Format],
     argv: Sequence[str] | None = None,
 ) -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         prog="j2",
         description="Command-line interface to Jinja2 for templating in shell scripts.",
         epilog="",
     )
@@ -185,32 +186,32 @@
         type=Path,
         help='Input data file name/path; "-" to use stdin',
     )
 
     return parser.parse_args(argv)
 
 
-def get_hook_callers() -> plugin.PluginHookCallers:
+def get_hook_callers() -> jinjanator_plugins.PluginHookCallers:
     pm = pluggy.PluginManager("jinjanator")
-    pm.add_hookspecs(plugin.PluginHooks)
+    pm.add_hookspecs(jinjanator_plugins.PluginHooks)
     pm.register(filters)
     pm.register(formats)
     pm.load_setuptools_entrypoints("jinjanator")
-    return cast(plugin.PluginHookCallers, pm.hook)
+    return cast(jinjanator_plugins.PluginHookCallers, pm.hook)
 
 
 def render_command(
     cwd: Path,
     environ: Mapping[str, str],
     stdin: TextIO | None,
     argv: Sequence[str],
 ) -> str:
     plugin_hook_callers = get_hook_callers()
 
-    available_formats: dict[str, plugin.Format] = {}
+    available_formats: dict[str, jinjanator_plugins.Format] = {}
 
     for plugin_formats in plugin_hook_callers.plugin_formats():
         available_formats.update(plugin_formats)
 
     args = parse_args(available_formats, argv[1:])
 
     if not args.quiet:
```

### Comparing `jinjanator-23.3.0/src/jinjanator/context.py` & `jinjanator-23.4.0/src/jinjanator/context.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Mapping, TextIO
 
 
 if TYPE_CHECKING:  # pragma: no cover
-    from .plugin import Format
+    from jinjanator_plugins import Format
 
 
 def read_context_data(
     fmt: Format,
     f: TextIO | None,
     environ: Mapping[str, str],
     import_env: str | None = None,
```

### Comparing `jinjanator-23.3.0/src/jinjanator/filters.py` & `jinjanator-23.4.0/src/jinjanator/filters.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 from __future__ import annotations
 
 import os
 
-from .plugin import Filters, Globals, plugin_filters_hook, plugin_globals_hook
+from jinjanator_plugins import (
+    Filters,
+    Globals,
+    plugin_filters_hook,
+    plugin_globals_hook,
+)
 
 
 def env(varname: str, default: str | None = None) -> str:
     """Use an environment variable's value inside your template.
 
     This filter is available even when your data source is something other that the environment.
```

### Comparing `jinjanator-23.3.0/src/jinjanator/formats.py` & `jinjanator-23.4.0/src/jinjanator/formats.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import configparser
 import json
 
 from typing import Any, Mapping
 
 import yaml
 
-from .plugin import Format, Formats, plugin_formats_hook
+from jinjanator_plugins import Format, Formats, plugin_formats_hook
 
 
 def _parse_ini(
     data_string: str,
     options: list[str] | None = None,  # noqa: ARG001
 ) -> Mapping[str, Any]:
     """INI data input format.
```

### Comparing `jinjanator-23.3.0/tests/__init__.py` & `jinjanator-23.4.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.3.0/tests/conftest.py` & `jinjanator-23.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.3.0/tests/test_argparse.py` & `jinjanator-23.4.0/tests/test_argparse.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 
 from typing import Any, Mapping
 
 import pytest
 
+from jinjanator_plugins import Format
+
 from jinjanator.cli import parse_args
-from jinjanator.plugin import Format
 
 
 def fake_env_parser(
     data: str, options: list[str] | None = None  # noqa: ARG001
 ) -> Mapping[str, Any]:
     return {"foo": "bar"}
 
@@ -42,15 +43,15 @@
     parse_args({"env": fake_env_format}, [*args, "template"])
 
 
 def test_version() -> None:
     """Ensure that '--version' argument is accepted and program exits without an error."""
     with pytest.raises(SystemExit) as excinfo:
         parse_args({}, ["--version"])
-    assert excinfo.value.code == 0
+    assert 0 == excinfo.value.code
 
 
 @pytest.mark.xfail()
 @pytest.mark.parametrize(
     "args",
     [
         ["--format", "env", "-f", "env"],
```

### Comparing `jinjanator-23.3.0/tests/test_cli.py` & `jinjanator-23.4.0/tests/test_cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 )
 
 
 def test_quiet(make_file_pair: FilePairFactory, capsys: Any) -> None:
     files = make_file_pair("Hello {{name}}!", "name=Blart", "env")
     render_file(files, ["--quiet"])
     captured = capsys.readouterr()
-    assert len(captured.err) == 0
+    assert 0 == len(captured.err)
 
 
 def test_unavailable_suffix(make_file_pair: FilePairFactory) -> None:
     files = make_file_pair("Hello {{name}}!", "name=Blart", "xyz")
     with pytest.raises(
         SystemExit,
         match="no format which can read '.xyz' files available",
@@ -31,16 +31,15 @@
 def test_main_normal(make_file_pair: FilePairFactory, capsys: Any) -> None:
     files = make_file_pair("Hello {{name}}!", "name=Blart", "env")
     assert (
         jinjanator.cli.main(["--quiet", str(files.template_file), str(files.data_file)])
         is None
     )
     captured = capsys.readouterr()
-    assert captured.out == "Hello Blart!"
+    assert "Hello Blart!" == captured.out
 
 
 def test_main_failure(make_file_pair: FilePairFactory) -> None:
     files = make_file_pair("Hello {{name}}!", "name=Blart", "xyz")
-    assert (
-        jinjanator.cli.main(["--quiet", str(files.template_file), str(files.data_file)])
-        == 1
+    assert 1 == jinjanator.cli.main(
+        ["--quiet", str(files.template_file), str(files.data_file)]
     )
```

### Comparing `jinjanator-23.3.0/tests/test_env.py` & `jinjanator-23.4.0/tests/test_env.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,82 +15,82 @@
     render_implicit_stream,
 )
 
 
 def test_import(make_file_pair: FilePairFactory) -> None:
     # Import environment into a variable
     files = make_file_pair("{{ a }}/{{ env.B }}", '{"a":1}', "json")
-    assert render_file_env(files, ["--import-env=env"], env={"B": "2"}) == "1/2"
+    assert "1/2" == render_file_env(files, ["--import-env=env"], env={"B": "2"})
 
     # Import environment into global scope
     files = make_file_pair("{{ a }}/{{ B }}", '{"a":1, "B": 1}', "json")
-    assert render_file_env(files, ["--import-env="], env={"B": "2"}) == "1/2"
+    assert "1/2" == render_file_env(files, ["--import-env="], env={"B": "2"})
 
 
 def test_equals_sign_in_file_value(make_file_pair: FilePairFactory) -> None:
     files = make_file_pair(
         "{{ A|default() }}/{{ B }}/{{ C }}",
         "A\nB=1\nC=val=1\n",
         "env",
     )
-    assert render_file(files, []) == "/1/val=1"
+    assert "/1/val=1" == render_file(files, [])
 
 
 def test_filter(make_file_pair: FilePairFactory, monkeypatch: Any) -> None:
     assert "USER_PASS" not in os.environ
 
     files = make_file_pair(
         '{{ user_login }}:{{ "USER_PASS"|env }}',
         "user_login: kolypto",
         "yaml",
     )
 
     # Value provided by environment
     monkeypatch.setenv("USER_PASS", "qwerty123")
-    assert render_file(files, []) == "kolypto:qwerty123"
+    assert "kolypto:qwerty123" == render_file(files, [])
 
     # Value not provided
     monkeypatch.delenv("USER_PASS")
     with pytest.raises(KeyError):
-        assert render_file(files, []) == "kolypto:qwerty123"
+        assert "kolypto:qwerty123" == render_file(files, [])
 
     # Default value
     files = make_file_pair(
         '{{ user_login }}:{{ "USER_PASS"|env("-none-") }}',
         "user_login: kolypto",
         "yaml",
     )
 
-    assert render_file(files, []) == "kolypto:-none-"
+    assert "kolypto:-none-" == render_file(files, [])
 
 
 def test_function(make_file_pair: FilePairFactory, monkeypatch: Any) -> None:
     assert "USER_PASS" not in os.environ
 
     files = make_file_pair(
         '{{ user_login }}:{{ env("USER_PASS") }}',
         "user_login: kolypto",
         "yaml",
     )
 
     # Value provided by environment
     monkeypatch.setenv("USER_PASS", "qwerty123")
-    assert render_file(files, []) == "kolypto:qwerty123"
+    assert "kolypto:qwerty123" == render_file(files, [])
 
     # Value not provided
     monkeypatch.delenv("USER_PASS")
     with pytest.raises(KeyError):
-        assert render_file(files, []) == "kolypto:qwerty123"
+        assert "kolypto:qwerty123" == render_file(files, [])
 
     # Default value
     files = make_file_pair(
         '{{ user_login }}:{{ env("USER_PASS", "-none-") }}',
         "user_login: kolypto",
         "yaml",
     )
-    assert render_file(files, []) == "kolypto:-none-"
+    assert "kolypto:-none-" == render_file(files, [])
 
 
 def test_env_stream(make_file_pair: FilePairFactory) -> None:
     files = make_file_pair("{{ a }}", "foo=bar", "env")
     with pytest.raises(UndefinedError, match="If you're trying to pipe a .env file"):
         render_implicit_stream(files, ["--format=env"])
```

### Comparing `jinjanator-23.3.0/tests/test_invalid_data.py` & `jinjanator-23.4.0/tests/test_invalid_data.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.3.0/tests/test_nginx_config.py` & `jinjanator-23.4.0/tests/test_nginx_config.py`

 * *Files 18% similar despite different names*

```diff
@@ -55,30 +55,24 @@
 hostname=localhost
 webroot=/var/www/project
 logs=/var/log/nginx
 """
 
     files = make_file_pair(DATA_TEMPLATE, ini_data, "ini")
 
-    assert render_file(files, []) == EXPECTED_OUTPUT
-    assert render_file(files, ["--format=ini"]) == EXPECTED_OUTPUT
+    assert EXPECTED_OUTPUT == render_file(files, [])
+    assert EXPECTED_OUTPUT == render_file(files, ["--format=ini"])
 
-    assert (
-        render_implicit_stream(
-            files,
-            ["--format=ini"],
-        )
-        == EXPECTED_OUTPUT
-    )
-    assert (
-        render_explicit_stream(
-            files,
-            ["--format=ini"],
-        )
-        == EXPECTED_OUTPUT
+    assert EXPECTED_OUTPUT == render_implicit_stream(
+        files,
+        ["--format=ini"],
+    )
+    assert EXPECTED_OUTPUT == render_explicit_stream(
+        files,
+        ["--format=ini"],
     )
 
 
 def test_json(make_file_pair: FilePairFactory) -> None:
     json_data = """
 {
     "nginx":{
@@ -87,94 +81,76 @@
         "logs": "/var/log/nginx"
     }
 }
 """
 
     files = make_file_pair(DATA_TEMPLATE, json_data, "json")
 
-    assert render_file(files, []) == EXPECTED_OUTPUT
-    assert render_file(files, ["--format=json"]) == EXPECTED_OUTPUT
+    assert EXPECTED_OUTPUT == render_file(files, [])
+    assert EXPECTED_OUTPUT == render_file(files, ["--format=json"])
 
-    assert (
-        render_implicit_stream(
-            files,
-            ["--format=json"],
-        )
-        == EXPECTED_OUTPUT
-    )
-    assert (
-        render_explicit_stream(
-            files,
-            ["--format=json"],
-        )
-        == EXPECTED_OUTPUT
+    assert EXPECTED_OUTPUT == render_implicit_stream(
+        files,
+        ["--format=json"],
+    )
+    assert EXPECTED_OUTPUT == render_explicit_stream(
+        files,
+        ["--format=json"],
     )
 
 
 def test_yaml(make_file_pair: FilePairFactory) -> None:
     yaml_data = """
 nginx:
   hostname: localhost
   webroot: /var/www/project
   logs: /var/log/nginx
 """
 
     files = make_file_pair(DATA_TEMPLATE, yaml_data, "yaml")
 
-    assert render_file(files, []) == EXPECTED_OUTPUT
-    assert render_file(files, ["--format=yaml"]) == EXPECTED_OUTPUT
+    assert EXPECTED_OUTPUT == render_file(files, [])
+    assert EXPECTED_OUTPUT == render_file(files, ["--format=yaml"])
 
-    assert (
-        render_implicit_stream(
-            files,
-            ["--format=yaml"],
-        )
-        == EXPECTED_OUTPUT
-    )
-    assert (
-        render_explicit_stream(
-            files,
-            ["--format=yaml"],
-        )
-        == EXPECTED_OUTPUT
+    assert EXPECTED_OUTPUT == render_implicit_stream(
+        files,
+        ["--format=yaml"],
+    )
+    assert EXPECTED_OUTPUT == render_explicit_stream(
+        files,
+        ["--format=yaml"],
     )
 
     files = make_file_pair(DATA_TEMPLATE, yaml_data, "yml")
 
-    assert render_file(files, []) == EXPECTED_OUTPUT
+    assert EXPECTED_OUTPUT == render_file(files, [])
 
 
 def test_env(make_file_pair: FilePairFactory) -> None:
     env_data = """
 NGINX_HOSTNAME=localhost
 NGINX_WEBROOT=/var/www/project
 NGINX_LOGS=/var/log/nginx
 """
 
     files = make_file_pair(ENV_TEMPLATE, env_data, "env")
 
-    assert render_file(files, []) == EXPECTED_OUTPUT
-    assert render_file(files, ["--format=env"]) == EXPECTED_OUTPUT
+    assert EXPECTED_OUTPUT == render_file(files, [])
+    assert EXPECTED_OUTPUT == render_file(files, ["--format=env"])
 
-    assert (
-        render_explicit_stream(
-            files,
-            [],
-        )
-        == EXPECTED_OUTPUT
-    )
-    assert (
-        render_explicit_stream(
-            files,
-            ["--format=env"],
-        )
-        == EXPECTED_OUTPUT
+    assert EXPECTED_OUTPUT == render_explicit_stream(
+        files,
+        [],
+    )
+    assert EXPECTED_OUTPUT == render_explicit_stream(
+        files,
+        ["--format=env"],
     )
 
     env = {
         "NGINX_HOSTNAME": "localhost",
         "NGINX_WEBROOT": "/var/www/project",
         "NGINX_LOGS": "/var/log/nginx",
     }
 
-    assert render_env(files, [], env) == EXPECTED_OUTPUT
-    assert render_env(files, ["--format=env"], env) == EXPECTED_OUTPUT
+    assert EXPECTED_OUTPUT == render_env(files, [], env)
+    assert EXPECTED_OUTPUT == render_env(files, ["--format=env"], env)
```

### Comparing `jinjanator-23.3.0/tests/test_output_file.py` & `jinjanator-23.4.0/tests/test_output_file.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 
 def test_short_option(
     make_file_pair: FilePairFactory,
     tmp_path: pathlib.Path,
 ) -> None:
     files = make_file_pair("{{ a }}", "", "json")
     out_file = tmp_path / "j2-out"
-    assert render_env(files, ["-o", str(out_file)], env={"a": "123"}) == ""
-    assert out_file.read_text() == "123"
+    assert "" == render_env(files, ["-o", str(out_file)], env={"a": "123"})
+    assert "123" == out_file.read_text()
 
 
 def test_long_option(
     make_file_pair: FilePairFactory,
     tmp_path: pathlib.Path,
 ) -> None:
     files = make_file_pair("{{ a }}", "", "json")
     out_file = tmp_path / "j2-out"
-    assert render_env(files, ["--output-file", str(out_file)], env={"a": "123"}) == ""
-    assert out_file.read_text() == "123"
+    assert "" == render_env(files, ["--output-file", str(out_file)], env={"a": "123"})
+    assert "123" == out_file.read_text()
```

### Comparing `jinjanator-23.3.0/tests/test_unicode.py` & `jinjanator-23.4.0/tests/test_unicode.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,14 @@
 def test_json(make_file_pair: FilePairFactory) -> None:
     # I'm using Russian language for unicode :)
     files = make_file_pair(
         "Проверка {{ a }} связи!",
         '{"a": "широкополосной"}',
         "json",
     )
-    assert render_file(files, []) == "Проверка широкополосной связи!"
+    assert "Проверка широкополосной связи!" == render_file(files, [])
 
 
 def test_env(make_file_pair: FilePairFactory) -> None:
     files = make_file_pair("Hello {{name}}!", "", "env")
-    # Test case from issue #17 (in original repo): unicode environment variables
-    assert render_env(files, [], env={"name": "Jürgen"}) == "Hello Jürgen!"
+    # Test case from issue #17 (in j2cli repo): unicode environment variables
+    assert "Hello Jürgen!" == render_env(files, [], env={"name": "Jürgen"})
```

### Comparing `jinjanator-23.3.0/LICENSE.apache-2.0` & `jinjanator-23.4.0/LICENSE.apache-2.0`

 * *Files identical despite different names*

### Comparing `jinjanator-23.3.0/LICENSE.bsd-2-clause` & `jinjanator-23.4.0/LICENSE.bsd-2-clause`

 * *Files identical despite different names*

### Comparing `jinjanator-23.3.0/pyproject.toml` & `jinjanator-23.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 dynamic = [
   "readme",
   "version",
 ]
 dependencies = [
   "attrs",
   "jinja2>=2.7.2",
-  "pluggy",
+  "jinjanator-plugins==23.1.*",
   "PyYAML",
   "typing-extensions",
 ]
 [project.urls]
 "Bug Tracker" = "https://github.com/kpfleming/jinjanator/issues"
 "Homepage" = "https://github.com/kpfleming/jinjanator"
 [project.scripts]
@@ -55,15 +55,15 @@
 [tool.hatch.envs.changelog.scripts]
 draft = [
   "rm -f changelog.d/*~",
   "towncrier build --version main --draft",
 ]
 release = [
   "rm -f changelog.d/*~",
-  "towncrier build --version {args}",
+  "towncrier build --yes --version {args}",
 ]
 
 [tool.hatch.version]
 source = "vcs"
 
 [tool.hatch.build.hooks.vcs]
 version-file = "src/jinjanator/version.py"
@@ -77,15 +77,14 @@
   ".github",
 ]
 
 [tool.hatch.build.targets.sdist]
 include = [
     "src",
     "tests",
-    "plugin_example",
     "*.md",
 ]
 
 [tool.hatch.build.targets.wheel]
 packages = [
     "src/jinjanator",
 ]
@@ -100,27 +99,25 @@
     "mypy",
     "pytest", # needed for type-checking tests
     "types-PyYAML",
 ]
 
 [tool.hatch.envs.lint.scripts]
 lint = [
-     "black --preview src tests plugin_example",
-     "ruff check --fix -- src tests plugin_example",
+     "black --preview src tests",
+     "ruff check --fix -- src tests",
      "mypy --package jinjanator",
      "mypy tests",
-     "mypy plugin_example/*.py",
      "shellcheck workflow-support/*.sh",
 ]
 lint-action = [
-     "black --check --diff --preview src tests plugin_example",
-     "ruff check --format=github -- src tests plugin_example",
+     "black --check --diff --preview src tests",
+     "ruff check --format=github -- src tests",
      "mypy --package jinjanator",
      "mypy tests",
-     "mypy plugin_example/*.py",
      "shellcheck workflow-support/*.sh",
 ]
 
 [tool.hatch.envs.ci]
 dependencies = [
     "coverage[toml]",
     "pytest",
@@ -136,35 +133,37 @@
 "3.10",
 "3.11",
 "3.12",
 ]
 
 [tool.hatch.envs.ci.scripts]
 ci = [
-    "pip install ./plugin_example",
     "rm -f .coverage",
     # run tests
-    "pytest --verbose --cov-append  --cov-branch --cov-fail-under=98 --cov=jinjanator",
+    "pytest --verbose --cov-append  --cov-branch --cov-fail-under=97 --cov=jinjanator",
     # produce a coverage report with 'missing' lines indicated
     "coverage report -m",
 ]
 
+[tool.hatch.metadata]
+allow-direct-references = true
+
 [tool.hatch.metadata.hooks.fancy-pypi-readme]
 content-type = "text/markdown"
 
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
 text = """
 # *jinjanator*: CLI tool for rendering Jinja2 templates
 
 """
 
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
 path = "README.md"
-start-at = "Features:"
-end-before = "## Credits"
+start-after = "<!-- fancy-readme start -->"
+end-before = "<!-- fancy-readme end -->"
 
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
 text = """
 ## Release Information
 """
 
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
@@ -204,39 +203,30 @@
   "PLR0912",  # Leave complexity to me.
   "TRY301",   # Raise in try blocks can totally make sense.
 ]
 unfixable = ["F401"]
 
 [tool.ruff.per-file-ignores]
 "src/jinjanator/cli.py" = ["T201"]
-"plugin_example/jinjanator_plugin_example.py" = ["INP001"]
-"plugin_example/tests/test_plugin.py" = ["INP001"]
 "tests/*" = [
   "PLC1901", # empty strings are falsey, but are less specific in tests
   "PT005",   # we use always underscores and explicit names
   "S101",    # assert
   "SIM300",  # Yoda rocks in tests
 ]
-"plugin_example/tests/*" = [
-  "PLC1901", # empty strings are falsey, but are less specific in tests
-  "PT005",   # we use always underscores and explicit names
-  "S101",    # assert
-  "SIM300",  # Yoda rocks in tests
-]
 
 [tool.ruff.isort]
 lines-between-types = 1
 lines-after-imports = 2
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 xfail_strict = true
 testpaths = [
     "tests",
-    "plugin_example/tests",
 ]
 addopts = [
     "-ra",
     "--strict-markers",
 ]
 
 [tool.mypy]
```

### Comparing `jinjanator-23.3.0/PKG-INFO` & `jinjanator-23.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jinjanator
-Version: 23.3.0
+Version: 23.4.0
 Summary: Command-line interface to Jinja2 for templating in shell scripts.
 Project-URL: Bug Tracker, https://github.com/kpfleming/jinjanator/issues
 Project-URL: Homepage, https://github.com/kpfleming/jinjanator
 Author-email: "Kevin P. Fleming" <jinjanator@kevin.km6g.us>, Mark Vartanyan <kolypto@gmail.com>
 License: Apache-2.0
 License-File: LICENSE.apache-2.0
 License-File: LICENSE.bsd-2-clause
@@ -19,38 +19,41 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: attrs
 Requires-Dist: jinja2>=2.7.2
-Requires-Dist: pluggy
+Requires-Dist: jinjanator-plugins==23.1.*
 Requires-Dist: pyyaml
 Requires-Dist: typing-extensions
 Description-Content-Type: text/markdown
 
 # *jinjanator*: CLI tool for rendering Jinja2 templates
 
+
 Features:
 
 * Jinja2 templating
 * INI, YAML, JSON data sources supported
 * Environment variables can be used with or without data files
 * Plugins can provide additional formats, filters, tests, and global
-  functions (see [Plugins](https://github.com/kpfleming/jinjanator/tree/main/PLUGINS.md) for details).
+  functions (see
+  [jinjanator-plugins](https://github.com/kpfleming/jinjanator-plugins)
+  for details)
 
 ## Installation
 
 ```
 pip install jinjanator
 ```
 
 ## Tutorial
 
-Suppose, you have an NGINX configuration file template, `nginx.j2`:
+Suppose you have an NGINX configuration file template, `nginx.j2`:
 
 ```jinja2
 server {
   listen 80;
   server_name {{ nginx.hostname }};
 
   root {{ nginx.webroot }};
@@ -309,19 +312,16 @@
 ```jinja2
 User: {{ user_login }}
 Pass: {{ env("USER_PASSWORD") }}
 ```
 
 Notice that there must be quotes around the environment variable name
 when it is a literal string.
+"## Release Information
+### Backwards-incompatible Changes
 
-## Release Information
-### Fixes
-
-- Disabled Jinja2 'autoescape' feature since it can produce incorrect output.
-  [[#8](https://github.com/kpfleming/jinjanator/issues/8)](https://github.com/kpfleming/jinjanator/issues/8)
-- Add missing 'attrs' package to project dependencies.
-  [[#9](https://github.com/kpfleming/jinjanator/issues/9)](https://github.com/kpfleming/jinjanator/issues/9)
+- Moved plugin API to the jinjanator-plugins package.
+  [[#12](https://github.com/kpfleming/jinjanator/issues/12)](https://github.com/kpfleming/jinjanator/issues/12)
 
 
 ---
 [→ Full Changelog](https://github.com/kpfleming/jinjanator/blob/main/CHANGELOG.md)
```

