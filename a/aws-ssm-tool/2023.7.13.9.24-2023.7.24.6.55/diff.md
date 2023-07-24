# Comparing `tmp/aws-ssm-tool-2023.7.13.9.24.tar.gz` & `tmp/aws-ssm-tool-2023.7.24.6.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-ssm-tool-2023.7.13.9.24.tar", last modified: Thu Jul 13 16:24:37 2023, max compression
+gzip compressed data, was "aws-ssm-tool-2023.7.24.6.55.tar", last modified: Mon Jul 24 06:55:09 2023, max compression
```

## Comparing `aws-ssm-tool-2023.7.13.9.24.tar` & `aws-ssm-tool-2023.7.24.6.55.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-13 16:24:37.793945 aws-ssm-tool-2023.7.13.9.24/
--rw-rw-r--   0 matt      (1000) matt      (1000)      653 2023-07-13 16:24:37.793945 aws-ssm-tool-2023.7.13.9.24/PKG-INFO
--rw-rw-r--   0 matt      (1000) matt      (1000)     2333 2023-07-13 14:54:53.000000 aws-ssm-tool-2023.7.13.9.24/README.md
--rw-rw-r--   0 matt      (1000) matt      (1000)     1278 2023-07-13 16:24:37.797945 aws-ssm-tool-2023.7.13.9.24/setup.cfg
--rw-rw-r--   0 matt      (1000) matt      (1000)      765 2023-07-13 15:47:55.000000 aws-ssm-tool-2023.7.13.9.24/setup.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-13 16:24:37.789945 aws-ssm-tool-2023.7.13.9.24/src/
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-13 16:24:37.793945 aws-ssm-tool-2023.7.13.9.24/src/aws_ssm_tool.egg-info/
--rw-rw-r--   0 matt      (1000) matt      (1000)      653 2023-07-13 16:24:37.000000 aws-ssm-tool-2023.7.13.9.24/src/aws_ssm_tool.egg-info/PKG-INFO
--rw-rw-r--   0 matt      (1000) matt      (1000)      651 2023-07-13 16:24:37.000000 aws-ssm-tool-2023.7.13.9.24/src/aws_ssm_tool.egg-info/SOURCES.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        1 2023-07-13 16:24:37.000000 aws-ssm-tool-2023.7.13.9.24/src/aws_ssm_tool.egg-info/dependency_links.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)       42 2023-07-13 16:24:37.000000 aws-ssm-tool-2023.7.13.9.24/src/aws_ssm_tool.egg-info/entry_points.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        1 2023-07-13 16:24:37.000000 aws-ssm-tool-2023.7.13.9.24/src/aws_ssm_tool.egg-info/not-zip-safe
--rw-rw-r--   0 matt      (1000) matt      (1000)      206 2023-07-13 16:24:37.000000 aws-ssm-tool-2023.7.13.9.24/src/aws_ssm_tool.egg-info/requires.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        4 2023-07-13 16:24:37.000000 aws-ssm-tool-2023.7.13.9.24/src/aws_ssm_tool.egg-info/top_level.txt
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-13 16:24:37.793945 aws-ssm-tool-2023.7.13.9.24/src/ssm/
--rw-rw-r--   0 matt      (1000) matt      (1000)       12 2023-07-13 15:47:55.000000 aws-ssm-tool-2023.7.13.9.24/src/ssm/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)       78 2023-07-13 15:47:55.000000 aws-ssm-tool-2023.7.13.9.24/src/ssm/__main__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)       77 2023-07-13 16:24:35.000000 aws-ssm-tool-2023.7.13.9.24/src/ssm/_version.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-13 16:24:37.793945 aws-ssm-tool-2023.7.13.9.24/src/ssm/abcs/
--rw-rw-r--   0 matt      (1000) matt      (1000)       97 2023-07-13 16:21:21.000000 aws-ssm-tool-2023.7.13.9.24/src/ssm/abcs/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      506 2023-07-13 15:47:55.000000 aws-ssm-tool-2023.7.13.9.24/src/ssm/abcs/loggable.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-13 16:24:37.793945 aws-ssm-tool-2023.7.13.9.24/src/ssm/api/
--rw-rw-r--   0 matt      (1000) matt      (1000)     4086 2023-07-13 15:47:55.000000 aws-ssm-tool-2023.7.13.9.24/src/ssm/api/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     5528 2023-07-13 15:47:55.000000 aws-ssm-tool-2023.7.13.9.24/src/ssm/api/environment.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2879 2023-07-13 15:47:55.000000 aws-ssm-tool-2023.7.13.9.24/src/ssm/api/manager.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-13 16:24:37.793945 aws-ssm-tool-2023.7.13.9.24/src/ssm/bin/
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-07-13 15:47:55.000000 aws-ssm-tool-2023.7.13.9.24/src/ssm/bin/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2662 2023-07-13 16:22:40.000000 aws-ssm-tool-2023.7.13.9.24/src/ssm/bin/ssm.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-13 16:24:37.793945 aws-ssm-tool-2023.7.13.9.24/src/ssm/cli/
--rw-rw-r--   0 matt      (1000) matt      (1000)     1578 2023-07-13 16:23:49.000000 aws-ssm-tool-2023.7.13.9.24/src/ssm/cli/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      198 2023-07-13 15:47:55.000000 aws-ssm-tool-2023.7.13.9.24/src/ssm/cli/args.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     5037 2023-07-13 15:47:55.000000 aws-ssm-tool-2023.7.13.9.24/src/ssm/cli/options.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3640 2023-07-13 15:47:55.000000 aws-ssm-tool-2023.7.13.9.24/src/ssm/cli/wrapper.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-13 16:24:37.793945 aws-ssm-tool-2023.7.13.9.24/src/ssm/util/
--rw-rw-r--   0 matt      (1000) matt      (1000)     1784 2023-07-13 15:47:55.000000 aws-ssm-tool-2023.7.13.9.24/src/ssm/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:55:09.438927 aws-ssm-tool-2023.7.24.6.55/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-24 06:55:09.438927 aws-ssm-tool-2023.7.24.6.55/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-24 06:54:26.000000 aws-ssm-tool-2023.7.24.6.55/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-24 06:55:09.438927 aws-ssm-tool-2023.7.24.6.55/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-24 06:54:26.000000 aws-ssm-tool-2023.7.24.6.55/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:55:09.426927 aws-ssm-tool-2023.7.24.6.55/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:55:09.430927 aws-ssm-tool-2023.7.24.6.55/src/aws_ssm_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-24 06:55:09.000000 aws-ssm-tool-2023.7.24.6.55/src/aws_ssm_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-24 06:55:09.000000 aws-ssm-tool-2023.7.24.6.55/src/aws_ssm_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 06:55:09.000000 aws-ssm-tool-2023.7.24.6.55/src/aws_ssm_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-24 06:55:09.000000 aws-ssm-tool-2023.7.24.6.55/src/aws_ssm_tool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 06:55:09.000000 aws-ssm-tool-2023.7.24.6.55/src/aws_ssm_tool.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-24 06:55:09.000000 aws-ssm-tool-2023.7.24.6.55/src/aws_ssm_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-24 06:55:09.000000 aws-ssm-tool-2023.7.24.6.55/src/aws_ssm_tool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:55:09.430927 aws-ssm-tool-2023.7.24.6.55/src/ssm/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-24 06:54:26.000000 aws-ssm-tool-2023.7.24.6.55/src/ssm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-24 06:54:26.000000 aws-ssm-tool-2023.7.24.6.55/src/ssm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-24 06:55:05.000000 aws-ssm-tool-2023.7.24.6.55/src/ssm/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:55:09.434927 aws-ssm-tool-2023.7.24.6.55/src/ssm/abcs/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-24 06:54:26.000000 aws-ssm-tool-2023.7.24.6.55/src/ssm/abcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-24 06:54:26.000000 aws-ssm-tool-2023.7.24.6.55/src/ssm/abcs/loggable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:55:09.434927 aws-ssm-tool-2023.7.24.6.55/src/ssm/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-24 06:54:26.000000 aws-ssm-tool-2023.7.24.6.55/src/ssm/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-07-24 06:54:26.000000 aws-ssm-tool-2023.7.24.6.55/src/ssm/api/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-07-24 06:54:26.000000 aws-ssm-tool-2023.7.24.6.55/src/ssm/api/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:55:09.434927 aws-ssm-tool-2023.7.24.6.55/src/ssm/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 06:54:26.000000 aws-ssm-tool-2023.7.24.6.55/src/ssm/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-24 06:54:26.000000 aws-ssm-tool-2023.7.24.6.55/src/ssm/bin/ssm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:55:09.438927 aws-ssm-tool-2023.7.24.6.55/src/ssm/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-24 06:54:26.000000 aws-ssm-tool-2023.7.24.6.55/src/ssm/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-24 06:54:26.000000 aws-ssm-tool-2023.7.24.6.55/src/ssm/cli/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-07-24 06:54:26.000000 aws-ssm-tool-2023.7.24.6.55/src/ssm/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-07-24 06:54:26.000000 aws-ssm-tool-2023.7.24.6.55/src/ssm/cli/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:55:09.438927 aws-ssm-tool-2023.7.24.6.55/src/ssm/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-24 06:54:26.000000 aws-ssm-tool-2023.7.24.6.55/src/ssm/util/__init__.py
```

### Comparing `aws-ssm-tool-2023.7.13.9.24/PKG-INFO` & `aws-ssm-tool-2023.7.24.6.55/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-ssm-tool
-Version: 2023.7.13.9.24
+Version: 2023.7.24.6.55
 Summary: AWS SSM tool
 Home-page: https://github.com/Robot-Wranglers/aws-ssm-tool/
 Author: Robot-Wranglers
 License: MIT
 Project-URL: Documentation, https://github.com/Robot-Wranglers/aws-ssm-tool/
 Project-URL: Source, https://github.com/Robot-Wranglers/aws-ssm-tool/
 Project-URL: Download, https://github.com/Robot-Wranglers/aws-ssm-tool/#files
```

### Comparing `aws-ssm-tool-2023.7.13.9.24/setup.cfg` & `aws-ssm-tool-2023.7.24.6.55/setup.cfg`

 * *Files identical despite different names*

### Comparing `aws-ssm-tool-2023.7.13.9.24/setup.py` & `aws-ssm-tool-2023.7.24.6.55/setup.py`

 * *Files identical despite different names*

### Comparing `aws-ssm-tool-2023.7.13.9.24/src/aws_ssm_tool.egg-info/PKG-INFO` & `aws-ssm-tool-2023.7.24.6.55/src/aws_ssm_tool.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-ssm-tool
-Version: 2023.7.13.9.24
+Version: 2023.7.24.6.55
 Summary: AWS SSM tool
 Home-page: https://github.com/Robot-Wranglers/aws-ssm-tool/
 Author: Robot-Wranglers
 License: MIT
 Project-URL: Documentation, https://github.com/Robot-Wranglers/aws-ssm-tool/
 Project-URL: Source, https://github.com/Robot-Wranglers/aws-ssm-tool/
 Project-URL: Download, https://github.com/Robot-Wranglers/aws-ssm-tool/#files
```

### Comparing `aws-ssm-tool-2023.7.13.9.24/src/aws_ssm_tool.egg-info/SOURCES.txt` & `aws-ssm-tool-2023.7.24.6.55/src/aws_ssm_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aws-ssm-tool-2023.7.13.9.24/src/ssm/api/__init__.py` & `aws-ssm-tool-2023.7.24.6.55/src/ssm/api/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-ssm-tool-2023.7.13.9.24/src/ssm/api/environment.py` & `aws-ssm-tool-2023.7.24.6.55/src/ssm/api/environment.py`

 * *Files identical despite different names*

### Comparing `aws-ssm-tool-2023.7.13.9.24/src/ssm/api/manager.py` & `aws-ssm-tool-2023.7.24.6.55/src/ssm/api/manager.py`

 * *Files identical despite different names*

### Comparing `aws-ssm-tool-2023.7.13.9.24/src/ssm/bin/ssm.py` & `aws-ssm-tool-2023.7.24.6.55/src/ssm/bin/ssm.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import functools
 
 import click
 
 from ssm import api, cli, util
 from ssm.cli.wrapper import ApiWrapper
+
 LOGGER = util.get_logger(__name__)
 
 
 @click.command(cls=cli.Group)
 def entry(*args, **kargs):  # noqa
     """
     Tool for accessing secrets
```

### Comparing `aws-ssm-tool-2023.7.13.9.24/src/ssm/cli/__init__.py` & `aws-ssm-tool-2023.7.24.6.55/src/ssm/cli/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """ ssm.cli (click boilerplate)
 """
 
 import click
-from . import options, args # noqa
 
 from ssm import util
+
+from . import args, options  # noqa
+
 LOGGER = util.get_logger(__name__)
 
 
 class Group(click.Group):
     """
     Subclass of click.Group, mostly just for supporting command aliases
     """
@@ -21,22 +23,22 @@
         """
         result = click.Group.list_commands(self, ctx)
         root_commands = [x for x in result if not self.commands[x].is_alias]
         alias_commands = [x for x in result if self.commands[x].is_alias]
         result = root_commands + alias_commands
         return result
 
-    def command(self, *args, **kwargs):
+    def command(self, *_args, **kwargs):
         """
         Override  from super.
         """
         aliases = kwargs.pop("aliases", [])
 
         def decorator(f):
-            cmd = click.decorators.command(*args, **kwargs)(click.pass_context(f))
+            cmd = click.decorators.command(*_args, **kwargs)(click.pass_context(f))
             self.add_command(cmd)
             cmd.is_alias = False
             for alias in aliases:
                 zz = kwargs.copy()
 
                 def g(*aa, **kk):
                     return f(*aa, **kk)
```

### Comparing `aws-ssm-tool-2023.7.13.9.24/src/ssm/cli/options.py` & `aws-ssm-tool-2023.7.24.6.55/src/ssm/cli/options.py`

 * *Files identical despite different names*

### Comparing `aws-ssm-tool-2023.7.13.9.24/src/ssm/cli/wrapper.py` & `aws-ssm-tool-2023.7.24.6.55/src/ssm/cli/wrapper.py`

 * *Files 7% similar despite different names*

```diff
@@ -70,27 +70,20 @@
         if self.is_subcommand:
             # otherwise base options would be added twice for stand-alone style CLIs
             options += self.__class__.BASE_OPTIONS
 
         @functools.wraps(self.fxn)
         def proxy(*args, **kwargs):
             """ """
-            # if args and isinstance(args[0],(click.core.Context,)):
-            #     # none of the api commands are anticipating the click context
-            #     args = args[1:]
             args = [x for x in args if not isinstance(x, (click.core.Context,))]
-            LOGGER.debug(f"proxying args={args}, kwargs={kwargs}")
+            # LOGGER.info(f"proxying args={args}, kwargs={kwargs}")
             api_result = self.fxn(*args, **kwargs)
             print(api_result)
-            if not isinstance(api_result, (dict, list)):
-                LOGGER.warning("api result returned was not JSON!")
-            # if util.is_string(api_result):
-            #     print(result)
-            # else:
-            #     print(json.dumps(api_result, indent=2))
+            # if not isinstance(api_result, (dict, list)):
+            #     LOGGER.warning("api result returned was not JSON!")
             return api_result
 
         for option in options:
             proxy = option(proxy)
 
         if self.is_subcommand:
             if self.aliases:
@@ -103,9 +96,8 @@
             result = click.command()(proxy)
         else:
             err = "unknown entry type '{}' for '{}'".format(
                 type(self.entry), self.entry
             )
             LOGGER.critical(err)
             raise RuntimeError(err)
-        # print(result)
         return result
```

### Comparing `aws-ssm-tool-2023.7.13.9.24/src/ssm/util/__init__.py` & `aws-ssm-tool-2023.7.24.6.55/src/ssm/util/__init__.py`

 * *Files identical despite different names*

